# Comparing `tmp/flwr_nightly-1.5.0.dev20230529.tar.gz` & `tmp/flwr_nightly-1.5.0.dev20230608.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.5.0.dev20230529.tar", max compression
+gzip compressed data, was "flwr_nightly-1.5.0.dev20230608.tar", max compression
```

## Comparing `flwr_nightly-1.5.0.dev20230529.tar` & `flwr_nightly-1.5.0.dev20230608.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0    11358 2023-05-29 23:02:24.697131 flwr_nightly-1.5.0.dev20230529/LICENSE
--rw-r--r--   0        0        0    10363 2023-05-29 23:02:24.697131 flwr_nightly-1.5.0.dev20230529/README.md
--rw-r--r--   0        0        0     4333 2023-05-29 23:02:47.817319 flwr_nightly-1.5.0.dev20230529/pyproject.toml
--rw-r--r--   0        0        0      952 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/__init__.py
--rw-r--r--   0        0        0     1164 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    13838 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     6503 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     3351 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      728 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     4293 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      745 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     5476 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0      712 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     5077 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1686 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     5100 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      728 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0     8336 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     2877 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1876 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     1113 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0      884 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     1828 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     1890 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     3483 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0     2120 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0    16316 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7805 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     3714 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      848 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      809 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/driver/__init__.py
--rw-r--r--   0        0        0     4826 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/driver/app.py
--rw-r--r--   0        0        0     3909 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/driver/driver.py
--rw-r--r--   0        0        0     4414 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/driver/driver_client_manager.py
--rw-r--r--   0        0        0     5654 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/driver/driver_client_proxy.py
--rw-r--r--   0        0        0      676 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     4663 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     3815 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     5727 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     1617 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     4982 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     4554 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     4275 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     1495 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1188 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     3217 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4286 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0    18721 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1370 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    26342 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     5941 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2228 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0     1058 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      705 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     3919 2023-05-29 23:02:24.953132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/driver/driver_servicer.py
--rw-r--r--   0        0        0      704 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/__init__.py
--rw-r--r--   0        0        0      728 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     4467 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
--rw-r--r--   0        0        0     5602 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6416 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4651 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11523 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0     6314 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
--rw-r--r--   0        0        0      751 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     1858 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      724 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      728 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     3718 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0     4457 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/history.py
--rw-r--r--   0        0        0    15963 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/server.py
--rw-r--r--   0        0        0      996 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/state/__init__.py
--rw-r--r--   0        0        0     6521 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/state/in_memory_state.py
--rw-r--r--   0        0        0    19296 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/state/sqlite_state.py
--rw-r--r--   0        0        0     4805 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/state/state.py
--rw-r--r--   0        0        0     1648 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/state/state_factory.py
--rw-r--r--   0        0        0     1667 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0     6099 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     4511 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     4867 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5830 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6722 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7004 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11487 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9977 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8244 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2666 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5385 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     7057 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5916 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     3368 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     7036 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6302 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10139 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7484 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      901 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5114 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     4941 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0     1271 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0     7763 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      727 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     5472 2023-05-29 23:02:24.957132 flwr_nightly-1.5.0.dev20230529/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230529/setup.py
--rw-r--r--   0        0        0    12838 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230529/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-08 23:02:45.679186 flwr_nightly-1.5.0.dev20230608/LICENSE
+-rw-r--r--   0        0        0    10363 2023-06-08 23:02:45.679186 flwr_nightly-1.5.0.dev20230608/README.md
+-rw-r--r--   0        0        0     4333 2023-06-08 23:03:20.659572 flwr_nightly-1.5.0.dev20230608/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0     1164 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    13838 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     7681 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     3351 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      728 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     4293 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      745 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     5476 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0      712 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     5077 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1686 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     5319 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      728 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0     8336 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     2877 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1876 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     1113 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0      884 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     1828 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     1890 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     3483 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0     2120 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0    16316 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7805 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     3714 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      848 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      809 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/__init__.py
+-rw-r--r--   0        0        0     4826 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/app.py
+-rw-r--r--   0        0        0     3909 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/driver.py
+-rw-r--r--   0        0        0     4414 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/driver_client_manager.py
+-rw-r--r--   0        0        0     5654 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/driver_client_proxy.py
+-rw-r--r--   0        0        0      676 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     4663 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     3815 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     5727 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     1617 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4982 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     4554 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0     4275 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     1495 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1188 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3217 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4286 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18721 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1370 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    26342 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     5941 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2228 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0     1058 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      705 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     3919 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/driver/driver_servicer.py
+-rw-r--r--   0        0        0      704 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     4467 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
+-rw-r--r--   0        0        0     5602 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6416 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4651 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11523 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0     6314 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
+-rw-r--r--   0        0        0      751 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     1858 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      724 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     2026 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      728 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     3718 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0     4457 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0    15963 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0      996 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/__init__.py
+-rw-r--r--   0        0        0     6521 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/in_memory_state.py
+-rw-r--r--   0        0        0    19280 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/sqlite_state.py
+-rw-r--r--   0        0        0     4805 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/state.py
+-rw-r--r--   0        0        0     1648 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/state_factory.py
+-rw-r--r--   0        0        0     1667 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0     6099 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     4508 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     4867 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5830 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6722 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7004 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11487 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9977 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8244 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2666 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5385 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     7057 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5916 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     3368 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     7036 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6302 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10139 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7484 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      901 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5098 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     4941 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0     1271 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0     7763 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     5472 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230608/setup.py
+-rw-r--r--   0        0        0    12838 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230608/PKG-INFO
```

### Comparing `flwr_nightly-1.5.0.dev20230529/LICENSE` & `flwr_nightly-1.5.0.dev20230608/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/README.md` & `flwr_nightly-1.5.0.dev20230608/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/pyproject.toml` & `flwr_nightly-1.5.0.dev20230608/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.5.0-dev20230529"
+version = "1.5.0-dev20230608"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.dev>"]
 readme = "README.md"
 homepage = "https://flower.dev"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.dev"
