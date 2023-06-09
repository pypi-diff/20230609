# Comparing `tmp/rasa-3.5.9.tar.gz` & `tmp/rasa-3.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasa-3.5.9.tar", max compression
+gzip compressed data, was "rasa-3.6.0a1.tar", max compression
```

## Comparing `rasa-3.5.9.tar` & `rasa-3.6.0a1.tar`

### file list

```diff
@@ -1,314 +1,314 @@
--rw-r--r--   0        0        0    11352 2023-05-22 07:56:09.620166 rasa-3.5.9/LICENSE.txt
--rw-r--r--   0        0        0    20451 2023-05-22 07:56:09.620166 rasa-3.5.9/README.md
--rw-r--r--   0        0        0     8933 2023-05-22 07:56:09.780168 rasa-3.5.9/pyproject.toml
--rw-r--r--   0        0        0      280 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/__init__.py
--rw-r--r--   0        0        0     5188 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/__main__.py
--rw-r--r--   0        0        0     5314 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/api.py
--rw-r--r--   0        0        0      115 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/arguments/__init__.py
--rw-r--r--   0        0        0     2388 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/arguments/data.py
--rw-r--r--   0        0        0     5242 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/arguments/default_arguments.py
--rw-r--r--   0        0        0     2199 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/arguments/evaluate.py
--rw-r--r--   0        0        0     1499 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/arguments/export.py
--rw-r--r--   0        0        0     2685 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/arguments/interactive.py
--rw-r--r--   0        0        0     5674 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/arguments/run.py
--rw-r--r--   0        0        0      367 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/arguments/shell.py
--rw-r--r--   0        0        0     6853 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/arguments/test.py
--rw-r--r--   0        0        0     7355 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/arguments/train.py
--rw-r--r--   0        0        0      861 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/arguments/visualize.py
--rw-r--r--   0        0        0     1027 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/arguments/x.py
--rw-r--r--   0        0        0     8906 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/data.py
--rw-r--r--   0        0        0     7948 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/evaluate.py
--rw-r--r--   0        0        0     8204 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/export.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/initial_project/actions/__init__.py
--rw-r--r--   0        0        0      742 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/initial_project/actions/actions.py
--rw-r--r--   0        0        0     1505 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/initial_project/config.yml
--rw-r--r--   0        0        0      998 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/initial_project/credentials.yml
--rw-r--r--   0        0        0     1433 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/initial_project/data/nlu.yml
--rw-r--r--   0        0        0      244 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/initial_project/data/rules.yml
--rw-r--r--   0        0        0      542 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/initial_project/data/stories.yml
--rw-r--r--   0        0        0      565 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/initial_project/domain.yml
--rw-r--r--   0        0        0     1411 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/initial_project/endpoints.yml
--rw-r--r--   0        0        0     1664 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/initial_project/tests/test_stories.yml
--rw-r--r--   0        0        0     5827 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/interactive.py
--rw-r--r--   0        0        0     4196 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/run.py
--rw-r--r--   0        0        0     6846 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/scaffold.py
--rw-r--r--   0        0        0     4264 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/shell.py
--rw-r--r--   0        0        0     3118 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/telemetry.py
--rw-r--r--   0        0        0     8888 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/test.py
--rw-r--r--   0        0        0     6871 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/train.py
--rw-r--r--   0        0        0     9670 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/utils.py
--rw-r--r--   0        0        0     1256 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/visualize.py
--rw-r--r--   0        0        0     6785 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/cli/x.py
--rw-r--r--   0        0        0     1172 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/constants.py
--rw-r--r--   0        0        0      123 2023-05-22 07:56:09.780168 rasa-3.5.9/rasa/core/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/actions/__init__.py
--rw-r--r--   0        0        0    45519 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/actions/action.py
--rw-r--r--   0        0        0       78 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/actions/constants.py
--rw-r--r--   0        0        0    25982 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/actions/forms.py
--rw-r--r--   0        0        0     3322 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/actions/loops.py
--rw-r--r--   0        0        0     6078 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/actions/two_stage_fallback.py
--rw-r--r--   0        0        0    20361 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/agent.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/brokers/__init__.py
--rw-r--r--   0        0        0     4398 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/brokers/broker.py
--rw-r--r--   0        0        0     1801 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/brokers/file.py
--rw-r--r--   0        0        0    11870 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/brokers/kafka.py
--rw-r--r--   0        0        0    14045 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/brokers/pika.py
--rw-r--r--   0        0        0     2754 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/brokers/sql.py
--rw-r--r--   0        0        0     1656 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/channels/__init__.py
--rw-r--r--   0        0        0    11686 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/channels/botframework.py
--rw-r--r--   0        0        0     2746 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/channels/callback.py
--rw-r--r--   0        0        0    13331 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/channels/channel.py
--rw-r--r--   0        0        0     8073 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/channels/console.py
--rw-r--r--   0        0        0    15789 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/channels/facebook.py
--rw-r--r--   0        0        0    11532 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/channels/hangouts.py
--rw-r--r--   0        0        0     7743 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/channels/mattermost.py
--rw-r--r--   0        0        0     4814 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/channels/rasa_chat.py
--rw-r--r--   0        0        0     6937 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/channels/rest.py
--rw-r--r--   0        0        0     5999 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/channels/rocketchat.py
--rw-r--r--   0        0        0    24405 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/channels/slack.py
--rw-r--r--   0        0        0    10163 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/channels/socketio.py
--rw-r--r--   0        0        0    10630 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/channels/telegram.py
--rw-r--r--   0        0        0     5389 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/channels/twilio.py
--rw-r--r--   0        0        0    13181 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/channels/twilio_voice.py
--rw-r--r--   0        0        0     4845 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/channels/webexteams.py
--rw-r--r--   0        0        0     3047 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/constants.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/evaluation/__init__.py
--rw-r--r--   0        0        0     9154 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/evaluation/marker.py
--rw-r--r--   0        0        0    36811 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/evaluation/marker_base.py
--rw-r--r--   0        0        0    12086 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/evaluation/marker_stats.py
--rw-r--r--   0        0        0     3658 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/evaluation/marker_tracker_loader.py
--rw-r--r--   0        0        0      901 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/exceptions.py
--rw-r--r--   0        0        0    10220 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/exporter.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/featurizers/__init__.py
--rw-r--r--   0        0        0    17964 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/featurizers/precomputation.py
--rw-r--r--   0        0        0    15447 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/featurizers/single_state_featurizer.py
--rw-r--r--   0        0        0    43363 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/featurizers/tracker_featurizers.py
--rw-r--r--   0        0        0     2906 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/http_interpreter.py
--rw-r--r--   0        0        0     2018 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/jobs.py
--rw-r--r--   0        0        0     4719 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/lock.py
--rw-r--r--   0        0        0    11678 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/lock_store.py
--rw-r--r--   0        0        0    14821 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/migrate.py
--rw-r--r--   0        0        0      240 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/nlg/__init__.py
--rw-r--r--   0        0        0     3745 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/nlg/callback.py
--rw-r--r--   0        0        0     3285 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/nlg/generator.py
--rw-r--r--   0        0        0     2794 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/nlg/interpolator.py
--rw-r--r--   0        0        0     7503 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/nlg/response.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/policies/__init__.py
--rw-r--r--   0        0        0    12959 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/policies/ensemble.py
--rw-r--r--   0        0        0    19062 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/policies/memoization.py
--rw-r--r--   0        0        0    25038 2023-05-22 07:56:09.784168 rasa-3.5.9/rasa/core/policies/policy.py
--rw-r--r--   0        0        0    50189 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/core/policies/rule_policy.py
--rw-r--r--   0        0        0    86521 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/core/policies/ted_policy.py
--rw-r--r--   0        0        0    39329 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/core/policies/unexpected_intent_policy.py
--rw-r--r--   0        0        0    39091 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/core/processor.py
--rw-r--r--   0        0        0     9150 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/core/run.py
--rw-r--r--   0        0        0    48935 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/core/test.py
--rw-r--r--   0        0        0    58298 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/core/tracker_store.py
--rw-r--r--   0        0        0     3543 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/core/train.py
--rw-r--r--   0        0        0     3218 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/core/training/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/core/training/converters/__init__.py
--rw-r--r--   0        0        0     3889 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/core/training/converters/responses_prefix_converter.py
--rw-r--r--   0        0        0    59595 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/core/training/interactive.py
--rw-r--r--   0        0        0    13604 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/core/training/story_conflict.py
--rw-r--r--   0        0        0     3067 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/core/training/training.py
--rw-r--r--   0        0        0    10782 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/core/utils.py
--rw-r--r--   0        0        0     2125 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/core/visualize.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/__init__.py
--rw-r--r--   0        0        0    16744 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/caching.py
--rw-r--r--   0        0        0      469 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/constants.py
--rw-r--r--   0        0        0      437 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/exceptions.py
--rw-r--r--   0        0        0    22059 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/graph.py
--rw-r--r--   0        0        0     1384 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/loader.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/recipes/__init__.py
--rw-r--r--   0        0        0     1139 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/recipes/config_files/default_config.yml
--rw-r--r--   0        0        0     3244 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/recipes/default_components.py
--rw-r--r--   0        0        0    42860 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/recipes/default_recipe.py
--rw-r--r--   0        0        0     3260 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/recipes/graph_recipe.py
--rw-r--r--   0        0        0     3354 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/recipes/recipe.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/runner/__init__.py
--rw-r--r--   0        0        0     4302 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/runner/dask.py
--rw-r--r--   0        0        0     1672 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/runner/interface.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/storage/__init__.py
--rw-r--r--   0        0        0     9534 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/storage/local_model_storage.py
--rw-r--r--   0        0        0     3931 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/storage/resource.py
--rw-r--r--   0        0        0     6739 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/storage/storage.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/training/__init__.py
--rw-r--r--   0        0        0     6524 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/training/components.py
--rw-r--r--   0        0        0     1848 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/training/fingerprinting.py
--rw-r--r--   0        0        0    10516 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/training/graph_trainer.py
--rw-r--r--   0        0        0     5036 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/training/hooks.py
--rw-r--r--   0        0        0    22639 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/engine/validation.py
--rw-r--r--   0        0        0     2132 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/graph_components/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/graph_components/converters/__init__.py
--rw-r--r--   0        0        0     1576 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/graph_components/converters/nlu_message_converter.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/graph_components/providers/__init__.py
--rw-r--r--   0        0        0     3832 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/graph_components/providers/domain_for_core_training_provider.py
--rw-r--r--   0        0        0     2571 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/graph_components/providers/domain_provider.py
--rw-r--r--   0        0        0     1294 2023-05-22 07:56:09.788168 rasa-3.5.9/rasa/graph_components/providers/forms_provider.py
--rw-r--r--   0        0        0     2119 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/graph_components/providers/nlu_training_data_provider.py
--rw-r--r--   0        0        0     1354 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/graph_components/providers/responses_provider.py
--rw-r--r--   0        0        0     1540 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/graph_components/providers/rule_only_provider.py
--rw-r--r--   0        0        0     1466 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/graph_components/providers/story_graph_provider.py
--rw-r--r--   0        0        0     1965 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/graph_components/providers/training_tracker_provider.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/graph_components/validators/__init__.py
--rw-r--r--   0        0        0    22668 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/graph_components/validators/default_recipe_validator.py
--rw-r--r--   0        0        0    12863 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/graph_components/validators/finetuning_validator.py
--rw-r--r--   0        0        0     1782 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/jupyter.py
--rw-r--r--   0        0        0      101 2023-05-22 07:56:26.992457 rasa-3.5.9/rasa/keys
--rw-r--r--   0        0        0     3490 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/model.py
--rw-r--r--   0        0        0    14961 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/model_testing.py
--rw-r--r--   0        0        0    16760 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/model_training.py
--rw-r--r--   0        0        0      123 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/__init__.py
--rw-r--r--   0        0        0      118 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/classifiers/__init__.py
--rw-r--r--   0        0        0      133 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/classifiers/classifier.py
--rw-r--r--   0        0        0    71640 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/classifiers/diet_classifier.py
--rw-r--r--   0        0        0     7150 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/classifiers/fallback_classifier.py
--rw-r--r--   0        0        0     7581 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/classifiers/keyword_intent_classifier.py
--rw-r--r--   0        0        0     7568 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/classifiers/logistic_regression_classifier.py
--rw-r--r--   0        0        0     5559 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/classifiers/mitie_intent_classifier.py
--rw-r--r--   0        0        0     1989 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/classifiers/regex_message_handler.py
--rw-r--r--   0        0        0    11915 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/classifiers/sklearn_intent_classifier.py
--rw-r--r--   0        0        0     2757 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/constants.py
--rw-r--r--   0        0        0     1317 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/convert.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/emulators/__init__.py
--rw-r--r--   0        0        0     1748 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/emulators/dialogflow.py
--rw-r--r--   0        0        0     1367 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/emulators/emulator.py
--rw-r--r--   0        0        0     3032 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/emulators/luis.py
--rw-r--r--   0        0        0      334 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/emulators/no_emulator.py
--rw-r--r--   0        0        0     1930 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/emulators/wit.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/extractors/__init__.py
--rw-r--r--   0        0        0    26499 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/extractors/crf_entity_extractor.py
--rw-r--r--   0        0        0     7685 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/extractors/duckling_entity_extractor.py
--rw-r--r--   0        0        0     7160 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/extractors/entity_synonyms.py
--rw-r--r--   0        0        0    17530 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/extractors/extractor.py
--rw-r--r--   0        0        0    10973 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/extractors/mitie_entity_extractor.py
--rw-r--r--   0        0        0     8289 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/extractors/regex_entity_extractor.py
--rw-r--r--   0        0        0     3366 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/extractors/spacy_entity_extractor.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/featurizers/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/featurizers/dense_featurizer/__init__.py
--rw-r--r--   0        0        0    17142 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py
--rw-r--r--   0        0        0     2433 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py
--rw-r--r--   0        0        0    30361 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py
--rw-r--r--   0        0        0     5861 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py
--rw-r--r--   0        0        0     4888 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py
--rw-r--r--   0        0        0     3347 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/featurizers/featurizer.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/featurizers/sparse_featurizer/__init__.py
--rw-r--r--   0        0        0    33295 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py
--rw-r--r--   0        0        0    21810 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py
--rw-r--r--   0        0        0    10289 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py
--rw-r--r--   0        0        0      220 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/featurizers/sparse_featurizer/sparse_featurizer.py
--rw-r--r--   0        0        0      557 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/model.py
--rw-r--r--   0        0        0     8333 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/persistor.py
--rw-r--r--   0        0        0      803 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/run.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/selectors/__init__.py
--rw-r--r--   0        0        0    39012 2023-05-22 07:56:09.792168 rasa-3.5.9/rasa/nlu/selectors/response_selector.py
--rw-r--r--   0        0        0    66681 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/nlu/test.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/nlu/tokenizers/__init__.py
--rw-r--r--   0        0        0     5276 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/nlu/tokenizers/jieba_tokenizer.py
--rw-r--r--   0        0        0     2520 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/nlu/tokenizers/mitie_tokenizer.py
--rw-r--r--   0        0        0     2280 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/nlu/tokenizers/spacy_tokenizer.py
--rw-r--r--   0        0        0     7655 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/nlu/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     3652 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/nlu/tokenizers/whitespace_tokenizer.py
--rw-r--r--   0        0        0      928 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/nlu/utils/__init__.py
--rw-r--r--   0        0        0    14703 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/nlu/utils/bilou_utils.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/nlu/utils/hugging_face/__init__.py
--rw-r--r--   0        0        0     3380 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/nlu/utils/hugging_face/registry.py
--rw-r--r--   0        0        0     9143 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py
--rw-r--r--   0        0        0     3887 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/nlu/utils/mitie_utils.py
--rw-r--r--   0        0        0     5386 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/nlu/utils/pattern_utils.py
--rw-r--r--   0        0        0    11795 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/nlu/utils/spacy_utils.py
--rw-r--r--   0        0        0     2241 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/plugin.py
--rw-r--r--   0        0        0    55529 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/server.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/__init__.py
--rw-r--r--   0        0        0     4294 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/constants.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/__init__.py
--rw-r--r--   0        0        0     4346 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/constants.py
--rw-r--r--   0        0        0     1366 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/conversation.py
--rw-r--r--   0        0        0    75018 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/domain.py
--rw-r--r--   0        0        0    65833 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/events.py
--rw-r--r--   0        0        0    35597 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/generator.py
--rw-r--r--   0        0        0     8286 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/slot_mappings.py
--rw-r--r--   0        0        0    16371 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/slots.py
--rw-r--r--   0        0        0    33176 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/trackers.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/training_data/__init__.py
--rw-r--r--   0        0        0     2895 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/training_data/loading.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/training_data/story_reader/__init__.py
--rw-r--r--   0        0        0     4449 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/training_data/story_reader/story_reader.py
--rw-r--r--   0        0        0     6671 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/training_data/story_reader/story_step_builder.py
--rw-r--r--   0        0        0    32873 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/training_data/story_reader/yaml_story_reader.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/training_data/story_writer/__init__.py
--rw-r--r--   0        0        0     2543 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/training_data/story_writer/story_writer.py
--rw-r--r--   0        0        0    14903 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/training_data/story_writer/yaml_story_writer.py
--rw-r--r--   0        0        0    29313 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/training_data/structures.py
--rw-r--r--   0        0        0     3500 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/training_data/visualization.html
--rw-r--r--   0        0        0    20341 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/core/training_data/visualization.py
--rw-r--r--   0        0        0     5479 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/data.py
--rw-r--r--   0        0        0     3633 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/importers/__init__.py
--rw-r--r--   0        0        0    21555 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/importers/importer.py
--rw-r--r--   0        0        0     7836 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/importers/multi_project.py
--rw-r--r--   0        0        0     3388 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/importers/rasa.py
--rw-r--r--   0        0        0      861 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/importers/utils.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/nlu/__init__.py
--rw-r--r--   0        0        0     1388 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/nlu/constants.py
--rw-r--r--   0        0        0      188 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/nlu/interpreter.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.796168 rasa-3.5.9/rasa/shared/nlu/training_data/__init__.py
--rw-r--r--   0        0        0     6759 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/entities_parser.py
--rw-r--r--   0        0        0    14835 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/features.py
--rw-r--r--   0        0        0      453 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/formats/__init__.py
--rw-r--r--   0        0        0     6123 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/formats/dialogflow.py
--rw-r--r--   0        0        0     3014 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/formats/luis.py
--rw-r--r--   0        0        0     4495 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/formats/rasa.py
--rw-r--r--   0        0        0    22353 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/formats/rasa_yaml.py
--rw-r--r--   0        0        0     8540 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/formats/readerwriter.py
--rw-r--r--   0        0        0     1820 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/formats/wit.py
--rw-r--r--   0        0        0     4258 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/loading.py
--rw-r--r--   0        0        0     1116 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/lookup_tables_parser.py
--rw-r--r--   0        0        0    16662 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/message.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/schemas/__init__.py
--rw-r--r--   0        0        0     2565 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/schemas/data_schema.py
--rw-r--r--   0        0        0     1179 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/schemas/nlu.yml
--rw-r--r--   0        0        0     1595 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/schemas/responses.yml
--rw-r--r--   0        0        0     1476 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/synonyms_parser.py
--rw-r--r--   0        0        0    28493 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/training_data.py
--rw-r--r--   0        0        0     7040 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/nlu/training_data/util.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/utils/__init__.py
--rw-r--r--   0        0        0     1225 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/utils/cli.py
--rw-r--r--   0        0        0     8731 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/utils/common.py
--rw-r--r--   0        0        0    20533 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/utils/io.py
--rw-r--r--   0        0        0      883 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/utils/pykwalify_extensions.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/utils/schemas/__init__.py
--rw-r--r--   0        0        0       27 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/utils/schemas/config.yml
--rw-r--r--   0        0        0     3267 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/utils/schemas/domain.yml
--rw-r--r--   0        0        0     5569 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/utils/schemas/events.py
--rw-r--r--   0        0        0      779 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/utils/schemas/model_config.yml
--rw-r--r--   0        0        0     4034 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/utils/schemas/stories.yml
--rw-r--r--   0        0        0    10178 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/shared/utils/validation.py
--rw-r--r--   0        0        0    36084 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/telemetry.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/__init__.py
--rw-r--r--   0        0        0    19852 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/common.py
--rw-r--r--   0        0        0     1647 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/converter.py
--rw-r--r--   0        0        0     8796 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/endpoints.py
--rw-r--r--   0        0        0     7831 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/io.py
--rw-r--r--   0        0        0    12246 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/plotting.py
--rw-r--r--   0        0        0        0 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/tensorflow/__init__.py
--rw-r--r--   0        0        0     4036 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/tensorflow/callback.py
--rw-r--r--   0        0        0     3140 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/tensorflow/constants.py
--rw-r--r--   0        0        0     9020 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/tensorflow/crf.py
--rw-r--r--   0        0        0    15526 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/tensorflow/data_generator.py
--rw-r--r--   0        0        0     5576 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/tensorflow/environment.py
--rw-r--r--   0        0        0      168 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/tensorflow/exceptions.py
--rw-r--r--   0        0        0    59313 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/tensorflow/layers.py
--rw-r--r--   0        0        0     3319 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/tensorflow/layers_utils.py
--rw-r--r--   0        0        0    34572 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/tensorflow/model_data.py
--rw-r--r--   0        0        0    18667 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/tensorflow/model_data_utils.py
--rw-r--r--   0        0        0    36004 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/tensorflow/models.py
--rw-r--r--   0        0        0    49066 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/tensorflow/rasa_layers.py
--rw-r--r--   0        0        0    25509 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/tensorflow/transformer.py
--rw-r--r--   0        0        0      204 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/tensorflow/types.py
--rw-r--r--   0        0        0    20984 2023-05-22 07:56:09.800168 rasa-3.5.9/rasa/utils/train_utils.py
--rw-r--r--   0        0        0    17708 2023-05-22 07:56:09.804168 rasa-3.5.9/rasa/validator.py
--rw-r--r--   0        0        0      116 2023-05-22 07:56:09.804168 rasa-3.5.9/rasa/version.py
--rw-r--r--   0        0        0    26607 1970-01-01 00:00:00.000000 rasa-3.5.9/PKG-INFO
+-rw-r--r--   0        0        0    11352 2023-05-19 14:34:46.563489 rasa-3.6.0a1/LICENSE.txt
+-rw-r--r--   0        0        0    21489 2023-05-19 14:34:46.563489 rasa-3.6.0a1/README.md
+-rw-r--r--   0        0        0     9471 2023-05-19 14:34:46.751494 rasa-3.6.0a1/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/__init__.py
+-rw-r--r--   0        0        0     5188 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/__main__.py
+-rw-r--r--   0        0        0     5314 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/api.py
+-rw-r--r--   0        0        0      115 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/__init__.py
+-rw-r--r--   0        0        0     2388 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/data.py
+-rw-r--r--   0        0        0     5242 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/default_arguments.py
+-rw-r--r--   0        0        0     2199 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/evaluate.py
+-rw-r--r--   0        0        0     1499 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/export.py
+-rw-r--r--   0        0        0     2685 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/interactive.py
+-rw-r--r--   0        0        0     5674 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/run.py
+-rw-r--r--   0        0        0      367 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/shell.py
+-rw-r--r--   0        0        0     6853 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/test.py
+-rw-r--r--   0        0        0     8279 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/train.py
+-rw-r--r--   0        0        0      861 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/visualize.py
+-rw-r--r--   0        0        0     1027 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/arguments/x.py
+-rw-r--r--   0        0        0     9506 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/data.py
+-rw-r--r--   0        0        0     7948 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/evaluate.py
+-rw-r--r--   0        0        0     8204 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/export.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/actions/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/actions/actions.py
+-rw-r--r--   0        0        0     1505 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/config.yml
+-rw-r--r--   0        0        0      998 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/credentials.yml
+-rw-r--r--   0        0        0     1433 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/data/nlu.yml
+-rw-r--r--   0        0        0      244 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/data/rules.yml
+-rw-r--r--   0        0        0      542 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/data/stories.yml
+-rw-r--r--   0        0        0      565 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/domain.yml
+-rw-r--r--   0        0        0     1411 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/endpoints.yml
+-rw-r--r--   0        0        0     1664 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/initial_project/tests/test_stories.yml
+-rw-r--r--   0        0        0     5943 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/interactive.py
+-rw-r--r--   0        0        0     4196 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/run.py
+-rw-r--r--   0        0        0     6846 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/scaffold.py
+-rw-r--r--   0        0        0     4264 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/shell.py
+-rw-r--r--   0        0        0     3118 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/telemetry.py
+-rw-r--r--   0        0        0     8888 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/test.py
+-rw-r--r--   0        0        0     7798 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/train.py
+-rw-r--r--   0        0        0    11981 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/utils.py
+-rw-r--r--   0        0        0     1256 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/visualize.py
+-rw-r--r--   0        0        0     6785 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/cli/x.py
+-rw-r--r--   0        0        0     1172 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/constants.py
+-rw-r--r--   0        0        0      123 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/actions/__init__.py
+-rw-r--r--   0        0        0    45908 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/actions/action.py
+-rw-r--r--   0        0        0       78 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/actions/constants.py
+-rw-r--r--   0        0        0    25982 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/actions/forms.py
+-rw-r--r--   0        0        0     3322 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/actions/loops.py
+-rw-r--r--   0        0        0     6078 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/actions/two_stage_fallback.py
+-rw-r--r--   0        0        0    20968 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/agent.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/brokers/__init__.py
+-rw-r--r--   0        0        0     4398 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/brokers/broker.py
+-rw-r--r--   0        0        0     1801 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/brokers/file.py
+-rw-r--r--   0        0        0    11870 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/brokers/kafka.py
+-rw-r--r--   0        0        0    14045 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/brokers/pika.py
+-rw-r--r--   0        0        0     2754 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/brokers/sql.py
+-rw-r--r--   0        0        0     1656 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/__init__.py
+-rw-r--r--   0        0        0    11685 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/botframework.py
+-rw-r--r--   0        0        0     2746 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/callback.py
+-rw-r--r--   0        0        0    13331 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/channel.py
+-rw-r--r--   0        0        0     8073 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/console.py
+-rw-r--r--   0        0        0    15789 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/facebook.py
+-rw-r--r--   0        0        0    11532 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/hangouts.py
+-rw-r--r--   0        0        0     7743 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/mattermost.py
+-rw-r--r--   0        0        0     4814 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/rasa_chat.py
+-rw-r--r--   0        0        0     6937 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/rest.py
+-rw-r--r--   0        0        0     5999 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/rocketchat.py
+-rw-r--r--   0        0        0    24405 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/slack.py
+-rw-r--r--   0        0        0    10163 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/socketio.py
+-rw-r--r--   0        0        0    10630 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/telegram.py
+-rw-r--r--   0        0        0     5938 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/twilio.py
+-rw-r--r--   0        0        0    13181 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/twilio_voice.py
+-rw-r--r--   0        0        0     4845 2023-05-19 14:34:46.751494 rasa-3.6.0a1/rasa/core/channels/webexteams.py
+-rw-r--r--   0        0        0     3047 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/constants.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/evaluation/__init__.py
+-rw-r--r--   0        0        0     9154 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/evaluation/marker.py
+-rw-r--r--   0        0        0    36811 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/evaluation/marker_base.py
+-rw-r--r--   0        0        0    12086 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/evaluation/marker_stats.py
+-rw-r--r--   0        0        0     3658 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/evaluation/marker_tracker_loader.py
+-rw-r--r--   0        0        0      901 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/exceptions.py
+-rw-r--r--   0        0        0    10220 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/exporter.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/featurizers/__init__.py
+-rw-r--r--   0        0        0    17964 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/featurizers/precomputation.py
+-rw-r--r--   0        0        0    15447 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/featurizers/single_state_featurizer.py
+-rw-r--r--   0        0        0    43363 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/featurizers/tracker_featurizers.py
+-rw-r--r--   0        0        0     2906 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/http_interpreter.py
+-rw-r--r--   0        0        0     2018 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/jobs.py
+-rw-r--r--   0        0        0     4719 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/lock.py
+-rw-r--r--   0        0        0    11678 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/lock_store.py
+-rw-r--r--   0        0        0    14821 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/migrate.py
+-rw-r--r--   0        0        0      240 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/nlg/__init__.py
+-rw-r--r--   0        0        0     3745 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/nlg/callback.py
+-rw-r--r--   0        0        0     3285 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/nlg/generator.py
+-rw-r--r--   0        0        0     2794 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/nlg/interpolator.py
+-rw-r--r--   0        0        0     7503 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/nlg/response.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/policies/__init__.py
+-rw-r--r--   0        0        0    12959 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/policies/ensemble.py
+-rw-r--r--   0        0        0    19062 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/policies/memoization.py
+-rw-r--r--   0        0        0    25038 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/policies/policy.py
+-rw-r--r--   0        0        0    50189 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/policies/rule_policy.py
+-rw-r--r--   0        0        0    86521 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/policies/ted_policy.py
+-rw-r--r--   0        0        0    39329 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/policies/unexpected_intent_policy.py
+-rw-r--r--   0        0        0    40540 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/processor.py
+-rw-r--r--   0        0        0     9150 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/run.py
+-rw-r--r--   0        0        0    48935 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/test.py
+-rw-r--r--   0        0        0    58040 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/tracker_store.py
+-rw-r--r--   0        0        0     3543 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/train.py
+-rw-r--r--   0        0        0     3218 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/training/converters/__init__.py
+-rw-r--r--   0        0        0     3889 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/training/converters/responses_prefix_converter.py
+-rw-r--r--   0        0        0    59595 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/training/interactive.py
+-rw-r--r--   0        0        0    13604 2023-05-19 14:34:46.755494 rasa-3.6.0a1/rasa/core/training/story_conflict.py
+-rw-r--r--   0        0        0     3067 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/core/training/training.py
+-rw-r--r--   0        0        0    11447 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/core/utils.py
+-rw-r--r--   0        0        0     2125 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/core/visualize.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/__init__.py
+-rw-r--r--   0        0        0    16744 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/caching.py
+-rw-r--r--   0        0        0      469 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/constants.py
+-rw-r--r--   0        0        0      437 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/exceptions.py
+-rw-r--r--   0        0        0    22105 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/graph.py
+-rw-r--r--   0        0        0     1384 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/loader.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/recipes/__init__.py
+-rw-r--r--   0        0        0     1139 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/recipes/config_files/default_config.yml
+-rw-r--r--   0        0        0     3244 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/recipes/default_components.py
+-rw-r--r--   0        0        0    43587 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/recipes/default_recipe.py
+-rw-r--r--   0        0        0     3301 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/recipes/graph_recipe.py
+-rw-r--r--   0        0        0     3354 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/recipes/recipe.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/runner/__init__.py
+-rw-r--r--   0        0        0     4302 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/runner/dask.py
+-rw-r--r--   0        0        0     1672 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/runner/interface.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/storage/__init__.py
+-rw-r--r--   0        0        0     9581 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/storage/local_model_storage.py
+-rw-r--r--   0        0        0     3931 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/storage/resource.py
+-rw-r--r--   0        0        0     6923 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/storage/storage.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/training/__init__.py
+-rw-r--r--   0        0        0     6524 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/training/components.py
+-rw-r--r--   0        0        0     1848 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/training/fingerprinting.py
+-rw-r--r--   0        0        0    10516 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/training/graph_trainer.py
+-rw-r--r--   0        0        0     5036 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/training/hooks.py
+-rw-r--r--   0        0        0    22697 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/engine/validation.py
+-rw-r--r--   0        0        0     2132 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/converters/__init__.py
+-rw-r--r--   0        0        0     1576 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/converters/nlu_message_converter.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/__init__.py
+-rw-r--r--   0        0        0     3832 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/domain_for_core_training_provider.py
+-rw-r--r--   0        0        0     2571 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/domain_provider.py
+-rw-r--r--   0        0        0     1294 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/forms_provider.py
+-rw-r--r--   0        0        0     2119 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/nlu_training_data_provider.py
+-rw-r--r--   0        0        0     1354 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/responses_provider.py
+-rw-r--r--   0        0        0     1540 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/rule_only_provider.py
+-rw-r--r--   0        0        0     1466 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/story_graph_provider.py
+-rw-r--r--   0        0        0     1965 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/providers/training_tracker_provider.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/validators/__init__.py
+-rw-r--r--   0        0        0    22668 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/validators/default_recipe_validator.py
+-rw-r--r--   0        0        0    12863 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/graph_components/validators/finetuning_validator.py
+-rw-r--r--   0        0        0     1782 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/jupyter.py
+-rw-r--r--   0        0        0      101 2023-05-19 14:35:05.111915 rasa-3.6.0a1/rasa/keys
+-rw-r--r--   0        0        0     3490 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/model.py
+-rw-r--r--   0        0        0    14961 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/model_testing.py
+-rw-r--r--   0        0        0    16836 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/model_training.py
+-rw-r--r--   0        0        0      123 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/__init__.py
+-rw-r--r--   0        0        0      133 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/classifier.py
+-rw-r--r--   0        0        0    71637 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/diet_classifier.py
+-rw-r--r--   0        0        0     7150 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/fallback_classifier.py
+-rw-r--r--   0        0        0     7581 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/keyword_intent_classifier.py
+-rw-r--r--   0        0        0     7568 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/logistic_regression_classifier.py
+-rw-r--r--   0        0        0     5559 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/mitie_intent_classifier.py
+-rw-r--r--   0        0        0     1989 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/regex_message_handler.py
+-rw-r--r--   0        0        0    11915 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/classifiers/sklearn_intent_classifier.py
+-rw-r--r--   0        0        0     2757 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/constants.py
+-rw-r--r--   0        0        0     1317 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/convert.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/emulators/__init__.py
+-rw-r--r--   0        0        0     1748 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/emulators/dialogflow.py
+-rw-r--r--   0        0        0     1367 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/emulators/emulator.py
+-rw-r--r--   0        0        0     3032 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/emulators/luis.py
+-rw-r--r--   0        0        0      334 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/emulators/no_emulator.py
+-rw-r--r--   0        0        0     1930 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/emulators/wit.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.759494 rasa-3.6.0a1/rasa/nlu/extractors/__init__.py
+-rw-r--r--   0        0        0    26499 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/extractors/crf_entity_extractor.py
+-rw-r--r--   0        0        0     7685 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/extractors/duckling_entity_extractor.py
+-rw-r--r--   0        0        0     7160 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/extractors/entity_synonyms.py
+-rw-r--r--   0        0        0    17530 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/extractors/extractor.py
+-rw-r--r--   0        0        0    10973 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/extractors/mitie_entity_extractor.py
+-rw-r--r--   0        0        0     8289 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/extractors/regex_entity_extractor.py
+-rw-r--r--   0        0        0     3366 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/extractors/spacy_entity_extractor.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/__init__.py
+-rw-r--r--   0        0        0    17142 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py
+-rw-r--r--   0        0        0     2433 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py
+-rw-r--r--   0        0        0    30361 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py
+-rw-r--r--   0        0        0     5861 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py
+-rw-r--r--   0        0        0     4888 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py
+-rw-r--r--   0        0        0     3347 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/featurizer.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/sparse_featurizer/__init__.py
+-rw-r--r--   0        0        0    33295 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py
+-rw-r--r--   0        0        0    21810 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py
+-rw-r--r--   0        0        0    10289 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py
+-rw-r--r--   0        0        0      220 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/featurizers/sparse_featurizer/sparse_featurizer.py
+-rw-r--r--   0        0        0      557 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/model.py
+-rw-r--r--   0        0        0     8333 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/persistor.py
+-rw-r--r--   0        0        0      803 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/run.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/selectors/__init__.py
+-rw-r--r--   0        0        0    39012 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/selectors/response_selector.py
+-rw-r--r--   0        0        0    67521 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/test.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/tokenizers/__init__.py
+-rw-r--r--   0        0        0     5374 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/tokenizers/jieba_tokenizer.py
+-rw-r--r--   0        0        0     2618 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/tokenizers/mitie_tokenizer.py
+-rw-r--r--   0        0        0     2378 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/tokenizers/spacy_tokenizer.py
+-rw-r--r--   0        0        0     8196 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     3750 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/tokenizers/whitespace_tokenizer.py
+-rw-r--r--   0        0        0      928 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/utils/__init__.py
+-rw-r--r--   0        0        0    14703 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/utils/bilou_utils.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/utils/hugging_face/__init__.py
+-rw-r--r--   0        0        0     3380 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/utils/hugging_face/registry.py
+-rw-r--r--   0        0        0     9143 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py
+-rw-r--r--   0        0        0     3887 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/utils/mitie_utils.py
+-rw-r--r--   0        0        0     5386 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/utils/pattern_utils.py
+-rw-r--r--   0        0        0    11795 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/nlu/utils/spacy_utils.py
+-rw-r--r--   0        0        0     4628 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/plugin.py
+-rw-r--r--   0        0        0    55589 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/server.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/shared/__init__.py
+-rw-r--r--   0        0        0     4294 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/shared/constants.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/shared/core/__init__.py
+-rw-r--r--   0        0        0     4346 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/shared/core/constants.py
+-rw-r--r--   0        0        0     1366 2023-05-19 14:34:46.763494 rasa-3.6.0a1/rasa/shared/core/conversation.py
+-rw-r--r--   0        0        0    75018 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/domain.py
+-rw-r--r--   0        0        0    65833 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/events.py
+-rw-r--r--   0        0        0    35597 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/generator.py
+-rw-r--r--   0        0        0     8286 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/slot_mappings.py
+-rw-r--r--   0        0        0    16371 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/slots.py
+-rw-r--r--   0        0        0    33790 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/trackers.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/__init__.py
+-rw-r--r--   0        0        0     2895 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/loading.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/story_reader/__init__.py
+-rw-r--r--   0        0        0     4449 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/story_reader/story_reader.py
+-rw-r--r--   0        0        0     6671 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/story_reader/story_step_builder.py
+-rw-r--r--   0        0        0    32873 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/story_reader/yaml_story_reader.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/story_writer/__init__.py
+-rw-r--r--   0        0        0     2543 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/story_writer/story_writer.py
+-rw-r--r--   0        0        0    14903 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/story_writer/yaml_story_writer.py
+-rw-r--r--   0        0        0    29313 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/structures.py
+-rw-r--r--   0        0        0     3500 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/visualization.html
+-rw-r--r--   0        0        0    20341 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/core/training_data/visualization.py
+-rw-r--r--   0        0        0     5479 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/data.py
+-rw-r--r--   0        0        0     3633 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/importers/__init__.py
+-rw-r--r--   0        0        0    21866 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/importers/importer.py
+-rw-r--r--   0        0        0     7836 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/importers/multi_project.py
+-rw-r--r--   0        0        0     3388 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/importers/rasa.py
+-rw-r--r--   0        0        0      861 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/importers/utils.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/__init__.py
+-rw-r--r--   0        0        0     1388 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/constants.py
+-rw-r--r--   0        0        0      188 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/interpreter.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/__init__.py
+-rw-r--r--   0        0        0     6759 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/entities_parser.py
+-rw-r--r--   0        0        0    14835 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/features.py
+-rw-r--r--   0        0        0      453 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/__init__.py
+-rw-r--r--   0        0        0     6123 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/dialogflow.py
+-rw-r--r--   0        0        0     3014 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/luis.py
+-rw-r--r--   0        0        0     4495 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/rasa.py
+-rw-r--r--   0        0        0    22353 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/rasa_yaml.py
+-rw-r--r--   0        0        0     8540 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/readerwriter.py
+-rw-r--r--   0        0        0     1820 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/wit.py
+-rw-r--r--   0        0        0     4258 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/loading.py
+-rw-r--r--   0        0        0     1116 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/lookup_tables_parser.py
+-rw-r--r--   0        0        0    16662 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/message.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/schemas/__init__.py
+-rw-r--r--   0        0        0     2565 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/schemas/data_schema.py
+-rw-r--r--   0        0        0     1179 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/schemas/nlu.yml
+-rw-r--r--   0        0        0     1595 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/schemas/responses.yml
+-rw-r--r--   0        0        0     1476 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/synonyms_parser.py
+-rw-r--r--   0        0        0    28493 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/training_data.py
+-rw-r--r--   0        0        0     7040 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/nlu/training_data/util.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/__init__.py
+-rw-r--r--   0        0        0     2078 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/cli.py
+-rw-r--r--   0        0        0     8731 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/common.py
+-rw-r--r--   0        0        0    20533 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/io.py
+-rw-r--r--   0        0        0      883 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/pykwalify_extensions.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/schemas/__init__.py
+-rw-r--r--   0        0        0       27 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/schemas/config.yml
+-rw-r--r--   0        0        0     3267 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/schemas/domain.yml
+-rw-r--r--   0        0        0     5569 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/schemas/events.py
+-rw-r--r--   0        0        0      998 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/schemas/model_config.yml
+-rw-r--r--   0        0        0     4034 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/schemas/stories.yml
+-rw-r--r--   0        0        0    10317 2023-05-19 14:34:46.767494 rasa-3.6.0a1/rasa/shared/utils/validation.py
+-rw-r--r--   0        0        0    36084 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/telemetry.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/__init__.py
+-rw-r--r--   0        0        0    19852 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/common.py
+-rw-r--r--   0        0        0     1647 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/converter.py
+-rw-r--r--   0        0        0     8796 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/endpoints.py
+-rw-r--r--   0        0        0     7831 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/io.py
+-rw-r--r--   0        0        0    12246 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/plotting.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/__init__.py
+-rw-r--r--   0        0        0     4036 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/callback.py
+-rw-r--r--   0        0        0     3140 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/constants.py
+-rw-r--r--   0        0        0     9020 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/crf.py
+-rw-r--r--   0        0        0    15526 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/data_generator.py
+-rw-r--r--   0        0        0     5576 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/environment.py
+-rw-r--r--   0        0        0      168 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/exceptions.py
+-rw-r--r--   0        0        0    59313 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/layers.py
+-rw-r--r--   0        0        0     3319 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/layers_utils.py
+-rw-r--r--   0        0        0    34572 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/model_data.py
+-rw-r--r--   0        0        0    18667 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/model_data_utils.py
+-rw-r--r--   0        0        0    36004 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/models.py
+-rw-r--r--   0        0        0    49066 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/rasa_layers.py
+-rw-r--r--   0        0        0    25509 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/transformer.py
+-rw-r--r--   0        0        0      204 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/tensorflow/types.py
+-rw-r--r--   0        0        0    20984 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/utils/train_utils.py
+-rw-r--r--   0        0        0    17708 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/validator.py
+-rw-r--r--   0        0        0      118 2023-05-19 14:34:46.771494 rasa-3.6.0a1/rasa/version.py
+-rw-r--r--   0        0        0    28015 1970-01-01 00:00:00.000000 rasa-3.6.0a1/PKG-INFO
```

### Comparing `rasa-3.5.9/LICENSE.txt` & `rasa-3.6.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/README.md` & `rasa-3.6.0a1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -122,16 +122,16 @@
 ### Managing environments
 
 The official [Poetry guide](https://python-poetry.org/docs/managing-environments/) suggests to use
 [pyenv](https://github.com/pyenv/pyenv) or any other similar tool to easily switch between Python versions.
 This is how it can be done:
 
 ```bash
-pyenv install 3.7.9
-pyenv local 3.7.9  # Activate Python 3.7.9 for the current project
+pyenv install 3.10.10
+pyenv local 3.10.10  # Activate Python 3.10.10 for the current project
 ```
 *Note*: If you have trouble installing a specific version of python on your system
 it might be worth trying other supported versions.
 
 By default, Poetry will try to use the currently activated Python version to create the virtual environment
 for the current project automatically. You can also create and activate a virtual environment manually — in this
 case, Poetry should pick it up and use it to install the dependencies. For example:
@@ -306,14 +306,15 @@
 ```
 make types
 ```
 
 ### Deploying documentation updates
 
 We use `Docusaurus v2` to build docs for tagged versions and for the `main` branch.
+To run Docusaurus, install `Node.js 12.x`.
 The static site that gets built is pushed to the `documentation` branch of this repo.
 
 We host the site on netlify. On `main` branch builds (see `.github/workflows/documentation.yml`), we push the built docs to
 the `documentation` branch. Netlify automatically re-deploys the docs pages whenever there is a change to that branch.
 
 ## Releases
 Rasa has implemented robust policies governing version naming, as well as release pace for major, minor, and patch releases.
@@ -422,20 +423,28 @@
 to add.
 2. Make sure the bugfix(es) are in the release branch you will use (p.e if you are cutting a `2.0.4` patch, you will
 need your fixes to be on the `2.0.x` release branch). All patch releases must come from a `.x` branch!
 3. Once you're ready to release the Rasa Open Source patch, checkout the branch, run `make release` and follow the
 steps + get the PR merged.
 4. Once the PR is in, pull the `.x` branch again and push the tag!
 
+### Additional Release Tasks 
+**Note: This is only required if the released version is the highest version available.
+For instance, perform the following steps when version > [version](https://github.com/RasaHQ/rasa/blob/main/rasa/version.py) on main.**
+
+In order to check compatibility between the new released Rasa version to the latest version of Rasa X/Enterprise, we perform the following steps:
+1. Following a new Rasa release, an automated pull request is created in [Rasa-X-Demo](https://github.com/RasaHQ/rasa-x-demo/pulls). 
+2. Once the above PR is merged, follow instructions [here](https://github.com/RasaHQ/rasa-x-demo/blob/master/.github/VERSION_BUMPER_PR_COMMENT.md), to release a version.
+3. Update the new version in the Rasa X/Enterprise [env file](https://github.com/RasaHQ/rasa-x/blob/main/.env).
+The [Rasa-X-Demo](https://github.com/RasaHQ/rasa-x-demo) project uses the new updated Rasa version to train and test a model which in turn is used by our CI to run tests in the Rasa X/Enterprise repository, 
+thus validating compatibility between Rasa and Rasa X/Enterprise.
+
 ### Actively maintained versions
 
-We're actively maintaining _any minor on our latest major release_ and _the latest minor of the previous major release_.
-Currently, this means the following minor versions will receive bugfixes updates:
-- 2.8
-- Every minor version on 3.x
+Please refer to the [Rasa Product Release and Maintenance Policy](https://rasa.com/rasa-product-release-and-maintenance-policy/) page.
 
 ## License
 Licensed under the Apache License, Version 2.0.
 Copyright 2022 Rasa Technologies GmbH. [Copy of the license](LICENSE.txt).
 
 A list of the Licenses of the dependencies of the project can be found at
 the bottom of the
```

### Comparing `rasa-3.5.9/pyproject.toml` & `rasa-3.6.0a1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.black]
 line-length = 88
 target-version = [ "py37", "py38", "py39", "py310",]
 exclude = "((.eggs | .git | .pytest_cache | build | dist))"
 
 [tool.poetry]
 name = "rasa"
-version = "3.5.9"
+version = "3.6.0a1"
 description = "Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants"
 authors = [ "Rasa Technologies GmbH <hi@rasa.com>",]
 maintainers = [ "Tom Bocklisch <tom@rasa.com>",]
 homepage = "https://rasa.com"
 repository = "https://github.com/rasahq/rasa"
 documentation = "https://rasa.com/docs"
 classifiers = [ "Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "License :: OSI Approved :: Apache Software License", "Topic :: Software Development :: Libraries",]
@@ -83,38 +83,39 @@
 
 [tool.ruff]
 ignore = [ "D100", "D104", "D105", "RUF001", "RUF002", "RUF003", "RUF005",]
 line-length = 88
 select = [ "D", "E", "F", "W", "RUF",]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.11"
-boto3 = "^1.12"
+python = ">=3.8,<3.11"
+boto3 = "^1.26.124"
 requests = "^2.23"
 matplotlib = ">=3.1,<3.6"
 attrs = ">=19.3,<22.2"
 jsonpickle = ">=1.3,<3.1"
 redis = ">=4.5.3, <5.0"
 absl-py = ">=0.9,<1.4"
 apscheduler = ">=3.6,<3.10"
 tqdm = "^4.31"
 networkx = ">=2.4,<2.7"
 fbmessenger = "~6.0.0"
 pykwalify = ">=1.7,<1.9"
 coloredlogs = ">=10,<16"
 "ruamel.yaml" = ">=0.16.5,<0.18.0"
-twilio = ">=6.26,<7.15"
+pyyaml = ">=5.3.1,<6.0"
+twilio = ">=6.26,<8.2"
 webexteamssdk = ">=1.1.1,<1.7.0"
 mattermostwrapper = "~2.2"
-rocketchat_API = ">=0.6.31,<1.29.0"
+rocketchat_API = ">=0.6.31,<1.30.0"
 colorhash = ">=1.0.2,<1.3.0"
 jsonschema = ">=3.2,<4.18"
 packaging = ">=20.0,<21.0"
 pytz = ">=2019.1,<2023.0"
-rasa-sdk = "~3.5.0"
+rasa-sdk = "~3.6.0a1"
 colorclass = "~2.2"
 terminaltables = "~3.1.0"
 sanic = "~21.12"
 sanic-cors = "~2.0.0"
 sanic-jwt = "^1.6.0"
 sanic-routing = "^0.7.2"
 websockets = ">=10.0,<11.0"
@@ -127,31 +128,30 @@
 pydot = "~1.4"
 SQLAlchemy = ">=1.4.0,<1.5.0"
 sklearn-crfsuite = "~0.3"
 psycopg2-binary = ">=2.8.2,<2.10.0"
 python-dateutil = "~2.8"
 protobuf = ">=3.9.2,< 3.20"
 tensorflow_hub = "~0.12.0"
-tensorflow-addons = ">=0.18,<0.20"
 setuptools = ">=41.0.0"
 ujson = ">=1.35,<6.0"
 regex = ">=2020.6,<2022.11"
 joblib = ">=0.15.1,<1.3.0"
 sentry-sdk = ">=0.17.0,<1.15.0"
 aio-pika = ">=6.7.1,<8.2.4"
 aiogram = "<2.26"
 typing-extensions = ">=4.1.1,<5.0.0"
 typing-utils = "^0.1.0"
-tarsafe = "^0.0.3"
+tarsafe = ">=0.0.3,<0.0.5"
 google-auth = "<3"
 CacheControl = "^0.12.9"
 randomname = "^0.1.5"
 pluggy = "^1.0.0"
 slack-sdk = "^3.19.2"
-confluent-kafka = "^1.9.2"
+confluent-kafka = ">=1.9.2,<3.0.0"
 portalocker = "^2.7.0"
 [[tool.poetry.dependencies.dask]]
 version = "2022.2.0"
 python = "~=3.7.0"
 
 [[tool.poetry.dependencies.dask]]
 version = "2022.10.2"
@@ -162,15 +162,15 @@
 python = "~=3.7.0"
 
 [[tool.poetry.dependencies.numpy]]
 version = ">=1.19.2,<1.25.0"
 python = ">=3.8,<3.11"
 
 [[tool.poetry.dependencies.scipy]]
-version = ">=1.4.1,<1.8.0"
+version = ">=1.4.1,<1.7.3"
 python = "~=3.7.0"
 
 [[tool.poetry.dependencies.scipy]]
 version = ">=1.4.1,<1.9.0"
 python = ">=3.8,<3.11"
 
 [[tool.poetry.dependencies.scikit-learn]]
@@ -191,47 +191,55 @@
 markers = "sys_platform != 'darwin' or platform_machine != 'arm64'"
 optional = true
 
 [[tool.poetry.dependencies.pydantic]]
 version = "<1.10.3"
 optional = true
 
+[[tool.poetry.dependencies.tensorflow-addons]]
+version = ">=0.18,<0.20"
+markers = "sys_platform != 'linux' or (platform_machine != 'arm64' and platform_machine != 'aarch64')"
+
+[[tool.poetry.dependencies.tensorflow-addons]]
+version = "0.19.0"
+markers = "sys_platform == 'linux' and (platform_machine == 'arm64' or platform_machine == 'aarch64')"
+
 [tool.poetry.dev-dependencies]
 pytest-cov = "^4.0.0"
 pytest-asyncio = "^0.20.0"
-pytest-xdist = "^3.0.2"
+pytest-xdist = "^3.2.1"
 pytest = "^7.1.3"
 freezegun = "^1.0.0"
 responses = "^0.22.0"
 aioresponses = "^0.7.2"
 moto = "~=4.1.2"
-fakeredis = "^2.2.0"
+fakeredis = "^2.11.2"
 mongomock = "^4.1.2"
 black = "^22.10.0"
 google-cloud-storage = "^2.4.0"
-azure-storage-blob = "<12.15.0"
+azure-storage-blob = "<12.16.0"
 coveralls = "^3.0.1"
 towncrier = "^22.8.0"
 toml = "^0.10.0"
 pep440-version-utils = "^0.3.0"
 pydoc-markdown = "^4.5.1"
 pytest-timeout = "^2.1.0"
 mypy = "^1.0.0"
 bandit = "^1.6.3"
 types-pytz = "^2022.1.1"
-types-python-dateutil = "^2.8.12"
+types-python-dateutil = "^2.8.19"
 types-requests = "^2.25.0"
 types-setuptools = "^67.2.0"
 memory-profiler = "^0.61.0"
 psutil = "^5.8.0"
 mypy-extensions = "^0.4.3"
 sanic-testing = ">=21.12.0,<22.9.0"
 analytics-python = "^1.4.0"
 datadog-api-client = "^2.0.0"
-datadog = "^0.44.0"
+datadog = "^0.45.0"
 types-redis = "^4.3.20"
 httpx = "0.23.3"
 
 [tool.poetry.extras]
 spacy = [ "spacy",]
 jieba = [ "jieba",]
 transformers = [ "transformers", "sentencepiece",]
@@ -253,23 +261,28 @@
 python_functions = "test_"
 filterwarnings = [ "ignore::ResourceWarning:ruamel[.*]",]
 log_cli_level = "WARNING"
 log_cli = true
 markers = [ "skip_on_windows", "skip_on_ci", "sequential", "category_cli", "category_core_featurizers", "category_policies", "category_nlu_featurizers", "category_nlu_predictors", "category_full_model_training", "category_other_unit_tests", "category_performance", "flaky",]
 timeout = 60
 timeout_func_only = true
+asyncio_mode = "auto"
 
 [tool.poetry.dependencies.tensorflow]
 version = "2.11.0"
 markers = "sys_platform != 'darwin' or platform_machine != 'arm64'"
 
 [tool.poetry.dependencies.tensorflow-intel]
 version = "2.11.0"
 markers = "sys_platform == 'win32'"
 
+[tool.poetry.dependencies.tensorflow-io-gcs-filesystem]
+version = ">=0.23.1,<0.32"
+markers = "sys_platform == 'win32'"
+
 [tool.poetry.dependencies.tensorflow-cpu-aws]
 version = "2.11.0"
 markers = "sys_platform == 'linux' and (platform_machine == 'arm64' or platform_machine == 'aarch64')"
 
 [tool.poetry.dependencies.tensorflow-macos]
 version = "2.11.0"
 markers = "sys_platform == 'darwin' and platform_machine == 'arm64'"
@@ -285,35 +298,35 @@
 [tool.poetry.dependencies.tensorflow-metal]
 version = "0.5.1"
 markers = "sys_platform == 'darwin' and platform_machine == 'arm64'"
 optional = true
 
 [tool.poetry.dependencies.tensorflow-text]
 version = "2.11.0"
-markers = "sys_platform!='win32' and platform_machine!='arm64'"
+markers = "sys_platform != 'win32' and platform_machine != 'arm64' and platform_machine != 'aarch64'"
 
 [tool.poetry.dependencies."github3.py"]
 version = "~3.2.0"
 optional = true
 
 [tool.poetry.dependencies.transformers]
 version = ">=4.13.0, <=4.26.0"
 optional = true
 
 [tool.poetry.dependencies.sentencepiece]
-version = "~0.1.96"
+version = "~0.1.99"
 optional = true
 extras = [ "sentencepiece",]
 
 [tool.poetry.dependencies.jieba]
 version = ">=0.39, <0.43"
 optional = true
 
 [tool.poetry.dependencies.pymongo]
-version = ">=3.8,<3.11"
+version = ">=3.8,<4.4"
 extras = [ "tls", "srv",]
 
 [tool.poetry.dev-dependencies.pytest-sanic]
 git = "https://github.com/RasaHQ/pytest-sanic"
 branch = "fix_signal_issue"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `rasa-3.5.9/rasa/__main__.py` & `rasa-3.6.0a1/rasa/__main__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/api.py` & `rasa-3.6.0a1/rasa/api.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/arguments/data.py` & `rasa-3.6.0a1/rasa/cli/arguments/data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/arguments/default_arguments.py` & `rasa-3.6.0a1/rasa/cli/arguments/default_arguments.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/arguments/evaluate.py` & `rasa-3.6.0a1/rasa/cli/arguments/evaluate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/arguments/export.py` & `rasa-3.6.0a1/rasa/cli/arguments/export.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/arguments/interactive.py` & `rasa-3.6.0a1/rasa/cli/arguments/interactive.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/arguments/run.py` & `rasa-3.6.0a1/rasa/cli/arguments/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/arguments/test.py` & `rasa-3.6.0a1/rasa/cli/arguments/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/arguments/train.py` & `rasa-3.6.0a1/rasa/cli/arguments/train.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     """Specifies CLI arguments for `rasa train`."""
     add_data_param(parser)
     add_config_param(parser)
     add_domain_param(parser)
     add_out_param(parser, help_text="Directory where your models should be stored.")
 
     add_dry_run_param(parser)
+    add_validate_before_train(parser)
     add_augmentation_param(parser)
     add_debug_plots_param(parser)
 
     _add_num_threads_param(parser)
 
     _add_model_name_param(parser)
     add_persist_nlu_data_param(parser)
@@ -143,14 +144,45 @@
         "- 0 means that no extensive training is required (note that the responses "
         "still might require updating by running 'rasa train').\n"
         "- 1 means the model needs to be retrained\n"
         "- 8 means the training was forced (--force argument is specified)",
     )
 
 
+def add_validate_before_train(
+    parser: Union[argparse.ArgumentParser, argparse._ActionsContainer]
+) -> None:
+    """Adds parameters for validating the domain and data files before training.
+
+    Args:
+        parser: An instance of `ArgumentParser` or `_ActionsContainer`.
+    """
+    parser.add_argument(
+        "--skip-validation",
+        default=False,
+        action="store_true",
+        help="Skip validation step before training.",
+    )
+
+    parser.add_argument(
+        "--fail-on-validation-warnings",
+        default=False,
+        action="store_true",
+        help="Fail on validation warnings. "
+        "If omitted only errors will exit with a non zero status code",
+    )
+
+    parser.add_argument(
+        "--validation-max-history",
+        type=int,
+        default=None,
+        help="Number of turns taken into account for story structure validation.",
+    )
+
+
 def add_augmentation_param(
     parser: Union[argparse.ArgumentParser, argparse._ActionsContainer]
 ) -> None:
     """Sets the augmentation factor for the Core training.
 
     Args:
         parser: An instance of `ArgumentParser` or `_ActionsContainer`.
```

### Comparing `rasa-3.5.9/rasa/cli/arguments/visualize.py` & `rasa-3.6.0a1/rasa/cli/arguments/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/arguments/x.py` & `rasa-3.6.0a1/rasa/cli/arguments/x.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/data.py` & `rasa-3.6.0a1/rasa/cli/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import logging
-from typing import List, TYPE_CHECKING
+import pathlib
+from typing import List
 
 import rasa.shared.core.domain
 from rasa import telemetry
 from rasa.cli import SubParsersAction
 from rasa.cli.arguments import data as arguments
 from rasa.cli.arguments import default_arguments
 import rasa.cli.utils
@@ -13,17 +14,14 @@
 from rasa.shared.importers.importer import TrainingDataImporter
 import rasa.shared.nlu.training_data.loading
 import rasa.shared.nlu.training_data.util
 import rasa.shared.utils.cli
 import rasa.utils.common
 import rasa.shared.utils.io
 
-if TYPE_CHECKING:
-    from rasa.validator import Validator
-
 logger = logging.getLogger(__name__)
 
 
 def add_subparser(
     subparsers: SubParsersAction, parents: List[argparse.ArgumentParser]
 ) -> None:
     """Add all data parsers.
@@ -90,40 +88,73 @@
         help="Performs a split of your NLU data into training and test data "
         "according to the specified percentages.",
     )
     nlu_split_parser.set_defaults(func=split_nlu_data)
 
     arguments.set_split_arguments(nlu_split_parser)
 
+    stories_split_parser = split_subparsers.add_parser(
+        "stories",
+        parents=parents,
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        help="Performs a split of your stories into training and test data "
+        "according to the specified percentages.",
+    )
+    stories_split_parser.set_defaults(func=split_stories_data)
+
+    arguments.set_split_arguments(stories_split_parser)
+
 
 def _add_data_validate_parsers(
     data_subparsers: SubParsersAction, parents: List[argparse.ArgumentParser]
 ) -> None:
     validate_parser = data_subparsers.add_parser(
         "validate",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         parents=parents,
         help="Validates domain and data files to check for possible mistakes.",
     )
     _append_story_structure_arguments(validate_parser)
-    validate_parser.set_defaults(func=validate_files)
+    validate_parser.set_defaults(
+        func=lambda args: rasa.cli.utils.validate_files(
+            args.fail_on_warnings, args.max_history, _build_training_data_importer(args)
+        )
+    )
     arguments.set_validator_arguments(validate_parser)
 
     validate_subparsers = validate_parser.add_subparsers()
     story_structure_parser = validate_subparsers.add_parser(
         "stories",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         parents=parents,
         help="Checks for inconsistencies in the story files.",
     )
     _append_story_structure_arguments(story_structure_parser)
-    story_structure_parser.set_defaults(func=validate_stories)
+
+    story_structure_parser.set_defaults(
+        func=lambda args: rasa.cli.utils.validate_files(
+            args.fail_on_warnings,
+            args.max_history,
+            _build_training_data_importer(args),
+            stories_only=True,
+        )
+    )
     arguments.set_validator_arguments(story_structure_parser)
 
 
+def _build_training_data_importer(args: argparse.Namespace) -> "TrainingDataImporter":
+    config = rasa.cli.utils.get_validated_path(
+        args.config, "config", DEFAULT_CONFIG_PATH, none_is_valid=True
+    )
+
+    return TrainingDataImporter.load_from_config(
+        domain_path=args.domain, training_data_paths=args.data, config_path=config
+    )
+
+
 def _append_story_structure_arguments(parser: argparse.ArgumentParser) -> None:
     parser.add_argument(
         "--max-history",
         type=int,
         default=None,
         help="Number of turns taken into account for story structure validation.",
     )
@@ -146,86 +177,63 @@
 
     train.persist(args.out, filename=f"training_data{extension}")
     test.persist(args.out, filename=f"test_data{extension}")
 
     telemetry.track_data_split(args.training_fraction, "nlu")
 
 
-def validate_files(args: argparse.Namespace, stories_only: bool = False) -> None:
-    """Validates either the story structure or the entire project.
+def split_stories_data(args: argparse.Namespace) -> None:
+    """Load data from a file path and split stories into test and train examples.
 
     Args:
         args: Commandline arguments
-        stories_only: If `True`, only the story structure is validated.
     """
-    from rasa.validator import Validator
-
-    config = rasa.cli.utils.get_validated_path(
-        args.config, "config", DEFAULT_CONFIG_PATH, none_is_valid=True
+    from rasa.shared.core.training_data.story_reader.yaml_story_reader import (
+        YAMLStoryReader,
+        KEY_STORIES,
     )
+    from sklearn.model_selection import train_test_split
 
-    importer = TrainingDataImporter.load_from_config(
-        domain_path=args.domain, training_data_paths=args.data, config_path=config
+    data_path = rasa.cli.utils.get_validated_path(args.nlu, "nlu", DEFAULT_DATA_PATH)
+    data_files = rasa.shared.data.get_data_files(
+        data_path, YAMLStoryReader.is_stories_file
     )
+    out_path = pathlib.Path(args.out)
+    out_path.mkdir(parents=True, exist_ok=True)
 
-    validator = Validator.from_importer(importer)
-
-    if stories_only:
-        all_good = _validate_story_structure(validator, args)
-    else:
-        all_good = (
-            _validate_domain(validator)
-            and _validate_nlu(validator, args)
-            and _validate_story_structure(validator, args)
+    # load Yaml stories data
+    for file_name in data_files:
+        file_data = rasa.shared.utils.io.read_yaml_file(file_name)
+        assert isinstance(file_data, dict)
+        stories = file_data.get(KEY_STORIES, [])
+        if not stories:
+            logger.info(f"File {file_name} has no stories, skipped")
+            continue
+
+        file_path = pathlib.Path(file_name)
+
+        # everything besides stories are going into the training data
+        train, test = train_test_split(
+            stories, test_size=1 - args.training_fraction, random_state=args.random_seed
         )
+        out_file_train = out_path / ("train_" + file_path.name)
+        out_file_test = out_path / ("test_" + file_path.name)
 
-    validator.warn_if_config_mandatory_keys_are_not_set()
-
-    telemetry.track_validate_files(all_good)
-    if not all_good:
-        rasa.shared.utils.cli.print_error_and_exit(
-            "Project validation completed with errors."
-        )
-
-
-def validate_stories(args: argparse.Namespace) -> None:
-    """Validates that training data file content conforms to training data spec.
-
-    Args:
-        args: Commandline arguments
-    """
-    validate_files(args, stories_only=True)
-
-
-def _validate_domain(validator: "Validator") -> bool:
-    return (
-        validator.verify_domain_validity()
-        and validator.verify_actions_in_stories_rules()
-        and validator.verify_forms_in_stories_rules()
-        and validator.verify_form_slots()
-        and validator.verify_slot_mappings()
-    )
-
-
-def _validate_nlu(validator: "Validator", args: argparse.Namespace) -> bool:
-    return validator.verify_nlu(not args.fail_on_warnings)
-
-
-def _validate_story_structure(validator: "Validator", args: argparse.Namespace) -> bool:
-    # Check if a valid setting for `max_history` was given
-    if isinstance(args.max_history, int) and args.max_history < 1:
-        raise argparse.ArgumentTypeError(
-            f"The value of `--max-history {args.max_history}` "
-            f"is not a positive integer."
+        # train file contains everything else from the file + train stories
+        file_data[KEY_STORIES] = train
+        rasa.shared.utils.io.write_yaml(file_data, out_file_train)
+
+        # test file contains just test stories
+        rasa.shared.utils.io.write_yaml({KEY_STORIES: test}, out_file_test)
+        logger.info(
+            f"From {file_name} we produced {out_file_train} "
+            f"with {len(train)} stories and {out_file_test} "
+            f"with {len(test)} stories"
         )
 
-    return validator.verify_story_structure(
-        not args.fail_on_warnings, max_history=args.max_history
-    )
-
 
 def _convert_nlu_data(args: argparse.Namespace) -> None:
     import rasa.nlu.convert
 
     if args.format in ["json", "yaml"]:
         rasa.nlu.convert.convert_training_data(
             args.data, args.out, args.format, args.language
```

### Comparing `rasa-3.5.9/rasa/cli/evaluate.py` & `rasa-3.6.0a1/rasa/cli/evaluate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/export.py` & `rasa-3.6.0a1/rasa/cli/export.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/initial_project/actions/actions.py` & `rasa-3.6.0a1/rasa/cli/initial_project/actions/actions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/initial_project/config.yml` & `rasa-3.6.0a1/rasa/cli/initial_project/config.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/initial_project/credentials.yml` & `rasa-3.6.0a1/rasa/cli/initial_project/credentials.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/initial_project/data/nlu.yml` & `rasa-3.6.0a1/rasa/cli/initial_project/data/nlu.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/initial_project/data/stories.yml` & `rasa-3.6.0a1/rasa/cli/initial_project/data/stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/initial_project/domain.yml` & `rasa-3.6.0a1/rasa/cli/initial_project/domain.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/initial_project/endpoints.yml` & `rasa-3.6.0a1/rasa/cli/initial_project/endpoints.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/initial_project/tests/test_stories.yml` & `rasa-3.6.0a1/rasa/cli/initial_project/tests/test_stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/interactive.py` & `rasa-3.6.0a1/rasa/cli/interactive.py`

 * *Files 7% similar despite different names*

```diff
@@ -101,14 +101,17 @@
     perform_interactive_learning(args, zipped_model, file_importer)
 
 
 def _set_not_required_args(args: argparse.Namespace) -> None:
     args.fixed_model_name = None
     args.store_uncompressed = False
     args.dry_run = False
+    args.skip_validation = True
+    args.fail_on_validation_warnings = False
+    args.validation_max_history = None
 
 
 def perform_interactive_learning(
     args: argparse.Namespace,
     zipped_model: Union[Text, "Path"],
     file_importer: TrainingDataImporter,
 ) -> None:
```

### Comparing `rasa-3.5.9/rasa/cli/run.py` & `rasa-3.6.0a1/rasa/cli/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/scaffold.py` & `rasa-3.6.0a1/rasa/cli/scaffold.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/shell.py` & `rasa-3.6.0a1/rasa/cli/shell.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/telemetry.py` & `rasa-3.6.0a1/rasa/cli/telemetry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/test.py` & `rasa-3.6.0a1/rasa/cli/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/train.py` & `rasa-3.6.0a1/rasa/cli/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import argparse
+import logging
 import sys
 from typing import Dict, List, Optional, Text
 
 from rasa.cli import SubParsersAction
 import rasa.cli.arguments.train as train_arguments
 
 import rasa.cli.utils
+from rasa.shared.importers.importer import TrainingDataImporter
 import rasa.utils.common
 from rasa.core.train import do_compare_training
+from rasa.plugin import plugin_manager
 from rasa.shared.constants import (
     CONFIG_MANDATORY_KEYS_CORE,
     CONFIG_MANDATORY_KEYS_NLU,
     CONFIG_MANDATORY_KEYS,
     DEFAULT_DOMAIN_PATH,
     DEFAULT_DATA_PATH,
 )
 
+logger = logging.getLogger(__name__)
+
 
 def add_subparser(
     subparsers: SubParsersAction, parents: List[argparse.ArgumentParser]
 ) -> None:
     """Add all training parsers.
 
     Args:
@@ -80,24 +85,36 @@
     training_files = [
         rasa.cli.utils.get_validated_path(
             f, "data", DEFAULT_DATA_PATH, none_is_valid=True
         )
         for f in args.data
     ]
 
+    if not args.skip_validation:
+        logger.info("Started validating domain and training data...")
+        importer = TrainingDataImporter.load_from_config(
+            domain_path=args.domain, training_data_paths=args.data, config_path=config
+        )
+        rasa.cli.utils.validate_files(
+            args.fail_on_validation_warnings, args.validation_max_history, importer
+        )
+
     training_result = train_all(
         domain=domain,
         config=config,
         training_files=training_files,
         output=args.out,
         dry_run=args.dry_run,
         force_training=args.force,
         fixed_model_name=args.fixed_model_name,
         persist_nlu_training_data=args.persist_nlu_data,
-        core_additional_arguments=extract_core_additional_arguments(args),
+        core_additional_arguments={
+            **extract_core_additional_arguments(args),
+            **_extract_additional_arguments(args),
+        },
         nlu_additional_arguments=extract_nlu_additional_arguments(args),
         model_to_finetune=_model_for_finetuning(args),
         finetuning_epoch_fraction=args.epoch_fraction,
     )
     if training_result.code != 0 and can_exit:
         sys.exit(training_result.code)
 
@@ -127,15 +144,18 @@
 
     args.domain = rasa.cli.utils.get_validated_path(
         args.domain, "domain", DEFAULT_DOMAIN_PATH, none_is_valid=True
     )
     story_file = rasa.cli.utils.get_validated_path(
         args.stories, "stories", DEFAULT_DATA_PATH, none_is_valid=True
     )
-    additional_arguments = extract_core_additional_arguments(args)
+    additional_arguments = {
+        **extract_core_additional_arguments(args),
+        **_extract_additional_arguments(args),
+    }
 
     # Policies might be a list for the compare training. Do normal training
     # if only list item was passed.
     if not isinstance(args.config, list) or len(args.config) == 1:
         if isinstance(args.config, list):
             args.config = args.config[0]
 
@@ -181,15 +201,18 @@
 
     return train_nlu(
         config=config,
         nlu_data=nlu_data,
         output=args.out,
         fixed_model_name=args.fixed_model_name,
         persist_nlu_training_data=args.persist_nlu_data,
-        additional_arguments=extract_nlu_additional_arguments(args),
+        additional_arguments={
+            **extract_nlu_additional_arguments(args),
+            **_extract_additional_arguments(args),
+        },
         domain=args.domain,
         model_to_finetune=_model_for_finetuning(args),
         finetuning_epoch_fraction=args.epoch_fraction,
     )
 
 
 def extract_core_additional_arguments(args: argparse.Namespace) -> Dict:
@@ -206,7 +229,12 @@
 def extract_nlu_additional_arguments(args: argparse.Namespace) -> Dict:
     arguments = {}
 
     if "num_threads" in args:
         arguments["num_threads"] = args.num_threads
 
     return arguments
+
+
+def _extract_additional_arguments(args: argparse.Namespace) -> Dict:
+    space = plugin_manager().hook.handle_space_args(args=args)
+    return space or {}
```

### Comparing `rasa-3.5.9/rasa/cli/utils.py` & `rasa-3.6.0a1/rasa/cli/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import json
+import argparse
 import logging
 import os
 import sys
 import time
 from types import FrameType
 from typing import Any, Dict, List, Optional, TYPE_CHECKING, Text, Union, overload
 
 import randomname
 
 import rasa.shared.utils.cli
 import rasa.shared.utils.io
+from rasa.shared.importers.importer import TrainingDataImporter
 from rasa.shared.constants import (
     ASSISTANT_ID_DEFAULT_VALUE,
     ASSISTANT_ID_KEY,
     DEFAULT_CONFIG_PATH,
 )
 from rasa.shared.utils.cli import print_error
+from rasa import telemetry
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from questionary import Question
     from typing_extensions import Literal
+    from rasa.validator import Validator
 
 logger = logging.getLogger(__name__)
 
 FREE_TEXT_INPUT_PROMPT = "Type out your own message..."
 
 
 @overload
@@ -204,14 +208,78 @@
     validate_assistant_id_in_config(config)
 
     config = validate_mandatory_config_keys(config, mandatory_keys)
 
     return config
 
 
+def validate_files(
+    fail_on_warnings: bool,
+    max_history: Optional[int],
+    importer: TrainingDataImporter,
+    stories_only: bool = False,
+) -> None:
+    """Validates either the story structure or the entire project.
+
+    Args:
+        fail_on_warnings: `True` if the process should exit with a non-zero status
+        max_history: The max history to use when validating the story structure.
+        importer: The `TrainingDataImporter` to use to load the training data.
+        stories_only: If `True`, only the story structure is validated.
+    """
+    from rasa.validator import Validator
+
+    validator = Validator.from_importer(importer)
+
+    if stories_only:
+        all_good = _validate_story_structure(validator, max_history, fail_on_warnings)
+    else:
+        all_good = (
+            _validate_domain(validator)
+            and _validate_nlu(validator, fail_on_warnings)
+            and _validate_story_structure(validator, max_history, fail_on_warnings)
+        )
+
+    validator.warn_if_config_mandatory_keys_are_not_set()
+
+    telemetry.track_validate_files(all_good)
+    if not all_good:
+        rasa.shared.utils.cli.print_error_and_exit(
+            "Project validation completed with errors."
+        )
+
+
+def _validate_domain(validator: "Validator") -> bool:
+    return (
+        validator.verify_domain_validity()
+        and validator.verify_actions_in_stories_rules()
+        and validator.verify_forms_in_stories_rules()
+        and validator.verify_form_slots()
+        and validator.verify_slot_mappings()
+    )
+
+
+def _validate_nlu(validator: "Validator", fail_on_warnings: bool) -> bool:
+    return validator.verify_nlu(not fail_on_warnings)
+
+
+def _validate_story_structure(
+    validator: "Validator", max_history: Optional[int], fail_on_warnings: bool
+) -> bool:
+    # Check if a valid setting for `max_history` was given
+    if isinstance(max_history, int) and max_history < 1:
+        raise argparse.ArgumentTypeError(
+            f"The value of `--max-history {max_history}` " f"is not a positive integer."
+        )
+
+    return validator.verify_story_structure(
+        not fail_on_warnings, max_history=max_history
+    )
+
+
 def cancel_cause_not_found(
     current: Optional[Union["Path", Text]],
     parameter: Text,
     default: Optional[Union["Path", Text]],
 ) -> None:
     """Exits with an error because the given path was not valid.
```

### Comparing `rasa-3.5.9/rasa/cli/visualize.py` & `rasa-3.6.0a1/rasa/cli/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/cli/x.py` & `rasa-3.6.0a1/rasa/cli/x.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/constants.py` & `rasa-3.6.0a1/rasa/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/actions/action.py` & `rasa-3.6.0a1/rasa/core/actions/action.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from rasa.core.policies.policy import PolicyPrediction
 from rasa.nlu.constants import (
     RESPONSE_SELECTOR_DEFAULT_INTENT,
     RESPONSE_SELECTOR_PROPERTY_NAME,
     RESPONSE_SELECTOR_PREDICTION_KEY,
     RESPONSE_SELECTOR_UTTER_ACTION_KEY,
 )
+from rasa.plugin import plugin_manager
 from rasa.shared.constants import (
     DOCS_BASE_URL,
     DEFAULT_NLU_FALLBACK_INTENT_NAME,
     UTTER_PREFIX,
 )
 from rasa.shared.core import events
 from rasa.shared.core.constants import (
@@ -221,15 +222,14 @@
             # property to set it in the following line)
             "attachment": message.pop("attachment", None) or message.get("image", None),
             "image": message.pop("image", None),
             "custom": message.pop("custom", None),
         },
         metadata=message,
     )
-
     return bot_message
 
 
 class Action:
     """Next action to be taken in response to a dialogue state."""
 
     def name(self) -> Text:
@@ -760,21 +760,27 @@
             )
 
             should_compress = get_bool_env_variable(
                 COMPRESS_ACTION_SERVER_REQUEST_ENV_NAME,
                 DEFAULT_COMPRESS_ACTION_SERVER_REQUEST,
             )
 
+            modified_json = plugin_manager().hook.prefix_stripping_for_custom_actions(
+                json_body=json_body
+            )
             response: Any = await self.action_endpoint.request(
-                json=json_body,
+                json=modified_json if modified_json else json_body,
                 method="post",
                 timeout=DEFAULT_REQUEST_TIMEOUT,
                 compress=should_compress,
             )
-
+            if modified_json:
+                plugin_manager().hook.prefixing_custom_actions_response(
+                    json_body=json_body, response=response
+                )
             self._validate_action_result(response)
 
             events_json = response.get("events", [])
             responses = response.get("responses", [])
             bot_messages = await self._utter_responses(
                 responses, output_channel, nlg, tracker
             )
@@ -1282,15 +1288,14 @@
                         domain,
                     )
                     slot_events.extend(custom_evts)
 
         validated_events = await self._execute_validation_action(
             slot_events, output_channel, nlg, tracker, domain
         )
-
         return validated_events
 
 
 def extract_slot_value_from_predefined_mapping(
     mapping_type: SlotMappingType,
     mapping: Dict[Text, Any],
     tracker: "DialogueStateTracker",
```

### Comparing `rasa-3.5.9/rasa/core/actions/forms.py` & `rasa-3.6.0a1/rasa/core/actions/forms.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/actions/loops.py` & `rasa-3.6.0a1/rasa/core/actions/loops.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/actions/two_stage_fallback.py` & `rasa-3.6.0a1/rasa/core/actions/two_stage_fallback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/agent.py` & `rasa-3.6.0a1/rasa/core/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from __future__ import annotations
 from asyncio import AbstractEventLoop, CancelledError
 import functools
 import logging
 import os
-import tempfile
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Text, Union
 import uuid
 
 import aiohttp
 from aiohttp import ClientError
 
 from rasa.core import jobs
 from rasa.core.channels.channel import OutputChannel, UserMessage
 from rasa.core.constants import DEFAULT_REQUEST_TIMEOUT
 from rasa.core.http_interpreter import RasaNLUHttpInterpreter
+from rasa.plugin import plugin_manager
 from rasa.shared.core.domain import Domain
 from rasa.core.exceptions import AgentNotReady
 from rasa.shared.constants import DEFAULT_SENDER_ID
 from rasa.core.lock_store import InMemoryLockStore, LockStore
 from rasa.core.nlg import NaturalLanguageGenerator, TemplatedNaturalLanguageGenerator
 from rasa.core.policies.policy import PolicyPrediction
 from rasa.core.processor import MessageProcessor
 from rasa.core.tracker_store import FailSafeTrackerStore, InMemoryTrackerStore
 from rasa.shared.core.trackers import DialogueStateTracker, EventVerbosity
 from rasa.exceptions import ModelNotFound
 from rasa.nlu.utils import is_url
 from rasa.shared.exceptions import RasaException
 import rasa.shared.utils.io
+from rasa.utils.common import TempDirectoryPath, get_temp_dir_name
 from rasa.utils.endpoints import EndpointConfig
 
 from rasa.core.tracker_store import TrackerStore
 from rasa.core.utils import AvailableEndpoints
 
 logger = logging.getLogger(__name__)
 
@@ -72,15 +73,15 @@
 
 
 async def _update_model_from_server(model_server: EndpointConfig, agent: Agent) -> None:
     """Load a zipped Rasa Core model from a URL and update the passed agent."""
     if not is_url(model_server.url):
         raise aiohttp.InvalidURL(model_server.url)
 
-    with tempfile.TemporaryDirectory() as temporary_directory:
+    with TempDirectoryPath(get_temp_dir_name()) as temporary_directory:
         try:
             new_fingerprint = await _pull_model_and_fingerprint(
                 model_server, agent.fingerprint, temporary_directory
             )
 
             if new_fingerprint:
                 _load_and_set_updated_model(agent, temporary_directory, new_fingerprint)
@@ -215,35 +216,42 @@
     from rasa.core.brokers.broker import EventBroker
 
     tracker_store = None
     lock_store = None
     generator = None
     action_endpoint = None
     http_interpreter = None
+    anonymization_pipeline = None
 
     if endpoints:
         broker = await EventBroker.create(endpoints.event_broker, loop=loop)
         tracker_store = TrackerStore.create(
             endpoints.tracker_store, event_broker=broker
         )
         lock_store = LockStore.create(endpoints.lock_store)
         generator = endpoints.nlg
         action_endpoint = endpoints.action
         model_server = endpoints.model if endpoints.model else model_server
         if endpoints.nlu:
             http_interpreter = RasaNLUHttpInterpreter(endpoints.nlu)
 
+        anonymization_pipeline = plugin_manager().hook.create_anonymization_pipeline(
+            anonymization_rules=endpoints.anonymization_rules,
+            event_broker_config=endpoints.event_broker,
+        )
+
     agent = Agent(
         generator=generator,
         tracker_store=tracker_store,
         lock_store=lock_store,
         action_endpoint=action_endpoint,
         model_server=model_server,
         remote_storage=remote_storage,
         http_interpreter=http_interpreter,
+        anonymization_pipeline=anonymization_pipeline,
     )
 
     try:
         if model_server is not None:
             return await load_from_server(agent, model_server)
 
         elif remote_storage is not None:
@@ -260,15 +268,15 @@
             rasa.shared.utils.io.raise_warning(
                 "No valid configuration given to load agent. "
                 "Agent loaded with no model!"
             )
         return agent
 
     except Exception as e:
-        logger.error(f"Could not load model due to {e}.")
+        logger.error(f"Could not load model due to {e}.", exc_info=True)
         return agent
 
 
 def agent_must_be_ready(f: Callable[..., Any]) -> Callable[..., Any]:
     """Any Agent method decorated with this will raise if the agent is not ready."""
 
     @functools.wraps(f)
@@ -297,28 +305,30 @@
         tracker_store: Optional[TrackerStore] = None,
         lock_store: Optional[LockStore] = None,
         action_endpoint: Optional[EndpointConfig] = None,
         fingerprint: Optional[Text] = None,
         model_server: Optional[EndpointConfig] = None,
         remote_storage: Optional[Text] = None,
         http_interpreter: Optional[RasaNLUHttpInterpreter] = None,
+        anonymization_pipeline: Optional[Any] = None,
     ):
         """Initializes an `Agent`."""
         self.domain = domain
         self.processor: Optional[MessageProcessor] = None
 
         self.nlg = NaturalLanguageGenerator.create(generator, self.domain)
         self.tracker_store = self._create_tracker_store(tracker_store, self.domain)
         self.lock_store = self._create_lock_store(lock_store)
         self.action_endpoint = action_endpoint
         self.http_interpreter = http_interpreter
 
         self._set_fingerprint(fingerprint)
         self.model_server = model_server
         self.remote_storage = remote_storage
+        self.anonymization_pipeline = anonymization_pipeline
 
     @classmethod
     def load(
         cls,
         model_path: Union[Text, Path],
         domain: Optional[Domain] = None,
         generator: Union[EndpointConfig, NaturalLanguageGenerator, None] = None,
@@ -352,14 +362,15 @@
         self.processor = MessageProcessor(
             model_path=model_path,
             tracker_store=self.tracker_store,
             lock_store=self.lock_store,
             action_endpoint=self.action_endpoint,
             generator=self.nlg,
             http_interpreter=self.http_interpreter,
+            anonymization_pipeline=self.anonymization_pipeline,
         )
         self.domain = self.processor.domain
 
         self._set_fingerprint(fingerprint)
 
         # update domain on all instances
         self.tracker_store.domain = self.domain
@@ -537,15 +548,15 @@
     def load_model_from_remote_storage(self, model_name: Text) -> None:
         """Loads an Agent from remote storage."""
         from rasa.nlu.persistor import get_persistor
 
         persistor = get_persistor(self.remote_storage)
 
         if persistor is not None:
-            with tempfile.TemporaryDirectory() as temporary_directory:
+            with TempDirectoryPath(get_temp_dir_name()) as temporary_directory:
                 persistor.retrieve(model_name, temporary_directory)
                 self.load_model(temporary_directory)
 
         else:
             raise RasaException(
                 f"Persistor not found for remote storage: '{self.remote_storage}'."
             )
```

### Comparing `rasa-3.5.9/rasa/core/brokers/broker.py` & `rasa-3.6.0a1/rasa/core/brokers/broker.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/brokers/file.py` & `rasa-3.6.0a1/rasa/core/brokers/file.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/brokers/kafka.py` & `rasa-3.6.0a1/rasa/core/brokers/kafka.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/brokers/pika.py` & `rasa-3.6.0a1/rasa/core/brokers/pika.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/brokers/sql.py` & `rasa-3.6.0a1/rasa/core/brokers/sql.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/channels/__init__.py` & `rasa-3.6.0a1/rasa/core/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/channels/botframework.py` & `rasa-3.6.0a1/rasa/core/channels/botframework.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,14 @@
     def __init__(self, app_id: Text, app_password: Text) -> None:
         """Create a Bot Framework input channel.
 
         Args:
             app_id: Bot Framework's API id
             app_password: Bot Framework application secret
         """
-
         self.app_id = app_id
         self.app_password = app_password
 
         self.jwt_keys: Dict[Text, Any] = {}
         self.jwt_update_time = datetime.datetime.fromtimestamp(0)
 
         self._update_cached_jwk_keys()
```

### Comparing `rasa-3.5.9/rasa/core/channels/callback.py` & `rasa-3.6.0a1/rasa/core/channels/callback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/channels/channel.py` & `rasa-3.6.0a1/rasa/core/channels/channel.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/channels/console.py` & `rasa-3.6.0a1/rasa/core/channels/console.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/channels/facebook.py` & `rasa-3.6.0a1/rasa/core/channels/facebook.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/channels/hangouts.py` & `rasa-3.6.0a1/rasa/core/channels/hangouts.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/channels/mattermost.py` & `rasa-3.6.0a1/rasa/core/channels/mattermost.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/channels/rasa_chat.py` & `rasa-3.6.0a1/rasa/core/channels/rasa_chat.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/channels/rest.py` & `rasa-3.6.0a1/rasa/core/channels/rest.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/channels/rocketchat.py` & `rasa-3.6.0a1/rasa/core/channels/rocketchat.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/channels/slack.py` & `rasa-3.6.0a1/rasa/core/channels/slack.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/channels/socketio.py` & `rasa-3.6.0a1/rasa/core/channels/socketio.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/channels/telegram.py` & `rasa-3.6.0a1/rasa/core/channels/telegram.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/channels/twilio.py` & `rasa-3.6.0a1/rasa/core/channels/twilio.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 if TYPE_CHECKING:
     from twilio.rest.api.v2010.account.message import MessageInstance
 
 logger = logging.getLogger(__name__)
 
 
 class TwilioOutput(Client, OutputChannel):
-    """Output channel for Twilio"""
+    """Output channel for Twilio."""
 
     @classmethod
     def name(cls) -> Text:
         return "twilio"
 
     def __init__(
         self,
@@ -48,49 +48,46 @@
             logger.error("Failed to send message. Max number of retires exceeded.")
 
         return message
 
     async def send_text_message(
         self, recipient_id: Text, text: Text, **kwargs: Any
     ) -> None:
-        """Sends text message"""
-
+        """Sends text message."""
         message_data = {"to": recipient_id, "from_": self.twilio_number}
         for message_part in text.strip().split("\n\n"):
             message_data.update({"body": message_part})
             await self._send_message(message_data)
 
     async def send_image_url(
         self, recipient_id: Text, image: Text, **kwargs: Any
     ) -> None:
         """Sends an image."""
-
         message_data = {
             "to": recipient_id,
             "from_": self.twilio_number,
             "media_url": [image],
         }
         await self._send_message(message_data)
 
     async def send_custom_json(
         self, recipient_id: Text, json_message: Dict[Text, Any], **kwargs: Any
     ) -> None:
-        """Send custom json dict"""
-
+        """Send custom json dict."""
         json_message.setdefault("to", recipient_id)
         if not json_message.get("media_url"):
             json_message.setdefault("body", "")
         if not json_message.get("messaging_service_sid"):
             json_message.setdefault("from_", self.twilio_number)
 
         await self._send_message(json_message)
 
 
 class TwilioInput(InputChannel):
-    """Twilio input channel"""
+    """Twilio input channel."""
 
     @classmethod
     def name(cls) -> Text:
         return "twilio"
 
     @classmethod
     def from_credentials(cls, credentials: Optional[Dict[Text, Any]]) -> InputChannel:
@@ -99,14 +96,19 @@
 
         return cls(
             credentials.get("account_sid"),
             credentials.get("auth_token"),
             credentials.get("twilio_number"),
         )
 
+    @classmethod
+    def _is_location_message(cls, request: Request) -> bool:
+        """Check if the users message is a location."""
+        return request.form.get("Latitude") and request.form.get("Longitude")
+
     def __init__(
         self,
         account_sid: Optional[Text],
         auth_token: Optional[Text],
         twilio_number: Optional[Text],
         debug_mode: bool = True,
     ) -> None:
@@ -124,17 +126,22 @@
         async def health(_: Request) -> HTTPResponse:
             return response.json({"status": "ok"})
 
         @twilio_webhook.route("/webhook", methods=["POST"])
         async def message(request: Request) -> HTTPResponse:
             sender = request.form.get("From", None)
             text = request.form.get("Body", None)
-
             out_channel = self.get_output_channel()
 
+            if self._is_location_message(request):
+                # Text is always None with a location message/media from Twilio whatsapp
+                text = "/locationData{{'Latitude': {lat},'Longitude': {long}}}".format(
+                    lat=request.form.get("Latitude"), long=request.form.get("Longitude")
+                )
+
             if sender is not None and message is not None:
                 metadata = self.get_metadata(request)
                 try:
                     # @ signs get corrupted in SMSes by some carriers
                     text = text.replace("¡", "@")
                     await on_new_message(
                         UserMessage(
```

### Comparing `rasa-3.5.9/rasa/core/channels/twilio_voice.py` & `rasa-3.6.0a1/rasa/core/channels/twilio_voice.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/channels/webexteams.py` & `rasa-3.6.0a1/rasa/core/channels/webexteams.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/constants.py` & `rasa-3.6.0a1/rasa/core/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/evaluation/marker.py` & `rasa-3.6.0a1/rasa/core/evaluation/marker.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/evaluation/marker_base.py` & `rasa-3.6.0a1/rasa/core/evaluation/marker_base.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/evaluation/marker_stats.py` & `rasa-3.6.0a1/rasa/core/evaluation/marker_stats.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/evaluation/marker_tracker_loader.py` & `rasa-3.6.0a1/rasa/core/evaluation/marker_tracker_loader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/exceptions.py` & `rasa-3.6.0a1/rasa/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/exporter.py` & `rasa-3.6.0a1/rasa/core/exporter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/featurizers/precomputation.py` & `rasa-3.6.0a1/rasa/core/featurizers/precomputation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/featurizers/single_state_featurizer.py` & `rasa-3.6.0a1/rasa/core/featurizers/single_state_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/featurizers/tracker_featurizers.py` & `rasa-3.6.0a1/rasa/core/featurizers/tracker_featurizers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/http_interpreter.py` & `rasa-3.6.0a1/rasa/core/http_interpreter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/jobs.py` & `rasa-3.6.0a1/rasa/core/jobs.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/lock.py` & `rasa-3.6.0a1/rasa/core/lock.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/lock_store.py` & `rasa-3.6.0a1/rasa/core/lock_store.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/migrate.py` & `rasa-3.6.0a1/rasa/core/migrate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/nlg/callback.py` & `rasa-3.6.0a1/rasa/core/nlg/callback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/nlg/generator.py` & `rasa-3.6.0a1/rasa/core/nlg/generator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/nlg/interpolator.py` & `rasa-3.6.0a1/rasa/core/nlg/interpolator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/nlg/response.py` & `rasa-3.6.0a1/rasa/core/nlg/response.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/policies/ensemble.py` & `rasa-3.6.0a1/rasa/core/policies/ensemble.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/policies/memoization.py` & `rasa-3.6.0a1/rasa/core/policies/memoization.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/policies/policy.py` & `rasa-3.6.0a1/rasa/core/policies/policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/policies/rule_policy.py` & `rasa-3.6.0a1/rasa/core/policies/rule_policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/policies/ted_policy.py` & `rasa-3.6.0a1/rasa/core/policies/ted_policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/policies/unexpected_intent_policy.py` & `rasa-3.6.0a1/rasa/core/policies/unexpected_intent_policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/processor.py` & `rasa-3.6.0a1/rasa/core/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 import os
 from pathlib import Path
 import tarfile
-import tempfile
 import time
 from types import LambdaType
 from typing import Any, Dict, List, Optional, Text, Tuple, Union
 
 from rasa.core.http_interpreter import RasaNLUHttpInterpreter
 from rasa.engine import loader
 from rasa.engine.constants import PLACEHOLDER_MESSAGE, PLACEHOLDER_TRACKER
@@ -51,14 +50,15 @@
     DOCS_URL_DOMAINS,
     DEFAULT_SENDER_ID,
     DOCS_URL_POLICIES,
     UTTER_PREFIX,
 )
 from rasa.core.nlg import NaturalLanguageGenerator
 from rasa.core.lock_store import LockStore
+from rasa.utils.common import TempDirectoryPath, get_temp_dir_name
 import rasa.core.tracker_store
 import rasa.core.actions.action
 import rasa.shared.core.trackers
 from rasa.shared.core.trackers import DialogueStateTracker, EventVerbosity
 from rasa.shared.nlu.constants import (
     ENTITIES,
     INTENT,
@@ -82,14 +82,15 @@
         tracker_store: rasa.core.tracker_store.TrackerStore,
         lock_store: LockStore,
         generator: NaturalLanguageGenerator,
         action_endpoint: Optional[EndpointConfig] = None,
         max_number_of_predictions: int = MAX_NUMBER_OF_PREDICTIONS,
         on_circuit_break: Optional[LambdaType] = None,
         http_interpreter: Optional[RasaNLUHttpInterpreter] = None,
+        anonymization_pipeline: Optional[Any] = None,
     ) -> None:
         """Initializes a `MessageProcessor`."""
         self.nlg = generator
         self.tracker_store = tracker_store
         self.lock_store = lock_store
         self.max_number_of_predictions = max_number_of_predictions
         self.on_circuit_break = on_circuit_break
@@ -107,14 +108,15 @@
                 f"streaming events without a unique assistant identifier.",
                 UserWarning,
             )
 
         self.model_path = Path(model_path)
         self.domain = self.model_metadata.domain
         self.http_interpreter = http_interpreter
+        self.anonymization_pipeline = anonymization_pipeline
 
     @staticmethod
     def _load_model(
         model_path: Union[Text, Path]
     ) -> Tuple[Text, ModelMetadata, GraphRunner]:
         """Unpacks a model from a given path using the graph model loader."""
         try:
@@ -125,15 +127,15 @@
                 if not model_file_path:
                     raise ModelNotFound(f"No model found at path '{model_path}'.")
                 model_tar = model_file_path
         except TypeError:
             raise ModelNotFound(f"Model {model_path} can not be loaded.")
 
         logger.info(f"Loading model {model_tar}...")
-        with tempfile.TemporaryDirectory() as temporary_directory:
+        with TempDirectoryPath(get_temp_dir_name()) as temporary_directory:
             try:
                 metadata, runner = loader.load_predict_graph_runner(
                     Path(temporary_directory),
                     Path(model_tar),
                     LocalModelStorage,
                     DaskGraphRunner,
                 )
@@ -156,14 +158,16 @@
             )
             return None
 
         tracker = await self.run_action_extract_slots(message.output_channel, tracker)
 
         await self._run_prediction_loop(message.output_channel, tracker)
 
+        await self.run_anonymization_pipeline(tracker)
+
         await self.save_tracker(tracker)
 
         if isinstance(message.output_channel, CollectingOutputChannel):
             return message.output_channel.messages
 
         return None
 
@@ -194,14 +198,33 @@
         logger.debug(
             f"Default action '{ACTION_EXTRACT_SLOTS}' was executed, "
             f"resulting in {len(extraction_events)} events: {events_as_str}"
         )
 
         return tracker
 
+    async def run_anonymization_pipeline(self, tracker: DialogueStateTracker) -> None:
+        """Run the anonymization pipeline on the new tracker events.
+
+        Args:
+            tracker: A tracker representing a conversation state.
+        """
+        if self.anonymization_pipeline is None:
+            return None
+
+        old_tracker = await self.tracker_store.retrieve(tracker.sender_id)
+        new_events = rasa.shared.core.trackers.TrackerEventDiffEngine.event_difference(
+            old_tracker, tracker
+        )
+
+        for event in new_events:
+            body = {"sender_id": tracker.sender_id}
+            body.update(event.as_dict())
+            self.anonymization_pipeline.run(body)
+
     async def predict_next_for_sender_id(
         self, sender_id: Text
     ) -> Optional[Dict[Text, Any]]:
         """Predict the next action for the given sender_id.
 
         Args:
             sender_id: Conversation ID.
@@ -663,55 +686,69 @@
         self, action_name: Text
     ) -> Optional[rasa.core.actions.action.Action]:
         return rasa.core.actions.action.action_for_name_or_text(
             action_name, self.domain, self.action_endpoint
         )
 
     async def parse_message(
-        self, message: UserMessage, only_output_properties: bool = True
+        self,
+        message: UserMessage,
+        tracker: Optional[DialogueStateTracker] = None,
+        only_output_properties: bool = True,
     ) -> Dict[Text, Any]:
         """Interprets the passed message.
 
         Args:
             message: Message to handle.
+            tracker: Tracker to use.
             only_output_properties: If `True`, restrict the output to
                 Message.only_output_properties.
 
         Returns:
             Parsed data extracted from the message.
         """
         if self.http_interpreter:
             parse_data = await self.http_interpreter.parse(message)
         else:
-            parse_data = self._parse_message_with_graph(message, only_output_properties)
+            if tracker is None:
+                tracker = DialogueStateTracker.from_events(message.sender_id, [])
+            parse_data = self._parse_message_with_graph(
+                message, tracker, only_output_properties
+            )
 
         logger.debug(
             "Received user message '{}' with intent '{}' "
             "and entities '{}'".format(
                 parse_data["text"], parse_data["intent"], parse_data["entities"]
             )
         )
 
         self._check_for_unseen_features(parse_data)
 
         return parse_data
 
     def _parse_message_with_graph(
-        self, message: UserMessage, only_output_properties: bool = True
+        self,
+        message: UserMessage,
+        tracker: DialogueStateTracker,
+        only_output_properties: bool = True,
     ) -> Dict[Text, Any]:
         """Interprets the passed message.
 
         Arguments:
             message: Message to handle
+            tracker: Tracker to use
+            only_output_properties: If `True`, restrict the output to
+                Message.only_output_properties.
 
         Returns:
             Parsed data extracted from the message.
         """
         results = self.graph_runner.run(
-            inputs={PLACEHOLDER_MESSAGE: [message]},
+            inputs={PLACEHOLDER_MESSAGE: [message], PLACEHOLDER_TRACKER: tracker},
             targets=[self.model_metadata.nlu_target],
         )
         parsed_messages = results[self.model_metadata.nlu_target]
         parsed_message = parsed_messages[0]
         parse_data = {
             TEXT: "",
             INTENT: {INTENT_NAME_KEY: None, PREDICTED_CONFIDENCE_KEY: 0.0},
@@ -725,15 +762,15 @@
     async def _handle_message_with_tracker(
         self, message: UserMessage, tracker: DialogueStateTracker
     ) -> None:
 
         if message.parse_data:
             parse_data = message.parse_data
         else:
-            parse_data = await self.parse_message(message)
+            parse_data = await self.parse_message(message, tracker)
 
         # don't ever directly mutate the tracker
         # - instead pass its events to log
         tracker.update(
             UserUttered(
                 message.text,
                 parse_data["intent"],
```

### Comparing `rasa-3.5.9/rasa/core/run.py` & `rasa-3.6.0a1/rasa/core/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/test.py` & `rasa-3.6.0a1/rasa/core/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/tracker_store.py` & `rasa-3.6.0a1/rasa/core/tracker_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 from rasa.shared.core.conversation import Dialogue
 from rasa.shared.core.domain import Domain
 from rasa.shared.core.events import SessionStarted, Event
 from rasa.shared.core.trackers import (
     ActionExecuted,
     DialogueStateTracker,
     EventVerbosity,
+    TrackerEventDiffEngine,
 )
 from rasa.shared.exceptions import ConnectionException, RasaException
 from rasa.shared.nlu.constants import INTENT_NAME_KEY
 from rasa.utils.endpoints import EndpointConfig
 import sqlalchemy as sa
 from sqlalchemy.ext.declarative import declarative_base, DeclarativeMeta
 
@@ -314,17 +315,16 @@
 
     async def stream_events(self, tracker: DialogueStateTracker) -> None:
         """Streams events to a message broker."""
         if self.event_broker is None:
             logger.debug("No event broker configured. Skipping streaming events.")
             return None
 
-        offset = await self.number_of_existing_events(tracker.sender_id)
-        events = tracker.events
-        new_events = list(itertools.islice(events, offset, len(events)))
+        old_tracker = await self.retrieve(tracker.sender_id)
+        new_events = TrackerEventDiffEngine.event_difference(old_tracker, tracker)
 
         await self._stream_new_events(self.event_broker, new_events, tracker.sender_id)
 
     async def _stream_new_events(
         self,
         event_broker: EventBroker,
         new_events: List[Event],
@@ -332,20 +332,14 @@
     ) -> None:
         """Publishes new tracker events to a message broker."""
         for event in new_events:
             body = {"sender_id": sender_id}
             body.update(event.as_dict())
             event_broker.publish(body)
 
-    async def number_of_existing_events(self, sender_id: Text) -> int:
-        """Return number of stored events for a given sender id."""
-        old_tracker = await self.retrieve(sender_id)
-
-        return len(old_tracker.events) if old_tracker else 0
-
     async def keys(self) -> Iterable[Text]:
         """Returns the set of values for the tracker store's primary key."""
         raise NotImplementedError()
 
     def deserialise_tracker(
         self, sender_id: Text, serialised_tracker: Union[Text, bytes]
     ) -> Optional[DialogueStateTracker]:
@@ -774,22 +768,22 @@
         self,
         domain: Domain,
         host: Optional[Text] = "mongodb://localhost:27017",
         db: Optional[Text] = "rasa",
         username: Optional[Text] = None,
         password: Optional[Text] = None,
         auth_source: Optional[Text] = "admin",
-        collection: Optional[Text] = "conversations",
+        collection: Text = "conversations",
         event_broker: Optional[EventBroker] = None,
         **kwargs: Dict[Text, Any],
     ) -> None:
         from pymongo.database import Database
         from pymongo import MongoClient
 
-        self.client = MongoClient(
+        self.client: MongoClient = MongoClient(
             host,
             username=username,
             password=password,
             authSource=auth_source,
             # delay connect until process forking is done
             connect=False,
         )
```

### Comparing `rasa-3.5.9/rasa/core/train.py` & `rasa-3.6.0a1/rasa/core/train.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/training/__init__.py` & `rasa-3.6.0a1/rasa/core/training/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/training/converters/responses_prefix_converter.py` & `rasa-3.6.0a1/rasa/core/training/converters/responses_prefix_converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/training/interactive.py` & `rasa-3.6.0a1/rasa/core/training/interactive.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/training/story_conflict.py` & `rasa-3.6.0a1/rasa/core/training/story_conflict.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/training/training.py` & `rasa-3.6.0a1/rasa/core/training/training.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/core/utils.py` & `rasa-3.6.0a1/rasa/core/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import json
 import logging
 import os
 from decimal import Decimal
 from pathlib import Path
-from typing import Any, Dict, Optional, Set, Text, Tuple, Union
+from typing import Any, Dict, List, Optional, Set, Text, Tuple, Union
 
 import numpy as np
 
 import rasa.shared.utils.io
 from rasa.constants import DEFAULT_SANIC_WORKERS, ENV_SANIC_WORKERS
+from rasa.plugin import plugin_manager
 from rasa.shared.constants import DEFAULT_ENDPOINTS_PATH, TCP_PROTOCOL
 
 from rasa.core.lock_store import LockStore, RedisLockStore, InMemoryLockStore
 from rasa.utils.endpoints import EndpointConfig, read_endpoint_config
 from sanic import Sanic
 from socket import SOCK_DGRAM, SOCK_STREAM
 import rasa.cli.utils as cli_utils
@@ -131,16 +132,16 @@
 
 
 def extract_args(
     kwargs: Dict[Text, Any], keys_to_extract: Set[Text]
 ) -> Tuple[Dict[Text, Any], Dict[Text, Any]]:
     """Go through the kwargs and filter out the specified keys.
 
-    Return both, the filtered kwargs as well as the remaining kwargs."""
-
+    Return both, the filtered kwargs as well as the remaining kwargs.
+    """
     remaining = {}
     extracted = {}
     for k, v in kwargs.items():
         if k in keys_to_extract:
             extracted[k] = v
         else:
             remaining[k] = v
@@ -168,43 +169,64 @@
 
 
 class AvailableEndpoints:
     """Collection of configured endpoints."""
 
     @classmethod
     def read_endpoints(cls, endpoint_file: Text) -> "AvailableEndpoints":
+        """Read the different endpoints from a yaml file."""
         nlg = read_endpoint_config(endpoint_file, endpoint_type="nlg")
         nlu = read_endpoint_config(endpoint_file, endpoint_type="nlu")
         action = read_endpoint_config(endpoint_file, endpoint_type="action_endpoint")
         model = read_endpoint_config(endpoint_file, endpoint_type="models")
         tracker_store = read_endpoint_config(
             endpoint_file, endpoint_type="tracker_store"
         )
         lock_store = read_endpoint_config(endpoint_file, endpoint_type="lock_store")
         event_broker = read_endpoint_config(endpoint_file, endpoint_type="event_broker")
 
-        return cls(nlg, nlu, action, model, tracker_store, lock_store, event_broker)
+        anonymization_rules = plugin_manager().hook.read_anonymization_rules(
+            endpoints_file=endpoint_file
+        )
+
+        # explicitly set to `None` if the list is empty
+        if not anonymization_rules:
+            anonymization_rules = None
+
+        return cls(
+            nlg,
+            nlu,
+            action,
+            model,
+            tracker_store,
+            lock_store,
+            event_broker,
+            anonymization_rules,
+        )
 
     def __init__(
         self,
         nlg: Optional[EndpointConfig] = None,
         nlu: Optional[EndpointConfig] = None,
         action: Optional[EndpointConfig] = None,
         model: Optional[EndpointConfig] = None,
         tracker_store: Optional[EndpointConfig] = None,
         lock_store: Optional[EndpointConfig] = None,
         event_broker: Optional[EndpointConfig] = None,
+        anonymization_rules: Optional[List[Any]] = None,
     ) -> None:
+        """Create an `AvailableEndpoints` object."""
         self.model = model
         self.action = action
         self.nlu = nlu
         self.nlg = nlg
         self.tracker_store = tracker_store
         self.lock_store = lock_store
         self.event_broker = event_broker
+        self.anonymization_rules = anonymization_rules
 
 
 def read_endpoints_from_path(
     endpoints_path: Optional[Union[Path, Text]] = None
 ) -> AvailableEndpoints:
     """Get `AvailableEndpoints` object from specified path.
```

### Comparing `rasa-3.5.9/rasa/core/visualize.py` & `rasa-3.6.0a1/rasa/core/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/engine/caching.py` & `rasa-3.6.0a1/rasa/engine/caching.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/engine/graph.py` & `rasa-3.6.0a1/rasa/engine/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -576,7 +576,8 @@
     train_schema: GraphSchema
     predict_schema: GraphSchema
     training_type: TrainingType
     assistant_id: Optional[Text]
     language: Optional[Text]
     core_target: Optional[Text]
     nlu_target: Optional[Text]
+    spaces: Optional[Dict[Text, Text]] = None
```

### Comparing `rasa-3.5.9/rasa/engine/loader.py` & `rasa-3.6.0a1/rasa/engine/loader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/engine/recipes/config_files/default_config.yml` & `rasa-3.6.0a1/rasa/engine/recipes/config_files/default_config.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/engine/recipes/default_components.py` & `rasa-3.6.0a1/rasa/engine/recipes/default_components.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/engine/recipes/default_recipe.py` & `rasa-3.6.0a1/rasa/engine/recipes/default_recipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import dataclasses
 
 from rasa.core.featurizers.precomputation import (
     CoreFeaturizationInputConverter,
     CoreFeaturizationCollector,
 )
+from rasa.plugin import plugin_manager
 from rasa.shared.exceptions import FileNotFoundException
 from rasa.core.policies.ensemble import DefaultPolicyPredictionEnsemble
 
 from rasa.engine.graph import (
     GraphSchema,
     GraphComponent,
     SchemaNode,
@@ -221,14 +222,15 @@
 
         return GraphModelConfiguration(
             train_schema=GraphSchema(train_nodes),
             predict_schema=GraphSchema(predict_nodes),
             training_type=training_type,
             assistant_id=config.get(ASSISTANT_ID_KEY),
             language=config.get("language"),
+            spaces=config.get("spaces"),
             core_target=core_target,
             nlu_target=f"run_{RegexMessageHandler.__name__}",
         )
 
     def _create_train_nodes(
         self, config: Dict[Text, Any], cli_parameters: Dict[Text, Any]
     ) -> Tuple[Dict[Text, SchemaNode], List[Text]]:
@@ -276,14 +278,20 @@
 
     def _add_nlu_train_nodes(
         self,
         train_config: Dict[Text, Any],
         train_nodes: Dict[Text, SchemaNode],
         cli_parameters: Dict[Text, Any],
     ) -> List[Text]:
+        plugin_manager().hook.modify_default_recipe_graph_train_nodes(
+            train_config=train_config,
+            train_nodes=train_nodes,
+            cli_parameters=cli_parameters,
+        )
+
         persist_nlu_data = bool(cli_parameters.get("persist_nlu_training_data"))
         train_nodes["nlu_training_data_provider"] = SchemaNode(
             needs={"importer": "finetuning_validator"},
             uses=NLUTrainingDataProvider,
             constructor_name="create",
             fn="provide",
             config={
@@ -523,14 +531,19 @@
     def _add_core_train_nodes(
         self,
         train_config: Dict[Text, Any],
         train_nodes: Dict[Text, SchemaNode],
         preprocessors: List[Text],
         cli_parameters: Dict[Text, Any],
     ) -> None:
+        plugin_manager().hook.modify_default_recipe_graph_train_nodes(
+            train_config=train_config,
+            train_nodes=train_nodes,
+            cli_parameters=cli_parameters,
+        )
         train_nodes["domain_provider"] = SchemaNode(
             needs={"importer": "finetuning_validator"},
             uses=DomainProvider,
             constructor_name="create",
             fn="provide_train",
             config={},
             is_target=True,
@@ -699,14 +712,17 @@
     def _add_nlu_predict_nodes(
         self,
         last_run_node: Text,
         predict_config: Dict[Text, Any],
         predict_nodes: Dict[Text, SchemaNode],
         train_nodes: Dict[Text, SchemaNode],
     ) -> Text:
+        plugin_manager().hook.modify_default_recipe_graph_predict_nodes(
+            predict_nodes=predict_nodes
+        )
         for idx, config in enumerate(predict_config["pipeline"]):
             component_name = config.pop("name")
             component = self._from_registry(component_name)
             component_name = f"{component_name}{idx}"
             if self.ComponentType.MODEL_LOADER in component.types:
                 predict_nodes[f"provide_{component_name}"] = SchemaNode(
                     **DEFAULT_PREDICT_KWARGS,
@@ -808,14 +824,17 @@
     def _add_core_predict_nodes(
         self,
         predict_config: Dict[Text, Any],
         predict_nodes: Dict[Text, SchemaNode],
         train_nodes: Dict[Text, SchemaNode],
         preprocessors: List[Text],
     ) -> None:
+        plugin_manager().hook.modify_default_recipe_graph_predict_nodes(
+            predict_nodes=predict_nodes
+        )
         predict_nodes["domain_provider"] = SchemaNode(
             **DEFAULT_PREDICT_KWARGS,
             needs={},
             uses=DomainProvider,
             fn="provide_inference",
             config={},
             resource=Resource("domain_provider"),
```

### Comparing `rasa-3.5.9/rasa/engine/recipes/graph_recipe.py` & `rasa-3.6.0a1/rasa/engine/recipes/graph_recipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,10 +69,11 @@
 
         return GraphModelConfiguration(
             train_schema=GraphSchema.from_dict(config.get("train_schema")),
             predict_schema=GraphSchema.from_dict(config.get("predict_schema")),
             training_type=training_type,
             assistant_id=config.get(ASSISTANT_ID_KEY),
             language=config.get("language"),
+            spaces=config.get("spaces"),
             core_target=core_target,
             nlu_target=nlu_target,
         )
```

### Comparing `rasa-3.5.9/rasa/engine/recipes/recipe.py` & `rasa-3.6.0a1/rasa/engine/recipes/recipe.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/engine/runner/dask.py` & `rasa-3.6.0a1/rasa/engine/runner/dask.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/engine/runner/interface.py` & `rasa-3.6.0a1/rasa/engine/runner/interface.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/engine/storage/local_model_storage.py` & `rasa-3.6.0a1/rasa/engine/storage/local_model_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,11 +237,12 @@
             model_id=uuid.uuid4().hex,
             assistant_id=model_configuration.assistant_id,
             domain=domain,
             train_schema=model_configuration.train_schema,
             predict_schema=model_configuration.predict_schema,
             training_type=model_configuration.training_type,
             project_fingerprint=rasa.model.project_fingerprint(),
+            spaces=model_configuration.spaces,
             language=model_configuration.language,
             core_target=model_configuration.core_target,
             nlu_target=model_configuration.nlu_target,
         )
```

### Comparing `rasa-3.5.9/rasa/engine/storage/resource.py` & `rasa-3.6.0a1/rasa/engine/storage/resource.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/engine/storage/storage.py` & `rasa-3.6.0a1/rasa/engine/storage/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import abc
 import logging
 import typing
 from contextlib import contextmanager
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
-from typing import Tuple, Union, Text, Generator, Dict, Any, Optional
+from typing import List, Tuple, Union, Text, Generator, Dict, Any, Optional
 from packaging import version
 
 from rasa.constants import MINIMUM_COMPATIBLE_VERSION
 from rasa.exceptions import UnsupportedModelVersionError
 from rasa.engine.storage.resource import Resource
 from rasa.shared.core.domain import Domain
 from rasa.shared.data import TrainingType
@@ -136,14 +136,15 @@
     domain: Domain
     train_schema: GraphSchema
     predict_schema: GraphSchema
     project_fingerprint: Text
     core_target: Optional[Text]
     nlu_target: Text
     language: Optional[Text]
+    spaces: Optional[List[Dict[Text, Any]]] = None
     training_type: TrainingType = TrainingType.BOTH
 
     def __post_init__(self) -> None:
         """Raises an exception when the metadata indicates an unsupported version.
 
         Raises:
             `UnsupportedModelException` if the `rasa_open_source_version` is lower
@@ -165,14 +166,15 @@
             "train_schema": self.train_schema.as_dict(),
             "predict_schema": self.predict_schema.as_dict(),
             "training_type": self.training_type.value,
             "project_fingerprint": self.project_fingerprint,
             "core_target": self.core_target,
             "nlu_target": self.nlu_target,
             "language": self.language,
+            "spaces": self.spaces,
         }
 
     @classmethod
     def from_dict(cls, serialized: Dict[Text, Any]) -> ModelMetadata:
         """Loads `ModelMetadata` which has been serialized using `metadata.as_dict()`.
 
         Args:
@@ -192,8 +194,10 @@
             train_schema=GraphSchema.from_dict(serialized["train_schema"]),
             predict_schema=GraphSchema.from_dict(serialized["predict_schema"]),
             training_type=TrainingType(serialized["training_type"]),
             project_fingerprint=serialized["project_fingerprint"],
             core_target=serialized["core_target"],
             nlu_target=serialized["nlu_target"],
             language=serialized["language"],
+            # optional, since introduced later
+            spaces=serialized.get("spaces"),
         )
```

### Comparing `rasa-3.5.9/rasa/engine/training/components.py` & `rasa-3.6.0a1/rasa/engine/training/components.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/engine/training/fingerprinting.py` & `rasa-3.6.0a1/rasa/engine/training/fingerprinting.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/engine/training/graph_trainer.py` & `rasa-3.6.0a1/rasa/engine/training/graph_trainer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/engine/training/hooks.py` & `rasa-3.6.0a1/rasa/engine/training/hooks.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/engine/validation.py` & `rasa-3.6.0a1/rasa/engine/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,16 +432,17 @@
                 f"your component correctly and and that your model configuration is "
                 f"valid."
                 f"See {DOCS_URL_GRAPH_COMPONENTS} for more information."
             )
 
         if not _is_placeholder_input(parent_name) and parent_name not in graph.nodes:
             raise GraphSchemaValidationException(
+                f"Missing graph component '{parent_name}'."
                 f"Your model uses a component '{node.uses.__name__}' which expects "
-                f"input from a previous component but this component is not part of "
+                f"input from the missing component. The component is missing from "
                 f"your model configuration. Please make sure that you registered "
                 f"your component correctly and and that your model configuration is "
                 f"valid."
                 f"See {DOCS_URL_GRAPH_COMPONENTS} for more information."
             )
 
         required_type = available_args.get(param_name)
```

### Comparing `rasa-3.5.9/rasa/exceptions.py` & `rasa-3.6.0a1/rasa/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/graph_components/converters/nlu_message_converter.py` & `rasa-3.6.0a1/rasa/graph_components/converters/nlu_message_converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/graph_components/providers/domain_for_core_training_provider.py` & `rasa-3.6.0a1/rasa/graph_components/providers/domain_for_core_training_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/graph_components/providers/domain_provider.py` & `rasa-3.6.0a1/rasa/graph_components/providers/domain_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/graph_components/providers/forms_provider.py` & `rasa-3.6.0a1/rasa/graph_components/providers/forms_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/graph_components/providers/nlu_training_data_provider.py` & `rasa-3.6.0a1/rasa/graph_components/providers/nlu_training_data_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/graph_components/providers/responses_provider.py` & `rasa-3.6.0a1/rasa/graph_components/providers/responses_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/graph_components/providers/rule_only_provider.py` & `rasa-3.6.0a1/rasa/graph_components/providers/rule_only_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/graph_components/providers/story_graph_provider.py` & `rasa-3.6.0a1/rasa/graph_components/providers/story_graph_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/graph_components/providers/training_tracker_provider.py` & `rasa-3.6.0a1/rasa/graph_components/providers/training_tracker_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/graph_components/validators/default_recipe_validator.py` & `rasa-3.6.0a1/rasa/graph_components/validators/default_recipe_validator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/graph_components/validators/finetuning_validator.py` & `rasa-3.6.0a1/rasa/graph_components/validators/finetuning_validator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/jupyter.py` & `rasa-3.6.0a1/rasa/jupyter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/model.py` & `rasa-3.6.0a1/rasa/model.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/model_testing.py` & `rasa-3.6.0a1/rasa/model_testing.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/model_training.py` & `rasa-3.6.0a1/rasa/model_training.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         finetuning_epoch_fraction: The fraction currently specified training epochs
             in the model configuration which should be used for finetuning.
 
     Returns:
         An instance of `TrainingResult`.
     """
     file_importer = TrainingDataImporter.load_from_config(
-        config, domain, training_files
+        config, domain, training_files, core_additional_arguments
     )
 
     stories = file_importer.get_stories()
     nlu_data = file_importer.get_nlu_data()
 
     training_type = TrainingType.BOTH
 
@@ -353,15 +353,15 @@
             in the model configuration which should be used for finetuning.
 
     Returns:
         Path to the model archive.
 
     """
     file_importer = TrainingDataImporter.load_core_importer_from_config(
-        config, domain, [stories]
+        config, domain, [stories], additional_arguments
     )
     stories_data = file_importer.get_stories()
     nlu_data = file_importer.get_nlu_data()
     domain = file_importer.get_domain()
 
     if nlu_data.has_e2e_examples():
         rasa.shared.utils.cli.print_error(
@@ -434,15 +434,15 @@
             "No NLU data given. Please provide NLU data in order to train "
             "a Rasa NLU model using the '--nlu' argument."
         )
         return None
 
     # training NLU only hence the training files still have to be selected
     file_importer = TrainingDataImporter.load_nlu_importer_from_config(
-        config, domain, training_data_paths=[nlu_data]
+        config, domain, training_data_paths=[nlu_data], args=additional_arguments
     )
 
     training_data = file_importer.get_nlu_data()
     if training_data.contains_no_pure_nlu_data():
         rasa.shared.utils.cli.print_error(
             f"Path '{nlu_data}' doesn't contain valid NLU data in it. "
             f"Please verify the data format. "
```

### Comparing `rasa-3.5.9/rasa/nlu/classifiers/diet_classifier.py` & `rasa-3.6.0a1/rasa/nlu/classifiers/diet_classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,15 +414,14 @@
 
     # training data helpers:
     @staticmethod
     def _label_id_index_mapping(
         training_data: TrainingData, attribute: Text
     ) -> Dict[Text, int]:
         """Create label_id dictionary."""
-
         distinct_label_ids = {
             example.get(attribute) for example in training_data.intent_examples
         } - {None}
         return {
             label_id: idx for idx, label_id in enumerate(sorted(distinct_label_ids))
         }
 
@@ -430,15 +429,14 @@
     def _invert_mapping(mapping: Dict) -> Dict:
         return {value: key for key, value in mapping.items()}
 
     def _create_entity_tag_specs(
         self, training_data: TrainingData
     ) -> List[EntityTagSpec]:
         """Create entity tag specifications with their respective tag id mappings."""
-
         _tag_specs = []
 
         for tag_name in POSSIBLE_TAGS:
             if self.component_config[BILOU_FLAG]:
                 tag_id_index_mapping = bilou_utils.build_tag_id_dict(
                     training_data, tag_name
                 )
@@ -494,15 +492,14 @@
                 return ex
         return None
 
     def _check_labels_features_exist(
         self, labels_example: List[Message], attribute: Text
     ) -> bool:
         """Checks if all labels have features set."""
-
         return all(
             label_example.features_present(
                 attribute, self.component_config[FEATURIZERS]
             )
             for label_example in labels_example
         )
```

### Comparing `rasa-3.5.9/rasa/nlu/classifiers/fallback_classifier.py` & `rasa-3.6.0a1/rasa/nlu/classifiers/fallback_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/classifiers/keyword_intent_classifier.py` & `rasa-3.6.0a1/rasa/nlu/classifiers/keyword_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/classifiers/logistic_regression_classifier.py` & `rasa-3.6.0a1/rasa/nlu/classifiers/logistic_regression_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/classifiers/mitie_intent_classifier.py` & `rasa-3.6.0a1/rasa/nlu/classifiers/mitie_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/classifiers/regex_message_handler.py` & `rasa-3.6.0a1/rasa/nlu/classifiers/regex_message_handler.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/classifiers/sklearn_intent_classifier.py` & `rasa-3.6.0a1/rasa/nlu/classifiers/sklearn_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/constants.py` & `rasa-3.6.0a1/rasa/nlu/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/convert.py` & `rasa-3.6.0a1/rasa/nlu/convert.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/emulators/dialogflow.py` & `rasa-3.6.0a1/rasa/nlu/emulators/dialogflow.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/emulators/emulator.py` & `rasa-3.6.0a1/rasa/nlu/emulators/emulator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/emulators/luis.py` & `rasa-3.6.0a1/rasa/nlu/emulators/luis.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/emulators/wit.py` & `rasa-3.6.0a1/rasa/nlu/emulators/wit.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/extractors/crf_entity_extractor.py` & `rasa-3.6.0a1/rasa/nlu/extractors/crf_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/extractors/duckling_entity_extractor.py` & `rasa-3.6.0a1/rasa/nlu/extractors/duckling_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/extractors/entity_synonyms.py` & `rasa-3.6.0a1/rasa/nlu/extractors/entity_synonyms.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/extractors/extractor.py` & `rasa-3.6.0a1/rasa/nlu/extractors/extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/extractors/mitie_entity_extractor.py` & `rasa-3.6.0a1/rasa/nlu/extractors/mitie_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/extractors/regex_entity_extractor.py` & `rasa-3.6.0a1/rasa/nlu/extractors/regex_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/extractors/spacy_entity_extractor.py` & `rasa-3.6.0a1/rasa/nlu/extractors/spacy_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/featurizers/featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py` & `rasa-3.6.0a1/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/model.py` & `rasa-3.6.0a1/rasa/nlu/model.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/persistor.py` & `rasa-3.6.0a1/rasa/nlu/persistor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/run.py` & `rasa-3.6.0a1/rasa/nlu/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/selectors/response_selector.py` & `rasa-3.6.0a1/rasa/nlu/selectors/response_selector.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/test.py` & `rasa-3.6.0a1/rasa/nlu/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import itertools
 import os
 import logging
-import tempfile
 from pathlib import Path
 
 import numpy as np
 from collections import defaultdict, namedtuple
 from tqdm import tqdm
 from typing import (
     Iterable,
@@ -22,19 +21,20 @@
     TYPE_CHECKING,
 )
 
 from rasa import telemetry
 from rasa.core.agent import Agent
 from rasa.core.channels import UserMessage
 from rasa.core.processor import MessageProcessor
+from rasa.plugin import plugin_manager
 from rasa.shared.nlu.training_data.training_data import TrainingData
+from rasa.utils.common import TempDirectoryPath, get_temp_dir_name
 import rasa.shared.utils.io
 import rasa.utils.plotting as plot_utils
 import rasa.utils.io as io_utils
-import rasa.utils.common
 
 from rasa.constants import TEST_DATA_FILE, TRAIN_DATA_FILE, NLG_DATA_FILE
 import rasa.nlu.classifiers.fallback_classifier
 from rasa.nlu.constants import (
     RESPONSE_SELECTOR_DEFAULT_INTENT,
     RESPONSE_SELECTOR_PROPERTY_NAME,
     RESPONSE_SELECTOR_PREDICTION_KEY,
@@ -148,17 +148,17 @@
     response_results: List[ResponseSelectionEvaluationResult],
 ) -> List[ResponseSelectionEvaluationResult]:
     """Remove those examples without a response.
 
     Args:
         response_results: response selection evaluation results
 
-    Returns: response selection evaluation results
+    Returns:
+        Response selection evaluation results
     """
-
     filtered = []
     for r in response_results:
         # substitute None values with empty string
         # to enable sklearn evaluation
         if r.intent_response_key_prediction is None:
             r = r._replace(intent_response_key_prediction="")
 
@@ -263,15 +263,14 @@
 ) -> None:
     """Write successful response selection predictions to a file.
 
     Args:
         response_results: response selection evaluation result
         successes_filename: filename of file to save successful predictions to
     """
-
     successes = [
         {
             "text": r.message,
             "intent_response_key_target": r.intent_response_key_target,
             "intent_response_key_prediction": {
                 "name": r.intent_response_key_prediction,
                 "confidence": r.confidence,
@@ -700,17 +699,17 @@
     Takes the aligned prediction labels which are grouped for each message
     and concatenates them.
 
     Args:
         aligned_predictions: aligned predictions
         extractor: entity extractor name
 
-    Returns: concatenated predictions
+    Returns:
+        Concatenated predictions
     """
-
     if extractor:
         label_lists = [ap["extractor_labels"][extractor] for ap in aligned_predictions]
     else:
         label_lists = [ap["target_labels"] for ap in aligned_predictions]
 
     return list(itertools.chain(*label_lists))
 
@@ -723,17 +722,17 @@
     Takes the aligned prediction confidences which are grouped for each message
     and concatenates them.
 
     Args:
         aligned_predictions: aligned predictions
         extractor: entity extractor name
 
-    Returns: concatenated confidences
+    Returns:
+        Concatenated confidences
     """
-
     label_lists = [ap["confidences"][extractor] for ap in aligned_predictions]
     return list(itertools.chain(*label_lists))
 
 
 def substitute_labels(labels: List[Text], old: Text, new: Text) -> List[Text]:
     """Replaces label names in a list of labels.
 
@@ -873,38 +872,46 @@
 
     for extractor in extractors:
         merged_predictions = merge_labels(aligned_predictions, extractor)
         merged_predictions = substitute_labels(
             merged_predictions, NO_ENTITY_TAG, NO_ENTITY
         )
 
+        cleaned_targets = plugin_manager().hook.clean_entity_targets_for_evaluation(
+            merged_targets=merged_targets, extractor=extractor
+        )
+        if len(cleaned_targets) > 0:
+            cleaned_targets = cleaned_targets[0]
+        else:
+            cleaned_targets = merged_targets
+
         logger.info(f"Evaluation for entity extractor: {extractor} ")
 
         report, precision, f1, accuracy, confusion_matrix, labels = _calculate_report(
             output_directory,
-            merged_targets,
+            cleaned_targets,
             merged_predictions,
             report_as_dict,
             exclude_label=NO_ENTITY,
         )
         if output_directory:
 
             _dump_report(output_directory, f"{extractor}_report.json", report)
 
         if successes:
             successes_filename = f"{extractor}_successes.json"
             if output_directory:
                 successes_filename = os.path.join(output_directory, successes_filename)
             # save classified samples to file for debugging
             write_successful_entity_predictions(
-                entity_results, merged_targets, merged_predictions, successes_filename
+                entity_results, cleaned_targets, merged_predictions, successes_filename
             )
 
         entity_errors = collect_incorrect_entity_predictions(
-            entity_results, merged_predictions, merged_targets
+            entity_results, merged_predictions, cleaned_targets
         )
         if errors and output_directory:
             errors_filename = os.path.join(output_directory, f"{extractor}_errors.json")
 
             _write_errors(entity_errors, errors_filename, "entity")
 
         if not disable_plotting:
@@ -924,15 +931,15 @@
                 merged_confidences = merge_confidences(aligned_predictions, extractor)
                 histogram_filename = f"{extractor}_histogram.png"
                 if output_directory:
                     histogram_filename = os.path.join(
                         output_directory, histogram_filename
                     )
                 plot_entity_confidences(
-                    merged_targets,
+                    cleaned_targets,
                     merged_predictions,
                     merged_confidences,
                     title="Entity Prediction Confidence Distribution",
                     hist_filename=histogram_filename,
                 )
 
         result[extractor] = {
@@ -949,22 +956,20 @@
 def is_token_within_entity(token: Token, entity: Dict) -> bool:
     """Checks if a token is within the boundaries of an entity."""
     return determine_intersection(token, entity) == len(token.text)
 
 
 def does_token_cross_borders(token: Token, entity: Dict) -> bool:
     """Checks if a token crosses the boundaries of an entity."""
-
     num_intersect = determine_intersection(token, entity)
     return 0 < num_intersect < len(token.text)
 
 
 def determine_intersection(token: Token, entity: Dict) -> int:
     """Calculates how many characters a given token and entity share."""
-
     pos_token = set(range(token.start, token.end))
     pos_entity = set(range(entity["start"], entity["end"]))
     return len(pos_token.intersection(pos_entity))
 
 
 def do_entities_overlap(entities: List[Dict]) -> bool:
     """Checks if entities overlap.
@@ -1012,16 +1017,15 @@
             )
     return candidates
 
 
 def pick_best_entity_fit(
     token: Token, candidates: List[Dict[Text, Any]]
 ) -> Optional[Dict[Text, Any]]:
-    """
-    Determines the best fitting entity given intersecting entities.
+    """Determines the best fitting entity given intersecting entities.
 
     Args:
         token: a single token
         candidates: entities found by a single extractor
         attribute_key: the attribute key of interest
 
     Returns:
@@ -1038,16 +1042,15 @@
 
 def determine_token_labels(
     token: Token,
     entities: List[Dict],
     extractors: Optional[Set[Text]] = None,
     attribute_key: Text = ENTITY_ATTRIBUTE_TYPE,
 ) -> Text:
-    """
-    Determines the token label for the provided attribute key given entities that do
+    """Determines the token label for the provided attribute key given entities that do
     not overlap.
 
     Args:
         token: a single token
         entities: entities found by a single extractor
         extractors: list of extractors
         attribute_key: the attribute key for which the entity type should be returned
@@ -1068,16 +1071,15 @@
 
 
 def determine_entity_for_token(
     token: Token,
     entities: List[Dict[Text, Any]],
     extractors: Optional[Set[Text]] = None,
 ) -> Optional[Dict[Text, Any]]:
-    """
-    Determines the best fitting entity for the given token, given entities that do
+    """Determines the best fitting entity for the given token, given entities that do
     not overlap.
 
     Args:
         token: a single token
         entities: entities found by a single extractor
         extractors: list of extractors
 
@@ -1274,16 +1276,27 @@
     }
     intent_labels = {e.get(INTENT) for e in test_data.intent_examples}
     should_eval_intents = len(intent_labels) >= 2
     should_eval_response_selection = len(response_labels) >= 2
     should_eval_entities = len(test_data.entity_examples) > 0
 
     for example in tqdm(test_data.nlu_examples):
+        tracker = plugin_manager().hook.mock_tracker_for_evaluation(
+            example=example, model_metadata=processor.model_metadata
+        )
+        # if the user overwrites the default implementation take the last tracker
+        if isinstance(tracker, list):
+            if len(tracker) > 0:
+                tracker = tracker[-1]
+            else:
+                tracker = None
         result = await processor.parse_message(
-            UserMessage(text=example.get(TEXT)), only_output_properties=False
+            UserMessage(text=example.get(TEXT)),
+            tracker=tracker,
+            only_output_properties=False,
         )
         _remove_entities_of_extractors(result, PRETRAINED_EXTRACTORS)
         if should_eval_intents:
             if fallback_classifier.is_fallback_classifier_prediction(result):
                 # Revert fallback prediction to not shadow
                 # the wrongly predicted intent
                 # during the test phase.
@@ -1454,15 +1467,14 @@
     return result
 
 
 def generate_folds(
     n: int, training_data: TrainingData
 ) -> Iterator[Tuple[TrainingData, TrainingData]]:
     """Generates n cross validation folds for given training data."""
-
     from sklearn.model_selection import StratifiedKFold
 
     skf = StratifiedKFold(n_splits=n, shuffle=True)
     x = training_data.intent_examples
 
     # Get labels as they appear in the training data because we want a
     # stratified split on all intents(including retrieval intents if they exist)
@@ -1586,15 +1598,15 @@
 
     Returns:
         dictionary with key, list structure, where each entry in list
               corresponds to the relevant result for one fold
     """
     import rasa.model_training
 
-    with tempfile.TemporaryDirectory() as temp_dir:
+    with TempDirectoryPath(get_temp_dir_name()) as temp_dir:
         tmp_path = Path(temp_dir)
 
         if isinstance(nlu_config, Dict):
             config_path = tmp_path / "config.yml"
             rasa.shared.utils.io.write_yaml(nlu_config, config_path)
             nlu_config = str(config_path)
 
@@ -1638,14 +1650,15 @@
                 processor,
                 test,
                 intent_test_results,
                 entity_test_results,
                 response_selection_test_results,
             )
 
+        intent_evaluation = {}
         if intent_test_results:
             logger.info("Accumulated test folds intent evaluation results:")
             intent_evaluation = evaluate_intents(
                 intent_test_results,
                 output,
                 successes,
                 errors,
@@ -1766,16 +1779,15 @@
     data: TrainingData,
     exclusion_percentages: List[int],
     f_score_results: Dict[Text, List[List[float]]],
     model_names: List[Text],
     output: Text,
     runs: int,
 ) -> List[int]:
-    """
-    Trains and compares multiple NLU models.
+    """Trains and compares multiple NLU models.
     For each run and exclusion percentage a model per config file is trained.
     Thereby, the model is trained only on the current percentage of training data.
     Afterwards, the model is tested on the complete test data of that run.
     All results are stored in the provided output directory.
 
     Args:
         configs: config files needed for training
```

### Comparing `rasa-3.5.9/rasa/nlu/tokenizers/jieba_tokenizer.py` & `rasa-3.6.0a1/rasa/nlu/tokenizers/jieba_tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
             "dictionary_path": None,
             # Flag to check whether to split intents
             "intent_tokenization_flag": False,
             # Symbol on which intent should be split
             "intent_split_symbol": "_",
             # Regular expression to detect tokens
             "token_pattern": None,
+            # Symbol on which prefix should be split
+            "prefix_separator_symbol": None,
         }
 
     def __init__(
         self, config: Dict[Text, Any], model_storage: ModelStorage, resource: Resource
     ) -> None:
         """Initialize the tokenizer."""
         super().__init__(config)
```

### Comparing `rasa-3.5.9/rasa/nlu/tokenizers/mitie_tokenizer.py` & `rasa-3.6.0a1/rasa/nlu/tokenizers/mitie_tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,16 @@
         return {
             # Flag to check whether to split intents
             "intent_tokenization_flag": False,
             # Symbol on which intent should be split
             "intent_split_symbol": "_",
             # Regular expression to detect tokens
             "token_pattern": None,
+            # Symbol on which prefix should be split
+            "prefix_separator_symbol": None,
         }
 
     @staticmethod
     def required_packages() -> List[Text]:
         """Any extra python dependencies required for this component to run."""
         return ["mitie"]
```

### Comparing `rasa-3.5.9/rasa/nlu/tokenizers/spacy_tokenizer.py` & `rasa-3.6.0a1/rasa/nlu/tokenizers/spacy_tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,16 @@
         return {
             # Flag to check whether to split intents
             "intent_tokenization_flag": False,
             # Symbol on which intent should be split
             "intent_split_symbol": "_",
             # Regular expression to detect tokens
             "token_pattern": None,
+            # Symbol on which prefix should be split
+            "prefix_separator_symbol": None,
         }
 
     @staticmethod
     def required_packages() -> List[Text]:
         """Any extra python dependencies required for this component to run."""
         return ["spacy"]
```

### Comparing `rasa-3.5.9/rasa/nlu/tokenizers/tokenizer.py` & `rasa-3.6.0a1/rasa/nlu/tokenizers/tokenizer.py`

 * *Files 22% similar despite different names*

```diff
@@ -98,14 +98,16 @@
         # split symbol for intents
         self.intent_split_symbol = config["intent_split_symbol"]
         # token pattern to further split tokens
         token_pattern = config.get("token_pattern")
         self.token_pattern_regex = None
         if token_pattern:
             self.token_pattern_regex = re.compile(token_pattern)
+        # split intent to prefix and suffix greedily, None means don't split
+        self.prefix_separator_symbol = config.get("prefix_separator_symbol")
 
     @classmethod
     def create(
         cls,
         config: Dict[Text, Any],
         model_storage: ModelStorage,
         resource: Resource,
@@ -157,28 +159,39 @@
             if self.intent_tokenization_flag
             else [text]
         )
 
         return words
 
     def _split_name(self, message: Message, attribute: Text = INTENT) -> List[Token]:
-        text = message.get(attribute)
+        orig_text = message.get(attribute)
+
+        if (
+            self.prefix_separator_symbol is not None
+            and self.prefix_separator_symbol in orig_text
+        ):
+            prefix, text = orig_text.split(self.prefix_separator_symbol, maxsplit=1)
+        else:
+            prefix, text = None, orig_text
 
         # for INTENT_RESPONSE_KEY attribute,
         # first split by RESPONSE_IDENTIFIER_DELIMITER
         if attribute == INTENT_RESPONSE_KEY:
             intent, response_key = text.split(RESPONSE_IDENTIFIER_DELIMITER)
             words = self._tokenize_on_split_symbol(
                 intent
             ) + self._tokenize_on_split_symbol(response_key)
 
         else:
             words = self._tokenize_on_split_symbol(text)
 
-        return self._convert_words_to_tokens(words, text)
+        if prefix is not None:
+            words = self._tokenize_on_split_symbol(prefix) + words
+
+        return self._convert_words_to_tokens(words, orig_text)
 
     def _apply_token_pattern(self, tokens: List[Token]) -> List[Token]:
         """Apply the token pattern to the given tokens.
 
         Args:
             tokens: list of tokens to split
```

### Comparing `rasa-3.5.9/rasa/nlu/tokenizers/whitespace_tokenizer.py` & `rasa-3.6.0a1/rasa/nlu/tokenizers/whitespace_tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,16 @@
         return {
             # Flag to check whether to split intents
             "intent_tokenization_flag": False,
             # Symbol on which intent should be split
             "intent_split_symbol": "_",
             # Regular expression to detect tokens
             "token_pattern": None,
+            # Symbol on which prefix should be split
+            "prefix_separator_symbol": None,
         }
 
     def __init__(self, config: Dict[Text, Any]) -> None:
         """Initialize the tokenizer."""
         super().__init__(config)
         self.emoji_pattern = rasa.utils.io.get_emoji_regex()
```

### Comparing `rasa-3.5.9/rasa/nlu/utils/__init__.py` & `rasa-3.6.0a1/rasa/nlu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/utils/bilou_utils.py` & `rasa-3.6.0a1/rasa/nlu/utils/bilou_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/utils/hugging_face/registry.py` & `rasa-3.6.0a1/rasa/nlu/utils/hugging_face/registry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py` & `rasa-3.6.0a1/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/utils/mitie_utils.py` & `rasa-3.6.0a1/rasa/nlu/utils/mitie_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/utils/pattern_utils.py` & `rasa-3.6.0a1/rasa/nlu/utils/pattern_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/nlu/utils/spacy_utils.py` & `rasa-3.6.0a1/rasa/nlu/utils/spacy_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/server.py` & `rasa-3.6.0a1/rasa/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import asyncio
 import concurrent.futures
 import logging
 import multiprocessing
 import os
-import tempfile
 import traceback
 from collections import defaultdict
 from functools import reduce, wraps
 from inspect import isawaitable
 from pathlib import Path
 from http import HTTPStatus
 from typing import (
@@ -62,14 +61,15 @@
     CollectingOutputChannel,
     OutputChannel,
     UserMessage,
 )
 import rasa.shared.core.events
 from rasa.shared.core.events import Event
 from rasa.core.test import test
+from rasa.utils.common import TempDirectoryPath, get_temp_dir_name
 from rasa.shared.core.trackers import (
     DialogueStateTracker,
     EventVerbosity,
 )
 from rasa.core.utils import AvailableEndpoints
 from rasa.nlu.emulators.no_emulator import NoEmulator
 import rasa.nlu.test
@@ -626,15 +626,15 @@
 
     Returns:
         The decorated function.
     """
 
     @wraps(f)
     async def decorated_function(*args: Any, **kwargs: Any) -> HTTPResponse:
-        with tempfile.TemporaryDirectory() as directory:
+        with TempDirectoryPath(get_temp_dir_name()) as directory:
             # Decorated request handles need to have a parameter `temporary_directory`
             return await f(*args, temporary_directory=Path(directory), **kwargs)
 
     return decorated_function
 
 
 def create_app(
```

### Comparing `rasa-3.5.9/rasa/shared/constants.py` & `rasa-3.6.0a1/rasa/shared/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/core/constants.py` & `rasa-3.6.0a1/rasa/shared/core/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/core/conversation.py` & `rasa-3.6.0a1/rasa/shared/core/conversation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/core/domain.py` & `rasa-3.6.0a1/rasa/shared/core/domain.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/core/events.py` & `rasa-3.6.0a1/rasa/shared/core/events.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/core/generator.py` & `rasa-3.6.0a1/rasa/shared/core/generator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/core/slot_mappings.py` & `rasa-3.6.0a1/rasa/shared/core/slot_mappings.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/core/slots.py` & `rasa-3.6.0a1/rasa/shared/core/slots.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/core/trackers.py` & `rasa-3.6.0a1/rasa/shared/core/trackers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import dataclasses
+import itertools
 import logging
 import os
 import time
 from collections import deque
 from enum import Enum
 from typing import (
     Dict,
@@ -875,14 +876,32 @@
 
         if self.events:
             data["events"] = list(self.events)
 
         return rasa.shared.utils.io.get_dictionary_fingerprint(data)
 
 
+class TrackerEventDiffEngine:
+    """Computes event difference of two trackers."""
+
+    @staticmethod
+    def event_difference(
+        original: DialogueStateTracker, tracker: DialogueStateTracker
+    ) -> List[Event]:
+        """Returns all events from the new tracker which are not present
+        in the original tracker.
+
+        Args:
+            tracker: Tracker containing events from the current conversation session.
+        """
+        offset = len(original.events) if original else 0
+        events = tracker.events
+        return list(itertools.islice(events, offset, len(events)))
+
+
 def get_active_loop_name(
     state: State,
 ) -> Optional[Text]:
     """Get the name of current active loop.
 
     Args:
         state: The state from which the name of active loop should be extracted
```

### Comparing `rasa-3.5.9/rasa/shared/core/training_data/loading.py` & `rasa-3.6.0a1/rasa/shared/core/training_data/loading.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/core/training_data/story_reader/story_reader.py` & `rasa-3.6.0a1/rasa/shared/core/training_data/story_reader/story_reader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/core/training_data/story_reader/story_step_builder.py` & `rasa-3.6.0a1/rasa/shared/core/training_data/story_reader/story_step_builder.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/core/training_data/story_reader/yaml_story_reader.py` & `rasa-3.6.0a1/rasa/shared/core/training_data/story_reader/yaml_story_reader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/core/training_data/story_writer/story_writer.py` & `rasa-3.6.0a1/rasa/shared/core/training_data/story_writer/story_writer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/core/training_data/story_writer/yaml_story_writer.py` & `rasa-3.6.0a1/rasa/shared/core/training_data/story_writer/yaml_story_writer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/core/training_data/structures.py` & `rasa-3.6.0a1/rasa/shared/core/training_data/structures.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/core/training_data/visualization.html` & `rasa-3.6.0a1/rasa/shared/core/training_data/visualization.html`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/core/training_data/visualization.py` & `rasa-3.6.0a1/rasa/shared/core/training_data/visualization.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/data.py` & `rasa-3.6.0a1/rasa/shared/data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/exceptions.py` & `rasa-3.6.0a1/rasa/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/importers/importer.py` & `rasa-3.6.0a1/rasa/shared/importers/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,48 +94,51 @@
         ...
 
     @staticmethod
     def load_from_config(
         config_path: Text,
         domain_path: Optional[Text] = None,
         training_data_paths: Optional[List[Text]] = None,
+        args: Optional[Dict[Text, Any]] = {},
     ) -> "TrainingDataImporter":
         """Loads a `TrainingDataImporter` instance from a configuration file."""
         config = rasa.shared.utils.io.read_config_file(config_path)
         return TrainingDataImporter.load_from_dict(
-            config, config_path, domain_path, training_data_paths
+            config, config_path, domain_path, training_data_paths, args
         )
 
     @staticmethod
     def load_core_importer_from_config(
         config_path: Text,
         domain_path: Optional[Text] = None,
         training_data_paths: Optional[List[Text]] = None,
+        args: Optional[Dict[Text, Any]] = {},
     ) -> "TrainingDataImporter":
         """Loads core `TrainingDataImporter` instance.
 
         Instance loaded from configuration file will only read Core training data.
         """
         importer = TrainingDataImporter.load_from_config(
-            config_path, domain_path, training_data_paths
+            config_path, domain_path, training_data_paths, args
         )
         return importer
 
     @staticmethod
     def load_nlu_importer_from_config(
         config_path: Text,
         domain_path: Optional[Text] = None,
         training_data_paths: Optional[List[Text]] = None,
+        args: Optional[Dict[Text, Any]] = {},
     ) -> "TrainingDataImporter":
         """Loads nlu `TrainingDataImporter` instance.
 
         Instance loaded from configuration file will only read NLU training data.
         """
         importer = TrainingDataImporter.load_from_config(
-            config_path, domain_path, training_data_paths
+            config_path, domain_path, training_data_paths, args
         )
 
         if isinstance(importer, E2EImporter):
             # When we only train NLU then there is no need to enrich the data with
             # E2E data from Core training data.
             importer = importer.importer
 
@@ -143,23 +146,24 @@
 
     @staticmethod
     def load_from_dict(
         config: Optional[Dict] = None,
         config_path: Optional[Text] = None,
         domain_path: Optional[Text] = None,
         training_data_paths: Optional[List[Text]] = None,
+        args: Optional[Dict[Text, Any]] = {},
     ) -> "TrainingDataImporter":
         """Loads a `TrainingDataImporter` instance from a dictionary."""
         from rasa.shared.importers.rasa import RasaFileImporter
 
         config = config or {}
         importers = config.get("importers", [])
         importers = [
             TrainingDataImporter._importer_from_dict(
-                importer, config_path, domain_path, training_data_paths
+                importer, config_path, domain_path, training_data_paths, args
             )
             for importer in importers
         ]
         importers = [importer for importer in importers if importer]
         if not importers:
             importers = [
                 RasaFileImporter(config_path, domain_path, training_data_paths)
@@ -169,14 +173,15 @@
 
     @staticmethod
     def _importer_from_dict(
         importer_config: Dict,
         config_path: Text,
         domain_path: Optional[Text] = None,
         training_data_paths: Optional[List[Text]] = None,
+        args: Optional[Dict[Text, Any]] = {},
     ) -> Optional["TrainingDataImporter"]:
         from rasa.shared.importers.multi_project import MultiProjectImporter
         from rasa.shared.importers.rasa import RasaFileImporter
 
         module_path = importer_config.pop("name", None)
         if module_path == RasaFileImporter.__name__:
             importer_class: Type[TrainingDataImporter] = RasaFileImporter
@@ -188,19 +193,22 @@
                     module_path
                 )
             except (AttributeError, ImportError):
                 logging.warning(f"Importer '{module_path}' not found.")
                 return None
 
         constructor_arguments = rasa.shared.utils.common.minimal_kwargs(
-            importer_config, importer_class
+            {**importer_config, **(args or {})}, importer_class
         )
 
         return importer_class(
-            config_path, domain_path, training_data_paths, **constructor_arguments
+            config_path,
+            domain_path,
+            training_data_paths,
+            **constructor_arguments,
         )
 
     def fingerprint(self) -> Text:
         """Returns a random fingerprint as data shouldn't be cached."""
         return rasa.shared.utils.io.random_string(25)
 
     def __repr__(self) -> Text:
```

### Comparing `rasa-3.5.9/rasa/shared/importers/multi_project.py` & `rasa-3.6.0a1/rasa/shared/importers/multi_project.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/importers/rasa.py` & `rasa-3.6.0a1/rasa/shared/importers/rasa.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/importers/utils.py` & `rasa-3.6.0a1/rasa/shared/importers/utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/constants.py` & `rasa-3.6.0a1/rasa/shared/nlu/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/training_data/entities_parser.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/entities_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/training_data/features.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/features.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/training_data/formats/dialogflow.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/dialogflow.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/training_data/formats/luis.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/luis.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/training_data/formats/rasa.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/rasa.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/training_data/formats/rasa_yaml.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/rasa_yaml.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/training_data/formats/readerwriter.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/readerwriter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/training_data/formats/wit.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/formats/wit.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/training_data/loading.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/loading.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/training_data/lookup_tables_parser.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/lookup_tables_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/training_data/message.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/message.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/training_data/schemas/data_schema.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/schemas/data_schema.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/training_data/schemas/nlu.yml` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/schemas/nlu.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/training_data/schemas/responses.yml` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/schemas/responses.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/training_data/synonyms_parser.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/synonyms_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/training_data/training_data.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/training_data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/nlu/training_data/util.py` & `rasa-3.6.0a1/rasa/shared/nlu/training_data/util.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/utils/common.py` & `rasa-3.6.0a1/rasa/shared/utils/common.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/utils/io.py` & `rasa-3.6.0a1/rasa/shared/utils/io.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/utils/pykwalify_extensions.py` & `rasa-3.6.0a1/rasa/shared/utils/pykwalify_extensions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/utils/schemas/domain.yml` & `rasa-3.6.0a1/rasa/shared/utils/schemas/domain.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/utils/schemas/events.py` & `rasa-3.6.0a1/rasa/shared/utils/schemas/events.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/utils/schemas/model_config.yml` & `rasa-3.6.0a1/rasa/shared/utils/schemas/model_config.yml`

 * *Files 19% similar despite different names*

```diff
@@ -10,27 +10,37 @@
   assistant_id:
     type: "str"
     required: False
   pipeline:
     type: "seq"
     required: False
     sequence:
-    - type: "map"
-      # Only validate required items but do not validate each potential config param
-      # for the the components
-      allowempty: True
-      mapping:
-        name:
-          type: str
-          required: True
+      - type: "map"
+        # Only validate required items but do not validate each potential config param
+        # for the the components
+        allowempty: True
+        mapping:
+          name:
+            type: str
+            required: True
   policies:
     type: "seq"
     required: False
     sequence:
-    - type: "map"
-      # Only validate required items but do not validate each potential config param
-      # for the the policies
-      allowempty: True
-      mapping:
-        name:
-          type: str
-          required: True
+      - type: "map"
+        # Only validate required items but do not validate each potential config param
+        # for the the policies
+        allowempty: True
+        mapping:
+          name:
+            type: str
+            required: True
+  spaces:
+    type: "seq"
+    required: False
+    sequence:
+      - type: "map"
+        allowempty: True
+        mapping:
+          name:
+            type: str
+            required: True
```

### Comparing `rasa-3.5.9/rasa/shared/utils/schemas/stories.yml` & `rasa-3.6.0a1/rasa/shared/utils/schemas/stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/shared/utils/validation.py` & `rasa-3.6.0a1/rasa/shared/utils/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,21 +113,24 @@
             elif isinstance(current, list) and head.isdigit():
                 return self._line_number_for_path(current[int(head)], tail) or this_line
             else:
                 return this_line
         return self._line_number_for_path(current, tail) or this_line
 
 
-def validate_yaml_schema(yaml_file_content: Text, schema_path: Text) -> None:
-    """
-    Validate yaml content.
+def validate_yaml_schema(
+    yaml_file_content: Text, schema_path: Text, package_name: Text = PACKAGE_NAME
+) -> None:
+    """Validate yaml content.
 
     Args:
         yaml_file_content: the content of the yaml file to be validated
         schema_path: the schema of the yaml file
+        package_name: the name of the package the schema is located in. defaults
+            to `rasa`.
     """
     from pykwalify.core import Core
     from pykwalify.errors import SchemaError
     from ruamel.yaml import YAMLError
     import pkg_resources
     import logging
 
@@ -142,15 +145,15 @@
         # right line
         source_data = rasa.shared.utils.io.read_yaml(
             yaml_file_content, reader_type=["safe", "rt"]
         )
     except (YAMLError, DuplicateKeyError) as e:
         raise YamlSyntaxException(underlying_yaml_exception=e)
 
-    schema_file = pkg_resources.resource_filename(PACKAGE_NAME, schema_path)
+    schema_file = pkg_resources.resource_filename(package_name, schema_path)
     schema_utils_file = pkg_resources.resource_filename(
         PACKAGE_NAME, RESPONSES_SCHEMA_FILE
     )
     schema_extensions = pkg_resources.resource_filename(
         PACKAGE_NAME, SCHEMA_EXTENSIONS_FILE
     )
 
@@ -213,15 +216,14 @@
         yaml_file_content: Raw content of training data file as a dictionary.
         filename: Name of the validated file.
 
     Returns:
         `True` if the file can be processed by current version of Rasa Open Source,
         `False` otherwise.
     """
-
     if filename:
         filename = os.path.abspath(filename)
 
     if not isinstance(yaml_file_content, dict):
         raise YamlValidationException(
             "YAML content in is not a mapping, can not validate training "
             "data schema version.",
```

### Comparing `rasa-3.5.9/rasa/telemetry.py` & `rasa-3.6.0a1/rasa/telemetry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/common.py` & `rasa-3.6.0a1/rasa/utils/common.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/converter.py` & `rasa-3.6.0a1/rasa/utils/converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/endpoints.py` & `rasa-3.6.0a1/rasa/utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/io.py` & `rasa-3.6.0a1/rasa/utils/io.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/plotting.py` & `rasa-3.6.0a1/rasa/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/tensorflow/callback.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/callback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/tensorflow/constants.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/tensorflow/crf.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/crf.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/tensorflow/data_generator.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/data_generator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/tensorflow/environment.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/environment.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/tensorflow/layers.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/layers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/tensorflow/layers_utils.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/layers_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/tensorflow/model_data.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/model_data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/tensorflow/model_data_utils.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/model_data_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/tensorflow/models.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/models.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/tensorflow/rasa_layers.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/rasa_layers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/tensorflow/transformer.py` & `rasa-3.6.0a1/rasa/utils/tensorflow/transformer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/utils/train_utils.py` & `rasa-3.6.0a1/rasa/utils/train_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/rasa/validator.py` & `rasa-3.6.0a1/rasa/validator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.5.9/PKG-INFO` & `rasa-3.6.0a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: rasa
-Version: 3.5.9
+Version: 3.6.0a1
 Summary: Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants
 Home-page: https://rasa.com
 License: Apache-2.0
 Keywords: nlp,machine-learning,machine-learning-library,bot,bots,botkit,rasa conversational-agents,conversational-ai,chatbot,chatbot-framework,bot-framework
 Author: Rasa Technologies GmbH
 Author-email: hi@rasa.com
 Maintainer: Tom Bocklisch
 Maintainer-email: tom@rasa.com
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: full
 Provides-Extra: gh-release-notes
 Provides-Extra: jieba
@@ -30,21 +29,21 @@
 Requires-Dist: SQLAlchemy (>=1.4.0,<1.5.0)
 Requires-Dist: absl-py (>=0.9,<1.4)
 Requires-Dist: aio-pika (>=6.7.1,<8.2.4)
 Requires-Dist: aiogram (<2.26)
 Requires-Dist: aiohttp (>=3.6,!=3.7.4.post0,<3.9)
 Requires-Dist: apscheduler (>=3.6,<3.10)
 Requires-Dist: attrs (>=19.3,<22.2)
-Requires-Dist: boto3 (>=1.12,<2.0)
+Requires-Dist: boto3 (>=1.26.124,<2.0.0)
 Requires-Dist: cloudpickle (>=1.2,<2.3)
 Requires-Dist: colorama (>=0.4.4,<0.5.0) ; sys_platform == "win32"
 Requires-Dist: colorclass (>=2.2,<2.3)
 Requires-Dist: coloredlogs (>=10,<16)
 Requires-Dist: colorhash (>=1.0.2,<1.3.0)
-Requires-Dist: confluent-kafka (>=1.9.2,<2.0.0)
+Requires-Dist: confluent-kafka (>=1.9.2,<3.0.0)
 Requires-Dist: dask (==2022.10.2) ; python_version >= "3.8" and python_version < "3.11"
 Requires-Dist: dask (==2022.2.0) ; python_full_version >= "3.7.0" and python_full_version < "3.8.0"
 Requires-Dist: fbmessenger (>=6.0.0,<6.1.0)
 Requires-Dist: github3.py (>=3.2.0,<3.3.0) ; extra == "gh-release-notes"
 Requires-Dist: google-auth (<3)
 Requires-Dist: jieba (>=0.39,<0.43) ; extra == "jieba" or extra == "full"
 Requires-Dist: joblib (>=0.15.1,<1.3.0)
@@ -60,55 +59,58 @@
 Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: prompt-toolkit (>=3.0,<3.0.29)
 Requires-Dist: protobuf (>=3.9.2,<3.20)
 Requires-Dist: psycopg2-binary (>=2.8.2,<2.10.0)
 Requires-Dist: pydantic (<1.10.3)
 Requires-Dist: pydot (>=1.4,<1.5)
 Requires-Dist: pykwalify (>=1.7,<1.9)
-Requires-Dist: pymongo[srv,tls] (>=3.8,<3.11)
+Requires-Dist: pymongo[srv,tls] (>=3.8,<4.4)
 Requires-Dist: python-dateutil (>=2.8,<2.9)
 Requires-Dist: python-engineio (>=4,<6,!=5.0.0)
 Requires-Dist: python-socketio (>=4.4,<6)
 Requires-Dist: pytz (>=2019.1,<2023.0)
+Requires-Dist: pyyaml (>=5.3.1,<6.0)
 Requires-Dist: questionary (>=1.5.1,<1.11.0)
 Requires-Dist: randomname (>=0.1.5,<0.2.0)
-Requires-Dist: rasa-sdk (>=3.5.0,<3.6.0)
+Requires-Dist: rasa-sdk (>=3.6.0a1,<3.7.0)
 Requires-Dist: redis (>=4.5.3,<5.0)
 Requires-Dist: regex (>=2020.6,<2022.11)
 Requires-Dist: requests (>=2.23,<3.0)
-Requires-Dist: rocketchat_API (>=0.6.31,<1.29.0)
+Requires-Dist: rocketchat_API (>=0.6.31,<1.30.0)
 Requires-Dist: ruamel.yaml (>=0.16.5,<0.18.0)
 Requires-Dist: sanic (>=21.12,<21.13)
 Requires-Dist: sanic-cors (>=2.0.0,<2.1.0)
 Requires-Dist: sanic-jwt (>=1.6.0,<2.0.0)
 Requires-Dist: sanic-routing (>=0.7.2,<0.8.0)
 Requires-Dist: scikit-learn (>=0.22,<1.1) ; python_full_version >= "3.7.0" and python_full_version < "3.8.0"
 Requires-Dist: scikit-learn (>=0.22,<1.2) ; python_version >= "3.8" and python_version < "3.11"
-Requires-Dist: scipy (>=1.4.1,<1.8.0) ; python_full_version >= "3.7.0" and python_full_version < "3.8.0"
+Requires-Dist: scipy (>=1.4.1,<1.7.3) ; python_full_version >= "3.7.0" and python_full_version < "3.8.0"
 Requires-Dist: scipy (>=1.4.1,<1.9.0) ; python_version >= "3.8" and python_version < "3.11"
-Requires-Dist: sentencepiece[sentencepiece] (>=0.1.96,<0.2.0) ; extra == "transformers" or extra == "full"
+Requires-Dist: sentencepiece[sentencepiece] (>=0.1.99,<0.2.0) ; extra == "transformers" or extra == "full"
 Requires-Dist: sentry-sdk (>=0.17.0,<1.15.0)
 Requires-Dist: setuptools (>=41.0.0)
 Requires-Dist: sklearn-crfsuite (>=0.3,<0.4)
 Requires-Dist: slack-sdk (>=3.19.2,<4.0.0)
 Requires-Dist: spacy (>=3.1,<3.5) ; (sys_platform != "darwin" or platform_machine != "arm64") and (extra == "spacy" or extra == "full")
 Requires-Dist: spacy (>=3.4,<4.0) ; (sys_platform == "darwin" and platform_machine == "arm64") and (extra == "spacy" or extra == "full")
-Requires-Dist: tarsafe (>=0.0.3,<0.0.4)
+Requires-Dist: tarsafe (>=0.0.3,<0.0.5)
 Requires-Dist: tensorflow (==2.11.0) ; sys_platform != "darwin" or platform_machine != "arm64"
-Requires-Dist: tensorflow-addons (>=0.18,<0.20)
+Requires-Dist: tensorflow-addons (==0.19.0) ; sys_platform == "linux" and platform_machine == "arm64" or sys_platform == "linux" and platform_machine == "aarch64"
+Requires-Dist: tensorflow-addons (>=0.18,<0.20) ; sys_platform != "linux" or platform_machine != "arm64" and platform_machine != "aarch64"
 Requires-Dist: tensorflow-cpu-aws (==2.11.0) ; sys_platform == "linux" and platform_machine == "arm64" or sys_platform == "linux" and platform_machine == "aarch64"
 Requires-Dist: tensorflow-intel (==2.11.0) ; sys_platform == "win32"
+Requires-Dist: tensorflow-io-gcs-filesystem (>=0.23.1,<0.32) ; sys_platform == "win32"
 Requires-Dist: tensorflow-macos (==2.11.0) ; sys_platform == "darwin" and platform_machine == "arm64"
 Requires-Dist: tensorflow-metal (==0.5.1) ; (sys_platform == "darwin" and platform_machine == "arm64") and (extra == "metal")
-Requires-Dist: tensorflow-text (==2.11.0) ; sys_platform != "win32" and platform_machine != "arm64"
+Requires-Dist: tensorflow-text (==2.11.0) ; sys_platform != "win32" and platform_machine != "arm64" and platform_machine != "aarch64"
 Requires-Dist: tensorflow_hub (>=0.12.0,<0.13.0)
 Requires-Dist: terminaltables (>=3.1.0,<3.2.0)
 Requires-Dist: tqdm (>=4.31,<5.0)
 Requires-Dist: transformers (>=4.13.0,<=4.26.0) ; extra == "transformers" or extra == "full"
-Requires-Dist: twilio (>=6.26,<7.15)
+Requires-Dist: twilio (>=6.26,<8.2)
 Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
 Requires-Dist: typing-utils (>=0.1.0,<0.2.0)
 Requires-Dist: ujson (>=1.35,<6.0)
 Requires-Dist: webexteamssdk (>=1.1.1,<1.7.0)
 Requires-Dist: websockets (>=10.0,<11.0)
 Project-URL: Documentation, https://rasa.com/docs
 Project-URL: Repository, https://github.com/rasahq/rasa
@@ -238,16 +240,16 @@
 ### Managing environments
 
 The official [Poetry guide](https://python-poetry.org/docs/managing-environments/) suggests to use
 [pyenv](https://github.com/pyenv/pyenv) or any other similar tool to easily switch between Python versions.
 This is how it can be done:
 
 ```bash
-pyenv install 3.7.9
-pyenv local 3.7.9  # Activate Python 3.7.9 for the current project
+pyenv install 3.10.10
+pyenv local 3.10.10  # Activate Python 3.10.10 for the current project
 ```
 *Note*: If you have trouble installing a specific version of python on your system
 it might be worth trying other supported versions.
 
 By default, Poetry will try to use the currently activated Python version to create the virtual environment
 for the current project automatically. You can also create and activate a virtual environment manually — in this
 case, Poetry should pick it up and use it to install the dependencies. For example:
@@ -422,14 +424,15 @@
 ```
 make types
 ```
 
 ### Deploying documentation updates
 
 We use `Docusaurus v2` to build docs for tagged versions and for the `main` branch.
+To run Docusaurus, install `Node.js 12.x`.
 The static site that gets built is pushed to the `documentation` branch of this repo.
 
 We host the site on netlify. On `main` branch builds (see `.github/workflows/documentation.yml`), we push the built docs to
 the `documentation` branch. Netlify automatically re-deploys the docs pages whenever there is a change to that branch.
 
 ## Releases
 Rasa has implemented robust policies governing version naming, as well as release pace for major, minor, and patch releases.
@@ -538,20 +541,28 @@
 to add.
 2. Make sure the bugfix(es) are in the release branch you will use (p.e if you are cutting a `2.0.4` patch, you will
 need your fixes to be on the `2.0.x` release branch). All patch releases must come from a `.x` branch!
 3. Once you're ready to release the Rasa Open Source patch, checkout the branch, run `make release` and follow the
 steps + get the PR merged.
 4. Once the PR is in, pull the `.x` branch again and push the tag!
 
+### Additional Release Tasks 
+**Note: This is only required if the released version is the highest version available.
+For instance, perform the following steps when version > [version](https://github.com/RasaHQ/rasa/blob/main/rasa/version.py) on main.**
+
+In order to check compatibility between the new released Rasa version to the latest version of Rasa X/Enterprise, we perform the following steps:
+1. Following a new Rasa release, an automated pull request is created in [Rasa-X-Demo](https://github.com/RasaHQ/rasa-x-demo/pulls). 
+2. Once the above PR is merged, follow instructions [here](https://github.com/RasaHQ/rasa-x-demo/blob/master/.github/VERSION_BUMPER_PR_COMMENT.md), to release a version.
+3. Update the new version in the Rasa X/Enterprise [env file](https://github.com/RasaHQ/rasa-x/blob/main/.env).
+The [Rasa-X-Demo](https://github.com/RasaHQ/rasa-x-demo) project uses the new updated Rasa version to train and test a model which in turn is used by our CI to run tests in the Rasa X/Enterprise repository, 
+thus validating compatibility between Rasa and Rasa X/Enterprise.
+
 ### Actively maintained versions
 
-We're actively maintaining _any minor on our latest major release_ and _the latest minor of the previous major release_.
-Currently, this means the following minor versions will receive bugfixes updates:
-- 2.8
-- Every minor version on 3.x
+Please refer to the [Rasa Product Release and Maintenance Policy](https://rasa.com/rasa-product-release-and-maintenance-policy/) page.
 
 ## License
 Licensed under the Apache License, Version 2.0.
 Copyright 2022 Rasa Technologies GmbH. [Copy of the license](LICENSE.txt).
 
 A list of the Licenses of the dependencies of the project can be found at
 the bottom of the
```

