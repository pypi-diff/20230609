# Comparing `tmp/fractal_toolkit-4.0.0.tar.gz` & `tmp/fractal_toolkit-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_toolkit-4.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fractal_toolkit-4.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fractal_toolkit-4.0.0.tar` & `fractal_toolkit-4.0.1.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0        0        0      187 2023-06-08 07:52:00.656143 fractal_toolkit-4.0.0/.coveragerc
--rw-r--r--   0        0        0      100 2023-06-08 07:52:00.656143 fractal_toolkit-4.0.0/.flake8
--rw-r--r--   0        0        0      943 2023-06-08 07:52:00.656143 fractal_toolkit-4.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-06-08 07:52:00.656143 fractal_toolkit-4.0.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-06-08 07:52:00.656143 fractal_toolkit-4.0.0/.gitignore
--rw-r--r--   0        0        0      161 2023-06-08 07:52:00.656143 fractal_toolkit-4.0.0/.isort.cfg
--rw-r--r--   0        0        0     1964 2023-06-08 07:52:00.656143 fractal_toolkit-4.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1062 2023-06-08 07:52:00.656143 fractal_toolkit-4.0.0/LICENSE
--rw-r--r--   0        0        0     1563 2023-06-08 07:52:00.656143 fractal_toolkit-4.0.0/Makefile
--rw-r--r--   0        0        0    15008 2023-06-08 07:52:00.656143 fractal_toolkit-4.0.0/README.md
--rw-r--r--   0        0        0      780 2023-06-08 07:52:00.656143 fractal_toolkit-4.0.0/align_version.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/examples/basic/app/adapters/__init__.py
--rw-r--r--   0        0        0      245 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/examples/basic/app/adapters/products.py
--rw-r--r--   0        0        0      701 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/examples/basic/app/context.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/examples/basic/app/domain/__init__.py
--rw-r--r--   0        0        0      317 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/examples/basic/app/domain/products.py
--rw-r--r--   0        0        0      204 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/examples/basic/app/main.py
--rw-r--r--   0        0        0      369 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/examples/basic/app/settings.py
--rw-r--r--   0        0        0      720 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/django/__init__.py
--rw-r--r--   0        0        0     1660 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/django/middleware.py
--rw-r--r--   0        0        0      778 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/django/projectors.py
--rw-r--r--   0        0        0       27 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/django/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/fastapi/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/fastapi/exceptions/__init__.py
--rw-r--r--   0        0        0       95 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/fastapi/exceptions/error_message.py
--rw-r--r--   0        0        0     2297 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/fastapi/install.py
--rw-r--r--   0        0        0       68 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/fastapi/requirements.txt
--rw-r--r--   0        0        0       48 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/fastapi/routers/__init__.py
--rw-r--r--   0        0        0     8992 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/fastapi/routers/default.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/fastapi/routers/domain/__init__.py
--rw-r--r--   0        0        0      207 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/fastapi/routers/domain/models.py
--rw-r--r--   0        0        0     2948 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/fastapi/routers/tokens.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/fastapi/utils/__init__.py
--rw-r--r--   0        0        0      298 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/fastapi/utils/json_encoder.py
--rw-r--r--   0        0        0      216 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/gcp/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/gcp/cloudstorage/__init__.py
--rw-r--r--   0        0        0     2450 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/gcp/cloudstorage/repositories.py
--rw-r--r--   0        0        0       21 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/gcp/cloudstorage/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/gcp/firestore/__init__.py
--rw-r--r--   0        0        0      328 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/gcp/firestore/event_store.py
--rw-r--r--   0        0        0       38 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/gcp/firestore/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/gcp/pubsub/__init__.py
--rw-r--r--   0        0        0     3056 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/gcp/pubsub/event_bus.py
--rw-r--r--   0        0        0     2466 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/gcp/pubsub/projectors.py
--rw-r--r--   0        0        0       20 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/gcp/pubsub/requirements.txt
--rw-r--r--   0        0        0     1192 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/kafka/README.md
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/kafka/__init__.py
--rw-r--r--   0        0        0     1293 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/kafka/docker-compose.yml
--rw-r--r--   0        0        0     2233 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/kafka/event_bus.py
--rw-r--r--   0        0        0     1670 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/kafka/projectors.py
--rw-r--r--   0        0        0       13 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/kafka/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/rabbitmq/__init__.py
--rw-r--r--   0        0        0     3176 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/rabbitmq/event_bus.py
--rw-r--r--   0        0        0     2011 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/rabbitmq/projectors.py
--rw-r--r--   0        0        0        5 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/rabbitmq/requirements.txt
--rw-r--r--   0        0        0      603 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/contrib/rabbitmq/utils.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/command_bus/__init__.py
--rw-r--r--   0        0        0       71 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/command_bus/command.py
--rw-r--r--   0        0        0     1077 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/command_bus/command_bus.py
--rw-r--r--   0        0        0      376 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/command_bus/command_handler.py
--rw-r--r--   0        0        0      657 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/command_bus/commands.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/event_sourcing/__init__.py
--rw-r--r--   0        0        0      982 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/event_sourcing/event.py
--rw-r--r--   0        0        0       52 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/event_sourcing/event_bus.py
--rw-r--r--   0        0        0      297 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/event_sourcing/event_projector.py
--rw-r--r--   0        0        0      907 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/event_sourcing/event_publisher.py
--rw-r--r--   0        0        0     6447 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/event_sourcing/event_store.py
--rw-r--r--   0        0        0      303 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/event_sourcing/event_stream.py
--rw-r--r--   0        0        0      289 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/event_sourcing/message.py
--rw-r--r--   0        0        0      397 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/event_sourcing/models.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/event_sourcing/projectors/__init__.py
--rw-r--r--   0        0        0      985 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/event_sourcing/projectors/command_bus_projector.py
--rw-r--r--   0        0        0      588 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/event_sourcing/projectors/event_store_projector.py
--rw-r--r--   0        0        0      769 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/event_sourcing/projectors/print_projector.py
--rw-r--r--   0        0        0     1713 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/event_sourcing/repositories.py
--rw-r--r--   0        0        0      968 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/process/__init__.py
--rw-r--r--   0        0        0      195 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/process/action.py
--rw-r--r--   0        0        0     3752 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/process/actions/__init__.py
--rw-r--r--   0        0        0     1671 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/process/actions/control_flow.py
--rw-r--r--   0        0        0      473 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/process/process.py
--rw-r--r--   0        0        0      613 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/process/process_scope.py
--rw-r--r--   0        0        0      225 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/services/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/utils/__init__.py
--rw-r--r--   0        0        0     9665 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/utils/application_context.py
--rw-r--r--   0        0        0      411 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/utils/fractal.py
--rw-r--r--   0        0        0      636 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/utils/json_encoder.py
--rw-r--r--   0        0        0      447 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/utils/loggers.py
--rw-r--r--   0        0        0     1296 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/utils/settings.py
--rw-r--r--   0        0        0     1414 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/utils/string.py
--rw-r--r--   0        0        0      144 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/core/utils/subclasses.py
--rw-r--r--   0        0        0       77 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/fractal/py.typed
--rw-r--r--   0        0        0     1688 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/pyproject.toml
--rw-r--r--   0        0        0       69 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/setup.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/__init__.py
--rw-r--r--   0        0        0       45 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/contrib/fastapi/__init__.py
--rw-r--r--   0        0        0     2158 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/contrib/fastapi/test_routers.py
--rw-r--r--   0        0        0      451 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/contrib/fastapi/test_tokens.py
--rw-r--r--   0        0        0      392 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/contrib/fastapi/test_utils.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/core/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/core/command_bus/__init__.py
--rw-r--r--   0        0        0      844 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/core/command_bus/test_command_bus.py
--rw-r--r--   0        0        0      113 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/core/command_bus/test_command_handler.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/core/event_sourcing/__init__.py
--rw-r--r--   0        0        0      376 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/core/event_sourcing/test_event_publisher.py
--rw-r--r--   0        0        0     1675 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/core/event_sourcing/test_event_store.py
--rw-r--r--   0        0        0      294 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/core/event_sourcing/test_projectors.py
--rw-r--r--   0        0        0     1529 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/core/event_sourcing/test_repositories.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/core/services/__init__.py
--rw-r--r--   0        0        0      237 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/core/services/test_service.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/core/utils/__init__.py
--rw-r--r--   0        0        0     1638 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/core/utils/test_application_context.py
--rw-r--r--   0        0        0      850 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/core/utils/test_json_encoder.py
--rw-r--r--   0        0        0      542 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/core/utils/test_settings.py
--rw-r--r--   0        0        0      507 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/core/utils/test_string.py
--rw-r--r--   0        0        0      103 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      420 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/fixtures/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/fixtures/contrib/django/__init__.py
--rw-r--r--   0        0        0     2163 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/fixtures/contrib/fastapi.py
--rw-r--r--   0        0        0       67 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/fixtures/contrib/gcp/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/fixtures/contrib/gcp/firestore/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/fixtures/contrib/mongo/__init__.py
--rw-r--r--   0        0        0       68 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/fixtures/contrib/roles/__init__.py
--rw-r--r--   0        0        0      619 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/fixtures/contrib/roles/services.py
--rw-r--r--   0        0        0       77 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/fixtures/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     7365 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/fixtures/contrib/sqlalchemy/repositories.py
--rw-r--r--   0        0        0      203 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/fixtures/contrib/tokens/__init__.py
--rw-r--r--   0        0        0      485 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/fixtures/contrib/tokens/fractal.py
--rw-r--r--   0        0        0      195 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/fixtures/contrib/tokens/services.py
--rw-r--r--   0        0        0     1388 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/fixtures/contrib/tokens/utils.py
--rw-r--r--   0        0        0      363 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/fixtures/core/__init__.py
--rw-r--r--   0        0        0     1048 2023-06-08 07:52:00.660143 fractal_toolkit-4.0.0/tests/fixtures/core/command_bus.py
--rw-r--r--   0        0        0     3938 2023-06-08 07:52:00.664143 fractal_toolkit-4.0.0/tests/fixtures/core/event_sourcing.py
--rw-r--r--   0        0        0     1230 2023-06-08 07:52:00.664143 fractal_toolkit-4.0.0/tests/fixtures/core/fractal.py
--rw-r--r--   0        0        0     1513 2023-06-08 07:52:00.664143 fractal_toolkit-4.0.0/tests/fixtures/core/repositories.py
--rw-r--r--   0        0        0      457 2023-06-08 07:52:00.664143 fractal_toolkit-4.0.0/tests/fixtures/core/services.py
--rw-r--r--   0        0        0     1781 2023-06-08 07:52:00.664143 fractal_toolkit-4.0.0/tests/fixtures/core/utils.py
--rw-r--r--   0        0        0      645 2023-06-08 07:52:00.664143 fractal_toolkit-4.0.0/tox.ini
--rw-r--r--   0        0        0    15968 1970-01-01 00:00:00.000000 fractal_toolkit-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-06-09 06:38:52.991786 fractal_toolkit-4.0.1/.coveragerc
+-rw-r--r--   0        0        0      100 2023-06-09 06:38:52.991786 fractal_toolkit-4.0.1/.flake8
+-rw-r--r--   0        0        0      943 2023-06-09 06:38:52.991786 fractal_toolkit-4.0.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2023-06-09 06:38:52.991786 fractal_toolkit-4.0.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2023-06-09 06:38:52.991786 fractal_toolkit-4.0.1/.gitignore
+-rw-r--r--   0        0        0      161 2023-06-09 06:38:52.991786 fractal_toolkit-4.0.1/.isort.cfg
+-rw-r--r--   0        0        0     1964 2023-06-09 06:38:52.991786 fractal_toolkit-4.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1062 2023-06-09 06:38:52.991786 fractal_toolkit-4.0.1/LICENSE
+-rw-r--r--   0        0        0     1563 2023-06-09 06:38:52.991786 fractal_toolkit-4.0.1/Makefile
+-rw-r--r--   0        0        0    15008 2023-06-09 06:38:52.991786 fractal_toolkit-4.0.1/README.md
+-rw-r--r--   0        0        0      780 2023-06-09 06:38:52.991786 fractal_toolkit-4.0.1/align_version.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/examples/basic/app/adapters/__init__.py
+-rw-r--r--   0        0        0      245 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/examples/basic/app/adapters/products.py
+-rw-r--r--   0        0        0      701 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/examples/basic/app/context.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/examples/basic/app/domain/__init__.py
+-rw-r--r--   0        0        0      317 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/examples/basic/app/domain/products.py
+-rw-r--r--   0        0        0      204 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/examples/basic/app/main.py
+-rw-r--r--   0        0        0      369 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/examples/basic/app/settings.py
+-rw-r--r--   0        0        0      720 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/django/__init__.py
+-rw-r--r--   0        0        0     1660 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/django/middleware.py
+-rw-r--r--   0        0        0      778 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/django/projectors.py
+-rw-r--r--   0        0        0       27 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/django/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/fastapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/fastapi/exceptions/__init__.py
+-rw-r--r--   0        0        0       95 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/fastapi/exceptions/error_message.py
+-rw-r--r--   0        0        0     2297 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/fastapi/install.py
+-rw-r--r--   0        0        0       68 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/fastapi/requirements.txt
+-rw-r--r--   0        0        0       48 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/fastapi/routers/__init__.py
+-rw-r--r--   0        0        0     8992 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/fastapi/routers/default.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/fastapi/routers/domain/__init__.py
+-rw-r--r--   0        0        0      207 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/fastapi/routers/domain/models.py
+-rw-r--r--   0        0        0     2948 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/fastapi/routers/tokens.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/fastapi/utils/__init__.py
+-rw-r--r--   0        0        0      298 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/fastapi/utils/json_encoder.py
+-rw-r--r--   0        0        0      216 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/gcp/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/gcp/cloudstorage/__init__.py
+-rw-r--r--   0        0        0     2450 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/gcp/cloudstorage/repositories.py
+-rw-r--r--   0        0        0       21 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/gcp/cloudstorage/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/gcp/firestore/__init__.py
+-rw-r--r--   0        0        0      328 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/gcp/firestore/event_store.py
+-rw-r--r--   0        0        0       38 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/gcp/firestore/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/gcp/pubsub/__init__.py
+-rw-r--r--   0        0        0     3056 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/gcp/pubsub/event_bus.py
+-rw-r--r--   0        0        0     2466 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/gcp/pubsub/projectors.py
+-rw-r--r--   0        0        0       20 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/gcp/pubsub/requirements.txt
+-rw-r--r--   0        0        0     1192 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/kafka/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/kafka/__init__.py
+-rw-r--r--   0        0        0     1293 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/kafka/docker-compose.yml
+-rw-r--r--   0        0        0     2233 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/kafka/event_bus.py
+-rw-r--r--   0        0        0     1670 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/kafka/projectors.py
+-rw-r--r--   0        0        0       13 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/kafka/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     3176 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/rabbitmq/event_bus.py
+-rw-r--r--   0        0        0     2011 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/rabbitmq/projectors.py
+-rw-r--r--   0        0        0        5 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/rabbitmq/requirements.txt
+-rw-r--r--   0        0        0      603 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/contrib/rabbitmq/utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/command_bus/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/command_bus/command.py
+-rw-r--r--   0        0        0     1077 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/command_bus/command_bus.py
+-rw-r--r--   0        0        0      376 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/command_bus/command_handler.py
+-rw-r--r--   0        0        0      613 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/command_bus/commands.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/event_sourcing/__init__.py
+-rw-r--r--   0        0        0      982 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/event_sourcing/event.py
+-rw-r--r--   0        0        0       52 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/event_sourcing/event_bus.py
+-rw-r--r--   0        0        0      297 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/event_sourcing/event_projector.py
+-rw-r--r--   0        0        0      907 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/event_sourcing/event_publisher.py
+-rw-r--r--   0        0        0     6447 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/event_sourcing/event_store.py
+-rw-r--r--   0        0        0      303 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/event_sourcing/event_stream.py
+-rw-r--r--   0        0        0      289 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/event_sourcing/message.py
+-rw-r--r--   0        0        0      397 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/event_sourcing/models.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/event_sourcing/projectors/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/event_sourcing/projectors/command_bus_projector.py
+-rw-r--r--   0        0        0      588 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/event_sourcing/projectors/event_store_projector.py
+-rw-r--r--   0        0        0      769 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/event_sourcing/projectors/print_projector.py
+-rw-r--r--   0        0        0     1713 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/event_sourcing/repositories.py
+-rw-r--r--   0        0        0      968 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/process/__init__.py
+-rw-r--r--   0        0        0      195 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/process/action.py
+-rw-r--r--   0        0        0     3752 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/process/actions/__init__.py
+-rw-r--r--   0        0        0     1671 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/process/actions/control_flow.py
+-rw-r--r--   0        0        0      473 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/process/process.py
+-rw-r--r--   0        0        0      613 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/process/process_scope.py
+-rw-r--r--   0        0        0      225 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/utils/__init__.py
+-rw-r--r--   0        0        0     9665 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/utils/application_context.py
+-rw-r--r--   0        0        0      411 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/utils/fractal.py
+-rw-r--r--   0        0        0      636 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/utils/json_encoder.py
+-rw-r--r--   0        0        0      447 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/utils/loggers.py
+-rw-r--r--   0        0        0     1296 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/utils/settings.py
+-rw-r--r--   0        0        0     1414 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/utils/string.py
+-rw-r--r--   0        0        0      144 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/core/utils/subclasses.py
+-rw-r--r--   0        0        0       77 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/fractal/py.typed
+-rw-r--r--   0        0        0     1688 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/setup.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/__init__.py
+-rw-r--r--   0        0        0       45 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/contrib/fastapi/__init__.py
+-rw-r--r--   0        0        0     2158 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/contrib/fastapi/test_routers.py
+-rw-r--r--   0        0        0      451 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/contrib/fastapi/test_tokens.py
+-rw-r--r--   0        0        0      392 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/contrib/fastapi/test_utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/core/command_bus/__init__.py
+-rw-r--r--   0        0        0      844 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/core/command_bus/test_command_bus.py
+-rw-r--r--   0        0        0      113 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/core/command_bus/test_command_handler.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/core/event_sourcing/__init__.py
+-rw-r--r--   0        0        0      376 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/core/event_sourcing/test_event_publisher.py
+-rw-r--r--   0        0        0     1675 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/core/event_sourcing/test_event_store.py
+-rw-r--r--   0        0        0      294 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/core/event_sourcing/test_projectors.py
+-rw-r--r--   0        0        0     1529 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/core/event_sourcing/test_repositories.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/core/services/__init__.py
+-rw-r--r--   0        0        0      237 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/core/services/test_service.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/core/utils/__init__.py
+-rw-r--r--   0        0        0     1638 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/core/utils/test_application_context.py
+-rw-r--r--   0        0        0      850 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/core/utils/test_json_encoder.py
+-rw-r--r--   0        0        0      542 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/core/utils/test_settings.py
+-rw-r--r--   0        0        0      507 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/core/utils/test_string.py
+-rw-r--r--   0        0        0      103 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      420 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/contrib/django/__init__.py
+-rw-r--r--   0        0        0     2163 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/contrib/fastapi.py
+-rw-r--r--   0        0        0       67 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/contrib/gcp/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/contrib/gcp/firestore/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0       68 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/contrib/roles/__init__.py
+-rw-r--r--   0        0        0      619 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/contrib/roles/services.py
+-rw-r--r--   0        0        0       77 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     7365 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/contrib/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0      203 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/contrib/tokens/__init__.py
+-rw-r--r--   0        0        0      485 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/contrib/tokens/fractal.py
+-rw-r--r--   0        0        0      195 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/contrib/tokens/services.py
+-rw-r--r--   0        0        0     1388 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/contrib/tokens/utils.py
+-rw-r--r--   0        0        0      363 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/core/__init__.py
+-rw-r--r--   0        0        0     1048 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/core/command_bus.py
+-rw-r--r--   0        0        0     3938 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/core/event_sourcing.py
+-rw-r--r--   0        0        0     1230 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/core/fractal.py
+-rw-r--r--   0        0        0     1513 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/core/repositories.py
+-rw-r--r--   0        0        0      457 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/core/services.py
+-rw-r--r--   0        0        0     1781 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tests/fixtures/core/utils.py
+-rw-r--r--   0        0        0      645 2023-06-09 06:38:52.995786 fractal_toolkit-4.0.1/tox.ini
+-rw-r--r--   0        0        0    15968 1970-01-01 00:00:00.000000 fractal_toolkit-4.0.1/PKG-INFO
```

### Comparing `fractal_toolkit-4.0.0/.github/workflows/build.yml` & `fractal_toolkit-4.0.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/.github/workflows/publish.yml` & `fractal_toolkit-4.0.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/.gitignore` & `fractal_toolkit-4.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/.pre-commit-config.yaml` & `fractal_toolkit-4.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/LICENSE` & `fractal_toolkit-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/Makefile` & `fractal_toolkit-4.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/README.md` & `fractal_toolkit-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/align_version.py` & `fractal_toolkit-4.0.1/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/examples/basic/app/context.py` & `fractal_toolkit-4.0.1/examples/basic/app/context.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/__init__.py` & `fractal_toolkit-4.0.1/fractal/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Fractal is a scaffolding toolkit for building SOLID logic for your Python applications."""
 
-__version__ = "4.0.0"
+__version__ = "4.0.1"
 
 from abc import ABC
 
 from fractal.core.utils.application_context import ApplicationContext
 from fractal.core.utils.settings import Settings
```

### Comparing `fractal_toolkit-4.0.0/fractal/contrib/django/middleware.py` & `fractal_toolkit-4.0.1/fractal/contrib/django/middleware.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/contrib/django/projectors.py` & `fractal_toolkit-4.0.1/fractal/contrib/django/projectors.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/contrib/fastapi/install.py` & `fractal_toolkit-4.0.1/fractal/contrib/fastapi/install.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/contrib/fastapi/routers/default.py` & `fractal_toolkit-4.0.1/fractal/contrib/fastapi/routers/default.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/contrib/fastapi/routers/tokens.py` & `fractal_toolkit-4.0.1/fractal/contrib/fastapi/routers/tokens.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/contrib/gcp/cloudstorage/repositories.py` & `fractal_toolkit-4.0.1/fractal/contrib/gcp/cloudstorage/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/contrib/gcp/pubsub/event_bus.py` & `fractal_toolkit-4.0.1/fractal/contrib/gcp/pubsub/event_bus.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/contrib/gcp/pubsub/projectors.py` & `fractal_toolkit-4.0.1/fractal/contrib/gcp/pubsub/projectors.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/contrib/kafka/README.md` & `fractal_toolkit-4.0.1/fractal/contrib/kafka/README.md`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/contrib/kafka/docker-compose.yml` & `fractal_toolkit-4.0.1/fractal/contrib/kafka/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/contrib/kafka/event_bus.py` & `fractal_toolkit-4.0.1/fractal/contrib/kafka/event_bus.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/contrib/kafka/projectors.py` & `fractal_toolkit-4.0.1/fractal/contrib/kafka/projectors.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/contrib/rabbitmq/event_bus.py` & `fractal_toolkit-4.0.1/fractal/contrib/rabbitmq/event_bus.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/contrib/rabbitmq/projectors.py` & `fractal_toolkit-4.0.1/fractal/contrib/rabbitmq/projectors.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/contrib/rabbitmq/utils.py` & `fractal_toolkit-4.0.1/fractal/contrib/rabbitmq/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/core/command_bus/command_bus.py` & `fractal_toolkit-4.0.1/fractal/core/command_bus/command_bus.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/core/command_bus/commands.py` & `fractal_toolkit-4.0.1/fractal/core/command_bus/commands.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from dataclasses import dataclass
 from typing import Generic
 
-from fractal_repositories.core.entity import Entity
 from fractal_repositories.core.repositories import EntityType
 from fractal_specifications.generic.specification import Specification
 
 from fractal.core.command_bus.command import Command
 
 
 @dataclass
 class AddEntityCommand(Generic[EntityType], Command):
-    entity: Entity
+    entity: EntityType
     specification: Specification
 
 
 @dataclass
 class UpdateEntityCommand(Generic[EntityType], Command):
     id: str
-    entity: Entity
+    entity: EntityType
     specification: Specification
 
 
 @dataclass
 class DeleteEntityCommand(Generic[EntityType], Command):
     specification: Specification
```

### Comparing `fractal_toolkit-4.0.0/fractal/core/event_sourcing/event.py` & `fractal_toolkit-4.0.1/fractal/core/event_sourcing/event.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/core/event_sourcing/event_publisher.py` & `fractal_toolkit-4.0.1/fractal/core/event_sourcing/event_publisher.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/core/event_sourcing/event_store.py` & `fractal_toolkit-4.0.1/fractal/core/event_sourcing/event_store.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/core/event_sourcing/projectors/command_bus_projector.py` & `fractal_toolkit-4.0.1/fractal/core/event_sourcing/projectors/command_bus_projector.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/core/event_sourcing/projectors/event_store_projector.py` & `fractal_toolkit-4.0.1/fractal/core/event_sourcing/projectors/event_store_projector.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/core/event_sourcing/projectors/print_projector.py` & `fractal_toolkit-4.0.1/fractal/core/event_sourcing/projectors/print_projector.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/core/event_sourcing/repositories.py` & `fractal_toolkit-4.0.1/fractal/core/event_sourcing/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/core/exceptions/__init__.py` & `fractal_toolkit-4.0.1/fractal/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/core/process/actions/__init__.py` & `fractal_toolkit-4.0.1/fractal/core/process/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/core/process/actions/control_flow.py` & `fractal_toolkit-4.0.1/fractal/core/process/actions/control_flow.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/core/process/process_scope.py` & `fractal_toolkit-4.0.1/fractal/core/process/process_scope.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/core/utils/application_context.py` & `fractal_toolkit-4.0.1/fractal/core/utils/application_context.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/core/utils/json_encoder.py` & `fractal_toolkit-4.0.1/fractal/core/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/core/utils/settings.py` & `fractal_toolkit-4.0.1/fractal/core/utils/settings.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/fractal/core/utils/string.py` & `fractal_toolkit-4.0.1/fractal/core/utils/string.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/pyproject.toml` & `fractal_toolkit-4.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-toolkit"
-version = "4.0.0"
+version = "4.0.1"
 description = "Fractal is a scaffolding toolkit for building SOLID logic for your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
```

### Comparing `fractal_toolkit-4.0.0/tests/contrib/fastapi/test_routers.py` & `fractal_toolkit-4.0.1/tests/contrib/fastapi/test_routers.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/tests/core/command_bus/test_command_bus.py` & `fractal_toolkit-4.0.1/tests/core/command_bus/test_command_bus.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/tests/core/event_sourcing/test_event_store.py` & `fractal_toolkit-4.0.1/tests/core/event_sourcing/test_event_store.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/tests/core/event_sourcing/test_repositories.py` & `fractal_toolkit-4.0.1/tests/core/event_sourcing/test_repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/tests/core/utils/test_application_context.py` & `fractal_toolkit-4.0.1/tests/core/utils/test_application_context.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/tests/core/utils/test_json_encoder.py` & `fractal_toolkit-4.0.1/tests/core/utils/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/tests/core/utils/test_settings.py` & `fractal_toolkit-4.0.1/tests/core/utils/test_settings.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/tests/fixtures/contrib/fastapi.py` & `fractal_toolkit-4.0.1/tests/fixtures/contrib/fastapi.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/tests/fixtures/contrib/roles/services.py` & `fractal_toolkit-4.0.1/tests/fixtures/contrib/roles/services.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/tests/fixtures/contrib/sqlalchemy/repositories.py` & `fractal_toolkit-4.0.1/tests/fixtures/contrib/sqlalchemy/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/tests/fixtures/contrib/tokens/utils.py` & `fractal_toolkit-4.0.1/tests/fixtures/contrib/tokens/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/tests/fixtures/core/command_bus.py` & `fractal_toolkit-4.0.1/tests/fixtures/core/command_bus.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/tests/fixtures/core/event_sourcing.py` & `fractal_toolkit-4.0.1/tests/fixtures/core/event_sourcing.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/tests/fixtures/core/fractal.py` & `fractal_toolkit-4.0.1/tests/fixtures/core/fractal.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/tests/fixtures/core/repositories.py` & `fractal_toolkit-4.0.1/tests/fixtures/core/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/tests/fixtures/core/utils.py` & `fractal_toolkit-4.0.1/tests/fixtures/core/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/tox.ini` & `fractal_toolkit-4.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `fractal_toolkit-4.0.0/PKG-INFO` & `fractal_toolkit-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-toolkit
-Version: 4.0.0
+Version: 4.0.1
 Summary: Fractal is a scaffolding toolkit for building SOLID logic for your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