@@ -74,15 +74,15 @@
 types-protobuf = "==3.19.18"
 types-requests = "==2.28.11.17"
 types-setuptools = "==67.7.0.1"
 clang-format = "==16.0.3"
 isort = "==5.11.5"
 black = { version = "==23.3.0", extras = ["jupyter"] }
 docformatter = "==1.7.1"
-mypy = "==0.961"
+mypy = "==1.3.0"
 pylint = "==2.13.8"
 flake8 = "==3.9.2"
 pytest = "==7.1.2"
 pytest-cov = "==3.0.0"
 pytest-watch = "==4.2.0"
 grpcio-tools = "==1.48.2"
 mypy-protobuf = "==3.2.0"
```

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/app.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/client.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/numpy_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,198 +8,140 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Flower client (abstract base class)."""
+"""Flower client app."""
 
 
 from abc import ABC
+from typing import Dict, Tuple
 
-from flwr.common import (
-    Code,
-    EvaluateIns,
-    EvaluateRes,
-    FitIns,
-    FitRes,
-    GetParametersIns,
-    GetParametersRes,
-    GetPropertiesIns,
-    GetPropertiesRes,
-    Parameters,
-    Status,
-)
+from flwr.common import Config, NDArrays, Scalar
 
 
-class Client(ABC):
-    """Abstract base class for Flower clients."""
+class NumPyClient(ABC):
+    """Abstract base class for Flower clients using NumPy."""
 
-    def get_properties(self, ins: GetPropertiesIns) -> GetPropertiesRes:
-        """Return set of client's properties.
+    def get_properties(self, config: Config) -> Dict[str, Scalar]:
+        """Returns a client's set of properties.
 
         Parameters
         ----------
-        ins : GetPropertiesIns
-            The get properties instructions received from the server containing
-            a dictionary of configuration values.
+        config : Config
+            Configuration parameters requested by the server.
+            This can be used to tell the client which properties
+            are needed along with some Scalar attributes.
 
         Returns
         -------
-        GetPropertiesRes
-            The current client properties.
+        properties : Dict[str, Scalar]
+            A dictionary mapping arbitrary string keys to values of type
+            bool, bytes, float, int, or str. It can be used to communicate
+            arbitrary property values back to the server.
         """
+        _ = (self, config)
+        return {}
 
-    def get_parameters(self, ins: GetParametersIns) -> GetParametersRes:
+    def get_parameters(self, config: Dict[str, Scalar]) -> NDArrays:
         """Return the current local model parameters.
 
         Parameters
         ----------
-        ins : GetParametersIns
-            The get parameters instructions received from the server containing
-            a dictionary of configuration values.
+        config : Config
+            Configuration parameters requested by the server.
+            This can be used to tell the client which parameters
+            are needed along with some Scalar attributes.
 
         Returns
         -------
-        GetParametersRes
-            The current local model parameters.
+        parameters : NDArrays
+            The local model parameters as a list of NumPy ndarrays.
         """
+        _ = (self, config)
+        return []
 
-    def fit(self, ins: FitIns) -> FitRes:
-        """Refine the provided parameters using the locally held dataset.
+    def fit(
+        self, parameters: NDArrays, config: Dict[str, Scalar]
+    ) -> Tuple[NDArrays, int, Dict[str, Scalar]]:
+        """Train the provided parameters using the locally held dataset.
 
         Parameters
         ----------
-        ins : FitIns
-            The training instructions containing (global) model parameters
-            received from the server and a dictionary of configuration values
-            used to customize the local training process.
+        parameters : NDArrays
+            The current (global) model parameters.
+        config : Dict[str, Scalar]
+            Configuration parameters which allow the
+            server to influence training on the client. It can be used to
+            communicate arbitrary values from the server to the client, for
+            example, to set the number of (local) training epochs.
 
         Returns
         -------
-        FitRes
-            The training result containing updated parameters and other details
-            such as the number of local training examples used for training.
+        parameters : NDArrays
+            The locally updated model parameters.
+        num_examples : int
+            The number of examples used for training.
+        metrics : Dict[str, Scalar]
+            A dictionary mapping arbitrary string keys to values of type
+            bool, bytes, float, int, or str. It can be used to communicate
+            arbitrary values back to the server.
         """
+        _ = (self, parameters, config)
+        return [], 0, {}
 
-    def evaluate(self, ins: EvaluateIns) -> EvaluateRes:
+    def evaluate(
+        self, parameters: NDArrays, config: Dict[str, Scalar]
+    ) -> Tuple[float, int, Dict[str, Scalar]]:
         """Evaluate the provided parameters using the locally held dataset.
 
         Parameters
         ----------
-        ins : EvaluateIns
-            The evaluation instructions containing (global) model parameters
-            received from the server and a dictionary of configuration values
-            used to customize the local evaluation process.
+        parameters : NDArrays
+            The current (global) model parameters.
+        config : Dict[str, Scalar]
+            Configuration parameters which allow the server to influence
+            evaluation on the client. It can be used to communicate
+            arbitrary values from the server to the client, for example,
+            to influence the number of examples used for evaluation.
 
         Returns
         -------
-        EvaluateRes
-            The evaluation result containing the loss on the local dataset and
-            other details such as the number of local data examples used for
-            evaluation.
+        loss : float
+            The evaluation loss of the model on the local dataset.
+        num_examples : int
+            The number of examples used for evaluation.
+        metrics : Dict[str, Scalar]
+            A dictionary mapping arbitrary string keys to values of
+            type bool, bytes, float, int, or str. It can be used to
+            communicate arbitrary values back to the server.
+
+        Warning
+        -------
+        The previous return type format (int, float, float) and the
+        extended format (int, float, float, Dict[str, Scalar]) have been
+        deprecated and removed since Flower 0.19.
         """
+        _ = (self, parameters, config)
+        return 0.0, 0, {}
+
+
+def has_get_properties(client: NumPyClient) -> bool:
+    """Check if NumPyClient implements get_properties."""
+    return type(client).get_properties != NumPyClient.get_properties
+
+
+def has_get_parameters(client: NumPyClient) -> bool:
+    """Check if NumPyClient implements get_parameters."""
+    return type(client).get_parameters != NumPyClient.get_parameters
+
 
+def has_fit(client: NumPyClient) -> bool:
+    """Check if NumPyClient implements fit."""
+    return type(client).fit != NumPyClient.fit
 
-def has_get_properties(client: Client) -> bool:
-    """Check if Client implements get_properties."""
-    return type(client).get_properties != Client.get_properties
-
-
-def has_get_parameters(client: Client) -> bool:
-    """Check if Client implements get_parameters."""
-    return type(client).get_parameters != Client.get_parameters
-
-
-def has_fit(client: Client) -> bool:
-    """Check if Client implements fit."""
-    return type(client).fit != Client.fit
-
-
-def has_evaluate(client: Client) -> bool:
-    """Check if Client implements evaluate."""
-    return type(client).evaluate != Client.evaluate
-
-
-def maybe_call_get_properties(
-    client: Client, get_properties_ins: GetPropertiesIns
-) -> GetPropertiesRes:
-    """Call `get_properties` if the client overrides it."""
-
-    # Check if client overrides `get_properties`
-    if not has_get_properties(client=client):
-        # If client does not override `get_properties`, don't call it
-        status = Status(
-            code=Code.GET_PROPERTIES_NOT_IMPLEMENTED,
-            message="Client does not implement `get_properties`",
-        )
-        return GetPropertiesRes(
-            status=status,
-            properties={},
-        )
-
-    # If the client implements `get_properties`, call it
-    return client.get_properties(get_properties_ins)
-
-
-def maybe_call_get_parameters(
-    client: Client, get_parameters_ins: GetParametersIns
-) -> GetParametersRes:
-    """Call `get_parameters` if the client overrides it."""
-
-    # Check if client overrides `get_parameters`
-    if not has_get_parameters(client=client):
-        # If client does not override `get_parameters`, don't call it
-        status = Status(
-            code=Code.GET_PARAMETERS_NOT_IMPLEMENTED,
-            message="Client does not implement `get_parameters`",
-        )
-        return GetParametersRes(
-            status=status,
-            parameters=Parameters(tensor_type="", tensors=[]),
-        )
-
-    # If the client implements `get_parameters`, call it
-    return client.get_parameters(get_parameters_ins)
-
-
-def maybe_call_fit(client: Client, fit_ins: FitIns) -> FitRes:
-    """Call `fit` if the client overrides it."""
-
-    # Check if client overrides `fit`
-    if not has_fit(client=client):
-        # If client does not override `fit`, don't call it
-        status = Status(
-            code=Code.FIT_NOT_IMPLEMENTED,
-            message="Client does not implement `fit`",
-        )
-        return FitRes(
-            status=status,
-            parameters=Parameters(tensor_type="", tensors=[]),
-            num_examples=0,
-            metrics={},
-        )
-
-    # If the client implements `fit`, call it
-    return client.fit(fit_ins)
-
-
-def maybe_call_evaluate(client: Client, evaluate_ins: EvaluateIns) -> EvaluateRes:
-    """Call `evaluate` if the client overrides it."""
-
-    # Check if client overrides `evaluate`
-    if not has_evaluate(client=client):
-        # If client does not override `evaluate`, don't call it
-        status = Status(
-            code=Code.EVALUATE_NOT_IMPLEMENTED,
-            message="Client does not implement `evaluate`",
-        )
-        return EvaluateRes(
-            status=status,
-            loss=0.0,
-            num_examples=0,
-            metrics={},
-        )
 
-    # If the client implements `evaluate`, call it
-    return client.evaluate(evaluate_ins)
+def has_evaluate(client: NumPyClient) -> bool:
+    """Check if NumPyClient implements evaluate."""
+    return type(client).evaluate != NumPyClient.evaluate
```

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,132 +8,123 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Flower client app."""
+"""DP-FedAvg [McMahan et al., 2018] strategy.
 
+Paper: arxiv.org/pdf/1710.06963.pdf
+"""
 
-from abc import ABC
-from typing import Dict, Tuple
 
-from flwr.common import Config, NDArrays, Scalar
+from typing import Dict, List, Optional, Tuple, Union
 
-
-class NumPyClient(ABC):
-    """Abstract base class for Flower clients using NumPy."""
-
-    def get_properties(self, config: Config) -> Dict[str, Scalar]:
-        """Returns a client's set of properties.
-
-        Parameters
-        ----------
-        config : Config
-            Configuration parameters requested by the server.
-            This can be used to tell the client which properties
-            are needed along with some Scalar attributes.
-
-        Returns
-        -------
-        properties : Dict[str, Scalar]
-            A dictionary mapping arbitrary string keys to values of type
-            bool, bytes, float, int, or str. It can be used to communicate
-            arbitrary property values back to the server.
-        """
-
-    def get_parameters(self, config: Dict[str, Scalar]) -> NDArrays:
-        """Return the current local model parameters.
-
-        Parameters
-        ----------
-        config : Config
-            Configuration parameters requested by the server.
-            This can be used to tell the client which parameters
-            are needed along with some Scalar attributes.
-
-        Returns
-        -------
-        parameters : NDArrays
-            The local model parameters as a list of NumPy ndarrays.
-        """
-
-    def fit(
-        self, parameters: NDArrays, config: Dict[str, Scalar]
-    ) -> Tuple[NDArrays, int, Dict[str, Scalar]]:
-        """Train the provided parameters using the locally held dataset.
-
-        Parameters
-        ----------
-        parameters : NDArrays
-            The current (global) model parameters.
-        config : Dict[str, Scalar]
-            Configuration parameters which allow the
-            server to influence training on the client. It can be used to
-            communicate arbitrary values from the server to the client, for
-            example, to set the number of (local) training epochs.
-
-        Returns
-        -------
-        parameters : NDArrays
-            The locally updated model parameters.
-        num_examples : int
-            The number of examples used for training.
-        metrics : Dict[str, Scalar]
-            A dictionary mapping arbitrary string keys to values of type
-            bool, bytes, float, int, or str. It can be used to communicate
-            arbitrary values back to the server.
-        """
+from flwr.common import EvaluateIns, EvaluateRes, FitIns, FitRes, Parameters, Scalar
+from flwr.common.dp import add_gaussian_noise
+from flwr.common.parameter import ndarrays_to_parameters, parameters_to_ndarrays
+from flwr.server.client_manager import ClientManager
+from flwr.server.client_proxy import ClientProxy
+from flwr.server.strategy.strategy import Strategy
+
+
+class DPFedAvgFixed(Strategy):
+    """Wrapper for configuring a Strategy for DP with Fixed Clipping."""
+
+    # pylint: disable=too-many-arguments,too-many-instance-attributes
+    def __init__(
+        self,
+        strategy: Strategy,
+        num_sampled_clients: int,
+        clip_norm: float,
+        noise_multiplier: float = 1,
+        server_side_noising: bool = True,
+    ) -> None:
+        super().__init__()
+        self.strategy = strategy
+        # Doing fixed-size subsampling as in https://arxiv.org/abs/1905.03871.
+        self.num_sampled_clients = num_sampled_clients
+
+        if clip_norm <= 0:
+            raise Exception("The clipping threshold should be a positive value.")
+        self.clip_norm = clip_norm
+
+        if noise_multiplier < 0:
+            raise Exception("The noise multiplier should be a non-negative value.")
+        self.noise_multiplier = noise_multiplier
+
+        self.server_side_noising = server_side_noising
+
+    def __repr__(self) -> str:
+        rep = "Strategy with DP with Fixed Clipping enabled."
+        return rep
+
+    def _calc_client_noise_stddev(self) -> float:
+        return float(
+            self.noise_multiplier * self.clip_norm / (self.num_sampled_clients ** (0.5))
+        )
+
+    def initialize_parameters(
+        self, client_manager: ClientManager
+    ) -> Optional[Parameters]:
+        return self.strategy.initialize_parameters(client_manager)
+
+    def configure_fit(
+        self, server_round: int, parameters: Parameters, client_manager: ClientManager
+    ) -> List[Tuple[ClientProxy, FitIns]]:
+        """Configure the next round of training."""
+
+        additional_config = {"dpfedavg_clip_norm": self.clip_norm}
+        if not self.server_side_noising:
+            additional_config[
+                "dpfedavg_noise_stddev"
+            ] = self._calc_client_noise_stddev()
+
+        client_instructions = self.strategy.configure_fit(
+            server_round, parameters, client_manager
+        )
+
+        for _, fit_ins in client_instructions:
+            fit_ins.config.update(additional_config)
+
+        return client_instructions
+
+    def configure_evaluate(
+        self, server_round: int, parameters: Parameters, client_manager: ClientManager
+    ) -> List[Tuple[ClientProxy, EvaluateIns]]:
+        return self.strategy.configure_evaluate(
+            server_round, parameters, client_manager
+        )
+
+    def aggregate_fit(
+        self,
+        server_round: int,
+        results: List[Tuple[ClientProxy, FitRes]],
+        failures: List[Union[Tuple[ClientProxy, FitRes], BaseException]],
+    ) -> Tuple[Optional[Parameters], Dict[str, Scalar]]:
+        if failures:
+            return None, {}
+        # Forcing unweighted aggregation, as in https://arxiv.org/abs/1905.03871.
+        for _, fit_res in results:
+            fit_res.num_examples = 1
+            fit_res.parameters = ndarrays_to_parameters(
+                add_gaussian_noise(
+                    parameters_to_ndarrays(fit_res.parameters),
+                    self._calc_client_noise_stddev(),
+                )
+            )
+
+        return self.strategy.aggregate_fit(server_round, results, failures)
+
+    def aggregate_evaluate(
+        self,
+        server_round: int,
+        results: List[Tuple[ClientProxy, EvaluateRes]],
+        failures: List[Union[Tuple[ClientProxy, EvaluateRes], BaseException]],
+    ) -> Tuple[Optional[float], Dict[str, Scalar]]:
+        return self.strategy.aggregate_evaluate(server_round, results, failures)
 
     def evaluate(
-        self, parameters: NDArrays, config: Dict[str, Scalar]
-    ) -> Tuple[float, int, Dict[str, Scalar]]:
-        """Evaluate the provided parameters using the locally held dataset.
-
-        Parameters
-        ----------
-        parameters : NDArrays
-            The current (global) model parameters.
-        config : Dict[str, Scalar]
-            Configuration parameters which allow the server to influence
-            evaluation on the client. It can be used to communicate
-            arbitrary values from the server to the client, for example,
-            to influence the number of examples used for evaluation.
-
-        Returns
-        -------
-        loss : float
-            The evaluation loss of the model on the local dataset.
-        num_examples : int
-            The number of examples used for evaluation.
-        metrics : Dict[str, Scalar]
-            A dictionary mapping arbitrary string keys to values of
-            type bool, bytes, float, int, or str. It can be used to
-            communicate arbitrary values back to the server.
-
-        Warning
-        -------
-        The previous return type format (int, float, float) and the
-        extended format (int, float, float, Dict[str, Scalar]) have been
-        deprecated and removed since Flower 0.19.
-        """
-
-
-def has_get_properties(client: NumPyClient) -> bool:
-    """Check if NumPyClient implements get_properties."""
-    return type(client).get_properties != NumPyClient.get_properties
-
-
-def has_get_parameters(client: NumPyClient) -> bool:
-    """Check if NumPyClient implements get_parameters."""
-    return type(client).get_parameters != NumPyClient.get_parameters
-
-
-def has_fit(client: NumPyClient) -> bool:
-    """Check if NumPyClient implements fit."""
-    return type(client).fit != NumPyClient.fit
-
-
-def has_evaluate(client: NumPyClient) -> bool:
-    """Check if NumPyClient implements evaluate."""
-    return type(client).evaluate != NumPyClient.evaluate
+        self, server_round: int, parameters: Parameters
+    ) -> Optional[Tuple[float, Dict[str, Scalar]]]:
+        return self.strategy.evaluate(server_round, parameters)
```

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/address.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/constant.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/date.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/dp.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/grpc.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/logger.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/parameter.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/serde.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/typing.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/common/version.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/driver/app.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/driver/driver.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/driver/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/driver/driver_client_proxy.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/app.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/criterion.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/driver/driver_servicer.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/rest_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/history.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/server.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/state/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/state/in_memory_state.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/state/sqlite_state.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/sqlite_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,15 +463,15 @@
         rows = self.query(query)
         result: Set[int] = {row["node_id"] for row in rows}
         return result
 
 
 def dict_factory(
     cursor: sqlite3.Cursor,
-    row: sqlite3.Row,  # type: ignore
+    row: sqlite3.Row,
 ) -> Dict[str, Any]:
     """Used to turn SQLite results into dicts.
 
     Less efficent for retrival of large amounts of data but easier to
     use.
     """
     fields = [column[0] for column in cursor.description]
```

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/state/state.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/state/state_factory.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,34 +35,35 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
         self,
         strategy: Strategy,
         num_sampled_clients: int,
         init_clip_norm: float = 0.1,
-        noise_multiplier: float = 1,
+        noise_multiplier: float = 1.0,
         server_side_noising: bool = True,
         clip_norm_lr: float = 0.2,
         clip_norm_target_quantile: float = 0.5,
         clip_count_stddev: Optional[float] = None,
     ) -> None:
         super().__init__(
             strategy=strategy,
             num_sampled_clients=num_sampled_clients,
             clip_norm=init_clip_norm,
             noise_multiplier=noise_multiplier,
             server_side_noising=server_side_noising,
         )
         self.clip_norm_lr = clip_norm_lr
         self.clip_norm_target_quantile = clip_norm_target_quantile
-        self.clip_count_stddev = clip_count_stddev
-        if self.clip_count_stddev is None:
-            self.clip_count_stddev = 0
+
+        if clip_count_stddev is None:
+            clip_count_stddev = 0.0
             if noise_multiplier > 0:
-                self.clip_count_stddev = self.num_sampled_clients / 20.0
+                clip_count_stddev = self.num_sampled_clients / 20.0
+        self.clip_count_stddev: float = clip_count_stddev
 
         if noise_multiplier:
             self.noise_multiplier = (
                 self.noise_multiplier ** (-2) - (2 * self.clip_count_stddev) ** (-2)
             ) ** (-0.5)
 
     def __repr__(self) -> str:
```

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/utils/tensorboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,29 +13,27 @@
 # limitations under the License.
 # ==============================================================================
 """Flower TensorBoard utilities."""
 
 
 import os
 from datetime import datetime
-from typing import Callable, Dict, List, Optional, Tuple, TypeVar, Union, cast
-
-try:
-    import tensorflow as tf
-except ImportError:
-    tf = None
+from typing import Callable, Dict, List, Optional, Tuple, Union, cast
 
 from flwr.common import EvaluateRes, Scalar
 from flwr.server.client_proxy import ClientProxy
 from flwr.server.strategy import Strategy
 
-TBW = TypeVar("TBW")
+try:
+    import tensorflow as tf
+except ImportError:
+    tf = None
 
 
-def tensorboard(logdir: str) -> Callable[[Strategy], TBW]:
+def tensorboard(logdir: str) -> Callable[[Strategy], Strategy]:
     """TensorBoard logger for Flower strategies.
 
     It will log loss, num_examples and all metrics which are of type float or int.
 
     This can either be used as a decorator as shown in the example variant 1
     or directly as shown in the example variant 2.
 
@@ -67,15 +65,15 @@
                 if os.path.isdir(os.path.join(logdir, name))
             ]
         )
     )
     run_id = run_id + "-" + datetime.now().strftime("%Y%m%dT%H%M%S")
     logdir_run = os.path.join(logdir, run_id)
 
-    def decorator(strategy_class: Strategy) -> TBW:
+    def decorator(strategy_class: Strategy) -> Strategy:
         """Return overloaded Strategy Wrapper."""
 
         class TBWrapper(strategy_class):  # type: ignore
             """Strategy wrapper which hooks into some methods for TensorBoard
             logging."""
 
             def aggregate_evaluate(
@@ -132,10 +130,10 @@
                             for key, value in metrics.items():
                                 if type(value) in [int, float]:
                                     tf.summary.scalar(f"clients/{key}", value)
                         writer.flush()
 
                 return loss_aggregated, config
 
-        return cast(TBW, TBWrapper)
+        return cast(Strategy, TBWrapper)
 
     return decorator
```

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/simulation/app.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.5.0.dev20230608/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230529/setup.py` & `flwr_nightly-1.5.0.dev20230608/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 {'console_scripts': ['flower-client = flwr.client:run_client',
                      'flower-driver-api = flwr.server:run_driver_api',
                      'flower-fleet-api = flwr.server:run_fleet_api',
                      'flower-server = flwr.server:run_server']}
 
 setup_kwargs = {
     'name': 'flwr-nightly',
-    'version': '1.5.0.dev20230529',
+    'version': '1.5.0.dev20230608',
     'description': 'Flower: A Friendly Federated Learning Framework',
     'long_description': '# Flower: A Friendly Federated Learning Framework\n\n<p align="center">\n  <a href="https://flower.dev/">\n    <img src="https://flower.dev/_next/image/?url=%2F_next%2Fstatic%2Fmedia%2Fflower_white_border.c2012e70.png&w=640&q=75" width="140px" alt="Flower Website" />\n  </a>\n</p>\n<p align="center">\n    <a href="https://flower.dev/">Website</a> |\n    <a href="https://flower.dev/blog">Blog</a> |\n    <a href="https://flower.dev/docs/">Docs</a> |\n    <a href="https://flower.dev/conf/flower-summit-2022">Conference</a> |\n    <a href="https://flower.dev/join-slack">Slack</a>\n    <br /><br />\n</p>\n\n[![GitHub license](https://img.shields.io/github/license/adap/flower)](https://github.com/adap/flower/blob/main/LICENSE)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/flower/blob/main/CONTRIBUTING.md)\n![Build](https://github.com/adap/flower/actions/workflows/flower.yml/badge.svg)\n![Downloads](https://pepy.tech/badge/flwr)\n[![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack)\n\nFlower (`flwr`) is a framework for building federated learning systems. The\ndesign of Flower is based on a few guiding principles:\n\n* **Customizable**: Federated learning systems vary wildly from one use case to\n  another. Flower allows for a wide range of different configurations depending\n  on the needs of each individual use case.\n\n* **Extendable**: Flower originated from a research project at the University of\n  Oxford, so it was built with AI research in mind. Many components can be\n  extended and overridden to build new state-of-the-art systems.\n\n* **Framework-agnostic**: Different machine learning frameworks have different\n  strengths. Flower can be used with any machine learning framework, for\n  example, [PyTorch](https://pytorch.org),\n  [TensorFlow](https://tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch Lightning](https://pytorchlightning.ai/), [MXNet](https://mxnet.apache.org/), [scikit-learn](https://scikit-learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://tensorflow.org/lite/), [fastai](https://www.fast.ai/), [Pandas](https://pandas.pydata.org/\n) for federated analytics, or even raw [NumPy](https://numpy.org/)\n  for users who enjoy computing gradients by hand.\n\n* **Understandable**: Flower is written with maintainability in mind. The\n  community is encouraged to both read and contribute to the codebase.\n\nMeet the Flower community on [flower.dev](https://flower.dev)!\n\n## Federated Learning Tutorial\n\nFlower\'s goal is to make federated learning accessible to everyone. This series of tutorials introduces the fundamentals of federated learning and how to implement them in Flower.\n\n0. **What is Federated Learning?**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb))\n\n1. **An Introduction to Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb))\n\n2. **Using Strategies in Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb))\n   \n3. **Building Strategies for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb))\n   \n4. **Custom Clients for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb))\n\nStay tuned, more tutorials are coming soon. Topics include **Privacy and Security in Federated Learning**, and **Scaling Federated Learning**.\n\n## Documentation\n\n[Flower Docs](https://flower.dev/docs):\n* [Installation](https://flower.dev/docs/installation.html)\n* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)\n* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html)\n* [Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-huggingface.html)\n* [Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/quickstart-pytorch-lightning.html)\n* [Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-through.html)\n* [Quickstart (Pandas)](https://flower.dev/docs/quickstart-pandas.html)\n* [Quickstart (fastai)](https://flower.dev/docs/quickstart-fastai.html)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android [code example])](https://github.com/adap/flower/tree/main/examples/android)\n* [Quickstart (iOS)](https://flower.dev/docs/quickstart-ios.html)\n\n## Flower Baselines\n\nFlower Baselines is a collection of community-contributed experiments that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas:\n\n* [FedAvg](https://arxiv.org/abs/1602.05629):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedavg_mnist)\n* [FedProx](https://arxiv.org/abs/1812.06127):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedprox_mnist)\n* [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/abs/2102.07623):\n  * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/convergence_rate)\n* [Adaptive Federated Optimization](https://arxiv.org/abs/2003.00295):\n  * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/adaptive_federated_optimization)\n\nCheck the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html)\n\nThe Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/contributing-baselines.html)\n\n## Flower Usage Examples\n\nSeveral code examples show different usage scenarios of Flower (in combination with popular machine learning frameworks such as PyTorch or TensorFlow).\n\nQuickstart examples:\n\n* [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/examples/quickstart_tensorflow)\n* [Quickstart (PyTorch)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch)\n* [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/main/examples/quickstart_huggingface)\n* [Quickstart (PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch_lightning)\n* [Quickstart (fastai)](https://github.com/adap/flower/tree/main/examples/quickstart_fastai)\n* [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/quickstart_pandas)\n* [Quickstart (MXNet)](https://github.com/adap/flower/tree/main/examples/quickstart_mxnet)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android)](https://github.com/adap/flower/tree/main/examples/android)\n\nOther [examples](https://github.com/adap/flower/tree/main/examples):\n\n* [Raspberry Pi & Nvidia Jetson Tutorial](https://github.com/adap/flower/tree/main/examples/embedded_devices)\n* [Android & TFLite](https://github.com/adap/flower/tree/main/examples/android)\n* [PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/pytorch_from_centralized_to_federated)\n* [MXNet: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/mxnet_from_centralized_to_federated)\n* [Advanced Flower with TensorFlow/Keras](https://github.com/adap/flower/tree/main/examples/advanced_tensorflow)\n* [Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/advanced_pytorch)\n* Single-Machine Simulation of Federated Learning Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/simulation_pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/examples/simulation_tensorflow))\n\n## Community\n\nFlower is built by a wonderful community of researchers and engineers. [Join Slack](https://flower.dev/join-slack) to meet them, [contributions](#contributing-to-flower) are welcome.\n\n<a href="https://github.com/adap/flower/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=adap/flower" />\n</a>\n\n## Citation\n\nIf you publish work that uses Flower, please cite Flower as follows: \n\n```bibtex\n@article{beutel2020flower,\n  title={Flower: A Friendly Federated Learning Research Framework},\n  author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and Kwing, Hei Li and Parcollet, Titouan and Gusmão, Pedro PB de and Lane, Nicholas D}, \n  journal={arXiv preprint arXiv:2007.14390},\n  year={2020}\n}\n```\n\nPlease also consider adding your publication to the list of Flower-based publications in the docs, just open a Pull Request.\n\n## Contributing to Flower\n\nWe welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get started!\n',
     'author': 'The Flower Authors',
     'author_email': 'hello@flower.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://flower.dev',
```

#### html2text {}

```diff
@@ -12,15 +12,15 @@
 extras_require = \ {':python_version < "3.8"': ['importlib-
 metadata>=4.0.0,<5.0.0'], 'rest': ['requests>=2.28.2,<3.0.0',
 'fastapi>=0.95.0,<0.96.0', 'starlette>=0.26.1,<0.27.0', 'uvicorn
 [standard]>=0.21.1,<0.22.0'], 'simulation': ['ray[default]>=2.4.0,<3.0.0']}
 entry_points = \ {'console_scripts': ['flower-client = flwr.client:run_client',
 'flower-driver-api = flwr.server:run_driver_api', 'flower-fleet-api =
 flwr.server:run_fleet_api', 'flower-server = flwr.server:run_server']}
-setup_kwargs = { 'name': 'flwr-nightly', 'version': '1.5.0.dev20230529',
+setup_kwargs = { 'name': 'flwr-nightly', 'version': '1.5.0.dev20230608',
 'description': 'Flower: A Friendly Federated Learning Framework',
 'long_description': '# Flower: A Friendly Federated Learning Framework\n\n
                           \n \n_[Flower_Website]\n\n
 \n
            \n Website |\n Blog |\n Docs |\n Conference |\n Slack\n
 
                                       \n
```

### Comparing `flwr_nightly-1.5.0.dev20230529/PKG-INFO` & `flwr_nightly-1.5.0.dev20230608/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.5.0.dev20230529
+Version: 1.5.0.dev20230608
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.dev
 License: Apache-2.0
 Author: The Flower Authors
 Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230529 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230608 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.dev
 License: Apache-2.0 Author: The Flower Authors Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
```

