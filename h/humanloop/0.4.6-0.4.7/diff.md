# Comparing `tmp/humanloop-0.4.6.tar.gz` & `tmp/humanloop-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humanloop-0.4.6.tar", max compression
+gzip compressed data, was "humanloop-0.4.7.tar", max compression
```

## Comparing `humanloop-0.4.6.tar` & `humanloop-0.4.7.tar`

### file list

```diff
@@ -1,410 +1,410 @@
--rw-r--r--   0        0        0     1081 2023-05-31 20:33:30.451027 humanloop-0.4.6/LICENSE
--rw-r--r--   0        0        0     8475 2023-05-31 20:33:30.498301 humanloop-0.4.6/README.md
--rw-r--r--   0        0        0     1235 2023-05-31 20:33:30.357322 humanloop-0.4.6/humanloop/__init__.py
--rw-r--r--   0        0        0    73185 2023-05-31 20:33:30.357623 humanloop-0.4.6/humanloop/api_client.py
--rw-r--r--   0        0        0      663 2023-05-31 20:33:30.357818 humanloop-0.4.6/humanloop/api_response.py
--rw-r--r--   0        0        0      214 2023-05-31 20:33:30.357969 humanloop-0.4.6/humanloop/apis/__init__.py
--rw-r--r--   0        0        0     4698 2023-05-31 20:33:30.358109 humanloop-0.4.6/humanloop/apis/path_to_api.py
--rw-r--r--   0        0        0      236 2023-05-31 20:33:30.358271 humanloop-0.4.6/humanloop/apis/paths/__init__.py
--rw-r--r--   0        0        0       91 2023-05-31 20:33:30.358404 humanloop-0.4.6/humanloop/apis/paths/chat.py
--rw-r--r--   0        0        0      108 2023-05-31 20:33:30.358548 humanloop-0.4.6/humanloop/apis/paths/chat_deployed.py
--rw-r--r--   0        0        0      112 2023-05-31 20:33:30.358706 humanloop-0.4.6/humanloop/apis/paths/chat_experiment.py
--rw-r--r--   0        0        0      115 2023-05-31 20:33:30.358852 humanloop-0.4.6/humanloop/apis/paths/chat_model_config.py
--rw-r--r--   0        0        0      103 2023-05-31 20:33:30.358996 humanloop-0.4.6/humanloop/apis/paths/completion.py
--rw-r--r--   0        0        0      120 2023-05-31 20:33:30.359147 humanloop-0.4.6/humanloop/apis/paths/completion_deployed.py
--rw-r--r--   0        0        0      124 2023-05-31 20:33:30.359293 humanloop-0.4.6/humanloop/apis/paths/completion_experiment.py
--rw-r--r--   0        0        0      127 2023-05-31 20:33:30.359407 humanloop-0.4.6/humanloop/apis/paths/completion_model_config.py
--rw-r--r--   0        0        0      226 2023-05-31 20:33:30.359557 humanloop-0.4.6/humanloop/apis/paths/experiments_experiment_id.py
--rw-r--r--   0        0        0      152 2023-05-31 20:33:30.359708 humanloop-0.4.6/humanloop/apis/paths/experiments_experiment_id_model_config.py
--rw-r--r--   0        0        0       99 2023-05-31 20:33:30.359852 humanloop-0.4.6/humanloop/apis/paths/feedback.py
--rw-r--r--   0        0        0      159 2023-05-31 20:33:30.359995 humanloop-0.4.6/humanloop/apis/paths/logs.py
--rw-r--r--   0        0        0       99 2023-05-31 20:33:30.360135 humanloop-0.4.6/humanloop/apis/paths/logs_id.py
--rw-r--r--   0        0        0      108 2023-05-31 20:33:30.360275 humanloop-0.4.6/humanloop/apis/paths/model_configs.py
--rw-r--r--   0        0        0      110 2023-05-31 20:33:30.360412 humanloop-0.4.6/humanloop/apis/paths/model_configs_id.py
--rw-r--r--   0        0        0      165 2023-05-31 20:33:30.360556 humanloop-0.4.6/humanloop/apis/paths/projects.py
--rw-r--r--   0        0        0      176 2023-05-31 20:33:30.360705 humanloop-0.4.6/humanloop/apis/paths/projects_id.py
--rw-r--r--   0        0        0      219 2023-05-31 20:33:30.360858 humanloop-0.4.6/humanloop/apis/paths/projects_id_active_config.py
--rw-r--r--   0        0        0      144 2023-05-31 20:33:30.361011 humanloop-0.4.6/humanloop/apis/paths/projects_id_active_experiment.py
--rw-r--r--   0        0        0      116 2023-05-31 20:33:30.361150 humanloop-0.4.6/humanloop/apis/paths/projects_id_configs.py
--rw-r--r--   0        0        0      117 2023-05-31 20:33:30.361260 humanloop-0.4.6/humanloop/apis/paths/projects_id_export.py
--rw-r--r--   0        0        0      135 2023-05-31 20:33:30.361394 humanloop-0.4.6/humanloop/apis/paths/projects_id_feedback_types.py
--rw-r--r--   0        0        0      231 2023-05-31 20:33:30.361621 humanloop-0.4.6/humanloop/apis/paths/projects_project_id_experiments.py
--rw-r--r--   0        0        0      165 2023-05-31 20:33:30.361878 humanloop-0.4.6/humanloop/apis/paths/sessions.py
--rw-r--r--   0        0        0      101 2023-05-31 20:33:30.362022 humanloop-0.4.6/humanloop/apis/paths/sessions_id.py
--rw-r--r--   0        0        0       95 2023-05-31 20:33:30.362203 humanloop-0.4.6/humanloop/apis/paths/traces.py
--rw-r--r--   0        0        0     1654 2023-05-31 20:33:30.362361 humanloop-0.4.6/humanloop/apis/tag_to_api.py
--rw-r--r--   0        0        0      572 2023-05-31 20:33:30.362534 humanloop-0.4.6/humanloop/apis/tags/__init__.py
--rw-r--r--   0        0        0     1182 2023-05-31 20:33:30.362690 humanloop-0.4.6/humanloop/apis/tags/chats_api.py
--rw-r--r--   0        0        0     1196 2023-05-31 20:33:30.362818 humanloop-0.4.6/humanloop/apis/tags/completions_api.py
--rw-r--r--   0        0        0     1267 2023-05-31 20:33:30.362975 humanloop-0.4.6/humanloop/apis/tags/experiments_api.py
--rw-r--r--   0        0        0      897 2023-05-31 20:33:30.363122 humanloop-0.4.6/humanloop/apis/tags/feedback_api.py
--rw-r--r--   0        0        0     1028 2023-05-31 20:33:30.363256 humanloop-0.4.6/humanloop/apis/tags/logs_api.py
--rw-r--r--   0        0        0      979 2023-05-31 20:33:30.363467 humanloop-0.4.6/humanloop/apis/tags/model_configurations_api.py
--rw-r--r--   0        0        0     1662 2023-05-31 20:33:30.363666 humanloop-0.4.6/humanloop/apis/tags/projects_api.py
--rw-r--r--   0        0        0     1010 2023-05-31 20:33:30.363842 humanloop-0.4.6/humanloop/apis/tags/sessions_api.py
--rw-r--r--   0        0        0      893 2023-05-31 20:33:30.364021 humanloop-0.4.6/humanloop/apis/tags/traces_api.py
--rw-r--r--   0        0        0    28838 2023-05-31 20:33:30.364266 humanloop-0.4.6/humanloop/client.py
--rw-r--r--   0        0        0    28838 2023-05-31 20:33:30.364549 humanloop-0.4.6/humanloop/client.pyi
--rw-r--r--   0        0        0     6780 2023-05-31 20:33:30.449862 humanloop-0.4.6/humanloop/client_custom.py
--rw-r--r--   0        0        0    18850 2023-05-31 20:33:30.365043 humanloop-0.4.6/humanloop/configuration.py
--rw-r--r--   0        0        0     7854 2023-05-31 20:33:30.365246 humanloop-0.4.6/humanloop/exceptions.py
--rw-r--r--   0        0        0     2274 2023-05-31 20:33:30.365396 humanloop-0.4.6/humanloop/exceptions_base.py
--rw-r--r--   0        0        0      343 2023-05-31 20:33:30.365631 humanloop-0.4.6/humanloop/model/__init__.py
--rw-r--r--   0        0        0     9316 2023-05-31 20:33:30.365812 humanloop-0.4.6/humanloop/model/agent_config_request.py
--rw-r--r--   0        0        0     9151 2023-05-31 20:33:30.366066 humanloop-0.4.6/humanloop/model/agent_config_request.pyi
--rw-r--r--   0        0        0    11316 2023-05-31 20:33:30.366312 humanloop-0.4.6/humanloop/model/agent_config_response.py
--rw-r--r--   0        0        0    11316 2023-05-31 20:33:30.366521 humanloop-0.4.6/humanloop/model/agent_config_response.pyi
--rw-r--r--   0        0        0     6555 2023-05-31 20:33:30.366713 humanloop-0.4.6/humanloop/model/base_metric_response.py
--rw-r--r--   0        0        0     6555 2023-05-31 20:33:30.366826 humanloop-0.4.6/humanloop/model/base_metric_response.pyi
--rw-r--r--   0        0        0     5326 2023-05-31 20:33:30.366942 humanloop-0.4.6/humanloop/model/categorical_feedback_label.py
--rw-r--r--   0        0        0     5326 2023-05-31 20:33:30.367061 humanloop-0.4.6/humanloop/model/categorical_feedback_label.pyi
--rw-r--r--   0        0        0     9133 2023-05-31 20:33:30.367192 humanloop-0.4.6/humanloop/model/chat_data_response.py
--rw-r--r--   0        0        0     9133 2023-05-31 20:33:30.367338 humanloop-0.4.6/humanloop/model/chat_data_response.pyi
--rw-r--r--   0        0        0    10174 2023-05-31 20:33:30.367462 humanloop-0.4.6/humanloop/model/chat_deployed_request.py
--rw-r--r--   0        0        0    10174 2023-05-31 20:33:30.367593 humanloop-0.4.6/humanloop/model/chat_deployed_request.pyi
--rw-r--r--   0        0        0    10835 2023-05-31 20:33:30.367803 humanloop-0.4.6/humanloop/model/chat_experiment_request.py
--rw-r--r--   0        0        0    10835 2023-05-31 20:33:30.368021 humanloop-0.4.6/humanloop/model/chat_experiment_request.pyi
--rw-r--r--   0        0        0     3878 2023-05-31 20:33:30.368198 humanloop-0.4.6/humanloop/model/chat_message.py
--rw-r--r--   0        0        0     3878 2023-05-31 20:33:30.368359 humanloop-0.4.6/humanloop/model/chat_message.pyi
--rw-r--r--   0        0        0    10869 2023-05-31 20:33:30.368529 humanloop-0.4.6/humanloop/model/chat_model_config_request.py
--rw-r--r--   0        0        0    10869 2023-05-31 20:33:30.368724 humanloop-0.4.6/humanloop/model/chat_model_config_request.pyi
--rw-r--r--   0        0        0    12732 2023-05-31 20:33:30.368938 humanloop-0.4.6/humanloop/model/chat_request.py
--rw-r--r--   0        0        0    12732 2023-05-31 20:33:30.369152 humanloop-0.4.6/humanloop/model/chat_request.pyi
--rw-r--r--   0        0        0    11252 2023-05-31 20:33:30.369371 humanloop-0.4.6/humanloop/model/chat_response.py
--rw-r--r--   0        0        0    11252 2023-05-31 20:33:30.369593 humanloop-0.4.6/humanloop/model/chat_response.pyi
--rw-r--r--   0        0        0     1622 2023-05-31 20:33:30.369774 humanloop-0.4.6/humanloop/model/chat_role.py
--rw-r--r--   0        0        0     1461 2023-05-31 20:33:30.369914 humanloop-0.4.6/humanloop/model/chat_role.pyi
--rw-r--r--   0        0        0     9850 2023-05-31 20:33:30.370099 humanloop-0.4.6/humanloop/model/completion_deployed_request.py
--rw-r--r--   0        0        0     9850 2023-05-31 20:33:30.370337 humanloop-0.4.6/humanloop/model/completion_deployed_request.pyi
--rw-r--r--   0        0        0    10516 2023-05-31 20:33:30.370553 humanloop-0.4.6/humanloop/model/completion_experiment_request.py
--rw-r--r--   0        0        0    10516 2023-05-31 20:33:30.370785 humanloop-0.4.6/humanloop/model/completion_experiment_request.pyi
--rw-r--r--   0        0        0    10552 2023-05-31 20:33:30.370995 humanloop-0.4.6/humanloop/model/completion_model_config_request.py
--rw-r--r--   0        0        0    10552 2023-05-31 20:33:30.371145 humanloop-0.4.6/humanloop/model/completion_model_config_request.pyi
--rw-r--r--   0        0        0    12434 2023-05-31 20:33:30.371352 humanloop-0.4.6/humanloop/model/completion_request.py
--rw-r--r--   0        0        0    12434 2023-05-31 20:33:30.371611 humanloop-0.4.6/humanloop/model/completion_request.pyi
--rw-r--r--   0        0        0    11193 2023-05-31 20:33:30.371931 humanloop-0.4.6/humanloop/model/completion_response.py
--rw-r--r--   0        0        0    11193 2023-05-31 20:33:30.372171 humanloop-0.4.6/humanloop/model/completion_response.pyi
--rw-r--r--   0        0        0     2938 2023-05-31 20:33:30.372426 humanloop-0.4.6/humanloop/model/config_response.py
--rw-r--r--   0        0        0     2938 2023-05-31 20:33:30.372653 humanloop-0.4.6/humanloop/model/config_response.pyi
--rw-r--r--   0        0        0     1722 2023-05-31 20:33:30.372824 humanloop-0.4.6/humanloop/model/config_type.py
--rw-r--r--   0        0        0     1537 2023-05-31 20:33:30.372972 humanloop-0.4.6/humanloop/model/config_type.pyi
--rw-r--r--   0        0        0     6372 2023-05-31 20:33:30.373124 humanloop-0.4.6/humanloop/model/create_experiment_request.py
--rw-r--r--   0        0        0     6372 2023-05-31 20:33:30.373293 humanloop-0.4.6/humanloop/model/create_experiment_request.pyi
--rw-r--r--   0        0        0     3375 2023-05-31 20:33:30.373462 humanloop-0.4.6/humanloop/model/create_log_response.py
--rw-r--r--   0        0        0     3375 2023-05-31 20:33:30.373700 humanloop-0.4.6/humanloop/model/create_log_response.pyi
--rw-r--r--   0        0        0     4442 2023-05-31 20:33:30.373911 humanloop-0.4.6/humanloop/model/create_project_request.py
--rw-r--r--   0        0        0     4442 2023-05-31 20:33:30.374136 humanloop-0.4.6/humanloop/model/create_project_request.pyi
--rw-r--r--   0        0        0     2811 2023-05-31 20:33:30.374329 humanloop-0.4.6/humanloop/model/create_session_response.py
--rw-r--r--   0        0        0     2811 2023-05-31 20:33:30.374525 humanloop-0.4.6/humanloop/model/create_session_response.pyi
--rw-r--r--   0        0        0     3408 2023-05-31 20:33:30.374724 humanloop-0.4.6/humanloop/model/create_trace_request.py
--rw-r--r--   0        0        0     3408 2023-05-31 20:33:30.374996 humanloop-0.4.6/humanloop/model/create_trace_request.pyi
--rw-r--r--   0        0        0     3505 2023-05-31 20:33:30.375175 humanloop-0.4.6/humanloop/model/create_trace_response.py
--rw-r--r--   0        0        0     3505 2023-05-31 20:33:30.375355 humanloop-0.4.6/humanloop/model/create_trace_response.pyi
--rw-r--r--   0        0        0     7631 2023-05-31 20:33:30.375646 humanloop-0.4.6/humanloop/model/data_response.py
--rw-r--r--   0        0        0     7631 2023-05-31 20:33:30.375917 humanloop-0.4.6/humanloop/model/data_response.pyi
--rw-r--r--   0        0        0     9174 2023-05-31 20:33:30.376075 humanloop-0.4.6/humanloop/model/experiment_config_response.py
--rw-r--r--   0        0        0     9174 2023-05-31 20:33:30.376310 humanloop-0.4.6/humanloop/model/experiment_config_response.pyi
--rw-r--r--   0        0        0    13003 2023-05-31 20:33:30.376581 humanloop-0.4.6/humanloop/model/experiment_response.py
--rw-r--r--   0        0        0    13003 2023-05-31 20:33:30.376726 humanloop-0.4.6/humanloop/model/experiment_response.pyi
--rw-r--r--   0        0        0     1552 2023-05-31 20:33:30.376859 humanloop-0.4.6/humanloop/model/experiment_status.py
--rw-r--r--   0        0        0     1405 2023-05-31 20:33:30.376972 humanloop-0.4.6/humanloop/model/experiment_status.pyi
--rw-r--r--   0        0        0     1861 2023-05-31 20:33:30.377071 humanloop-0.4.6/humanloop/model/experiments_list_response.py
--rw-r--r--   0        0        0     1861 2023-05-31 20:33:30.377180 humanloop-0.4.6/humanloop/model/experiments_list_response.pyi
--rw-r--r--   0        0        0     6857 2023-05-31 20:33:30.377304 humanloop-0.4.6/humanloop/model/feedback.py
--rw-r--r--   0        0        0     6857 2023-05-31 20:33:30.377415 humanloop-0.4.6/humanloop/model/feedback.pyi
--rw-r--r--   0        0        0     1639 2023-05-31 20:33:30.377534 humanloop-0.4.6/humanloop/model/feedback_class.py
--rw-r--r--   0        0        0     1472 2023-05-31 20:33:30.377648 humanloop-0.4.6/humanloop/model/feedback_class.pyi
--rw-r--r--   0        0        0     3510 2023-05-31 20:33:30.377770 humanloop-0.4.6/humanloop/model/feedback_label_request.py
--rw-r--r--   0        0        0     3510 2023-05-31 20:33:30.377877 humanloop-0.4.6/humanloop/model/feedback_label_request.pyi
--rw-r--r--   0        0        0     7365 2023-05-31 20:33:30.377971 humanloop-0.4.6/humanloop/model/feedback_request.py
--rw-r--r--   0        0        0     7365 2023-05-31 20:33:30.378065 humanloop-0.4.6/humanloop/model/feedback_request.pyi
--rw-r--r--   0        0        0     7317 2023-05-31 20:33:30.378226 humanloop-0.4.6/humanloop/model/feedback_response.py
--rw-r--r--   0        0        0     7317 2023-05-31 20:33:30.378368 humanloop-0.4.6/humanloop/model/feedback_response.pyi
--rw-r--r--   0        0        0     3376 2023-05-31 20:33:30.378478 humanloop-0.4.6/humanloop/model/feedback_submit_request.py
--rw-r--r--   0        0        0     3376 2023-05-31 20:33:30.378577 humanloop-0.4.6/humanloop/model/feedback_submit_request.pyi
--rw-r--r--   0        0        0     3386 2023-05-31 20:33:30.378701 humanloop-0.4.6/humanloop/model/feedback_submit_response.py
--rw-r--r--   0        0        0     3386 2023-05-31 20:33:30.378808 humanloop-0.4.6/humanloop/model/feedback_submit_response.pyi
--rw-r--r--   0        0        0     1866 2023-05-31 20:33:30.378922 humanloop-0.4.6/humanloop/model/feedback_type.py
--rw-r--r--   0        0        0     1635 2023-05-31 20:33:30.379021 humanloop-0.4.6/humanloop/model/feedback_type.pyi
--rw-r--r--   0        0        0     6337 2023-05-31 20:33:30.379134 humanloop-0.4.6/humanloop/model/feedback_type_model.py
--rw-r--r--   0        0        0     6337 2023-05-31 20:33:30.379224 humanloop-0.4.6/humanloop/model/feedback_type_model.pyi
--rw-r--r--   0        0        0     6465 2023-05-31 20:33:30.379350 humanloop-0.4.6/humanloop/model/feedback_type_request.py
--rw-r--r--   0        0        0     6465 2023-05-31 20:33:30.379478 humanloop-0.4.6/humanloop/model/feedback_type_request.pyi
--rw-r--r--   0        0        0     1835 2023-05-31 20:33:30.379589 humanloop-0.4.6/humanloop/model/feedback_types.py
--rw-r--r--   0        0        0     1835 2023-05-31 20:33:30.379690 humanloop-0.4.6/humanloop/model/feedback_types.pyi
--rw-r--r--   0        0        0     4583 2023-05-31 20:33:30.379787 humanloop-0.4.6/humanloop/model/generic_config_request.py
--rw-r--r--   0        0        0     4414 2023-05-31 20:33:30.379894 humanloop-0.4.6/humanloop/model/generic_config_request.pyi
--rw-r--r--   0        0        0     6738 2023-05-31 20:33:30.380004 humanloop-0.4.6/humanloop/model/generic_config_response.py
--rw-r--r--   0        0        0     6738 2023-05-31 20:33:30.380115 humanloop-0.4.6/humanloop/model/generic_config_response.pyi
--rw-r--r--   0        0        0     9795 2023-05-31 20:33:30.380241 humanloop-0.4.6/humanloop/model/get_model_config_response.py
--rw-r--r--   0        0        0     9795 2023-05-31 20:33:30.380429 humanloop-0.4.6/humanloop/model/get_model_config_response.pyi
--rw-r--r--   0        0        0     3787 2023-05-31 20:33:30.380581 humanloop-0.4.6/humanloop/model/http_validation_error.py
--rw-r--r--   0        0        0     3787 2023-05-31 20:33:30.380704 humanloop-0.4.6/humanloop/model/http_validation_error.pyi
--rw-r--r--   0        0        0     1843 2023-05-31 20:33:30.380808 humanloop-0.4.6/humanloop/model/label_sentiment.py
--rw-r--r--   0        0        0     1644 2023-05-31 20:33:30.380922 humanloop-0.4.6/humanloop/model/label_sentiment.pyi
--rw-r--r--   0        0        0     3332 2023-05-31 20:33:30.381018 humanloop-0.4.6/humanloop/model/log_datapoint_request.py
--rw-r--r--   0        0        0     3332 2023-05-31 20:33:30.381126 humanloop-0.4.6/humanloop/model/log_datapoint_request.pyi
--rw-r--r--   0        0        0    17395 2023-05-31 20:33:30.381237 humanloop-0.4.6/humanloop/model/log_model_config_request.py
--rw-r--r--   0        0        0    17395 2023-05-31 20:33:30.381364 humanloop-0.4.6/humanloop/model/log_model_config_request.pyi
--rw-r--r--   0        0        0    17925 2023-05-31 20:33:30.381491 humanloop-0.4.6/humanloop/model/log_request.py
--rw-r--r--   0        0        0    17925 2023-05-31 20:33:30.381613 humanloop-0.4.6/humanloop/model/log_request.pyi
--rw-r--r--   0        0        0    22277 2023-05-31 20:33:30.381728 humanloop-0.4.6/humanloop/model/log_response.py
--rw-r--r--   0        0        0    22277 2023-05-31 20:33:30.381841 humanloop-0.4.6/humanloop/model/log_response.pyi
--rw-r--r--   0        0        0     3381 2023-05-31 20:33:30.381966 humanloop-0.4.6/humanloop/model/logs_log_response.py
--rw-r--r--   0        0        0     3381 2023-05-31 20:33:30.382060 humanloop-0.4.6/humanloop/model/logs_log_response.pyi
--rw-r--r--   0        0        0    16422 2023-05-31 20:33:30.382192 humanloop-0.4.6/humanloop/model/model_config_chat_request.py
--rw-r--r--   0        0        0    16422 2023-05-31 20:33:30.382352 humanloop-0.4.6/humanloop/model/model_config_chat_request.pyi
--rw-r--r--   0        0        0    15562 2023-05-31 20:33:30.382487 humanloop-0.4.6/humanloop/model/model_config_completion_request.py
--rw-r--r--   0        0        0    15562 2023-05-31 20:33:30.382631 humanloop-0.4.6/humanloop/model/model_config_completion_request.pyi
--rw-r--r--   0        0        0     1636 2023-05-31 20:33:30.382762 humanloop-0.4.6/humanloop/model/model_endpoints.py
--rw-r--r--   0        0        0     1481 2023-05-31 20:33:30.382855 humanloop-0.4.6/humanloop/model/model_endpoints.pyi
--rw-r--r--   0        0        0     2123 2023-05-31 20:33:30.382938 humanloop-0.4.6/humanloop/model/model_providers.py
--rw-r--r--   0        0        0     1820 2023-05-31 20:33:30.383036 humanloop-0.4.6/humanloop/model/model_providers.pyi
--rw-r--r--   0        0        0     5320 2023-05-31 20:33:30.383130 humanloop-0.4.6/humanloop/model/paginated_data_log_response.py
--rw-r--r--   0        0        0     5320 2023-05-31 20:33:30.383237 humanloop-0.4.6/humanloop/model/paginated_data_log_response.pyi
--rw-r--r--   0        0        0     5356 2023-05-31 20:33:30.383343 humanloop-0.4.6/humanloop/model/paginated_data_project_response.py
--rw-r--r--   0        0        0     5356 2023-05-31 20:33:30.383459 humanloop-0.4.6/humanloop/model/paginated_data_project_response.pyi
--rw-r--r--   0        0        0     5356 2023-05-31 20:33:30.383583 humanloop-0.4.6/humanloop/model/paginated_data_session_response.py
--rw-r--r--   0        0        0     5356 2023-05-31 20:33:30.383719 humanloop-0.4.6/humanloop/model/paginated_data_session_response.pyi
--rw-r--r--   0        0        0     3319 2023-05-31 20:33:30.383852 humanloop-0.4.6/humanloop/model/positive_label.py
--rw-r--r--   0        0        0     3319 2023-05-31 20:33:30.383973 humanloop-0.4.6/humanloop/model/positive_label.pyi
--rw-r--r--   0        0        0     9076 2023-05-31 20:33:30.384134 humanloop-0.4.6/humanloop/model/project_config_response.py
--rw-r--r--   0        0        0     9076 2023-05-31 20:33:30.384331 humanloop-0.4.6/humanloop/model/project_config_response.pyi
--rw-r--r--   0        0        0    18539 2023-05-31 20:33:30.384516 humanloop-0.4.6/humanloop/model/project_model_config_request.py
--rw-r--r--   0        0        0    18539 2023-05-31 20:33:30.384678 humanloop-0.4.6/humanloop/model/project_model_config_request.pyi
--rw-r--r--   0        0        0    24144 2023-05-31 20:33:30.384842 humanloop-0.4.6/humanloop/model/project_model_config_response.py
--rw-r--r--   0        0        0    24144 2023-05-31 20:33:30.385001 humanloop-0.4.6/humanloop/model/project_model_config_response.pyi
--rw-r--r--   0        0        0    14071 2023-05-31 20:33:30.385148 humanloop-0.4.6/humanloop/model/project_response.py
--rw-r--r--   0        0        0    14071 2023-05-31 20:33:30.385343 humanloop-0.4.6/humanloop/model/project_response.pyi
--rw-r--r--   0        0        0     1647 2023-05-31 20:33:30.385487 humanloop-0.4.6/humanloop/model/project_sort_by.py
--rw-r--r--   0        0        0     1476 2023-05-31 20:33:30.385614 humanloop-0.4.6/humanloop/model/project_sort_by.pyi
--rw-r--r--   0        0        0     3971 2023-05-31 20:33:30.385726 humanloop-0.4.6/humanloop/model/project_user_response.py
--rw-r--r--   0        0        0     3971 2023-05-31 20:33:30.385829 humanloop-0.4.6/humanloop/model/project_user_response.pyi
--rw-r--r--   0        0        0     1889 2023-05-31 20:33:30.385925 humanloop-0.4.6/humanloop/model/projects_get_configs_response.py
--rw-r--r--   0        0        0     1889 2023-05-31 20:33:30.386018 humanloop-0.4.6/humanloop/model/projects_get_configs_response.pyi
--rw-r--r--   0        0        0     1891 2023-05-31 20:33:30.386680 humanloop-0.4.6/humanloop/model/projects_update_feedback_types_request.py
--rw-r--r--   0        0        0     1891 2023-05-31 20:33:30.386826 humanloop-0.4.6/humanloop/model/projects_update_feedback_types_request.pyi
--rw-r--r--   0        0        0     6114 2023-05-31 20:33:30.386942 humanloop-0.4.6/humanloop/model/provider_api_keys.py
--rw-r--r--   0        0        0     6114 2023-05-31 20:33:30.387036 humanloop-0.4.6/humanloop/model/provider_api_keys.pyi
--rw-r--r--   0        0        0     3289 2023-05-31 20:33:30.387125 humanloop-0.4.6/humanloop/model/session_project_response.py
--rw-r--r--   0        0        0     3289 2023-05-31 20:33:30.387221 humanloop-0.4.6/humanloop/model/session_project_response.pyi
--rw-r--r--   0        0        0     6796 2023-05-31 20:33:30.387308 humanloop-0.4.6/humanloop/model/session_response.py
--rw-r--r--   0        0        0     6796 2023-05-31 20:33:30.387395 humanloop-0.4.6/humanloop/model/session_response.pyi
--rw-r--r--   0        0        0     1485 2023-05-31 20:33:30.387488 humanloop-0.4.6/humanloop/model/sort_order.py
--rw-r--r--   0        0        0     1368 2023-05-31 20:33:30.387614 humanloop-0.4.6/humanloop/model/sort_order.pyi
--rw-r--r--   0        0        0    18103 2023-05-31 20:33:30.387749 humanloop-0.4.6/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.py
--rw-r--r--   0        0        0    18103 2023-05-31 20:33:30.387895 humanloop-0.4.6/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.pyi
--rw-r--r--   0        0        0     5065 2023-05-31 20:33:30.388028 humanloop-0.4.6/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     5065 2023-05-31 20:33:30.388154 humanloop-0.4.6/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi
--rw-r--r--   0        0        0    20786 2023-05-31 20:33:30.388295 humanloop-0.4.6/humanloop/model/src_external_app_models_v4_configs_model_config_response.py
--rw-r--r--   0        0        0    20786 2023-05-31 20:33:30.388475 humanloop-0.4.6/humanloop/model/src_external_app_models_v4_configs_model_config_response.pyi
--rw-r--r--   0        0        0     5069 2023-05-31 20:33:30.388614 humanloop-0.4.6/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     5069 2023-05-31 20:33:30.388752 humanloop-0.4.6/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.pyi
--rw-r--r--   0        0        0     5124 2023-05-31 20:33:30.388934 humanloop-0.4.6/humanloop/model/tool_config_request.py
--rw-r--r--   0        0        0     4961 2023-05-31 20:33:30.389120 humanloop-0.4.6/humanloop/model/tool_config_request.pyi
--rw-r--r--   0        0        0     7237 2023-05-31 20:33:30.389262 humanloop-0.4.6/humanloop/model/tool_config_response.py
--rw-r--r--   0        0        0     7237 2023-05-31 20:33:30.389380 humanloop-0.4.6/humanloop/model/tool_config_response.pyi
--rw-r--r--   0        0        0     4408 2023-05-31 20:33:30.389489 humanloop-0.4.6/humanloop/model/tool_result_response.py
--rw-r--r--   0        0        0     4408 2023-05-31 20:33:30.389587 humanloop-0.4.6/humanloop/model/tool_result_response.pyi
--rw-r--r--   0        0        0    13253 2023-05-31 20:33:30.389695 humanloop-0.4.6/humanloop/model/trace_log_request.py
--rw-r--r--   0        0        0    13253 2023-05-31 20:33:30.389825 humanloop-0.4.6/humanloop/model/trace_log_request.pyi
--rw-r--r--   0        0        0    19686 2023-05-31 20:33:30.389975 humanloop-0.4.6/humanloop/model/trace_model_config_request.py
--rw-r--r--   0        0        0    19521 2023-05-31 20:33:30.390108 humanloop-0.4.6/humanloop/model/trace_model_config_request.pyi
--rw-r--r--   0        0        0     7478 2023-05-31 20:33:30.390216 humanloop-0.4.6/humanloop/model/update_experiment_request.py
--rw-r--r--   0        0        0     7478 2023-05-31 20:33:30.390312 humanloop-0.4.6/humanloop/model/update_experiment_request.pyi
--rw-r--r--   0        0        0     3876 2023-05-31 20:33:30.390397 humanloop-0.4.6/humanloop/model/update_log_request.py
--rw-r--r--   0        0        0     3876 2023-05-31 20:33:30.390489 humanloop-0.4.6/humanloop/model/update_log_request.pyi
--rw-r--r--   0        0        0     5223 2023-05-31 20:33:30.390572 humanloop-0.4.6/humanloop/model/update_project_request.py
--rw-r--r--   0        0        0     5223 2023-05-31 20:33:30.390674 humanloop-0.4.6/humanloop/model/update_project_request.pyi
--rw-r--r--   0        0        0     4294 2023-05-31 20:33:30.390775 humanloop-0.4.6/humanloop/model/usage.py
--rw-r--r--   0        0        0     4294 2023-05-31 20:33:30.390886 humanloop-0.4.6/humanloop/model/usage.pyi
--rw-r--r--   0        0        0     6981 2023-05-31 20:33:30.390982 humanloop-0.4.6/humanloop/model/validation_error.py
--rw-r--r--   0        0        0     6981 2023-05-31 20:33:30.391087 humanloop-0.4.6/humanloop/model/validation_error.pyi
--rw-r--r--   0        0        0     6580 2023-05-31 20:33:30.391193 humanloop-0.4.6/humanloop/models/__init__.py
--rw-r--r--   0        0        0     1431 2023-05-31 20:33:30.391294 humanloop-0.4.6/humanloop/paths/__init__.py
--rw-r--r--   0        0        0      285 2023-05-31 20:33:30.391404 humanloop-0.4.6/humanloop/paths/chat/__init__.py
--rw-r--r--   0        0        0    17604 2023-05-31 20:33:30.391517 humanloop-0.4.6/humanloop/paths/chat/post.py
--rw-r--r--   0        0        0    17461 2023-05-31 20:33:30.391649 humanloop-0.4.6/humanloop/paths/chat/post.pyi
--rw-r--r--   0        0        0      302 2023-05-31 20:33:30.391778 humanloop-0.4.6/humanloop/paths/chat_deployed/__init__.py
--rw-r--r--   0        0        0    17167 2023-05-31 20:33:30.391891 humanloop-0.4.6/humanloop/paths/chat_deployed/post.py
--rw-r--r--   0        0        0    17024 2023-05-31 20:33:30.392029 humanloop-0.4.6/humanloop/paths/chat_deployed/post.pyi
--rw-r--r--   0        0        0      306 2023-05-31 20:33:30.392147 humanloop-0.4.6/humanloop/paths/chat_experiment/__init__.py
--rw-r--r--   0        0        0    17610 2023-05-31 20:33:30.392258 humanloop-0.4.6/humanloop/paths/chat_experiment/post.py
--rw-r--r--   0        0        0    17467 2023-05-31 20:33:30.392385 humanloop-0.4.6/humanloop/paths/chat_experiment/post.pyi
--rw-r--r--   0        0        0      309 2023-05-31 20:33:30.392492 humanloop-0.4.6/humanloop/paths/chat_model_config/__init__.py
--rw-r--r--   0        0        0    17785 2023-05-31 20:33:30.392591 humanloop-0.4.6/humanloop/paths/chat_model_config/post.py
--rw-r--r--   0        0        0    17642 2023-05-31 20:33:30.392710 humanloop-0.4.6/humanloop/paths/chat_model_config/post.pyi
--rw-r--r--   0        0        0      297 2023-05-31 20:33:30.392815 humanloop-0.4.6/humanloop/paths/completion/__init__.py
--rw-r--r--   0        0        0    17920 2023-05-31 20:33:30.392928 humanloop-0.4.6/humanloop/paths/completion/post.py
--rw-r--r--   0        0        0    17777 2023-05-31 20:33:30.393047 humanloop-0.4.6/humanloop/paths/completion/post.pyi
--rw-r--r--   0        0        0      314 2023-05-31 20:33:30.393155 humanloop-0.4.6/humanloop/paths/completion_deployed/__init__.py
--rw-r--r--   0        0        0    17423 2023-05-31 20:33:30.393264 humanloop-0.4.6/humanloop/paths/completion_deployed/post.py
--rw-r--r--   0        0        0    17280 2023-05-31 20:33:30.393384 humanloop-0.4.6/humanloop/paths/completion_deployed/post.pyi
--rw-r--r--   0        0        0      318 2023-05-31 20:33:30.393502 humanloop-0.4.6/humanloop/paths/completion_experiment/__init__.py
--rw-r--r--   0        0        0    17866 2023-05-31 20:33:30.393604 humanloop-0.4.6/humanloop/paths/completion_experiment/post.py
--rw-r--r--   0        0        0    17723 2023-05-31 20:33:30.393746 humanloop-0.4.6/humanloop/paths/completion_experiment/post.pyi
--rw-r--r--   0        0        0      321 2023-05-31 20:33:30.393882 humanloop-0.4.6/humanloop/paths/completion_model_config/__init__.py
--rw-r--r--   0        0        0    18041 2023-05-31 20:33:30.394192 humanloop-0.4.6/humanloop/paths/completion_model_config/post.py
--rw-r--r--   0        0        0    17898 2023-05-31 20:33:30.394514 humanloop-0.4.6/humanloop/paths/completion_model_config/post.pyi
--rw-r--r--   0        0        0      327 2023-05-31 20:33:30.394708 humanloop-0.4.6/humanloop/paths/experiments_experiment_id/__init__.py
--rw-r--r--   0        0        0    12171 2023-05-31 20:33:30.394883 humanloop-0.4.6/humanloop/paths/experiments_experiment_id/delete.py
--rw-r--r--   0        0        0    12028 2023-05-31 20:33:30.395129 humanloop-0.4.6/humanloop/paths/experiments_experiment_id/delete.pyi
--rw-r--r--   0        0        0    17219 2023-05-31 20:33:30.395463 humanloop-0.4.6/humanloop/paths/experiments_experiment_id/patch.py
--rw-r--r--   0        0        0    17076 2023-05-31 20:33:30.395742 humanloop-0.4.6/humanloop/paths/experiments_experiment_id/patch.pyi
--rw-r--r--   0        0        0      352 2023-05-31 20:33:30.395975 humanloop-0.4.6/humanloop/paths/experiments_experiment_id_model_config/__init__.py
--rw-r--r--   0        0        0    12672 2023-05-31 20:33:30.396175 humanloop-0.4.6/humanloop/paths/experiments_experiment_id_model_config/get.py
--rw-r--r--   0        0        0    12529 2023-05-31 20:33:30.396471 humanloop-0.4.6/humanloop/paths/experiments_experiment_id_model_config/get.pyi
--rw-r--r--   0        0        0      293 2023-05-31 20:33:30.396686 humanloop-0.4.6/humanloop/paths/feedback/__init__.py
--rw-r--r--   0        0        0    15265 2023-05-31 20:33:30.396840 humanloop-0.4.6/humanloop/paths/feedback/post.py
--rw-r--r--   0        0        0    15122 2023-05-31 20:33:30.397050 humanloop-0.4.6/humanloop/paths/feedback/post.pyi
--rw-r--r--   0        0        0      285 2023-05-31 20:33:30.397273 humanloop-0.4.6/humanloop/paths/logs/__init__.py
--rw-r--r--   0        0        0    16442 2023-05-31 20:33:30.397468 humanloop-0.4.6/humanloop/paths/logs/patch.py
--rw-r--r--   0        0        0    16299 2023-05-31 20:33:30.397676 humanloop-0.4.6/humanloop/paths/logs/patch.pyi
--rw-r--r--   0        0        0    22798 2023-05-31 20:33:30.397902 humanloop-0.4.6/humanloop/paths/logs/post.py
--rw-r--r--   0        0        0    22655 2023-05-31 20:33:30.398153 humanloop-0.4.6/humanloop/paths/logs/post.pyi
--rw-r--r--   0        0        0      291 2023-05-31 20:33:30.398385 humanloop-0.4.6/humanloop/paths/logs_id/__init__.py
--rw-r--r--   0        0        0    15508 2023-05-31 20:33:30.398577 humanloop-0.4.6/humanloop/paths/logs_id/patch.py
--rw-r--r--   0        0        0    15365 2023-05-31 20:33:30.398799 humanloop-0.4.6/humanloop/paths/logs_id/patch.pyi
--rw-r--r--   0        0        0      302 2023-05-31 20:33:30.399018 humanloop-0.4.6/humanloop/paths/model_configs/__init__.py
--rw-r--r--   0        0        0    20442 2023-05-31 20:33:30.399237 humanloop-0.4.6/humanloop/paths/model_configs/post.py
--rw-r--r--   0        0        0    20299 2023-05-31 20:33:30.399462 humanloop-0.4.6/humanloop/paths/model_configs/post.pyi
--rw-r--r--   0        0        0      308 2023-05-31 20:33:30.399649 humanloop-0.4.6/humanloop/paths/model_configs_id/__init__.py
--rw-r--r--   0        0        0    12485 2023-05-31 20:33:30.399806 humanloop-0.4.6/humanloop/paths/model_configs_id/get.py
--rw-r--r--   0        0        0    12342 2023-05-31 20:33:30.400007 humanloop-0.4.6/humanloop/paths/model_configs_id/get.pyi
--rw-r--r--   0        0        0      293 2023-05-31 20:33:30.400284 humanloop-0.4.6/humanloop/paths/projects/__init__.py
--rw-r--r--   0        0        0    20694 2023-05-31 20:33:30.400489 humanloop-0.4.6/humanloop/paths/projects/get.py
--rw-r--r--   0        0        0    20551 2023-05-31 20:33:30.400696 humanloop-0.4.6/humanloop/paths/projects/get.pyi
--rw-r--r--   0        0        0    13183 2023-05-31 20:33:30.400900 humanloop-0.4.6/humanloop/paths/projects/post.py
--rw-r--r--   0        0        0    13040 2023-05-31 20:33:30.401489 humanloop-0.4.6/humanloop/paths/projects/post.pyi
--rw-r--r--   0        0        0      299 2023-05-31 20:33:30.401699 humanloop-0.4.6/humanloop/paths/projects_id/__init__.py
--rw-r--r--   0        0        0    12155 2023-05-31 20:33:30.401861 humanloop-0.4.6/humanloop/paths/projects_id/get.py
--rw-r--r--   0        0        0    12012 2023-05-31 20:33:30.402054 humanloop-0.4.6/humanloop/paths/projects_id/get.pyi
--rw-r--r--   0        0        0    16242 2023-05-31 20:33:30.402227 humanloop-0.4.6/humanloop/paths/projects_id/patch.py
--rw-r--r--   0        0        0    16099 2023-05-31 20:33:30.402417 humanloop-0.4.6/humanloop/paths/projects_id/patch.pyi
--rw-r--r--   0        0        0      326 2023-05-31 20:33:30.402647 humanloop-0.4.6/humanloop/paths/projects_id_active_config/__init__.py
--rw-r--r--   0        0        0    12474 2023-05-31 20:33:30.402807 humanloop-0.4.6/humanloop/paths/projects_id_active_config/delete.py
--rw-r--r--   0        0        0    12331 2023-05-31 20:33:30.403056 humanloop-0.4.6/humanloop/paths/projects_id_active_config/delete.pyi
--rw-r--r--   0        0        0    12324 2023-05-31 20:33:30.403275 humanloop-0.4.6/humanloop/paths/projects_id_active_config/get.py
--rw-r--r--   0        0        0    12181 2023-05-31 20:33:30.403522 humanloop-0.4.6/humanloop/paths/projects_id_active_config/get.pyi
--rw-r--r--   0        0        0      334 2023-05-31 20:33:30.403777 humanloop-0.4.6/humanloop/paths/projects_id_active_experiment/__init__.py
--rw-r--r--   0        0        0    12482 2023-05-31 20:33:30.403975 humanloop-0.4.6/humanloop/paths/projects_id_active_experiment/delete.py
--rw-r--r--   0        0        0    12339 2023-05-31 20:33:30.404184 humanloop-0.4.6/humanloop/paths/projects_id_active_experiment/delete.pyi
--rw-r--r--   0        0        0      315 2023-05-31 20:33:30.404366 humanloop-0.4.6/humanloop/paths/projects_id_configs/__init__.py
--rw-r--r--   0        0        0    12358 2023-05-31 20:33:30.404525 humanloop-0.4.6/humanloop/paths/projects_id_configs/get.py
--rw-r--r--   0        0        0    12215 2023-05-31 20:33:30.404747 humanloop-0.4.6/humanloop/paths/projects_id_configs/get.pyi
--rw-r--r--   0        0        0      313 2023-05-31 20:33:30.404956 humanloop-0.4.6/humanloop/paths/projects_id_export/__init__.py
--rw-r--r--   0        0        0    15904 2023-05-31 20:33:30.405140 humanloop-0.4.6/humanloop/paths/projects_id_export/post.py
--rw-r--r--   0        0        0    15761 2023-05-31 20:33:30.405357 humanloop-0.4.6/humanloop/paths/projects_id_export/post.pyi
--rw-r--r--   0        0        0      328 2023-05-31 20:33:30.405528 humanloop-0.4.6/humanloop/paths/projects_id_feedback_types/__init__.py
--rw-r--r--   0        0        0    14974 2023-05-31 20:33:30.405699 humanloop-0.4.6/humanloop/paths/projects_id_feedback_types/patch.py
--rw-r--r--   0        0        0    14831 2023-05-31 20:33:30.405917 humanloop-0.4.6/humanloop/paths/projects_id_feedback_types/patch.pyi
--rw-r--r--   0        0        0      339 2023-05-31 20:33:30.406123 humanloop-0.4.6/humanloop/paths/projects_project_id_experiments/__init__.py
--rw-r--r--   0        0        0    12432 2023-05-31 20:33:30.406412 humanloop-0.4.6/humanloop/paths/projects_project_id_experiments/get.py
--rw-r--r--   0        0        0    12289 2023-05-31 20:33:30.406685 humanloop-0.4.6/humanloop/paths/projects_project_id_experiments/get.pyi
--rw-r--r--   0        0        0    16426 2023-05-31 20:33:30.406945 humanloop-0.4.6/humanloop/paths/projects_project_id_experiments/post.py
--rw-r--r--   0        0        0    16283 2023-05-31 20:33:30.407162 humanloop-0.4.6/humanloop/paths/projects_project_id_experiments/post.pyi
--rw-r--r--   0        0        0      293 2023-05-31 20:33:30.407378 humanloop-0.4.6/humanloop/paths/sessions/__init__.py
--rw-r--r--   0        0        0    14288 2023-05-31 20:33:30.407576 humanloop-0.4.6/humanloop/paths/sessions/get.py
--rw-r--r--   0        0        0    14145 2023-05-31 20:33:30.407797 humanloop-0.4.6/humanloop/paths/sessions/get.pyi
--rw-r--r--   0        0        0     9368 2023-05-31 20:33:30.407999 humanloop-0.4.6/humanloop/paths/sessions/post.py
--rw-r--r--   0        0        0     9255 2023-05-31 20:33:30.408212 humanloop-0.4.6/humanloop/paths/sessions/post.pyi
--rw-r--r--   0        0        0      299 2023-05-31 20:33:30.408412 humanloop-0.4.6/humanloop/paths/sessions_id/__init__.py
--rw-r--r--   0        0        0    12155 2023-05-31 20:33:30.408562 humanloop-0.4.6/humanloop/paths/sessions_id/get.py
--rw-r--r--   0        0        0    12012 2023-05-31 20:33:30.408769 humanloop-0.4.6/humanloop/paths/sessions_id/get.pyi
--rw-r--r--   0        0        0      289 2023-05-31 20:33:30.408987 humanloop-0.4.6/humanloop/paths/traces/__init__.py
--rw-r--r--   0        0        0    12626 2023-05-31 20:33:30.409135 humanloop-0.4.6/humanloop/paths/traces/post.py
--rw-r--r--   0        0        0    12483 2023-05-31 20:33:30.409297 humanloop-0.4.6/humanloop/paths/traces/post.pyi
--rw-r--r--   0        0        0     1187 2023-05-31 20:33:30.409507 humanloop-0.4.6/humanloop/request_after_hook.py
--rw-r--r--   0        0        0     1783 2023-05-31 20:33:30.450091 humanloop-0.4.6/humanloop/request_before_hook.py
--rw-r--r--   0        0        0    11505 2023-05-31 20:33:30.409875 humanloop-0.4.6/humanloop/rest.py
--rw-r--r--   0        0        0    96089 2023-05-31 20:33:30.410144 humanloop-0.4.6/humanloop/schemas.py
--rw-r--r--   0        0        0        0 2023-05-31 20:33:30.410315 humanloop-0.4.6/humanloop/type/__init__.py
--rw-r--r--   0        0        0     1590 2023-05-31 20:33:30.410400 humanloop-0.4.6/humanloop/type/agent_config_request.py
--rw-r--r--   0        0        0     1784 2023-05-31 20:33:30.410528 humanloop-0.4.6/humanloop/type/agent_config_response.py
--rw-r--r--   0        0        0     1584 2023-05-31 20:33:30.410634 humanloop-0.4.6/humanloop/type/base_metric_response.py
--rw-r--r--   0        0        0     1238 2023-05-31 20:33:30.410726 humanloop-0.4.6/humanloop/type/categorical_feedback_label.py
--rw-r--r--   0        0        0     2359 2023-05-31 20:33:30.410867 humanloop-0.4.6/humanloop/type/chat_data_response.py
--rw-r--r--   0        0        0     2166 2023-05-31 20:33:30.411025 humanloop-0.4.6/humanloop/type/chat_deployed_request.py
--rw-r--r--   0        0        0     2411 2023-05-31 20:33:30.411198 humanloop-0.4.6/humanloop/type/chat_experiment_request.py
--rw-r--r--   0        0        0     1095 2023-05-31 20:33:30.411373 humanloop-0.4.6/humanloop/type/chat_message.py
--rw-r--r--   0        0        0     2280 2023-05-31 20:33:30.411663 humanloop-0.4.6/humanloop/type/chat_model_config_request.py
--rw-r--r--   0        0        0     2306 2023-05-31 20:33:30.411826 humanloop-0.4.6/humanloop/type/chat_request.py
--rw-r--r--   0        0        0     1994 2023-05-31 20:33:30.411980 humanloop-0.4.6/humanloop/type/chat_response.py
--rw-r--r--   0        0        0      887 2023-05-31 20:33:30.412133 humanloop-0.4.6/humanloop/type/chat_role.py
--rw-r--r--   0        0        0     2271 2023-05-31 20:33:30.412302 humanloop-0.4.6/humanloop/type/completion_deployed_request.py
--rw-r--r--   0        0        0     2519 2023-05-31 20:33:30.412583 humanloop-0.4.6/humanloop/type/completion_experiment_request.py
--rw-r--r--   0        0        0     2385 2023-05-31 20:33:30.412809 humanloop-0.4.6/humanloop/type/completion_model_config_request.py
--rw-r--r--   0        0        0     2415 2023-05-31 20:33:30.412969 humanloop-0.4.6/humanloop/type/completion_request.py
--rw-r--r--   0        0        0     2040 2023-05-31 20:33:30.413090 humanloop-0.4.6/humanloop/type/completion_response.py
--rw-r--r--   0        0        0     1320 2023-05-31 20:33:30.413257 humanloop-0.4.6/humanloop/type/config_response.py
--rw-r--r--   0        0        0      895 2023-05-31 20:33:30.413438 humanloop-0.4.6/humanloop/type/config_type.py
--rw-r--r--   0        0        0     1538 2023-05-31 20:33:30.413597 humanloop-0.4.6/humanloop/type/create_experiment_request.py
--rw-r--r--   0        0        0     1200 2023-05-31 20:33:30.413762 humanloop-0.4.6/humanloop/type/create_log_response.py
--rw-r--r--   0        0        0     1242 2023-05-31 20:33:30.413914 humanloop-0.4.6/humanloop/type/create_project_request.py
--rw-r--r--   0        0        0     1118 2023-05-31 20:33:30.414056 humanloop-0.4.6/humanloop/type/create_session_response.py
--rw-r--r--   0        0        0     1221 2023-05-31 20:33:30.414201 humanloop-0.4.6/humanloop/type/create_trace_request.py
--rw-r--r--   0        0        0     1174 2023-05-31 20:33:30.414315 humanloop-0.4.6/humanloop/type/create_trace_response.py
--rw-r--r--   0        0        0     2189 2023-05-31 20:33:30.414485 humanloop-0.4.6/humanloop/type/data_response.py
--rw-r--r--   0        0        0     1853 2023-05-31 20:33:30.414637 humanloop-0.4.6/humanloop/type/experiment_config_response.py
--rw-r--r--   0        0        0     1964 2023-05-31 20:33:30.414791 humanloop-0.4.6/humanloop/type/experiment_response.py
--rw-r--r--   0        0        0      894 2023-05-31 20:33:30.414936 humanloop-0.4.6/humanloop/type/experiment_status.py
--rw-r--r--   0        0        0      961 2023-05-31 20:33:30.415110 humanloop-0.4.6/humanloop/type/experiments_list_response.py
--rw-r--r--   0        0        0     1625 2023-05-31 20:33:30.415263 humanloop-0.4.6/humanloop/type/feedback.py
--rw-r--r--   0        0        0      895 2023-05-31 20:33:30.415412 humanloop-0.4.6/humanloop/type/feedback_class.py
--rw-r--r--   0        0        0     1146 2023-05-31 20:33:30.415567 humanloop-0.4.6/humanloop/type/feedback_label_request.py
--rw-r--r--   0        0        0     1722 2023-05-31 20:33:30.415724 humanloop-0.4.6/humanloop/type/feedback_request.py
--rw-r--r--   0        0        0     1754 2023-05-31 20:33:30.415870 humanloop-0.4.6/humanloop/type/feedback_response.py
--rw-r--r--   0        0        0      980 2023-05-31 20:33:30.416021 humanloop-0.4.6/humanloop/type/feedback_submit_request.py
--rw-r--r--   0        0        0      985 2023-05-31 20:33:30.416165 humanloop-0.4.6/humanloop/type/feedback_submit_response.py
--rw-r--r--   0        0        0      914 2023-05-31 20:33:30.416302 humanloop-0.4.6/humanloop/type/feedback_type.py
--rw-r--r--   0        0        0     1483 2023-05-31 20:33:30.416461 humanloop-0.4.6/humanloop/type/feedback_type_model.py
--rw-r--r--   0        0        0     1717 2023-05-31 20:33:30.416609 humanloop-0.4.6/humanloop/type/feedback_type_request.py
--rw-r--r--   0        0        0      949 2023-05-31 20:33:30.417556 humanloop-0.4.6/humanloop/type/feedback_types.py
--rw-r--r--   0        0        0     1240 2023-05-31 20:33:30.417698 humanloop-0.4.6/humanloop/type/generic_config_request.py
--rw-r--r--   0        0        0     1438 2023-05-31 20:33:30.417931 humanloop-0.4.6/humanloop/type/generic_config_response.py
--rw-r--r--   0        0        0     2076 2023-05-31 20:33:30.418118 humanloop-0.4.6/humanloop/type/get_model_config_response.py
--rw-r--r--   0        0        0     1148 2023-05-31 20:33:30.418256 humanloop-0.4.6/humanloop/type/http_validation_error.py
--rw-r--r--   0        0        0      906 2023-05-31 20:33:30.418415 humanloop-0.4.6/humanloop/type/label_sentiment.py
--rw-r--r--   0        0        0      958 2023-05-31 20:33:30.418579 humanloop-0.4.6/humanloop/type/log_datapoint_request.py
--rw-r--r--   0        0        0     3209 2023-05-31 20:33:30.418727 humanloop-0.4.6/humanloop/type/log_model_config_request.py
--rw-r--r--   0        0        0     3857 2023-05-31 20:33:30.418890 humanloop-0.4.6/humanloop/type/log_request.py
--rw-r--r--   0        0        0     4048 2023-05-31 20:33:30.419043 humanloop-0.4.6/humanloop/type/log_response.py
--rw-r--r--   0        0        0      983 2023-05-31 20:33:30.419196 humanloop-0.4.6/humanloop/type/logs_log_response.py
--rw-r--r--   0        0        0     2996 2023-05-31 20:33:30.419355 humanloop-0.4.6/humanloop/type/model_config_chat_request.py
--rw-r--r--   0        0        0     2889 2023-05-31 20:33:30.419502 humanloop-0.4.6/humanloop/type/model_config_completion_request.py
--rw-r--r--   0        0        0      890 2023-05-31 20:33:30.419643 humanloop-0.4.6/humanloop/type/model_endpoints.py
--rw-r--r--   0        0        0      940 2023-05-31 20:33:30.419785 humanloop-0.4.6/humanloop/type/model_providers.py
--rw-r--r--   0        0        0     1208 2023-05-31 20:33:30.419927 humanloop-0.4.6/humanloop/type/paginated_data_log_response.py
--rw-r--r--   0        0        0     1240 2023-05-31 20:33:30.420065 humanloop-0.4.6/humanloop/type/paginated_data_project_response.py
--rw-r--r--   0        0        0     1240 2023-05-31 20:33:30.420203 humanloop-0.4.6/humanloop/type/paginated_data_session_response.py
--rw-r--r--   0        0        0     1047 2023-05-31 20:33:30.420359 humanloop-0.4.6/humanloop/type/positive_label.py
--rw-r--r--   0        0        0     1996 2023-05-31 20:33:30.420529 humanloop-0.4.6/humanloop/type/project_config_response.py
--rw-r--r--   0        0        0     3586 2023-05-31 20:33:30.420692 humanloop-0.4.6/humanloop/type/project_model_config_request.py
--rw-r--r--   0        0        0     4229 2023-05-31 20:33:30.420942 humanloop-0.4.6/humanloop/type/project_model_config_response.py
--rw-r--r--   0        0        0     2208 2023-05-31 20:33:30.421146 humanloop-0.4.6/humanloop/type/project_response.py
--rw-r--r--   0        0        0      897 2023-05-31 20:33:30.421309 humanloop-0.4.6/humanloop/type/project_sort_by.py
--rw-r--r--   0        0        0     1198 2023-05-31 20:33:30.421473 humanloop-0.4.6/humanloop/type/project_user_response.py
--rw-r--r--   0        0        0      974 2023-05-31 20:33:30.421644 humanloop-0.4.6/humanloop/type/projects_get_configs_response.py
--rw-r--r--   0        0        0      976 2023-05-31 20:33:30.421805 humanloop-0.4.6/humanloop/type/projects_update_feedback_types_request.py
--rw-r--r--   0        0        0     1165 2023-05-31 20:33:30.421949 humanloop-0.4.6/humanloop/type/provider_api_keys.py
--rw-r--r--   0        0        0     1161 2023-05-31 20:33:30.422100 humanloop-0.4.6/humanloop/type/session_project_response.py
--rw-r--r--   0        0        0     1618 2023-05-31 20:33:30.422243 humanloop-0.4.6/humanloop/type/session_response.py
--rw-r--r--   0        0        0      872 2023-05-31 20:33:30.422384 humanloop-0.4.6/humanloop/type/sort_order.py
--rw-r--r--   0        0        0     3506 2023-05-31 20:33:30.422540 humanloop-0.4.6/humanloop/type/src_external_app_models_v3_model_configs_model_config_response.py
--rw-r--r--   0        0        0     1417 2023-05-31 20:33:30.422699 humanloop-0.4.6/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     3597 2023-05-31 20:33:30.422881 humanloop-0.4.6/humanloop/type/src_external_app_models_v4_configs_model_config_response.py
--rw-r--r--   0        0        0     1427 2023-05-31 20:33:30.423055 humanloop-0.4.6/humanloop/type/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     1242 2023-05-31 20:33:30.423217 humanloop-0.4.6/humanloop/type/tool_config_request.py
--rw-r--r--   0        0        0     1471 2023-05-31 20:33:30.423395 humanloop-0.4.6/humanloop/type/tool_config_response.py
--rw-r--r--   0        0        0     1106 2023-05-31 20:33:30.423571 humanloop-0.4.6/humanloop/type/tool_result_response.py
--rw-r--r--   0        0        0     2632 2023-05-31 20:33:30.423741 humanloop-0.4.6/humanloop/type/trace_log_request.py
--rw-r--r--   0        0        0     3271 2023-05-31 20:33:30.423890 humanloop-0.4.6/humanloop/type/trace_model_config_request.py
--rw-r--r--   0        0        0     1537 2023-05-31 20:33:30.424039 humanloop-0.4.6/humanloop/type/update_experiment_request.py
--rw-r--r--   0        0        0     1259 2023-05-31 20:33:30.424167 humanloop-0.4.6/humanloop/type/update_log_request.py
--rw-r--r--   0        0        0     1610 2023-05-31 20:33:30.424301 humanloop-0.4.6/humanloop/type/update_project_request.py
--rw-r--r--   0        0        0     1218 2023-05-31 20:33:30.424396 humanloop-0.4.6/humanloop/type/usage.py
--rw-r--r--   0        0        0     1127 2023-05-31 20:33:30.424527 humanloop-0.4.6/humanloop/type/validation_error.py
--rw-r--r--   0        0        0     1044 2023-05-31 20:33:30.424730 humanloop-0.4.6/humanloop/type_util.py
--rw-r--r--   0        0        0     3165 2023-05-31 20:33:30.424883 humanloop-0.4.6/humanloop/validation_metadata.py
--rw-r--r--   0        0        0      714 2023-05-31 20:33:30.425259 humanloop-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     9366 1970-01-01 00:00:00.000000 humanloop-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-02 17:30:52.283879 humanloop-0.4.7/LICENSE
+-rw-r--r--   0        0        0     8475 2023-06-02 17:30:52.333307 humanloop-0.4.7/README.md
+-rw-r--r--   0        0        0     1235 2023-06-02 17:30:52.196579 humanloop-0.4.7/humanloop/__init__.py
+-rw-r--r--   0        0        0    73185 2023-06-02 17:30:52.196891 humanloop-0.4.7/humanloop/api_client.py
+-rw-r--r--   0        0        0      663 2023-06-02 17:30:52.197081 humanloop-0.4.7/humanloop/api_response.py
+-rw-r--r--   0        0        0      214 2023-06-02 17:30:52.197233 humanloop-0.4.7/humanloop/apis/__init__.py
+-rw-r--r--   0        0        0     4698 2023-06-02 17:30:52.197384 humanloop-0.4.7/humanloop/apis/path_to_api.py
+-rw-r--r--   0        0        0      236 2023-06-02 17:30:52.197545 humanloop-0.4.7/humanloop/apis/paths/__init__.py
+-rw-r--r--   0        0        0       91 2023-06-02 17:30:52.197687 humanloop-0.4.7/humanloop/apis/paths/chat.py
+-rw-r--r--   0        0        0      108 2023-06-02 17:30:52.197829 humanloop-0.4.7/humanloop/apis/paths/chat_deployed.py
+-rw-r--r--   0        0        0      112 2023-06-02 17:30:52.197969 humanloop-0.4.7/humanloop/apis/paths/chat_experiment.py
+-rw-r--r--   0        0        0      115 2023-06-02 17:30:52.198108 humanloop-0.4.7/humanloop/apis/paths/chat_model_config.py
+-rw-r--r--   0        0        0      103 2023-06-02 17:30:52.198294 humanloop-0.4.7/humanloop/apis/paths/completion.py
+-rw-r--r--   0        0        0      120 2023-06-02 17:30:52.198501 humanloop-0.4.7/humanloop/apis/paths/completion_deployed.py
+-rw-r--r--   0        0        0      124 2023-06-02 17:30:52.198675 humanloop-0.4.7/humanloop/apis/paths/completion_experiment.py
+-rw-r--r--   0        0        0      127 2023-06-02 17:30:52.198844 humanloop-0.4.7/humanloop/apis/paths/completion_model_config.py
+-rw-r--r--   0        0        0      226 2023-06-02 17:30:52.199019 humanloop-0.4.7/humanloop/apis/paths/experiments_experiment_id.py
+-rw-r--r--   0        0        0      152 2023-06-02 17:30:52.199187 humanloop-0.4.7/humanloop/apis/paths/experiments_experiment_id_model_config.py
+-rw-r--r--   0        0        0       99 2023-06-02 17:30:52.199355 humanloop-0.4.7/humanloop/apis/paths/feedback.py
+-rw-r--r--   0        0        0      159 2023-06-02 17:30:52.199516 humanloop-0.4.7/humanloop/apis/paths/logs.py
+-rw-r--r--   0        0        0       99 2023-06-02 17:30:52.199691 humanloop-0.4.7/humanloop/apis/paths/logs_id.py
+-rw-r--r--   0        0        0      108 2023-06-02 17:30:52.199855 humanloop-0.4.7/humanloop/apis/paths/model_configs.py
+-rw-r--r--   0        0        0      110 2023-06-02 17:30:52.200008 humanloop-0.4.7/humanloop/apis/paths/model_configs_id.py
+-rw-r--r--   0        0        0      165 2023-06-02 17:30:52.200179 humanloop-0.4.7/humanloop/apis/paths/projects.py
+-rw-r--r--   0        0        0      176 2023-06-02 17:30:52.200323 humanloop-0.4.7/humanloop/apis/paths/projects_id.py
+-rw-r--r--   0        0        0      219 2023-06-02 17:30:52.200475 humanloop-0.4.7/humanloop/apis/paths/projects_id_active_config.py
+-rw-r--r--   0        0        0      144 2023-06-02 17:30:52.200650 humanloop-0.4.7/humanloop/apis/paths/projects_id_active_experiment.py
+-rw-r--r--   0        0        0      116 2023-06-02 17:30:52.200823 humanloop-0.4.7/humanloop/apis/paths/projects_id_configs.py
+-rw-r--r--   0        0        0      117 2023-06-02 17:30:52.201003 humanloop-0.4.7/humanloop/apis/paths/projects_id_export.py
+-rw-r--r--   0        0        0      135 2023-06-02 17:30:52.201218 humanloop-0.4.7/humanloop/apis/paths/projects_id_feedback_types.py
+-rw-r--r--   0        0        0      231 2023-06-02 17:30:52.201439 humanloop-0.4.7/humanloop/apis/paths/projects_project_id_experiments.py
+-rw-r--r--   0        0        0      165 2023-06-02 17:30:52.201605 humanloop-0.4.7/humanloop/apis/paths/sessions.py
+-rw-r--r--   0        0        0      101 2023-06-02 17:30:52.201777 humanloop-0.4.7/humanloop/apis/paths/sessions_id.py
+-rw-r--r--   0        0        0       95 2023-06-02 17:30:52.201944 humanloop-0.4.7/humanloop/apis/paths/traces.py
+-rw-r--r--   0        0        0     1654 2023-06-02 17:30:52.202170 humanloop-0.4.7/humanloop/apis/tag_to_api.py
+-rw-r--r--   0        0        0      572 2023-06-02 17:30:52.202411 humanloop-0.4.7/humanloop/apis/tags/__init__.py
+-rw-r--r--   0        0        0     1182 2023-06-02 17:30:52.202534 humanloop-0.4.7/humanloop/apis/tags/chats_api.py
+-rw-r--r--   0        0        0     1196 2023-06-02 17:30:52.202642 humanloop-0.4.7/humanloop/apis/tags/completions_api.py
+-rw-r--r--   0        0        0     1267 2023-06-02 17:30:52.202741 humanloop-0.4.7/humanloop/apis/tags/experiments_api.py
+-rw-r--r--   0        0        0      897 2023-06-02 17:30:52.202840 humanloop-0.4.7/humanloop/apis/tags/feedback_api.py
+-rw-r--r--   0        0        0     1028 2023-06-02 17:30:52.202929 humanloop-0.4.7/humanloop/apis/tags/logs_api.py
+-rw-r--r--   0        0        0      979 2023-06-02 17:30:52.203024 humanloop-0.4.7/humanloop/apis/tags/model_configurations_api.py
+-rw-r--r--   0        0        0     1662 2023-06-02 17:30:52.203118 humanloop-0.4.7/humanloop/apis/tags/projects_api.py
+-rw-r--r--   0        0        0     1010 2023-06-02 17:30:52.203211 humanloop-0.4.7/humanloop/apis/tags/sessions_api.py
+-rw-r--r--   0        0        0      893 2023-06-02 17:30:52.203300 humanloop-0.4.7/humanloop/apis/tags/traces_api.py
+-rw-r--r--   0        0        0    28838 2023-06-02 17:30:52.203413 humanloop-0.4.7/humanloop/client.py
+-rw-r--r--   0        0        0    28838 2023-06-02 17:30:52.203541 humanloop-0.4.7/humanloop/client.pyi
+-rw-r--r--   0        0        0     6780 2023-06-02 17:30:52.283222 humanloop-0.4.7/humanloop/client_custom.py
+-rw-r--r--   0        0        0    18850 2023-06-02 17:30:52.203764 humanloop-0.4.7/humanloop/configuration.py
+-rw-r--r--   0        0        0     7854 2023-06-02 17:30:52.203903 humanloop-0.4.7/humanloop/exceptions.py
+-rw-r--r--   0        0        0     2274 2023-06-02 17:30:52.204004 humanloop-0.4.7/humanloop/exceptions_base.py
+-rw-r--r--   0        0        0      343 2023-06-02 17:30:52.204208 humanloop-0.4.7/humanloop/model/__init__.py
+-rw-r--r--   0        0        0     9316 2023-06-02 17:30:52.204322 humanloop-0.4.7/humanloop/model/agent_config_request.py
+-rw-r--r--   0        0        0     9151 2023-06-02 17:30:52.204484 humanloop-0.4.7/humanloop/model/agent_config_request.pyi
+-rw-r--r--   0        0        0     9818 2023-06-02 17:30:52.204622 humanloop-0.4.7/humanloop/model/agent_config_response.py
+-rw-r--r--   0        0        0     9653 2023-06-02 17:30:52.204772 humanloop-0.4.7/humanloop/model/agent_config_response.pyi
+-rw-r--r--   0        0        0     6555 2023-06-02 17:30:52.204897 humanloop-0.4.7/humanloop/model/base_metric_response.py
+-rw-r--r--   0        0        0     6555 2023-06-02 17:30:52.205004 humanloop-0.4.7/humanloop/model/base_metric_response.pyi
+-rw-r--r--   0        0        0     5326 2023-06-02 17:30:52.205111 humanloop-0.4.7/humanloop/model/categorical_feedback_label.py
+-rw-r--r--   0        0        0     5326 2023-06-02 17:30:52.205291 humanloop-0.4.7/humanloop/model/categorical_feedback_label.pyi
+-rw-r--r--   0        0        0     9133 2023-06-02 17:30:52.205507 humanloop-0.4.7/humanloop/model/chat_data_response.py
+-rw-r--r--   0        0        0     9133 2023-06-02 17:30:52.205689 humanloop-0.4.7/humanloop/model/chat_data_response.pyi
+-rw-r--r--   0        0        0    10174 2023-06-02 17:30:52.205865 humanloop-0.4.7/humanloop/model/chat_deployed_request.py
+-rw-r--r--   0        0        0    10174 2023-06-02 17:30:52.206077 humanloop-0.4.7/humanloop/model/chat_deployed_request.pyi
+-rw-r--r--   0        0        0    10835 2023-06-02 17:30:52.206227 humanloop-0.4.7/humanloop/model/chat_experiment_request.py
+-rw-r--r--   0        0        0    10835 2023-06-02 17:30:52.206355 humanloop-0.4.7/humanloop/model/chat_experiment_request.pyi
+-rw-r--r--   0        0        0     3878 2023-06-02 17:30:52.206480 humanloop-0.4.7/humanloop/model/chat_message.py
+-rw-r--r--   0        0        0     3878 2023-06-02 17:30:52.206582 humanloop-0.4.7/humanloop/model/chat_message.pyi
+-rw-r--r--   0        0        0    10869 2023-06-02 17:30:52.206702 humanloop-0.4.7/humanloop/model/chat_model_config_request.py
+-rw-r--r--   0        0        0    10869 2023-06-02 17:30:52.206837 humanloop-0.4.7/humanloop/model/chat_model_config_request.pyi
+-rw-r--r--   0        0        0    12732 2023-06-02 17:30:52.206983 humanloop-0.4.7/humanloop/model/chat_request.py
+-rw-r--r--   0        0        0    12732 2023-06-02 17:30:52.207133 humanloop-0.4.7/humanloop/model/chat_request.pyi
+-rw-r--r--   0        0        0    11252 2023-06-02 17:30:52.207279 humanloop-0.4.7/humanloop/model/chat_response.py
+-rw-r--r--   0        0        0    11252 2023-06-02 17:30:52.207400 humanloop-0.4.7/humanloop/model/chat_response.pyi
+-rw-r--r--   0        0        0     1622 2023-06-02 17:30:52.207512 humanloop-0.4.7/humanloop/model/chat_role.py
+-rw-r--r--   0        0        0     1461 2023-06-02 17:30:52.207609 humanloop-0.4.7/humanloop/model/chat_role.pyi
+-rw-r--r--   0        0        0     9850 2023-06-02 17:30:52.207711 humanloop-0.4.7/humanloop/model/completion_deployed_request.py
+-rw-r--r--   0        0        0     9850 2023-06-02 17:30:52.207862 humanloop-0.4.7/humanloop/model/completion_deployed_request.pyi
+-rw-r--r--   0        0        0    10516 2023-06-02 17:30:52.208021 humanloop-0.4.7/humanloop/model/completion_experiment_request.py
+-rw-r--r--   0        0        0    10516 2023-06-02 17:30:52.208151 humanloop-0.4.7/humanloop/model/completion_experiment_request.pyi
+-rw-r--r--   0        0        0    10552 2023-06-02 17:30:52.208301 humanloop-0.4.7/humanloop/model/completion_model_config_request.py
+-rw-r--r--   0        0        0    10552 2023-06-02 17:30:52.208451 humanloop-0.4.7/humanloop/model/completion_model_config_request.pyi
+-rw-r--r--   0        0        0    12434 2023-06-02 17:30:52.208564 humanloop-0.4.7/humanloop/model/completion_request.py
+-rw-r--r--   0        0        0    12434 2023-06-02 17:30:52.208742 humanloop-0.4.7/humanloop/model/completion_request.pyi
+-rw-r--r--   0        0        0    11193 2023-06-02 17:30:52.208958 humanloop-0.4.7/humanloop/model/completion_response.py
+-rw-r--r--   0        0        0    11193 2023-06-02 17:30:52.209185 humanloop-0.4.7/humanloop/model/completion_response.pyi
+-rw-r--r--   0        0        0     3636 2023-06-02 17:30:52.209383 humanloop-0.4.7/humanloop/model/config_response.py
+-rw-r--r--   0        0        0     3636 2023-06-02 17:30:52.209526 humanloop-0.4.7/humanloop/model/config_response.pyi
+-rw-r--r--   0        0        0     1722 2023-06-02 17:30:52.209666 humanloop-0.4.7/humanloop/model/config_type.py
+-rw-r--r--   0        0        0     1537 2023-06-02 17:30:52.209774 humanloop-0.4.7/humanloop/model/config_type.pyi
+-rw-r--r--   0        0        0     6372 2023-06-02 17:30:52.209928 humanloop-0.4.7/humanloop/model/create_experiment_request.py
+-rw-r--r--   0        0        0     6372 2023-06-02 17:30:52.210080 humanloop-0.4.7/humanloop/model/create_experiment_request.pyi
+-rw-r--r--   0        0        0     3375 2023-06-02 17:30:52.210241 humanloop-0.4.7/humanloop/model/create_log_response.py
+-rw-r--r--   0        0        0     3375 2023-06-02 17:30:52.210492 humanloop-0.4.7/humanloop/model/create_log_response.pyi
+-rw-r--r--   0        0        0     4442 2023-06-02 17:30:52.210731 humanloop-0.4.7/humanloop/model/create_project_request.py
+-rw-r--r--   0        0        0     4442 2023-06-02 17:30:52.210881 humanloop-0.4.7/humanloop/model/create_project_request.pyi
+-rw-r--r--   0        0        0     2811 2023-06-02 17:30:52.211081 humanloop-0.4.7/humanloop/model/create_session_response.py
+-rw-r--r--   0        0        0     2811 2023-06-02 17:30:52.211266 humanloop-0.4.7/humanloop/model/create_session_response.pyi
+-rw-r--r--   0        0        0     3408 2023-06-02 17:30:52.211423 humanloop-0.4.7/humanloop/model/create_trace_request.py
+-rw-r--r--   0        0        0     3408 2023-06-02 17:30:52.211599 humanloop-0.4.7/humanloop/model/create_trace_request.pyi
+-rw-r--r--   0        0        0     3505 2023-06-02 17:30:52.211760 humanloop-0.4.7/humanloop/model/create_trace_response.py
+-rw-r--r--   0        0        0     3505 2023-06-02 17:30:52.211908 humanloop-0.4.7/humanloop/model/create_trace_response.pyi
+-rw-r--r--   0        0        0     7631 2023-06-02 17:30:52.212064 humanloop-0.4.7/humanloop/model/data_response.py
+-rw-r--r--   0        0        0     7631 2023-06-02 17:30:52.212237 humanloop-0.4.7/humanloop/model/data_response.pyi
+-rw-r--r--   0        0        0     9174 2023-06-02 17:30:52.212440 humanloop-0.4.7/humanloop/model/experiment_config_response.py
+-rw-r--r--   0        0        0     9174 2023-06-02 17:30:52.212737 humanloop-0.4.7/humanloop/model/experiment_config_response.pyi
+-rw-r--r--   0        0        0    13003 2023-06-02 17:30:52.213016 humanloop-0.4.7/humanloop/model/experiment_response.py
+-rw-r--r--   0        0        0    13003 2023-06-02 17:30:52.213326 humanloop-0.4.7/humanloop/model/experiment_response.pyi
+-rw-r--r--   0        0        0     1552 2023-06-02 17:30:52.213563 humanloop-0.4.7/humanloop/model/experiment_status.py
+-rw-r--r--   0        0        0     1405 2023-06-02 17:30:52.213732 humanloop-0.4.7/humanloop/model/experiment_status.pyi
+-rw-r--r--   0        0        0     1861 2023-06-02 17:30:52.213905 humanloop-0.4.7/humanloop/model/experiments_list_response.py
+-rw-r--r--   0        0        0     1861 2023-06-02 17:30:52.214042 humanloop-0.4.7/humanloop/model/experiments_list_response.pyi
+-rw-r--r--   0        0        0     6857 2023-06-02 17:30:52.214182 humanloop-0.4.7/humanloop/model/feedback.py
+-rw-r--r--   0        0        0     6857 2023-06-02 17:30:52.214388 humanloop-0.4.7/humanloop/model/feedback.pyi
+-rw-r--r--   0        0        0     1639 2023-06-02 17:30:52.214600 humanloop-0.4.7/humanloop/model/feedback_class.py
+-rw-r--r--   0        0        0     1472 2023-06-02 17:30:52.214761 humanloop-0.4.7/humanloop/model/feedback_class.pyi
+-rw-r--r--   0        0        0     3510 2023-06-02 17:30:52.214920 humanloop-0.4.7/humanloop/model/feedback_label_request.py
+-rw-r--r--   0        0        0     3510 2023-06-02 17:30:52.215073 humanloop-0.4.7/humanloop/model/feedback_label_request.pyi
+-rw-r--r--   0        0        0     7365 2023-06-02 17:30:52.215216 humanloop-0.4.7/humanloop/model/feedback_request.py
+-rw-r--r--   0        0        0     7365 2023-06-02 17:30:52.215359 humanloop-0.4.7/humanloop/model/feedback_request.pyi
+-rw-r--r--   0        0        0     7317 2023-06-02 17:30:52.215532 humanloop-0.4.7/humanloop/model/feedback_response.py
+-rw-r--r--   0        0        0     7317 2023-06-02 17:30:52.215713 humanloop-0.4.7/humanloop/model/feedback_response.pyi
+-rw-r--r--   0        0        0     3376 2023-06-02 17:30:52.215906 humanloop-0.4.7/humanloop/model/feedback_submit_request.py
+-rw-r--r--   0        0        0     3376 2023-06-02 17:30:52.216050 humanloop-0.4.7/humanloop/model/feedback_submit_request.pyi
+-rw-r--r--   0        0        0     3386 2023-06-02 17:30:52.216209 humanloop-0.4.7/humanloop/model/feedback_submit_response.py
+-rw-r--r--   0        0        0     3386 2023-06-02 17:30:52.216367 humanloop-0.4.7/humanloop/model/feedback_submit_response.pyi
+-rw-r--r--   0        0        0     1866 2023-06-02 17:30:52.216532 humanloop-0.4.7/humanloop/model/feedback_type.py
+-rw-r--r--   0        0        0     1635 2023-06-02 17:30:52.216680 humanloop-0.4.7/humanloop/model/feedback_type.pyi
+-rw-r--r--   0        0        0     6337 2023-06-02 17:30:52.216840 humanloop-0.4.7/humanloop/model/feedback_type_model.py
+-rw-r--r--   0        0        0     6337 2023-06-02 17:30:52.216997 humanloop-0.4.7/humanloop/model/feedback_type_model.pyi
+-rw-r--r--   0        0        0     6465 2023-06-02 17:30:52.217151 humanloop-0.4.7/humanloop/model/feedback_type_request.py
+-rw-r--r--   0        0        0     6465 2023-06-02 17:30:52.217304 humanloop-0.4.7/humanloop/model/feedback_type_request.pyi
+-rw-r--r--   0        0        0     1835 2023-06-02 17:30:52.217451 humanloop-0.4.7/humanloop/model/feedback_types.py
+-rw-r--r--   0        0        0     1835 2023-06-02 17:30:52.217608 humanloop-0.4.7/humanloop/model/feedback_types.pyi
+-rw-r--r--   0        0        0     4583 2023-06-02 17:30:52.217760 humanloop-0.4.7/humanloop/model/generic_config_request.py
+-rw-r--r--   0        0        0     4414 2023-06-02 17:30:52.217909 humanloop-0.4.7/humanloop/model/generic_config_request.pyi
+-rw-r--r--   0        0        0     5247 2023-06-02 17:30:52.218044 humanloop-0.4.7/humanloop/model/generic_config_response.py
+-rw-r--r--   0        0        0     5078 2023-06-02 17:30:52.218162 humanloop-0.4.7/humanloop/model/generic_config_response.pyi
+-rw-r--r--   0        0        0     9795 2023-06-02 17:30:52.218320 humanloop-0.4.7/humanloop/model/get_model_config_response.py
+-rw-r--r--   0        0        0     9795 2023-06-02 17:30:52.218529 humanloop-0.4.7/humanloop/model/get_model_config_response.pyi
+-rw-r--r--   0        0        0     3787 2023-06-02 17:30:52.218714 humanloop-0.4.7/humanloop/model/http_validation_error.py
+-rw-r--r--   0        0        0     3787 2023-06-02 17:30:52.218851 humanloop-0.4.7/humanloop/model/http_validation_error.pyi
+-rw-r--r--   0        0        0     1843 2023-06-02 17:30:52.218991 humanloop-0.4.7/humanloop/model/label_sentiment.py
+-rw-r--r--   0        0        0     1644 2023-06-02 17:30:52.219139 humanloop-0.4.7/humanloop/model/label_sentiment.pyi
+-rw-r--r--   0        0        0     3332 2023-06-02 17:30:52.219287 humanloop-0.4.7/humanloop/model/log_datapoint_request.py
+-rw-r--r--   0        0        0     3332 2023-06-02 17:30:52.219456 humanloop-0.4.7/humanloop/model/log_datapoint_request.pyi
+-rw-r--r--   0        0        0    17395 2023-06-02 17:30:52.219678 humanloop-0.4.7/humanloop/model/log_model_config_request.py
+-rw-r--r--   0        0        0    17395 2023-06-02 17:30:52.219965 humanloop-0.4.7/humanloop/model/log_model_config_request.pyi
+-rw-r--r--   0        0        0    17925 2023-06-02 17:30:52.220188 humanloop-0.4.7/humanloop/model/log_request.py
+-rw-r--r--   0        0        0    17925 2023-06-02 17:30:52.220421 humanloop-0.4.7/humanloop/model/log_request.pyi
+-rw-r--r--   0        0        0    22277 2023-06-02 17:30:52.220650 humanloop-0.4.7/humanloop/model/log_response.py
+-rw-r--r--   0        0        0    22277 2023-06-02 17:30:52.220936 humanloop-0.4.7/humanloop/model/log_response.pyi
+-rw-r--r--   0        0        0     3381 2023-06-02 17:30:52.221168 humanloop-0.4.7/humanloop/model/logs_log_response.py
+-rw-r--r--   0        0        0     3381 2023-06-02 17:30:52.221433 humanloop-0.4.7/humanloop/model/logs_log_response.pyi
+-rw-r--r--   0        0        0    16422 2023-06-02 17:30:52.221711 humanloop-0.4.7/humanloop/model/model_config_chat_request.py
+-rw-r--r--   0        0        0    16422 2023-06-02 17:30:52.222125 humanloop-0.4.7/humanloop/model/model_config_chat_request.pyi
+-rw-r--r--   0        0        0    15562 2023-06-02 17:30:52.222494 humanloop-0.4.7/humanloop/model/model_config_completion_request.py
+-rw-r--r--   0        0        0    15562 2023-06-02 17:30:52.222797 humanloop-0.4.7/humanloop/model/model_config_completion_request.pyi
+-rw-r--r--   0        0        0     1636 2023-06-02 17:30:52.223112 humanloop-0.4.7/humanloop/model/model_endpoints.py
+-rw-r--r--   0        0        0     1481 2023-06-02 17:30:52.223329 humanloop-0.4.7/humanloop/model/model_endpoints.pyi
+-rw-r--r--   0        0        0     2123 2023-06-02 17:30:52.223530 humanloop-0.4.7/humanloop/model/model_providers.py
+-rw-r--r--   0        0        0     1820 2023-06-02 17:30:52.223716 humanloop-0.4.7/humanloop/model/model_providers.pyi
+-rw-r--r--   0        0        0     5320 2023-06-02 17:30:52.223934 humanloop-0.4.7/humanloop/model/paginated_data_log_response.py
+-rw-r--r--   0        0        0     5320 2023-06-02 17:30:52.224167 humanloop-0.4.7/humanloop/model/paginated_data_log_response.pyi
+-rw-r--r--   0        0        0     5356 2023-06-02 17:30:52.224365 humanloop-0.4.7/humanloop/model/paginated_data_project_response.py
+-rw-r--r--   0        0        0     5356 2023-06-02 17:30:52.224556 humanloop-0.4.7/humanloop/model/paginated_data_project_response.pyi
+-rw-r--r--   0        0        0     5356 2023-06-02 17:30:52.224750 humanloop-0.4.7/humanloop/model/paginated_data_session_response.py
+-rw-r--r--   0        0        0     5356 2023-06-02 17:30:52.224963 humanloop-0.4.7/humanloop/model/paginated_data_session_response.pyi
+-rw-r--r--   0        0        0     3319 2023-06-02 17:30:52.225148 humanloop-0.4.7/humanloop/model/positive_label.py
+-rw-r--r--   0        0        0     3319 2023-06-02 17:30:52.225313 humanloop-0.4.7/humanloop/model/positive_label.pyi
+-rw-r--r--   0        0        0     9076 2023-06-02 17:30:52.225472 humanloop-0.4.7/humanloop/model/project_config_response.py
+-rw-r--r--   0        0        0     9076 2023-06-02 17:30:52.225675 humanloop-0.4.7/humanloop/model/project_config_response.pyi
+-rw-r--r--   0        0        0    18539 2023-06-02 17:30:52.225882 humanloop-0.4.7/humanloop/model/project_model_config_request.py
+-rw-r--r--   0        0        0    18539 2023-06-02 17:30:52.226092 humanloop-0.4.7/humanloop/model/project_model_config_request.pyi
+-rw-r--r--   0        0        0    24144 2023-06-02 17:30:52.226315 humanloop-0.4.7/humanloop/model/project_model_config_response.py
+-rw-r--r--   0        0        0    24144 2023-06-02 17:30:52.226590 humanloop-0.4.7/humanloop/model/project_model_config_response.pyi
+-rw-r--r--   0        0        0    14071 2023-06-02 17:30:52.226787 humanloop-0.4.7/humanloop/model/project_response.py
+-rw-r--r--   0        0        0    14071 2023-06-02 17:30:52.227005 humanloop-0.4.7/humanloop/model/project_response.pyi
+-rw-r--r--   0        0        0     1647 2023-06-02 17:30:52.227201 humanloop-0.4.7/humanloop/model/project_sort_by.py
+-rw-r--r--   0        0        0     1476 2023-06-02 17:30:52.227344 humanloop-0.4.7/humanloop/model/project_sort_by.pyi
+-rw-r--r--   0        0        0     3971 2023-06-02 17:30:52.227490 humanloop-0.4.7/humanloop/model/project_user_response.py
+-rw-r--r--   0        0        0     3971 2023-06-02 17:30:52.227629 humanloop-0.4.7/humanloop/model/project_user_response.pyi
+-rw-r--r--   0        0        0     1889 2023-06-02 17:30:52.227778 humanloop-0.4.7/humanloop/model/projects_get_configs_response.py
+-rw-r--r--   0        0        0     1889 2023-06-02 17:30:52.227916 humanloop-0.4.7/humanloop/model/projects_get_configs_response.pyi
+-rw-r--r--   0        0        0     1891 2023-06-02 17:30:52.228066 humanloop-0.4.7/humanloop/model/projects_update_feedback_types_request.py
+-rw-r--r--   0        0        0     1891 2023-06-02 17:30:52.228206 humanloop-0.4.7/humanloop/model/projects_update_feedback_types_request.pyi
+-rw-r--r--   0        0        0     6114 2023-06-02 17:30:52.228354 humanloop-0.4.7/humanloop/model/provider_api_keys.py
+-rw-r--r--   0        0        0     6114 2023-06-02 17:30:52.228492 humanloop-0.4.7/humanloop/model/provider_api_keys.pyi
+-rw-r--r--   0        0        0     3289 2023-06-02 17:30:52.228640 humanloop-0.4.7/humanloop/model/session_project_response.py
+-rw-r--r--   0        0        0     3289 2023-06-02 17:30:52.228784 humanloop-0.4.7/humanloop/model/session_project_response.pyi
+-rw-r--r--   0        0        0     6796 2023-06-02 17:30:52.228923 humanloop-0.4.7/humanloop/model/session_response.py
+-rw-r--r--   0        0        0     6796 2023-06-02 17:30:52.229064 humanloop-0.4.7/humanloop/model/session_response.pyi
+-rw-r--r--   0        0        0     1485 2023-06-02 17:30:52.229192 humanloop-0.4.7/humanloop/model/sort_order.py
+-rw-r--r--   0        0        0     1368 2023-06-02 17:30:52.229316 humanloop-0.4.7/humanloop/model/sort_order.pyi
+-rw-r--r--   0        0        0    18103 2023-06-02 17:30:52.229508 humanloop-0.4.7/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.py
+-rw-r--r--   0        0        0    18103 2023-06-02 17:30:52.229731 humanloop-0.4.7/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.pyi
+-rw-r--r--   0        0        0     5065 2023-06-02 17:30:52.229924 humanloop-0.4.7/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     5065 2023-06-02 17:30:52.230087 humanloop-0.4.7/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi
+-rw-r--r--   0        0        0    19288 2023-06-02 17:30:52.230285 humanloop-0.4.7/humanloop/model/src_external_app_models_v4_configs_model_config_response.py
+-rw-r--r--   0        0        0    19123 2023-06-02 17:30:52.230509 humanloop-0.4.7/humanloop/model/src_external_app_models_v4_configs_model_config_response.pyi
+-rw-r--r--   0        0        0     5069 2023-06-02 17:30:52.230687 humanloop-0.4.7/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     5069 2023-06-02 17:30:52.230841 humanloop-0.4.7/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.pyi
+-rw-r--r--   0        0        0     5124 2023-06-02 17:30:52.230983 humanloop-0.4.7/humanloop/model/tool_config_request.py
+-rw-r--r--   0        0        0     4961 2023-06-02 17:30:52.231139 humanloop-0.4.7/humanloop/model/tool_config_request.pyi
+-rw-r--r--   0        0        0     5734 2023-06-02 17:30:52.231279 humanloop-0.4.7/humanloop/model/tool_config_response.py
+-rw-r--r--   0        0        0     5571 2023-06-02 17:30:52.231426 humanloop-0.4.7/humanloop/model/tool_config_response.pyi
+-rw-r--r--   0        0        0     4408 2023-06-02 17:30:52.231568 humanloop-0.4.7/humanloop/model/tool_result_response.py
+-rw-r--r--   0        0        0     4408 2023-06-02 17:30:52.231752 humanloop-0.4.7/humanloop/model/tool_result_response.pyi
+-rw-r--r--   0        0        0    13253 2023-06-02 17:30:52.231965 humanloop-0.4.7/humanloop/model/trace_log_request.py
+-rw-r--r--   0        0        0    13253 2023-06-02 17:30:52.232226 humanloop-0.4.7/humanloop/model/trace_log_request.pyi
+-rw-r--r--   0        0        0    19686 2023-06-02 17:30:52.232540 humanloop-0.4.7/humanloop/model/trace_model_config_request.py
+-rw-r--r--   0        0        0    19521 2023-06-02 17:30:52.232775 humanloop-0.4.7/humanloop/model/trace_model_config_request.pyi
+-rw-r--r--   0        0        0     7478 2023-06-02 17:30:52.232968 humanloop-0.4.7/humanloop/model/update_experiment_request.py
+-rw-r--r--   0        0        0     7478 2023-06-02 17:30:52.233114 humanloop-0.4.7/humanloop/model/update_experiment_request.pyi
+-rw-r--r--   0        0        0     3876 2023-06-02 17:30:52.233245 humanloop-0.4.7/humanloop/model/update_log_request.py
+-rw-r--r--   0        0        0     3876 2023-06-02 17:30:52.233381 humanloop-0.4.7/humanloop/model/update_log_request.pyi
+-rw-r--r--   0        0        0     5223 2023-06-02 17:30:52.233533 humanloop-0.4.7/humanloop/model/update_project_request.py
+-rw-r--r--   0        0        0     5223 2023-06-02 17:30:52.233682 humanloop-0.4.7/humanloop/model/update_project_request.pyi
+-rw-r--r--   0        0        0     4294 2023-06-02 17:30:52.233822 humanloop-0.4.7/humanloop/model/usage.py
+-rw-r--r--   0        0        0     4294 2023-06-02 17:30:52.233960 humanloop-0.4.7/humanloop/model/usage.pyi
+-rw-r--r--   0        0        0     6981 2023-06-02 17:30:52.234099 humanloop-0.4.7/humanloop/model/validation_error.py
+-rw-r--r--   0        0        0     6981 2023-06-02 17:30:52.234229 humanloop-0.4.7/humanloop/model/validation_error.pyi
+-rw-r--r--   0        0        0     6580 2023-06-02 17:30:52.234377 humanloop-0.4.7/humanloop/models/__init__.py
+-rw-r--r--   0        0        0     1431 2023-06-02 17:30:52.234516 humanloop-0.4.7/humanloop/paths/__init__.py
+-rw-r--r--   0        0        0      285 2023-06-02 17:30:52.234671 humanloop-0.4.7/humanloop/paths/chat/__init__.py
+-rw-r--r--   0        0        0    17604 2023-06-02 17:30:52.234868 humanloop-0.4.7/humanloop/paths/chat/post.py
+-rw-r--r--   0        0        0    17461 2023-06-02 17:30:52.235097 humanloop-0.4.7/humanloop/paths/chat/post.pyi
+-rw-r--r--   0        0        0      302 2023-06-02 17:30:52.235285 humanloop-0.4.7/humanloop/paths/chat_deployed/__init__.py
+-rw-r--r--   0        0        0    17167 2023-06-02 17:30:52.235463 humanloop-0.4.7/humanloop/paths/chat_deployed/post.py
+-rw-r--r--   0        0        0    17024 2023-06-02 17:30:52.235690 humanloop-0.4.7/humanloop/paths/chat_deployed/post.pyi
+-rw-r--r--   0        0        0      306 2023-06-02 17:30:52.235900 humanloop-0.4.7/humanloop/paths/chat_experiment/__init__.py
+-rw-r--r--   0        0        0    17610 2023-06-02 17:30:52.236088 humanloop-0.4.7/humanloop/paths/chat_experiment/post.py
+-rw-r--r--   0        0        0    17467 2023-06-02 17:30:52.236305 humanloop-0.4.7/humanloop/paths/chat_experiment/post.pyi
+-rw-r--r--   0        0        0      309 2023-06-02 17:30:52.236486 humanloop-0.4.7/humanloop/paths/chat_model_config/__init__.py
+-rw-r--r--   0        0        0    17785 2023-06-02 17:30:52.236669 humanloop-0.4.7/humanloop/paths/chat_model_config/post.py
+-rw-r--r--   0        0        0    17642 2023-06-02 17:30:52.236878 humanloop-0.4.7/humanloop/paths/chat_model_config/post.pyi
+-rw-r--r--   0        0        0      297 2023-06-02 17:30:52.237084 humanloop-0.4.7/humanloop/paths/completion/__init__.py
+-rw-r--r--   0        0        0    17920 2023-06-02 17:30:52.237264 humanloop-0.4.7/humanloop/paths/completion/post.py
+-rw-r--r--   0        0        0    17777 2023-06-02 17:30:52.237486 humanloop-0.4.7/humanloop/paths/completion/post.pyi
+-rw-r--r--   0        0        0      314 2023-06-02 17:30:52.237664 humanloop-0.4.7/humanloop/paths/completion_deployed/__init__.py
+-rw-r--r--   0        0        0    17423 2023-06-02 17:30:52.237842 humanloop-0.4.7/humanloop/paths/completion_deployed/post.py
+-rw-r--r--   0        0        0    17280 2023-06-02 17:30:52.238072 humanloop-0.4.7/humanloop/paths/completion_deployed/post.pyi
+-rw-r--r--   0        0        0      318 2023-06-02 17:30:52.238247 humanloop-0.4.7/humanloop/paths/completion_experiment/__init__.py
+-rw-r--r--   0        0        0    17866 2023-06-02 17:30:52.238453 humanloop-0.4.7/humanloop/paths/completion_experiment/post.py
+-rw-r--r--   0        0        0    17723 2023-06-02 17:30:52.238684 humanloop-0.4.7/humanloop/paths/completion_experiment/post.pyi
+-rw-r--r--   0        0        0      321 2023-06-02 17:30:52.238885 humanloop-0.4.7/humanloop/paths/completion_model_config/__init__.py
+-rw-r--r--   0        0        0    18041 2023-06-02 17:30:52.239103 humanloop-0.4.7/humanloop/paths/completion_model_config/post.py
+-rw-r--r--   0        0        0    17898 2023-06-02 17:30:52.239266 humanloop-0.4.7/humanloop/paths/completion_model_config/post.pyi
+-rw-r--r--   0        0        0      327 2023-06-02 17:30:52.239414 humanloop-0.4.7/humanloop/paths/experiments_experiment_id/__init__.py
+-rw-r--r--   0        0        0    12171 2023-06-02 17:30:52.239542 humanloop-0.4.7/humanloop/paths/experiments_experiment_id/delete.py
+-rw-r--r--   0        0        0    12028 2023-06-02 17:30:52.239747 humanloop-0.4.7/humanloop/paths/experiments_experiment_id/delete.pyi
+-rw-r--r--   0        0        0    17219 2023-06-02 17:30:52.239951 humanloop-0.4.7/humanloop/paths/experiments_experiment_id/patch.py
+-rw-r--r--   0        0        0    17076 2023-06-02 17:30:52.240121 humanloop-0.4.7/humanloop/paths/experiments_experiment_id/patch.pyi
+-rw-r--r--   0        0        0      352 2023-06-02 17:30:52.240240 humanloop-0.4.7/humanloop/paths/experiments_experiment_id_model_config/__init__.py
+-rw-r--r--   0        0        0    12672 2023-06-02 17:30:52.240346 humanloop-0.4.7/humanloop/paths/experiments_experiment_id_model_config/get.py
+-rw-r--r--   0        0        0    12529 2023-06-02 17:30:52.240487 humanloop-0.4.7/humanloop/paths/experiments_experiment_id_model_config/get.pyi
+-rw-r--r--   0        0        0      293 2023-06-02 17:30:52.240674 humanloop-0.4.7/humanloop/paths/feedback/__init__.py
+-rw-r--r--   0        0        0    15265 2023-06-02 17:30:52.240863 humanloop-0.4.7/humanloop/paths/feedback/post.py
+-rw-r--r--   0        0        0    15122 2023-06-02 17:30:52.241061 humanloop-0.4.7/humanloop/paths/feedback/post.pyi
+-rw-r--r--   0        0        0      285 2023-06-02 17:30:52.241232 humanloop-0.4.7/humanloop/paths/logs/__init__.py
+-rw-r--r--   0        0        0    16442 2023-06-02 17:30:52.241414 humanloop-0.4.7/humanloop/paths/logs/patch.py
+-rw-r--r--   0        0        0    16299 2023-06-02 17:30:52.241610 humanloop-0.4.7/humanloop/paths/logs/patch.pyi
+-rw-r--r--   0        0        0    22798 2023-06-02 17:30:52.241925 humanloop-0.4.7/humanloop/paths/logs/post.py
+-rw-r--r--   0        0        0    22655 2023-06-02 17:30:52.242212 humanloop-0.4.7/humanloop/paths/logs/post.pyi
+-rw-r--r--   0        0        0      291 2023-06-02 17:30:52.242438 humanloop-0.4.7/humanloop/paths/logs_id/__init__.py
+-rw-r--r--   0        0        0    15508 2023-06-02 17:30:52.242630 humanloop-0.4.7/humanloop/paths/logs_id/patch.py
+-rw-r--r--   0        0        0    15365 2023-06-02 17:30:52.242844 humanloop-0.4.7/humanloop/paths/logs_id/patch.pyi
+-rw-r--r--   0        0        0      302 2023-06-02 17:30:52.243049 humanloop-0.4.7/humanloop/paths/model_configs/__init__.py
+-rw-r--r--   0        0        0    20442 2023-06-02 17:30:52.243231 humanloop-0.4.7/humanloop/paths/model_configs/post.py
+-rw-r--r--   0        0        0    20299 2023-06-02 17:30:52.243465 humanloop-0.4.7/humanloop/paths/model_configs/post.pyi
+-rw-r--r--   0        0        0      308 2023-06-02 17:30:52.243641 humanloop-0.4.7/humanloop/paths/model_configs_id/__init__.py
+-rw-r--r--   0        0        0    12485 2023-06-02 17:30:52.243784 humanloop-0.4.7/humanloop/paths/model_configs_id/get.py
+-rw-r--r--   0        0        0    12342 2023-06-02 17:30:52.244012 humanloop-0.4.7/humanloop/paths/model_configs_id/get.pyi
+-rw-r--r--   0        0        0      293 2023-06-02 17:30:52.244233 humanloop-0.4.7/humanloop/paths/projects/__init__.py
+-rw-r--r--   0        0        0    20694 2023-06-02 17:30:52.244410 humanloop-0.4.7/humanloop/paths/projects/get.py
+-rw-r--r--   0        0        0    20551 2023-06-02 17:30:52.244639 humanloop-0.4.7/humanloop/paths/projects/get.pyi
+-rw-r--r--   0        0        0    13183 2023-06-02 17:30:52.244846 humanloop-0.4.7/humanloop/paths/projects/post.py
+-rw-r--r--   0        0        0    13040 2023-06-02 17:30:52.245026 humanloop-0.4.7/humanloop/paths/projects/post.pyi
+-rw-r--r--   0        0        0      299 2023-06-02 17:30:52.245184 humanloop-0.4.7/humanloop/paths/projects_id/__init__.py
+-rw-r--r--   0        0        0    12155 2023-06-02 17:30:52.245334 humanloop-0.4.7/humanloop/paths/projects_id/get.py
+-rw-r--r--   0        0        0    12012 2023-06-02 17:30:52.245542 humanloop-0.4.7/humanloop/paths/projects_id/get.pyi
+-rw-r--r--   0        0        0    16242 2023-06-02 17:30:52.245737 humanloop-0.4.7/humanloop/paths/projects_id/patch.py
+-rw-r--r--   0        0        0    16099 2023-06-02 17:30:52.245936 humanloop-0.4.7/humanloop/paths/projects_id/patch.pyi
+-rw-r--r--   0        0        0      326 2023-06-02 17:30:52.246116 humanloop-0.4.7/humanloop/paths/projects_id_active_config/__init__.py
+-rw-r--r--   0        0        0    12474 2023-06-02 17:30:52.246276 humanloop-0.4.7/humanloop/paths/projects_id_active_config/delete.py
+-rw-r--r--   0        0        0    12331 2023-06-02 17:30:52.246472 humanloop-0.4.7/humanloop/paths/projects_id_active_config/delete.pyi
+-rw-r--r--   0        0        0    12324 2023-06-02 17:30:52.246689 humanloop-0.4.7/humanloop/paths/projects_id_active_config/get.py
+-rw-r--r--   0        0        0    12181 2023-06-02 17:30:52.246922 humanloop-0.4.7/humanloop/paths/projects_id_active_config/get.pyi
+-rw-r--r--   0        0        0      334 2023-06-02 17:30:52.247142 humanloop-0.4.7/humanloop/paths/projects_id_active_experiment/__init__.py
+-rw-r--r--   0        0        0    12482 2023-06-02 17:30:52.247309 humanloop-0.4.7/humanloop/paths/projects_id_active_experiment/delete.py
+-rw-r--r--   0        0        0    12339 2023-06-02 17:30:52.247456 humanloop-0.4.7/humanloop/paths/projects_id_active_experiment/delete.pyi
+-rw-r--r--   0        0        0      315 2023-06-02 17:30:52.247659 humanloop-0.4.7/humanloop/paths/projects_id_configs/__init__.py
+-rw-r--r--   0        0        0    12358 2023-06-02 17:30:52.247813 humanloop-0.4.7/humanloop/paths/projects_id_configs/get.py
+-rw-r--r--   0        0        0    12215 2023-06-02 17:30:52.248041 humanloop-0.4.7/humanloop/paths/projects_id_configs/get.pyi
+-rw-r--r--   0        0        0      313 2023-06-02 17:30:52.248227 humanloop-0.4.7/humanloop/paths/projects_id_export/__init__.py
+-rw-r--r--   0        0        0    15904 2023-06-02 17:30:52.248322 humanloop-0.4.7/humanloop/paths/projects_id_export/post.py
+-rw-r--r--   0        0        0    15761 2023-06-02 17:30:52.248426 humanloop-0.4.7/humanloop/paths/projects_id_export/post.pyi
+-rw-r--r--   0        0        0      328 2023-06-02 17:30:52.248539 humanloop-0.4.7/humanloop/paths/projects_id_feedback_types/__init__.py
+-rw-r--r--   0        0        0    14974 2023-06-02 17:30:52.248638 humanloop-0.4.7/humanloop/paths/projects_id_feedback_types/patch.py
+-rw-r--r--   0        0        0    14831 2023-06-02 17:30:52.248816 humanloop-0.4.7/humanloop/paths/projects_id_feedback_types/patch.pyi
+-rw-r--r--   0        0        0      339 2023-06-02 17:30:52.249052 humanloop-0.4.7/humanloop/paths/projects_project_id_experiments/__init__.py
+-rw-r--r--   0        0        0    12432 2023-06-02 17:30:52.249245 humanloop-0.4.7/humanloop/paths/projects_project_id_experiments/get.py
+-rw-r--r--   0        0        0    12289 2023-06-02 17:30:52.249465 humanloop-0.4.7/humanloop/paths/projects_project_id_experiments/get.pyi
+-rw-r--r--   0        0        0    16426 2023-06-02 17:30:52.249690 humanloop-0.4.7/humanloop/paths/projects_project_id_experiments/post.py
+-rw-r--r--   0        0        0    16283 2023-06-02 17:30:52.249899 humanloop-0.4.7/humanloop/paths/projects_project_id_experiments/post.pyi
+-rw-r--r--   0        0        0      293 2023-06-02 17:30:52.250097 humanloop-0.4.7/humanloop/paths/sessions/__init__.py
+-rw-r--r--   0        0        0    14288 2023-06-02 17:30:52.250269 humanloop-0.4.7/humanloop/paths/sessions/get.py
+-rw-r--r--   0        0        0    14145 2023-06-02 17:30:52.250480 humanloop-0.4.7/humanloop/paths/sessions/get.pyi
+-rw-r--r--   0        0        0     9368 2023-06-02 17:30:52.250679 humanloop-0.4.7/humanloop/paths/sessions/post.py
+-rw-r--r--   0        0        0     9255 2023-06-02 17:30:52.250897 humanloop-0.4.7/humanloop/paths/sessions/post.pyi
+-rw-r--r--   0        0        0      299 2023-06-02 17:30:52.251086 humanloop-0.4.7/humanloop/paths/sessions_id/__init__.py
+-rw-r--r--   0        0        0    12155 2023-06-02 17:30:52.251241 humanloop-0.4.7/humanloop/paths/sessions_id/get.py
+-rw-r--r--   0        0        0    12012 2023-06-02 17:30:52.251434 humanloop-0.4.7/humanloop/paths/sessions_id/get.pyi
+-rw-r--r--   0        0        0      289 2023-06-02 17:30:52.251643 humanloop-0.4.7/humanloop/paths/traces/__init__.py
+-rw-r--r--   0        0        0    12626 2023-06-02 17:30:52.251807 humanloop-0.4.7/humanloop/paths/traces/post.py
+-rw-r--r--   0        0        0    12483 2023-06-02 17:30:52.252001 humanloop-0.4.7/humanloop/paths/traces/post.pyi
+-rw-r--r--   0        0        0     1187 2023-06-02 17:30:52.252216 humanloop-0.4.7/humanloop/request_after_hook.py
+-rw-r--r--   0        0        0     1783 2023-06-02 17:30:52.283421 humanloop-0.4.7/humanloop/request_before_hook.py
+-rw-r--r--   0        0        0    11505 2023-06-02 17:30:52.252505 humanloop-0.4.7/humanloop/rest.py
+-rw-r--r--   0        0        0    96089 2023-06-02 17:30:52.252938 humanloop-0.4.7/humanloop/schemas.py
+-rw-r--r--   0        0        0        0 2023-06-02 17:30:52.253166 humanloop-0.4.7/humanloop/type/__init__.py
+-rw-r--r--   0        0        0     1590 2023-06-02 17:30:52.253328 humanloop-0.4.7/humanloop/type/agent_config_request.py
+-rw-r--r--   0        0        0     1705 2023-06-02 17:30:52.253472 humanloop-0.4.7/humanloop/type/agent_config_response.py
+-rw-r--r--   0        0        0     1584 2023-06-02 17:30:52.253614 humanloop-0.4.7/humanloop/type/base_metric_response.py
+-rw-r--r--   0        0        0     1238 2023-06-02 17:30:52.253758 humanloop-0.4.7/humanloop/type/categorical_feedback_label.py
+-rw-r--r--   0        0        0     2359 2023-06-02 17:30:52.253900 humanloop-0.4.7/humanloop/type/chat_data_response.py
+-rw-r--r--   0        0        0     2166 2023-06-02 17:30:52.254055 humanloop-0.4.7/humanloop/type/chat_deployed_request.py
+-rw-r--r--   0        0        0     2411 2023-06-02 17:30:52.254214 humanloop-0.4.7/humanloop/type/chat_experiment_request.py
+-rw-r--r--   0        0        0     1095 2023-06-02 17:30:52.254371 humanloop-0.4.7/humanloop/type/chat_message.py
+-rw-r--r--   0        0        0     2280 2023-06-02 17:30:52.254555 humanloop-0.4.7/humanloop/type/chat_model_config_request.py
+-rw-r--r--   0        0        0     2306 2023-06-02 17:30:52.254729 humanloop-0.4.7/humanloop/type/chat_request.py
+-rw-r--r--   0        0        0     1994 2023-06-02 17:30:52.254896 humanloop-0.4.7/humanloop/type/chat_response.py
+-rw-r--r--   0        0        0      887 2023-06-02 17:30:52.255055 humanloop-0.4.7/humanloop/type/chat_role.py
+-rw-r--r--   0        0        0     2271 2023-06-02 17:30:52.255222 humanloop-0.4.7/humanloop/type/completion_deployed_request.py
+-rw-r--r--   0        0        0     2519 2023-06-02 17:30:52.255380 humanloop-0.4.7/humanloop/type/completion_experiment_request.py
+-rw-r--r--   0        0        0     2385 2023-06-02 17:30:52.255537 humanloop-0.4.7/humanloop/type/completion_model_config_request.py
+-rw-r--r--   0        0        0     2415 2023-06-02 17:30:52.255685 humanloop-0.4.7/humanloop/type/completion_request.py
+-rw-r--r--   0        0        0     2040 2023-06-02 17:30:52.255820 humanloop-0.4.7/humanloop/type/completion_response.py
+-rw-r--r--   0        0        0     1320 2023-06-02 17:30:52.255905 humanloop-0.4.7/humanloop/type/config_response.py
+-rw-r--r--   0        0        0      895 2023-06-02 17:30:52.256001 humanloop-0.4.7/humanloop/type/config_type.py
+-rw-r--r--   0        0        0     1538 2023-06-02 17:30:52.256148 humanloop-0.4.7/humanloop/type/create_experiment_request.py
+-rw-r--r--   0        0        0     1200 2023-06-02 17:30:52.256302 humanloop-0.4.7/humanloop/type/create_log_response.py
+-rw-r--r--   0        0        0     1242 2023-06-02 17:30:52.256450 humanloop-0.4.7/humanloop/type/create_project_request.py
+-rw-r--r--   0        0        0     1118 2023-06-02 17:30:52.256580 humanloop-0.4.7/humanloop/type/create_session_response.py
+-rw-r--r--   0        0        0     1221 2023-06-02 17:30:52.256679 humanloop-0.4.7/humanloop/type/create_trace_request.py
+-rw-r--r--   0        0        0     1174 2023-06-02 17:30:52.256764 humanloop-0.4.7/humanloop/type/create_trace_response.py
+-rw-r--r--   0        0        0     2189 2023-06-02 17:30:52.256884 humanloop-0.4.7/humanloop/type/data_response.py
+-rw-r--r--   0        0        0     1853 2023-06-02 17:30:52.257022 humanloop-0.4.7/humanloop/type/experiment_config_response.py
+-rw-r--r--   0        0        0     1964 2023-06-02 17:30:52.257202 humanloop-0.4.7/humanloop/type/experiment_response.py
+-rw-r--r--   0        0        0      894 2023-06-02 17:30:52.257388 humanloop-0.4.7/humanloop/type/experiment_status.py
+-rw-r--r--   0        0        0      961 2023-06-02 17:30:52.257574 humanloop-0.4.7/humanloop/type/experiments_list_response.py
+-rw-r--r--   0        0        0     1625 2023-06-02 17:30:52.257759 humanloop-0.4.7/humanloop/type/feedback.py
+-rw-r--r--   0        0        0      895 2023-06-02 17:30:52.257958 humanloop-0.4.7/humanloop/type/feedback_class.py
+-rw-r--r--   0        0        0     1146 2023-06-02 17:30:52.258154 humanloop-0.4.7/humanloop/type/feedback_label_request.py
+-rw-r--r--   0        0        0     1722 2023-06-02 17:30:52.258338 humanloop-0.4.7/humanloop/type/feedback_request.py
+-rw-r--r--   0        0        0     1754 2023-06-02 17:30:52.258502 humanloop-0.4.7/humanloop/type/feedback_response.py
+-rw-r--r--   0        0        0      980 2023-06-02 17:30:52.258680 humanloop-0.4.7/humanloop/type/feedback_submit_request.py
+-rw-r--r--   0        0        0      985 2023-06-02 17:30:52.258826 humanloop-0.4.7/humanloop/type/feedback_submit_response.py
+-rw-r--r--   0        0        0      914 2023-06-02 17:30:52.258971 humanloop-0.4.7/humanloop/type/feedback_type.py
+-rw-r--r--   0        0        0     1483 2023-06-02 17:30:52.259123 humanloop-0.4.7/humanloop/type/feedback_type_model.py
+-rw-r--r--   0        0        0     1717 2023-06-02 17:30:52.259278 humanloop-0.4.7/humanloop/type/feedback_type_request.py
+-rw-r--r--   0        0        0      949 2023-06-02 17:30:52.259435 humanloop-0.4.7/humanloop/type/feedback_types.py
+-rw-r--r--   0        0        0     1240 2023-06-02 17:30:52.259596 humanloop-0.4.7/humanloop/type/generic_config_request.py
+-rw-r--r--   0        0        0     1359 2023-06-02 17:30:52.259762 humanloop-0.4.7/humanloop/type/generic_config_response.py
+-rw-r--r--   0        0        0     2076 2023-06-02 17:30:52.259926 humanloop-0.4.7/humanloop/type/get_model_config_response.py
+-rw-r--r--   0        0        0     1148 2023-06-02 17:30:52.260083 humanloop-0.4.7/humanloop/type/http_validation_error.py
+-rw-r--r--   0        0        0      906 2023-06-02 17:30:52.260228 humanloop-0.4.7/humanloop/type/label_sentiment.py
+-rw-r--r--   0        0        0      958 2023-06-02 17:30:52.260367 humanloop-0.4.7/humanloop/type/log_datapoint_request.py
+-rw-r--r--   0        0        0     3209 2023-06-02 17:30:52.260515 humanloop-0.4.7/humanloop/type/log_model_config_request.py
+-rw-r--r--   0        0        0     3857 2023-06-02 17:30:52.260670 humanloop-0.4.7/humanloop/type/log_request.py
+-rw-r--r--   0        0        0     4048 2023-06-02 17:30:52.260823 humanloop-0.4.7/humanloop/type/log_response.py
+-rw-r--r--   0        0        0      983 2023-06-02 17:30:52.260988 humanloop-0.4.7/humanloop/type/logs_log_response.py
+-rw-r--r--   0        0        0     2996 2023-06-02 17:30:52.261154 humanloop-0.4.7/humanloop/type/model_config_chat_request.py
+-rw-r--r--   0        0        0     2889 2023-06-02 17:30:52.261322 humanloop-0.4.7/humanloop/type/model_config_completion_request.py
+-rw-r--r--   0        0        0      890 2023-06-02 17:30:52.261473 humanloop-0.4.7/humanloop/type/model_endpoints.py
+-rw-r--r--   0        0        0      940 2023-06-02 17:30:52.261640 humanloop-0.4.7/humanloop/type/model_providers.py
+-rw-r--r--   0        0        0     1208 2023-06-02 17:30:52.261810 humanloop-0.4.7/humanloop/type/paginated_data_log_response.py
+-rw-r--r--   0        0        0     1240 2023-06-02 17:30:52.261948 humanloop-0.4.7/humanloop/type/paginated_data_project_response.py
+-rw-r--r--   0        0        0     1240 2023-06-02 17:30:52.262088 humanloop-0.4.7/humanloop/type/paginated_data_session_response.py
+-rw-r--r--   0        0        0     1047 2023-06-02 17:30:52.262220 humanloop-0.4.7/humanloop/type/positive_label.py
+-rw-r--r--   0        0        0     1996 2023-06-02 17:30:52.262391 humanloop-0.4.7/humanloop/type/project_config_response.py
+-rw-r--r--   0        0        0     3586 2023-06-02 17:30:52.262558 humanloop-0.4.7/humanloop/type/project_model_config_request.py
+-rw-r--r--   0        0        0     4229 2023-06-02 17:30:52.262724 humanloop-0.4.7/humanloop/type/project_model_config_response.py
+-rw-r--r--   0        0        0     2208 2023-06-02 17:30:52.262887 humanloop-0.4.7/humanloop/type/project_response.py
+-rw-r--r--   0        0        0      897 2023-06-02 17:30:52.263035 humanloop-0.4.7/humanloop/type/project_sort_by.py
+-rw-r--r--   0        0        0     1198 2023-06-02 17:30:52.263161 humanloop-0.4.7/humanloop/type/project_user_response.py
+-rw-r--r--   0        0        0      974 2023-06-02 17:30:52.263324 humanloop-0.4.7/humanloop/type/projects_get_configs_response.py
+-rw-r--r--   0        0        0      976 2023-06-02 17:30:52.263546 humanloop-0.4.7/humanloop/type/projects_update_feedback_types_request.py
+-rw-r--r--   0        0        0     1165 2023-06-02 17:30:52.263736 humanloop-0.4.7/humanloop/type/provider_api_keys.py
+-rw-r--r--   0        0        0     1161 2023-06-02 17:30:52.264081 humanloop-0.4.7/humanloop/type/session_project_response.py
+-rw-r--r--   0        0        0     1618 2023-06-02 17:30:52.264288 humanloop-0.4.7/humanloop/type/session_response.py
+-rw-r--r--   0        0        0      872 2023-06-02 17:30:52.264472 humanloop-0.4.7/humanloop/type/sort_order.py
+-rw-r--r--   0        0        0     3506 2023-06-02 17:30:52.264627 humanloop-0.4.7/humanloop/type/src_external_app_models_v3_model_configs_model_config_response.py
+-rw-r--r--   0        0        0     1417 2023-06-02 17:30:52.264770 humanloop-0.4.7/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     3518 2023-06-02 17:30:52.264926 humanloop-0.4.7/humanloop/type/src_external_app_models_v4_configs_model_config_response.py
+-rw-r--r--   0        0        0     1427 2023-06-02 17:30:52.265073 humanloop-0.4.7/humanloop/type/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     1242 2023-06-02 17:30:52.265201 humanloop-0.4.7/humanloop/type/tool_config_request.py
+-rw-r--r--   0        0        0     1392 2023-06-02 17:30:52.265316 humanloop-0.4.7/humanloop/type/tool_config_response.py
+-rw-r--r--   0        0        0     1106 2023-06-02 17:30:52.265465 humanloop-0.4.7/humanloop/type/tool_result_response.py
+-rw-r--r--   0        0        0     2632 2023-06-02 17:30:52.265631 humanloop-0.4.7/humanloop/type/trace_log_request.py
+-rw-r--r--   0        0        0     3271 2023-06-02 17:30:52.265774 humanloop-0.4.7/humanloop/type/trace_model_config_request.py
+-rw-r--r--   0        0        0     1537 2023-06-02 17:30:52.265908 humanloop-0.4.7/humanloop/type/update_experiment_request.py
+-rw-r--r--   0        0        0     1259 2023-06-02 17:30:52.266021 humanloop-0.4.7/humanloop/type/update_log_request.py
+-rw-r--r--   0        0        0     1610 2023-06-02 17:30:52.266130 humanloop-0.4.7/humanloop/type/update_project_request.py
+-rw-r--r--   0        0        0     1218 2023-06-02 17:30:52.266236 humanloop-0.4.7/humanloop/type/usage.py
+-rw-r--r--   0        0        0     1127 2023-06-02 17:30:52.266350 humanloop-0.4.7/humanloop/type/validation_error.py
+-rw-r--r--   0        0        0     1044 2023-06-02 17:30:52.266475 humanloop-0.4.7/humanloop/type_util.py
+-rw-r--r--   0        0        0     3165 2023-06-02 17:30:52.266590 humanloop-0.4.7/humanloop/validation_metadata.py
+-rw-r--r--   0        0        0      714 2023-06-02 17:30:52.267007 humanloop-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     9366 1970-01-01 00:00:00.000000 humanloop-0.4.7/PKG-INFO
```

### Comparing `humanloop-0.4.6/LICENSE` & `humanloop-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/README.md` & `humanloop-0.4.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# humanloop@0.4.6
+# humanloop@0.4.7
 
 
 ## Requirements
 
 Python >=3.7
 
 ## Installing
 
 ```sh
-pip install humanloop==0.4.6
+pip install humanloop==0.4.7
 ```
 
 ## Getting Started
 
 ```python
 from pprint import pprint
 from humanloop import Humanloop, ApiException
```

### Comparing `humanloop-0.4.6/humanloop/__init__.py` & `humanloop-0.4.7/humanloop/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The Humanloop API allows you to interact with Humanloop from your product or service.  You can do this through HTTP requests from any language or via our official Python or TypeScript SDK.  To install the official [Python SDK](https://pypi.org/project/humanloop/), run the following command:  ```bash pip install humanloop ```  To install the official [TypeScript SDK](https://www.npmjs.com/package/humanloop), run the following command:  ```bash npm i humanloop ```  ---  Guides and further details about key concepts can be found in [our docs](https://docs.humanloop.com/).
 
     The version of the OpenAPI document: 4.0.0
     Generated by: https://konfigthis.com
 """
 
-__version__ = "0.4.6"
+__version__ = "0.4.7"
 
 # import ApiClient
 from humanloop.api_client import ApiClient
 
 # import Configuration
 from humanloop.configuration import Configuration
```

### Comparing `humanloop-0.4.6/humanloop/api_client.py` & `humanloop-0.4.7/humanloop/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2770,15 +2770,15 @@
 0000ad10: 6164 6572 5f6e 616d 655d 203d 2068 6561  ader_name] = hea
 0000ad20: 6465 725f 7661 6c75 650a 2020 2020 2020  der_value.      
 0000ad30: 2020 7365 6c66 2e63 6f6f 6b69 6520 3d20    self.cookie = 
 0000ad40: 636f 6f6b 6965 0a20 2020 2020 2020 2023  cookie.        #
 0000ad50: 2053 6574 2064 6566 6175 6c74 2055 7365   Set default Use
 0000ad60: 722d 4167 656e 742e 0a20 2020 2020 2020  r-Agent..       
 0000ad70: 2073 656c 662e 7573 6572 5f61 6765 6e74   self.user_agent
-0000ad80: 203d 2027 4b6f 6e66 6967 2f30 2e34 2e36   = 'Konfig/0.4.6
+0000ad80: 203d 2027 4b6f 6e66 6967 2f30 2e34 2e37   = 'Konfig/0.4.7
 0000ad90: 2f70 7974 686f 6e27 0a0a 2020 2020 6465  /python'..    de
 0000ada0: 6620 5f5f 656e 7465 725f 5f28 7365 6c66  f __enter__(self
 0000adb0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
 0000adc0: 6e20 7365 6c66 0a0a 2020 2020 6465 6620  n self..    def 
 0000add0: 5f5f 6578 6974 5f5f 2873 656c 662c 2065  __exit__(self, e
 0000ade0: 7863 5f74 7970 652c 2065 7863 5f76 616c  xc_type, exc_val
 0000adf0: 7565 2c20 7472 6163 6562 6163 6b29 3a0a  ue, traceback):.
```

### Comparing `humanloop-0.4.6/humanloop/api_response.py` & `humanloop-0.4.7/humanloop/api_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/apis/path_to_api.py` & `humanloop-0.4.7/humanloop/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/apis/tag_to_api.py` & `humanloop-0.4.7/humanloop/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/apis/tags/__init__.py` & `humanloop-0.4.7/humanloop/apis/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/apis/tags/chats_api.py` & `humanloop-0.4.7/humanloop/apis/tags/chats_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/apis/tags/completions_api.py` & `humanloop-0.4.7/humanloop/apis/tags/completions_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/apis/tags/experiments_api.py` & `humanloop-0.4.7/humanloop/apis/tags/experiments_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/apis/tags/feedback_api.py` & `humanloop-0.4.7/humanloop/apis/tags/feedback_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/apis/tags/logs_api.py` & `humanloop-0.4.7/humanloop/apis/tags/logs_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/apis/tags/model_configurations_api.py` & `humanloop-0.4.7/humanloop/apis/tags/model_configurations_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/apis/tags/projects_api.py` & `humanloop-0.4.7/humanloop/apis/tags/projects_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/apis/tags/sessions_api.py` & `humanloop-0.4.7/humanloop/apis/tags/sessions_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/apis/tags/traces_api.py` & `humanloop-0.4.7/humanloop/apis/tags/traces_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/client.py` & `humanloop-0.4.7/humanloop/client.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/client.pyi` & `humanloop-0.4.7/humanloop/client.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/client_custom.py` & `humanloop-0.4.7/humanloop/client_custom.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/configuration.py` & `humanloop-0.4.7/humanloop/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 4.0.0\n"\
-               "SDK Package Version: 0.4.6".\
+               "SDK Package Version: 0.4.7".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `humanloop-0.4.6/humanloop/exceptions.py` & `humanloop-0.4.7/humanloop/exceptions.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/exceptions_base.py` & `humanloop-0.4.7/humanloop/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/agent_config_request.py` & `humanloop-0.4.7/humanloop/model/agent_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/agent_config_request.pyi` & `humanloop-0.4.7/humanloop/model/agent_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/agent_config_response.py` & `humanloop-0.4.7/humanloop/model/chat_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,36 +19,62 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class AgentConfigResponse(
+class ChatRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Base chat request.
     """
 
 
     class MetaOapg:
         required = {
             "model_config",
-            "agent_class",
-            "name",
-            "id",
-            "type",
+            "messages",
+            "project",
         }
         
         class properties:
-            id = schemas.StrSchema
+            project = schemas.StrSchema
+            
             
+            class messages(
+                schemas.ListSchema
+            ):
+            
+            
+                class MetaOapg:
+                    
+                    @staticmethod
+                    def items() -> typing.Type['ChatMessage']:
+                        return ChatMessage
             
-            class type(
+                def __new__(
+                    cls,
+                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'messages':
+                    return super().__new__(
+                        cls,
+                        arg,
+                        _configuration=_configuration,
+                    )
+            
+                def __getitem__(self, i: int) -> 'ChatMessage':
+                    return super().__getitem__(i)
+            
+            
+            class model_config(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
@@ -58,35 +84,35 @@
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            ConfigType,
+                            ModelConfigChatRequest,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'type':
+                ) -> 'model_config':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            name = schemas.StrSchema
-            agent_class = schemas.StrSchema
+            inputs = schemas.DictSchema
+            source = schemas.StrSchema
             
             
-            class model_config(
+            class provider_api_keys(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
@@ -96,163 +122,146 @@
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            LogModelConfigRequest,
+                            ProviderApiKeys,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'model_config':
+                ) -> 'provider_api_keys':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            description = schemas.StrSchema
-            other = schemas.DictSchema
-            
-            
-            class tools(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['ToolConfigRequest']:
-                        return ToolConfigRequest
-            
-                def __new__(
-                    cls,
-                    arg: typing.Union[typing.Tuple['ToolConfigRequest'], typing.List['ToolConfigRequest']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'tools':
-                    return super().__new__(
-                        cls,
-                        arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'ToolConfigRequest':
-                    return super().__getitem__(i)
+            num_samples = schemas.IntSchema
+            stream = schemas.BoolSchema
+            user = schemas.StrSchema
+            metadata = schemas.DictSchema
             __annotations__ = {
-                "id": id,
-                "type": type,
-                "name": name,
-                "agent_class": agent_class,
+                "project": project,
+                "messages": messages,
                 "model_config": model_config,
-                "description": description,
-                "other": other,
-                "tools": tools,
+                "inputs": inputs,
+                "source": source,
+                "provider_api_keys": provider_api_keys,
+                "num_samples": num_samples,
+                "stream": stream,
+                "user": user,
+                "metadata": metadata,
             }
+        additional_properties = schemas.NotAnyTypeSchema
     
     model_config: MetaOapg.properties.model_config
-    agent_class: MetaOapg.properties.agent_class
-    name: MetaOapg.properties.name
-    id: MetaOapg.properties.id
-    type: MetaOapg.properties.type
+    messages: MetaOapg.properties.messages
+    project: MetaOapg.properties.project
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def __getitem__(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
+    def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
+    def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["agent_class"]) -> MetaOapg.properties.agent_class: ...
+    def __getitem__(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
+    def __getitem__(self, name: typing_extensions.Literal["provider_api_keys"]) -> MetaOapg.properties.provider_api_keys: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
+    def __getitem__(self, name: typing_extensions.Literal["num_samples"]) -> MetaOapg.properties.num_samples: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["tools"]) -> MetaOapg.properties.tools: ...
+    def __getitem__(self, name: typing_extensions.Literal["stream"]) -> MetaOapg.properties.stream: ...
     
     @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    def __getitem__(self, name: typing_extensions.Literal["user"]) -> MetaOapg.properties.user: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "agent_class", "model_config", "description", "other", "tools", ], str]):
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model_config"], typing_extensions.Literal["messages"], typing_extensions.Literal["project"], typing_extensions.Literal["inputs"], typing_extensions.Literal["source"], typing_extensions.Literal["provider_api_keys"], typing_extensions.Literal["num_samples"], typing_extensions.Literal["stream"], typing_extensions.Literal["user"], typing_extensions.Literal["metadata"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> typing.Union[MetaOapg.properties.inputs, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["agent_class"]) -> MetaOapg.properties.agent_class: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["provider_api_keys"]) -> typing.Union[MetaOapg.properties.provider_api_keys, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["num_samples"]) -> typing.Union[MetaOapg.properties.num_samples, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["stream"]) -> typing.Union[MetaOapg.properties.stream, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["tools"]) -> typing.Union[MetaOapg.properties.tools, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["user"]) -> typing.Union[MetaOapg.properties.user, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "agent_class", "model_config", "description", "other", "tools", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model_config"], typing_extensions.Literal["messages"], typing_extensions.Literal["project"], typing_extensions.Literal["inputs"], typing_extensions.Literal["source"], typing_extensions.Literal["provider_api_keys"], typing_extensions.Literal["num_samples"], typing_extensions.Literal["stream"], typing_extensions.Literal["user"], typing_extensions.Literal["metadata"], ]):
         return super().get_item_oapg(name)
-    
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         model_config: typing.Union[MetaOapg.properties.model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        agent_class: typing.Union[MetaOapg.properties.agent_class, str, ],
-        name: typing.Union[MetaOapg.properties.name, str, ],
-        id: typing.Union[MetaOapg.properties.id, str, ],
-        type: typing.Union[MetaOapg.properties.type, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
-        other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
-        tools: typing.Union[MetaOapg.properties.tools, list, tuple, schemas.Unset] = schemas.unset,
+        messages: typing.Union[MetaOapg.properties.messages, list, tuple, ],
+        project: typing.Union[MetaOapg.properties.project, str, ],
+        inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
+        provider_api_keys: typing.Union[MetaOapg.properties.provider_api_keys, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        num_samples: typing.Union[MetaOapg.properties.num_samples, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        stream: typing.Union[MetaOapg.properties.stream, bool, schemas.Unset] = schemas.unset,
+        user: typing.Union[MetaOapg.properties.user, str, schemas.Unset] = schemas.unset,
+        metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'AgentConfigResponse':
+    ) -> 'ChatRequest':
         return super().__new__(
             cls,
             *args,
             model_config=model_config,
-            agent_class=agent_class,
-            name=name,
-            id=id,
-            type=type,
-            description=description,
-            other=other,
-            tools=tools,
+            messages=messages,
+            project=project,
+            inputs=inputs,
+            source=source,
+            provider_api_keys=provider_api_keys,
+            num_samples=num_samples,
+            stream=stream,
+            user=user,
+            metadata=metadata,
             _configuration=_configuration,
-            **kwargs,
         )
 
-from humanloop.model.config_type import ConfigType
-from humanloop.model.log_model_config_request import LogModelConfigRequest
-from humanloop.model.tool_config_request import ToolConfigRequest
+from humanloop.model.chat_message import ChatMessage
+from humanloop.model.model_config_chat_request import ModelConfigChatRequest
+from humanloop.model.provider_api_keys import ProviderApiKeys
```

### Comparing `humanloop-0.4.6/humanloop/model/agent_config_response.pyi` & `humanloop-0.4.7/humanloop/model/chat_request.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -19,36 +19,62 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class AgentConfigResponse(
+class ChatRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Base chat request.
     """
 
 
     class MetaOapg:
         required = {
             "model_config",
-            "agent_class",
-            "name",
-            "id",
-            "type",
+            "messages",
+            "project",
         }
         
         class properties:
-            id = schemas.StrSchema
+            project = schemas.StrSchema
+            
             
+            class messages(
+                schemas.ListSchema
+            ):
+            
+            
+                class MetaOapg:
+                    
+                    @staticmethod
+                    def items() -> typing.Type['ChatMessage']:
+                        return ChatMessage
             
-            class type(
+                def __new__(
+                    cls,
+                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'messages':
+                    return super().__new__(
+                        cls,
+                        arg,
+                        _configuration=_configuration,
+                    )
+            
+                def __getitem__(self, i: int) -> 'ChatMessage':
+                    return super().__getitem__(i)
+            
+            
+            class model_config(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
@@ -58,35 +84,35 @@
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            ConfigType,
+                            ModelConfigChatRequest,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'type':
+                ) -> 'model_config':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            name = schemas.StrSchema
-            agent_class = schemas.StrSchema
+            inputs = schemas.DictSchema
+            source = schemas.StrSchema
             
             
-            class model_config(
+            class provider_api_keys(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
@@ -96,163 +122,146 @@
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            LogModelConfigRequest,
+                            ProviderApiKeys,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'model_config':
+                ) -> 'provider_api_keys':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            description = schemas.StrSchema
-            other = schemas.DictSchema
-            
-            
-            class tools(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['ToolConfigRequest']:
-                        return ToolConfigRequest
-            
-                def __new__(
-                    cls,
-                    arg: typing.Union[typing.Tuple['ToolConfigRequest'], typing.List['ToolConfigRequest']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'tools':
-                    return super().__new__(
-                        cls,
-                        arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'ToolConfigRequest':
-                    return super().__getitem__(i)
+            num_samples = schemas.IntSchema
+            stream = schemas.BoolSchema
+            user = schemas.StrSchema
+            metadata = schemas.DictSchema
             __annotations__ = {
-                "id": id,
-                "type": type,
-                "name": name,
-                "agent_class": agent_class,
+                "project": project,
+                "messages": messages,
                 "model_config": model_config,
-                "description": description,
-                "other": other,
-                "tools": tools,
+                "inputs": inputs,
+                "source": source,
+                "provider_api_keys": provider_api_keys,
+                "num_samples": num_samples,
+                "stream": stream,
+                "user": user,
+                "metadata": metadata,
             }
+        additional_properties = schemas.NotAnyTypeSchema
     
     model_config: MetaOapg.properties.model_config
-    agent_class: MetaOapg.properties.agent_class
-    name: MetaOapg.properties.name
-    id: MetaOapg.properties.id
-    type: MetaOapg.properties.type
+    messages: MetaOapg.properties.messages
+    project: MetaOapg.properties.project
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def __getitem__(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
+    def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
+    def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["agent_class"]) -> MetaOapg.properties.agent_class: ...
+    def __getitem__(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
+    def __getitem__(self, name: typing_extensions.Literal["provider_api_keys"]) -> MetaOapg.properties.provider_api_keys: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
+    def __getitem__(self, name: typing_extensions.Literal["num_samples"]) -> MetaOapg.properties.num_samples: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["tools"]) -> MetaOapg.properties.tools: ...
+    def __getitem__(self, name: typing_extensions.Literal["stream"]) -> MetaOapg.properties.stream: ...
     
     @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    def __getitem__(self, name: typing_extensions.Literal["user"]) -> MetaOapg.properties.user: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "agent_class", "model_config", "description", "other", "tools", ], str]):
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model_config"], typing_extensions.Literal["messages"], typing_extensions.Literal["project"], typing_extensions.Literal["inputs"], typing_extensions.Literal["source"], typing_extensions.Literal["provider_api_keys"], typing_extensions.Literal["num_samples"], typing_extensions.Literal["stream"], typing_extensions.Literal["user"], typing_extensions.Literal["metadata"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> typing.Union[MetaOapg.properties.inputs, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["agent_class"]) -> MetaOapg.properties.agent_class: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["provider_api_keys"]) -> typing.Union[MetaOapg.properties.provider_api_keys, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["num_samples"]) -> typing.Union[MetaOapg.properties.num_samples, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["stream"]) -> typing.Union[MetaOapg.properties.stream, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["tools"]) -> typing.Union[MetaOapg.properties.tools, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["user"]) -> typing.Union[MetaOapg.properties.user, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "agent_class", "model_config", "description", "other", "tools", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model_config"], typing_extensions.Literal["messages"], typing_extensions.Literal["project"], typing_extensions.Literal["inputs"], typing_extensions.Literal["source"], typing_extensions.Literal["provider_api_keys"], typing_extensions.Literal["num_samples"], typing_extensions.Literal["stream"], typing_extensions.Literal["user"], typing_extensions.Literal["metadata"], ]):
         return super().get_item_oapg(name)
-    
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         model_config: typing.Union[MetaOapg.properties.model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        agent_class: typing.Union[MetaOapg.properties.agent_class, str, ],
-        name: typing.Union[MetaOapg.properties.name, str, ],
-        id: typing.Union[MetaOapg.properties.id, str, ],
-        type: typing.Union[MetaOapg.properties.type, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
-        other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
-        tools: typing.Union[MetaOapg.properties.tools, list, tuple, schemas.Unset] = schemas.unset,
+        messages: typing.Union[MetaOapg.properties.messages, list, tuple, ],
+        project: typing.Union[MetaOapg.properties.project, str, ],
+        inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
+        provider_api_keys: typing.Union[MetaOapg.properties.provider_api_keys, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        num_samples: typing.Union[MetaOapg.properties.num_samples, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        stream: typing.Union[MetaOapg.properties.stream, bool, schemas.Unset] = schemas.unset,
+        user: typing.Union[MetaOapg.properties.user, str, schemas.Unset] = schemas.unset,
+        metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'AgentConfigResponse':
+    ) -> 'ChatRequest':
         return super().__new__(
             cls,
             *args,
             model_config=model_config,
-            agent_class=agent_class,
-            name=name,
-            id=id,
-            type=type,
-            description=description,
-            other=other,
-            tools=tools,
+            messages=messages,
+            project=project,
+            inputs=inputs,
+            source=source,
+            provider_api_keys=provider_api_keys,
+            num_samples=num_samples,
+            stream=stream,
+            user=user,
+            metadata=metadata,
             _configuration=_configuration,
-            **kwargs,
         )
 
-from humanloop.model.config_type import ConfigType
-from humanloop.model.log_model_config_request import LogModelConfigRequest
-from humanloop.model.tool_config_request import ToolConfigRequest
+from humanloop.model.chat_message import ChatMessage
+from humanloop.model.model_config_chat_request import ModelConfigChatRequest
+from humanloop.model.provider_api_keys import ProviderApiKeys
```

### Comparing `humanloop-0.4.6/humanloop/model/base_metric_response.py` & `humanloop-0.4.7/humanloop/model/base_metric_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/base_metric_response.pyi` & `humanloop-0.4.7/humanloop/model/base_metric_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/categorical_feedback_label.py` & `humanloop-0.4.7/humanloop/model/categorical_feedback_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/categorical_feedback_label.pyi` & `humanloop-0.4.7/humanloop/model/categorical_feedback_label.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/chat_data_response.py` & `humanloop-0.4.7/humanloop/model/chat_data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/chat_data_response.pyi` & `humanloop-0.4.7/humanloop/model/chat_data_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/chat_deployed_request.py` & `humanloop-0.4.7/humanloop/model/chat_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/chat_deployed_request.pyi` & `humanloop-0.4.7/humanloop/model/chat_deployed_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/chat_experiment_request.py` & `humanloop-0.4.7/humanloop/model/chat_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/chat_experiment_request.pyi` & `humanloop-0.4.7/humanloop/model/chat_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/chat_message.py` & `humanloop-0.4.7/humanloop/model/chat_message.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/chat_message.pyi` & `humanloop-0.4.7/humanloop/model/chat_message.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/chat_model_config_request.py` & `humanloop-0.4.7/humanloop/model/chat_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/chat_model_config_request.pyi` & `humanloop-0.4.7/humanloop/model/chat_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/chat_request.py` & `humanloop-0.4.7/humanloop/model/completion_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,59 +19,34 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class ChatRequest(
+class CompletionRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    Base chat request.
+    Completion request with a provided model config.
     """
 
 
     class MetaOapg:
         required = {
             "model_config",
-            "messages",
+            "inputs",
             "project",
         }
         
         class properties:
             project = schemas.StrSchema
-            
-            
-            class messages(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['ChatMessage']:
-                        return ChatMessage
-            
-                def __new__(
-                    cls,
-                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'messages':
-                    return super().__new__(
-                        cls,
-                        arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'ChatMessage':
-                    return super().__getitem__(i)
+            inputs = schemas.DictSchema
             
             
             class model_config(
                 schemas.ComposedSchema,
             ):
             
             
@@ -84,15 +59,15 @@
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            ModelConfigChatRequest,
+                            ModelConfigCompletionRequest,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
@@ -100,15 +75,14 @@
                 ) -> 'model_config':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            inputs = schemas.DictSchema
             source = schemas.StrSchema
             
             
             class provider_api_keys(
                 schemas.ComposedSchema,
             ):
             
@@ -139,129 +113,139 @@
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             num_samples = schemas.IntSchema
+            logprobs = schemas.IntSchema
             stream = schemas.BoolSchema
+            suffix = schemas.StrSchema
             user = schemas.StrSchema
             metadata = schemas.DictSchema
             __annotations__ = {
                 "project": project,
-                "messages": messages,
-                "model_config": model_config,
                 "inputs": inputs,
+                "model_config": model_config,
                 "source": source,
                 "provider_api_keys": provider_api_keys,
                 "num_samples": num_samples,
+                "logprobs": logprobs,
                 "stream": stream,
+                "suffix": suffix,
                 "user": user,
                 "metadata": metadata,
             }
         additional_properties = schemas.NotAnyTypeSchema
     
     model_config: MetaOapg.properties.model_config
-    messages: MetaOapg.properties.messages
+    inputs: MetaOapg.properties.inputs
     project: MetaOapg.properties.project
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
+    def __getitem__(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["provider_api_keys"]) -> MetaOapg.properties.provider_api_keys: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["num_samples"]) -> MetaOapg.properties.num_samples: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["logprobs"]) -> MetaOapg.properties.logprobs: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["stream"]) -> MetaOapg.properties.stream: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["suffix"]) -> MetaOapg.properties.suffix: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["user"]) -> MetaOapg.properties.user: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model_config"], typing_extensions.Literal["messages"], typing_extensions.Literal["project"], typing_extensions.Literal["inputs"], typing_extensions.Literal["source"], typing_extensions.Literal["provider_api_keys"], typing_extensions.Literal["num_samples"], typing_extensions.Literal["stream"], typing_extensions.Literal["user"], typing_extensions.Literal["metadata"], ]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model_config"], typing_extensions.Literal["inputs"], typing_extensions.Literal["project"], typing_extensions.Literal["source"], typing_extensions.Literal["provider_api_keys"], typing_extensions.Literal["num_samples"], typing_extensions.Literal["logprobs"], typing_extensions.Literal["stream"], typing_extensions.Literal["suffix"], typing_extensions.Literal["user"], typing_extensions.Literal["metadata"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> typing.Union[MetaOapg.properties.inputs, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["provider_api_keys"]) -> typing.Union[MetaOapg.properties.provider_api_keys, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["num_samples"]) -> typing.Union[MetaOapg.properties.num_samples, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["logprobs"]) -> typing.Union[MetaOapg.properties.logprobs, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["stream"]) -> typing.Union[MetaOapg.properties.stream, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["suffix"]) -> typing.Union[MetaOapg.properties.suffix, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["user"]) -> typing.Union[MetaOapg.properties.user, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model_config"], typing_extensions.Literal["messages"], typing_extensions.Literal["project"], typing_extensions.Literal["inputs"], typing_extensions.Literal["source"], typing_extensions.Literal["provider_api_keys"], typing_extensions.Literal["num_samples"], typing_extensions.Literal["stream"], typing_extensions.Literal["user"], typing_extensions.Literal["metadata"], ]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model_config"], typing_extensions.Literal["inputs"], typing_extensions.Literal["project"], typing_extensions.Literal["source"], typing_extensions.Literal["provider_api_keys"], typing_extensions.Literal["num_samples"], typing_extensions.Literal["logprobs"], typing_extensions.Literal["stream"], typing_extensions.Literal["suffix"], typing_extensions.Literal["user"], typing_extensions.Literal["metadata"], ]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         model_config: typing.Union[MetaOapg.properties.model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        messages: typing.Union[MetaOapg.properties.messages, list, tuple, ],
+        inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, ],
         project: typing.Union[MetaOapg.properties.project, str, ],
-        inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
         provider_api_keys: typing.Union[MetaOapg.properties.provider_api_keys, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         num_samples: typing.Union[MetaOapg.properties.num_samples, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        logprobs: typing.Union[MetaOapg.properties.logprobs, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         stream: typing.Union[MetaOapg.properties.stream, bool, schemas.Unset] = schemas.unset,
+        suffix: typing.Union[MetaOapg.properties.suffix, str, schemas.Unset] = schemas.unset,
         user: typing.Union[MetaOapg.properties.user, str, schemas.Unset] = schemas.unset,
         metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> 'ChatRequest':
+    ) -> 'CompletionRequest':
         return super().__new__(
             cls,
             *args,
             model_config=model_config,
-            messages=messages,
-            project=project,
             inputs=inputs,
+            project=project,
             source=source,
             provider_api_keys=provider_api_keys,
             num_samples=num_samples,
+            logprobs=logprobs,
             stream=stream,
+            suffix=suffix,
             user=user,
             metadata=metadata,
             _configuration=_configuration,
         )
 
-from humanloop.model.chat_message import ChatMessage
-from humanloop.model.model_config_chat_request import ModelConfigChatRequest
+from humanloop.model.model_config_completion_request import ModelConfigCompletionRequest
 from humanloop.model.provider_api_keys import ProviderApiKeys
```

### Comparing `humanloop-0.4.6/humanloop/model/chat_request.pyi` & `humanloop-0.4.7/humanloop/model/completion_request.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -19,59 +19,34 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class ChatRequest(
+class CompletionRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    Base chat request.
+    Completion request with a provided model config.
     """
 
 
     class MetaOapg:
         required = {
             "model_config",
-            "messages",
+            "inputs",
             "project",
         }
         
         class properties:
             project = schemas.StrSchema
-            
-            
-            class messages(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['ChatMessage']:
-                        return ChatMessage
-            
-                def __new__(
-                    cls,
-                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'messages':
-                    return super().__new__(
-                        cls,
-                        arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'ChatMessage':
-                    return super().__getitem__(i)
+            inputs = schemas.DictSchema
             
             
             class model_config(
                 schemas.ComposedSchema,
             ):
             
             
@@ -84,15 +59,15 @@
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            ModelConfigChatRequest,
+                            ModelConfigCompletionRequest,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
@@ -100,15 +75,14 @@
                 ) -> 'model_config':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            inputs = schemas.DictSchema
             source = schemas.StrSchema
             
             
             class provider_api_keys(
                 schemas.ComposedSchema,
             ):
             
@@ -139,129 +113,139 @@
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             num_samples = schemas.IntSchema
+            logprobs = schemas.IntSchema
             stream = schemas.BoolSchema
+            suffix = schemas.StrSchema
             user = schemas.StrSchema
             metadata = schemas.DictSchema
             __annotations__ = {
                 "project": project,
-                "messages": messages,
-                "model_config": model_config,
                 "inputs": inputs,
+                "model_config": model_config,
                 "source": source,
                 "provider_api_keys": provider_api_keys,
                 "num_samples": num_samples,
+                "logprobs": logprobs,
                 "stream": stream,
+                "suffix": suffix,
                 "user": user,
                 "metadata": metadata,
             }
         additional_properties = schemas.NotAnyTypeSchema
     
     model_config: MetaOapg.properties.model_config
-    messages: MetaOapg.properties.messages
+    inputs: MetaOapg.properties.inputs
     project: MetaOapg.properties.project
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
+    def __getitem__(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["provider_api_keys"]) -> MetaOapg.properties.provider_api_keys: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["num_samples"]) -> MetaOapg.properties.num_samples: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["logprobs"]) -> MetaOapg.properties.logprobs: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["stream"]) -> MetaOapg.properties.stream: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["suffix"]) -> MetaOapg.properties.suffix: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["user"]) -> MetaOapg.properties.user: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model_config"], typing_extensions.Literal["messages"], typing_extensions.Literal["project"], typing_extensions.Literal["inputs"], typing_extensions.Literal["source"], typing_extensions.Literal["provider_api_keys"], typing_extensions.Literal["num_samples"], typing_extensions.Literal["stream"], typing_extensions.Literal["user"], typing_extensions.Literal["metadata"], ]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model_config"], typing_extensions.Literal["inputs"], typing_extensions.Literal["project"], typing_extensions.Literal["source"], typing_extensions.Literal["provider_api_keys"], typing_extensions.Literal["num_samples"], typing_extensions.Literal["logprobs"], typing_extensions.Literal["stream"], typing_extensions.Literal["suffix"], typing_extensions.Literal["user"], typing_extensions.Literal["metadata"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> typing.Union[MetaOapg.properties.inputs, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["provider_api_keys"]) -> typing.Union[MetaOapg.properties.provider_api_keys, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["num_samples"]) -> typing.Union[MetaOapg.properties.num_samples, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["logprobs"]) -> typing.Union[MetaOapg.properties.logprobs, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["stream"]) -> typing.Union[MetaOapg.properties.stream, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["suffix"]) -> typing.Union[MetaOapg.properties.suffix, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["user"]) -> typing.Union[MetaOapg.properties.user, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model_config"], typing_extensions.Literal["messages"], typing_extensions.Literal["project"], typing_extensions.Literal["inputs"], typing_extensions.Literal["source"], typing_extensions.Literal["provider_api_keys"], typing_extensions.Literal["num_samples"], typing_extensions.Literal["stream"], typing_extensions.Literal["user"], typing_extensions.Literal["metadata"], ]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model_config"], typing_extensions.Literal["inputs"], typing_extensions.Literal["project"], typing_extensions.Literal["source"], typing_extensions.Literal["provider_api_keys"], typing_extensions.Literal["num_samples"], typing_extensions.Literal["logprobs"], typing_extensions.Literal["stream"], typing_extensions.Literal["suffix"], typing_extensions.Literal["user"], typing_extensions.Literal["metadata"], ]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         model_config: typing.Union[MetaOapg.properties.model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        messages: typing.Union[MetaOapg.properties.messages, list, tuple, ],
+        inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, ],
         project: typing.Union[MetaOapg.properties.project, str, ],
-        inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
         provider_api_keys: typing.Union[MetaOapg.properties.provider_api_keys, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         num_samples: typing.Union[MetaOapg.properties.num_samples, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        logprobs: typing.Union[MetaOapg.properties.logprobs, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         stream: typing.Union[MetaOapg.properties.stream, bool, schemas.Unset] = schemas.unset,
+        suffix: typing.Union[MetaOapg.properties.suffix, str, schemas.Unset] = schemas.unset,
         user: typing.Union[MetaOapg.properties.user, str, schemas.Unset] = schemas.unset,
         metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> 'ChatRequest':
+    ) -> 'CompletionRequest':
         return super().__new__(
             cls,
             *args,
             model_config=model_config,
-            messages=messages,
-            project=project,
             inputs=inputs,
+            project=project,
             source=source,
             provider_api_keys=provider_api_keys,
             num_samples=num_samples,
+            logprobs=logprobs,
             stream=stream,
+            suffix=suffix,
             user=user,
             metadata=metadata,
             _configuration=_configuration,
         )
 
-from humanloop.model.chat_message import ChatMessage
-from humanloop.model.model_config_chat_request import ModelConfigChatRequest
+from humanloop.model.model_config_completion_request import ModelConfigCompletionRequest
 from humanloop.model.provider_api_keys import ProviderApiKeys
```

### Comparing `humanloop-0.4.6/humanloop/model/chat_response.py` & `humanloop-0.4.7/humanloop/model/chat_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/chat_response.pyi` & `humanloop-0.4.7/humanloop/model/chat_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/chat_role.py` & `humanloop-0.4.7/humanloop/model/chat_role.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/chat_role.pyi` & `humanloop-0.4.7/humanloop/model/chat_role.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/completion_deployed_request.py` & `humanloop-0.4.7/humanloop/model/completion_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/completion_deployed_request.pyi` & `humanloop-0.4.7/humanloop/model/completion_deployed_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/completion_experiment_request.py` & `humanloop-0.4.7/humanloop/model/completion_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/completion_experiment_request.pyi` & `humanloop-0.4.7/humanloop/model/completion_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/completion_model_config_request.py` & `humanloop-0.4.7/humanloop/model/completion_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/completion_model_config_request.pyi` & `humanloop-0.4.7/humanloop/model/completion_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/completion_request.py` & `humanloop-0.4.7/humanloop/model/trace_log_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,233 +19,263 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class CompletionRequest(
+class TraceLogRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    Completion request with a provided model config.
+    Simplified version of LogRequest.
+
+Changes:
+    - Renamed `project` to `function_name`. TODO: Allow either `function_name` or `function_id`.
     """
 
 
     class MetaOapg:
         required = {
-            "model_config",
-            "inputs",
-            "project",
+            "function_name",
         }
         
         class properties:
-            project = schemas.StrSchema
+            function_name = schemas.StrSchema
+            trial_id = schemas.StrSchema
             inputs = schemas.DictSchema
             
             
-            class model_config(
-                schemas.ComposedSchema,
+            class messages(
+                schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
-                    @classmethod
-                    @functools.lru_cache()
-                    def all_of(cls):
-                        # we need this here to make our import statements work
-                        # we must store _composed_schemas in here so the code is only run
-                        # when we invoke this method. If we kept this at the class
-                        # level we would get an error because the class level
-                        # code would be run when this module is imported, and these composed
-                        # classes don't exist yet because their module has not finished
-                        # loading
-                        return [
-                            ModelConfigCompletionRequest,
-                        ]
-            
+                    @staticmethod
+                    def items() -> typing.Type['ChatMessage']:
+                        return ChatMessage
             
                 def __new__(
                     cls,
-                    *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'model_config':
+                ) -> 'messages':
                     return super().__new__(
                         cls,
-                        *args,
+                        arg,
                         _configuration=_configuration,
-                        **kwargs,
                     )
+            
+                def __getitem__(self, i: int) -> 'ChatMessage':
+                    return super().__getitem__(i)
+            output = schemas.StrSchema
             source = schemas.StrSchema
             
             
-            class provider_api_keys(
+            class config(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
                     @functools.lru_cache()
-                    def all_of(cls):
+                    def one_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            ProviderApiKeys,
+                            TraceModelConfigRequest,
+                            ToolConfigRequest,
+                            GenericConfigRequest,
+                            AgentConfigRequest,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'provider_api_keys':
+                ) -> 'config':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            num_samples = schemas.IntSchema
-            logprobs = schemas.IntSchema
-            stream = schemas.BoolSchema
-            suffix = schemas.StrSchema
-            user = schemas.StrSchema
             metadata = schemas.DictSchema
+            error = schemas.StrSchema
+            duration = schemas.NumberSchema
+            created_at = schemas.DateTimeSchema
+            
+            
+            class children(
+                schemas.ListSchema
+            ):
+            
+            
+                class MetaOapg:
+                    
+                    @staticmethod
+                    def items() -> typing.Type['TraceLogRequest']:
+                        return TraceLogRequest
+            
+                def __new__(
+                    cls,
+                    arg: typing.Union[typing.Tuple['TraceLogRequest'], typing.List['TraceLogRequest']],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'children':
+                    return super().__new__(
+                        cls,
+                        arg,
+                        _configuration=_configuration,
+                    )
+            
+                def __getitem__(self, i: int) -> 'TraceLogRequest':
+                    return super().__getitem__(i)
             __annotations__ = {
-                "project": project,
+                "function_name": function_name,
+                "trial_id": trial_id,
                 "inputs": inputs,
-                "model_config": model_config,
+                "messages": messages,
+                "output": output,
                 "source": source,
-                "provider_api_keys": provider_api_keys,
-                "num_samples": num_samples,
-                "logprobs": logprobs,
-                "stream": stream,
-                "suffix": suffix,
-                "user": user,
+                "config": config,
                 "metadata": metadata,
+                "error": error,
+                "duration": duration,
+                "created_at": created_at,
+                "children": children,
             }
         additional_properties = schemas.NotAnyTypeSchema
     
-    model_config: MetaOapg.properties.model_config
-    inputs: MetaOapg.properties.inputs
-    project: MetaOapg.properties.project
+    function_name: MetaOapg.properties.function_name
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    def __getitem__(self, name: typing_extensions.Literal["function_name"]) -> MetaOapg.properties.function_name: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["trial_id"]) -> MetaOapg.properties.trial_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
+    def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
+    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["provider_api_keys"]) -> MetaOapg.properties.provider_api_keys: ...
+    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["num_samples"]) -> MetaOapg.properties.num_samples: ...
+    def __getitem__(self, name: typing_extensions.Literal["config"]) -> MetaOapg.properties.config: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["logprobs"]) -> MetaOapg.properties.logprobs: ...
+    def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["stream"]) -> MetaOapg.properties.stream: ...
+    def __getitem__(self, name: typing_extensions.Literal["error"]) -> MetaOapg.properties.error: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["suffix"]) -> MetaOapg.properties.suffix: ...
+    def __getitem__(self, name: typing_extensions.Literal["duration"]) -> MetaOapg.properties.duration: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["user"]) -> MetaOapg.properties.user: ...
+    def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
+    def __getitem__(self, name: typing_extensions.Literal["children"]) -> MetaOapg.properties.children: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model_config"], typing_extensions.Literal["inputs"], typing_extensions.Literal["project"], typing_extensions.Literal["source"], typing_extensions.Literal["provider_api_keys"], typing_extensions.Literal["num_samples"], typing_extensions.Literal["logprobs"], typing_extensions.Literal["stream"], typing_extensions.Literal["suffix"], typing_extensions.Literal["user"], typing_extensions.Literal["metadata"], ]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["function_name"], typing_extensions.Literal["trial_id"], typing_extensions.Literal["inputs"], typing_extensions.Literal["messages"], typing_extensions.Literal["output"], typing_extensions.Literal["source"], typing_extensions.Literal["config"], typing_extensions.Literal["metadata"], typing_extensions.Literal["error"], typing_extensions.Literal["duration"], typing_extensions.Literal["created_at"], typing_extensions.Literal["children"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["function_name"]) -> MetaOapg.properties.function_name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["trial_id"]) -> typing.Union[MetaOapg.properties.trial_id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> typing.Union[MetaOapg.properties.inputs, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> typing.Union[MetaOapg.properties.messages, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["provider_api_keys"]) -> typing.Union[MetaOapg.properties.provider_api_keys, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> typing.Union[MetaOapg.properties.output, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["num_samples"]) -> typing.Union[MetaOapg.properties.num_samples, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["logprobs"]) -> typing.Union[MetaOapg.properties.logprobs, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["config"]) -> typing.Union[MetaOapg.properties.config, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["stream"]) -> typing.Union[MetaOapg.properties.stream, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["suffix"]) -> typing.Union[MetaOapg.properties.suffix, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["error"]) -> typing.Union[MetaOapg.properties.error, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["user"]) -> typing.Union[MetaOapg.properties.user, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["duration"]) -> typing.Union[MetaOapg.properties.duration, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> typing.Union[MetaOapg.properties.created_at, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["children"]) -> typing.Union[MetaOapg.properties.children, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model_config"], typing_extensions.Literal["inputs"], typing_extensions.Literal["project"], typing_extensions.Literal["source"], typing_extensions.Literal["provider_api_keys"], typing_extensions.Literal["num_samples"], typing_extensions.Literal["logprobs"], typing_extensions.Literal["stream"], typing_extensions.Literal["suffix"], typing_extensions.Literal["user"], typing_extensions.Literal["metadata"], ]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["function_name"], typing_extensions.Literal["trial_id"], typing_extensions.Literal["inputs"], typing_extensions.Literal["messages"], typing_extensions.Literal["output"], typing_extensions.Literal["source"], typing_extensions.Literal["config"], typing_extensions.Literal["metadata"], typing_extensions.Literal["error"], typing_extensions.Literal["duration"], typing_extensions.Literal["created_at"], typing_extensions.Literal["children"], ]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        model_config: typing.Union[MetaOapg.properties.model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, ],
-        project: typing.Union[MetaOapg.properties.project, str, ],
+        function_name: typing.Union[MetaOapg.properties.function_name, str, ],
+        trial_id: typing.Union[MetaOapg.properties.trial_id, str, schemas.Unset] = schemas.unset,
+        inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        messages: typing.Union[MetaOapg.properties.messages, list, tuple, schemas.Unset] = schemas.unset,
+        output: typing.Union[MetaOapg.properties.output, str, schemas.Unset] = schemas.unset,
         source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
-        provider_api_keys: typing.Union[MetaOapg.properties.provider_api_keys, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        num_samples: typing.Union[MetaOapg.properties.num_samples, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        logprobs: typing.Union[MetaOapg.properties.logprobs, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        stream: typing.Union[MetaOapg.properties.stream, bool, schemas.Unset] = schemas.unset,
-        suffix: typing.Union[MetaOapg.properties.suffix, str, schemas.Unset] = schemas.unset,
-        user: typing.Union[MetaOapg.properties.user, str, schemas.Unset] = schemas.unset,
+        config: typing.Union[MetaOapg.properties.config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        error: typing.Union[MetaOapg.properties.error, str, schemas.Unset] = schemas.unset,
+        duration: typing.Union[MetaOapg.properties.duration, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, schemas.Unset] = schemas.unset,
+        children: typing.Union[MetaOapg.properties.children, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> 'CompletionRequest':
+    ) -> 'TraceLogRequest':
         return super().__new__(
             cls,
             *args,
-            model_config=model_config,
+            function_name=function_name,
+            trial_id=trial_id,
             inputs=inputs,
-            project=project,
+            messages=messages,
+            output=output,
             source=source,
-            provider_api_keys=provider_api_keys,
-            num_samples=num_samples,
-            logprobs=logprobs,
-            stream=stream,
-            suffix=suffix,
-            user=user,
+            config=config,
             metadata=metadata,
+            error=error,
+            duration=duration,
+            created_at=created_at,
+            children=children,
             _configuration=_configuration,
         )
 
-from humanloop.model.model_config_completion_request import ModelConfigCompletionRequest
-from humanloop.model.provider_api_keys import ProviderApiKeys
+from humanloop.model.agent_config_request import AgentConfigRequest
+from humanloop.model.chat_message import ChatMessage
+from humanloop.model.generic_config_request import GenericConfigRequest
+from humanloop.model.tool_config_request import ToolConfigRequest
+from humanloop.model.trace_model_config_request import TraceModelConfigRequest
```

### Comparing `humanloop-0.4.6/humanloop/model/completion_request.pyi` & `humanloop-0.4.7/humanloop/model/trace_log_request.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -19,233 +19,263 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class CompletionRequest(
+class TraceLogRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    Completion request with a provided model config.
+    Simplified version of LogRequest.
+
+Changes:
+    - Renamed `project` to `function_name`. TODO: Allow either `function_name` or `function_id`.
     """
 
 
     class MetaOapg:
         required = {
-            "model_config",
-            "inputs",
-            "project",
+            "function_name",
         }
         
         class properties:
-            project = schemas.StrSchema
+            function_name = schemas.StrSchema
+            trial_id = schemas.StrSchema
             inputs = schemas.DictSchema
             
             
-            class model_config(
-                schemas.ComposedSchema,
+            class messages(
+                schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
-                    @classmethod
-                    @functools.lru_cache()
-                    def all_of(cls):
-                        # we need this here to make our import statements work
-                        # we must store _composed_schemas in here so the code is only run
-                        # when we invoke this method. If we kept this at the class
-                        # level we would get an error because the class level
-                        # code would be run when this module is imported, and these composed
-                        # classes don't exist yet because their module has not finished
-                        # loading
-                        return [
-                            ModelConfigCompletionRequest,
-                        ]
-            
+                    @staticmethod
+                    def items() -> typing.Type['ChatMessage']:
+                        return ChatMessage
             
                 def __new__(
                     cls,
-                    *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'model_config':
+                ) -> 'messages':
                     return super().__new__(
                         cls,
-                        *args,
+                        arg,
                         _configuration=_configuration,
-                        **kwargs,
                     )
+            
+                def __getitem__(self, i: int) -> 'ChatMessage':
+                    return super().__getitem__(i)
+            output = schemas.StrSchema
             source = schemas.StrSchema
             
             
-            class provider_api_keys(
+            class config(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
                     @functools.lru_cache()
-                    def all_of(cls):
+                    def one_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            ProviderApiKeys,
+                            TraceModelConfigRequest,
+                            ToolConfigRequest,
+                            GenericConfigRequest,
+                            AgentConfigRequest,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'provider_api_keys':
+                ) -> 'config':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            num_samples = schemas.IntSchema
-            logprobs = schemas.IntSchema
-            stream = schemas.BoolSchema
-            suffix = schemas.StrSchema
-            user = schemas.StrSchema
             metadata = schemas.DictSchema
+            error = schemas.StrSchema
+            duration = schemas.NumberSchema
+            created_at = schemas.DateTimeSchema
+            
+            
+            class children(
+                schemas.ListSchema
+            ):
+            
+            
+                class MetaOapg:
+                    
+                    @staticmethod
+                    def items() -> typing.Type['TraceLogRequest']:
+                        return TraceLogRequest
+            
+                def __new__(
+                    cls,
+                    arg: typing.Union[typing.Tuple['TraceLogRequest'], typing.List['TraceLogRequest']],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'children':
+                    return super().__new__(
+                        cls,
+                        arg,
+                        _configuration=_configuration,
+                    )
+            
+                def __getitem__(self, i: int) -> 'TraceLogRequest':
+                    return super().__getitem__(i)
             __annotations__ = {
-                "project": project,
+                "function_name": function_name,
+                "trial_id": trial_id,
                 "inputs": inputs,
-                "model_config": model_config,
+                "messages": messages,
+                "output": output,
                 "source": source,
-                "provider_api_keys": provider_api_keys,
-                "num_samples": num_samples,
-                "logprobs": logprobs,
-                "stream": stream,
-                "suffix": suffix,
-                "user": user,
+                "config": config,
                 "metadata": metadata,
+                "error": error,
+                "duration": duration,
+                "created_at": created_at,
+                "children": children,
             }
         additional_properties = schemas.NotAnyTypeSchema
     
-    model_config: MetaOapg.properties.model_config
-    inputs: MetaOapg.properties.inputs
-    project: MetaOapg.properties.project
+    function_name: MetaOapg.properties.function_name
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    def __getitem__(self, name: typing_extensions.Literal["function_name"]) -> MetaOapg.properties.function_name: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["trial_id"]) -> MetaOapg.properties.trial_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
+    def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
+    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["provider_api_keys"]) -> MetaOapg.properties.provider_api_keys: ...
+    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["num_samples"]) -> MetaOapg.properties.num_samples: ...
+    def __getitem__(self, name: typing_extensions.Literal["config"]) -> MetaOapg.properties.config: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["logprobs"]) -> MetaOapg.properties.logprobs: ...
+    def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["stream"]) -> MetaOapg.properties.stream: ...
+    def __getitem__(self, name: typing_extensions.Literal["error"]) -> MetaOapg.properties.error: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["suffix"]) -> MetaOapg.properties.suffix: ...
+    def __getitem__(self, name: typing_extensions.Literal["duration"]) -> MetaOapg.properties.duration: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["user"]) -> MetaOapg.properties.user: ...
+    def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
+    def __getitem__(self, name: typing_extensions.Literal["children"]) -> MetaOapg.properties.children: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model_config"], typing_extensions.Literal["inputs"], typing_extensions.Literal["project"], typing_extensions.Literal["source"], typing_extensions.Literal["provider_api_keys"], typing_extensions.Literal["num_samples"], typing_extensions.Literal["logprobs"], typing_extensions.Literal["stream"], typing_extensions.Literal["suffix"], typing_extensions.Literal["user"], typing_extensions.Literal["metadata"], ]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["function_name"], typing_extensions.Literal["trial_id"], typing_extensions.Literal["inputs"], typing_extensions.Literal["messages"], typing_extensions.Literal["output"], typing_extensions.Literal["source"], typing_extensions.Literal["config"], typing_extensions.Literal["metadata"], typing_extensions.Literal["error"], typing_extensions.Literal["duration"], typing_extensions.Literal["created_at"], typing_extensions.Literal["children"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["function_name"]) -> MetaOapg.properties.function_name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["trial_id"]) -> typing.Union[MetaOapg.properties.trial_id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> typing.Union[MetaOapg.properties.inputs, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> typing.Union[MetaOapg.properties.messages, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["provider_api_keys"]) -> typing.Union[MetaOapg.properties.provider_api_keys, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> typing.Union[MetaOapg.properties.output, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["num_samples"]) -> typing.Union[MetaOapg.properties.num_samples, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["logprobs"]) -> typing.Union[MetaOapg.properties.logprobs, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["config"]) -> typing.Union[MetaOapg.properties.config, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["stream"]) -> typing.Union[MetaOapg.properties.stream, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["suffix"]) -> typing.Union[MetaOapg.properties.suffix, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["error"]) -> typing.Union[MetaOapg.properties.error, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["user"]) -> typing.Union[MetaOapg.properties.user, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["duration"]) -> typing.Union[MetaOapg.properties.duration, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> typing.Union[MetaOapg.properties.created_at, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["children"]) -> typing.Union[MetaOapg.properties.children, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model_config"], typing_extensions.Literal["inputs"], typing_extensions.Literal["project"], typing_extensions.Literal["source"], typing_extensions.Literal["provider_api_keys"], typing_extensions.Literal["num_samples"], typing_extensions.Literal["logprobs"], typing_extensions.Literal["stream"], typing_extensions.Literal["suffix"], typing_extensions.Literal["user"], typing_extensions.Literal["metadata"], ]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["function_name"], typing_extensions.Literal["trial_id"], typing_extensions.Literal["inputs"], typing_extensions.Literal["messages"], typing_extensions.Literal["output"], typing_extensions.Literal["source"], typing_extensions.Literal["config"], typing_extensions.Literal["metadata"], typing_extensions.Literal["error"], typing_extensions.Literal["duration"], typing_extensions.Literal["created_at"], typing_extensions.Literal["children"], ]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        model_config: typing.Union[MetaOapg.properties.model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, ],
-        project: typing.Union[MetaOapg.properties.project, str, ],
+        function_name: typing.Union[MetaOapg.properties.function_name, str, ],
+        trial_id: typing.Union[MetaOapg.properties.trial_id, str, schemas.Unset] = schemas.unset,
+        inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        messages: typing.Union[MetaOapg.properties.messages, list, tuple, schemas.Unset] = schemas.unset,
+        output: typing.Union[MetaOapg.properties.output, str, schemas.Unset] = schemas.unset,
         source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
-        provider_api_keys: typing.Union[MetaOapg.properties.provider_api_keys, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        num_samples: typing.Union[MetaOapg.properties.num_samples, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        logprobs: typing.Union[MetaOapg.properties.logprobs, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        stream: typing.Union[MetaOapg.properties.stream, bool, schemas.Unset] = schemas.unset,
-        suffix: typing.Union[MetaOapg.properties.suffix, str, schemas.Unset] = schemas.unset,
-        user: typing.Union[MetaOapg.properties.user, str, schemas.Unset] = schemas.unset,
+        config: typing.Union[MetaOapg.properties.config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        error: typing.Union[MetaOapg.properties.error, str, schemas.Unset] = schemas.unset,
+        duration: typing.Union[MetaOapg.properties.duration, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, schemas.Unset] = schemas.unset,
+        children: typing.Union[MetaOapg.properties.children, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> 'CompletionRequest':
+    ) -> 'TraceLogRequest':
         return super().__new__(
             cls,
             *args,
-            model_config=model_config,
+            function_name=function_name,
+            trial_id=trial_id,
             inputs=inputs,
-            project=project,
+            messages=messages,
+            output=output,
             source=source,
-            provider_api_keys=provider_api_keys,
-            num_samples=num_samples,
-            logprobs=logprobs,
-            stream=stream,
-            suffix=suffix,
-            user=user,
+            config=config,
             metadata=metadata,
+            error=error,
+            duration=duration,
+            created_at=created_at,
+            children=children,
             _configuration=_configuration,
         )
 
-from humanloop.model.model_config_completion_request import ModelConfigCompletionRequest
-from humanloop.model.provider_api_keys import ProviderApiKeys
+from humanloop.model.agent_config_request import AgentConfigRequest
+from humanloop.model.chat_message import ChatMessage
+from humanloop.model.generic_config_request import GenericConfigRequest
+from humanloop.model.tool_config_request import ToolConfigRequest
+from humanloop.model.trace_model_config_request import TraceModelConfigRequest
```

### Comparing `humanloop-0.4.6/humanloop/model/completion_response.py` & `humanloop-0.4.7/humanloop/model/completion_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/completion_response.pyi` & `humanloop-0.4.7/humanloop/model/completion_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/config_response.py` & `humanloop-0.4.7/humanloop/model/feedback_submit_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,52 +19,73 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class ConfigResponse(
+class FeedbackSubmitRequest(
     schemas.ComposedSchema,
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
+        
+        class any_of_0(
+            schemas.ListSchema
+        ):
+        
+        
+            class MetaOapg:
+                
+                @staticmethod
+                def items() -> typing.Type['FeedbackRequest']:
+                    return FeedbackRequest
+        
+            def __new__(
+                cls,
+                arg: typing.Union[typing.Tuple['FeedbackRequest'], typing.List['FeedbackRequest']],
+                _configuration: typing.Optional[schemas.Configuration] = None,
+            ) -> 'any_of_0':
+                return super().__new__(
+                    cls,
+                    arg,
+                    _configuration=_configuration,
+                )
+        
+            def __getitem__(self, i: int) -> 'FeedbackRequest':
+                return super().__getitem__(i)
+        
         @classmethod
         @functools.lru_cache()
         def any_of(cls):
             # we need this here to make our import statements work
             # we must store _composed_schemas in here so the code is only run
             # when we invoke this method. If we kept this at the class
             # level we would get an error because the class level
             # code would be run when this module is imported, and these composed
             # classes don't exist yet because their module has not finished
             # loading
             return [
-                SrcExternalAppModelsV4ConfigsModelConfigResponse,
-                ToolConfigResponse,
-                AgentConfigResponse,
-                GenericConfigResponse,
+                cls.any_of_0,
+                FeedbackRequest,
             ]
 
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'ConfigResponse':
+    ) -> 'FeedbackSubmitRequest':
         return super().__new__(
             cls,
             *args,
             _configuration=_configuration,
             **kwargs,
         )
 
-from humanloop.model.agent_config_response import AgentConfigResponse
-from humanloop.model.generic_config_response import GenericConfigResponse
-from humanloop.model.src_external_app_models_v4_configs_model_config_response import SrcExternalAppModelsV4ConfigsModelConfigResponse
-from humanloop.model.tool_config_response import ToolConfigResponse
+from humanloop.model.feedback_request import FeedbackRequest
```

### Comparing `humanloop-0.4.6/humanloop/model/config_response.pyi` & `humanloop-0.4.7/humanloop/model/feedback_submit_request.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -19,52 +19,73 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class ConfigResponse(
+class FeedbackSubmitRequest(
     schemas.ComposedSchema,
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
+        
+        class any_of_0(
+            schemas.ListSchema
+        ):
+        
+        
+            class MetaOapg:
+                
+                @staticmethod
+                def items() -> typing.Type['FeedbackRequest']:
+                    return FeedbackRequest
+        
+            def __new__(
+                cls,
+                arg: typing.Union[typing.Tuple['FeedbackRequest'], typing.List['FeedbackRequest']],
+                _configuration: typing.Optional[schemas.Configuration] = None,
+            ) -> 'any_of_0':
+                return super().__new__(
+                    cls,
+                    arg,
+                    _configuration=_configuration,
+                )
+        
+            def __getitem__(self, i: int) -> 'FeedbackRequest':
+                return super().__getitem__(i)
+        
         @classmethod
         @functools.lru_cache()
         def any_of(cls):
             # we need this here to make our import statements work
             # we must store _composed_schemas in here so the code is only run
             # when we invoke this method. If we kept this at the class
             # level we would get an error because the class level
             # code would be run when this module is imported, and these composed
             # classes don't exist yet because their module has not finished
             # loading
             return [
-                SrcExternalAppModelsV4ConfigsModelConfigResponse,
-                ToolConfigResponse,
-                AgentConfigResponse,
-                GenericConfigResponse,
+                cls.any_of_0,
+                FeedbackRequest,
             ]
 
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'ConfigResponse':
+    ) -> 'FeedbackSubmitRequest':
         return super().__new__(
             cls,
             *args,
             _configuration=_configuration,
             **kwargs,
         )
 
-from humanloop.model.agent_config_response import AgentConfigResponse
-from humanloop.model.generic_config_response import GenericConfigResponse
-from humanloop.model.src_external_app_models_v4_configs_model_config_response import SrcExternalAppModelsV4ConfigsModelConfigResponse
-from humanloop.model.tool_config_response import ToolConfigResponse
+from humanloop.model.feedback_request import FeedbackRequest
```

### Comparing `humanloop-0.4.6/humanloop/model/config_type.py` & `humanloop-0.4.7/humanloop/model/config_type.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/config_type.pyi` & `humanloop-0.4.7/humanloop/model/config_type.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/create_experiment_request.py` & `humanloop-0.4.7/humanloop/model/create_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/create_experiment_request.pyi` & `humanloop-0.4.7/humanloop/model/create_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/create_log_response.py` & `humanloop-0.4.7/humanloop/model/create_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/create_log_response.pyi` & `humanloop-0.4.7/humanloop/model/create_log_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/create_project_request.py` & `humanloop-0.4.7/humanloop/model/create_project_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/create_project_request.pyi` & `humanloop-0.4.7/humanloop/model/create_project_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/create_session_response.py` & `humanloop-0.4.7/humanloop/model/create_session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/create_session_response.pyi` & `humanloop-0.4.7/humanloop/model/create_session_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/create_trace_request.py` & `humanloop-0.4.7/humanloop/model/create_trace_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/create_trace_request.pyi` & `humanloop-0.4.7/humanloop/model/create_trace_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/create_trace_response.py` & `humanloop-0.4.7/humanloop/model/create_trace_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/create_trace_response.pyi` & `humanloop-0.4.7/humanloop/model/create_trace_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/data_response.py` & `humanloop-0.4.7/humanloop/model/data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/data_response.pyi` & `humanloop-0.4.7/humanloop/model/data_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/experiment_config_response.py` & `humanloop-0.4.7/humanloop/model/experiment_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/experiment_config_response.pyi` & `humanloop-0.4.7/humanloop/model/experiment_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/experiment_response.py` & `humanloop-0.4.7/humanloop/model/experiment_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/experiment_response.pyi` & `humanloop-0.4.7/humanloop/model/experiment_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/experiment_status.py` & `humanloop-0.4.7/humanloop/model/experiment_status.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/experiment_status.pyi` & `humanloop-0.4.7/humanloop/model/experiment_status.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/experiments_list_response.py` & `humanloop-0.4.7/humanloop/model/experiments_list_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/experiments_list_response.pyi` & `humanloop-0.4.7/humanloop/model/experiments_list_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback.py` & `humanloop-0.4.7/humanloop/model/feedback.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback.pyi` & `humanloop-0.4.7/humanloop/model/feedback.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback_class.py` & `humanloop-0.4.7/humanloop/model/feedback_class.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback_class.pyi` & `humanloop-0.4.7/humanloop/model/feedback_class.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback_label_request.py` & `humanloop-0.4.7/humanloop/model/feedback_label_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback_label_request.pyi` & `humanloop-0.4.7/humanloop/model/feedback_label_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback_request.py` & `humanloop-0.4.7/humanloop/model/feedback_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback_request.pyi` & `humanloop-0.4.7/humanloop/model/feedback_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback_response.py` & `humanloop-0.4.7/humanloop/model/feedback_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback_response.pyi` & `humanloop-0.4.7/humanloop/model/feedback_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback_submit_request.py` & `humanloop-0.4.7/humanloop/model/feedback_submit_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class FeedbackSubmitRequest(
+class FeedbackSubmitResponse(
     schemas.ComposedSchema,
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
@@ -38,54 +38,54 @@
             schemas.ListSchema
         ):
         
         
             class MetaOapg:
                 
                 @staticmethod
-                def items() -> typing.Type['FeedbackRequest']:
-                    return FeedbackRequest
+                def items() -> typing.Type['FeedbackResponse']:
+                    return FeedbackResponse
         
             def __new__(
                 cls,
-                arg: typing.Union[typing.Tuple['FeedbackRequest'], typing.List['FeedbackRequest']],
+                arg: typing.Union[typing.Tuple['FeedbackResponse'], typing.List['FeedbackResponse']],
                 _configuration: typing.Optional[schemas.Configuration] = None,
             ) -> 'any_of_0':
                 return super().__new__(
                     cls,
                     arg,
                     _configuration=_configuration,
                 )
         
-            def __getitem__(self, i: int) -> 'FeedbackRequest':
+            def __getitem__(self, i: int) -> 'FeedbackResponse':
                 return super().__getitem__(i)
         
         @classmethod
         @functools.lru_cache()
         def any_of(cls):
             # we need this here to make our import statements work
             # we must store _composed_schemas in here so the code is only run
             # when we invoke this method. If we kept this at the class
             # level we would get an error because the class level
             # code would be run when this module is imported, and these composed
             # classes don't exist yet because their module has not finished
             # loading
             return [
                 cls.any_of_0,
-                FeedbackRequest,
+                FeedbackResponse,
             ]
 
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'FeedbackSubmitRequest':
+    ) -> 'FeedbackSubmitResponse':
         return super().__new__(
             cls,
             *args,
             _configuration=_configuration,
             **kwargs,
         )
 
-from humanloop.model.feedback_request import FeedbackRequest
+from humanloop.model.feedback_response import FeedbackResponse
```

### Comparing `humanloop-0.4.6/humanloop/model/feedback_submit_request.pyi` & `humanloop-0.4.7/humanloop/model/feedback_submit_response.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class FeedbackSubmitRequest(
+class FeedbackSubmitResponse(
     schemas.ComposedSchema,
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
@@ -38,54 +38,54 @@
             schemas.ListSchema
         ):
         
         
             class MetaOapg:
                 
                 @staticmethod
-                def items() -> typing.Type['FeedbackRequest']:
-                    return FeedbackRequest
+                def items() -> typing.Type['FeedbackResponse']:
+                    return FeedbackResponse
         
             def __new__(
                 cls,
-                arg: typing.Union[typing.Tuple['FeedbackRequest'], typing.List['FeedbackRequest']],
+                arg: typing.Union[typing.Tuple['FeedbackResponse'], typing.List['FeedbackResponse']],
                 _configuration: typing.Optional[schemas.Configuration] = None,
             ) -> 'any_of_0':
                 return super().__new__(
                     cls,
                     arg,
                     _configuration=_configuration,
                 )
         
-            def __getitem__(self, i: int) -> 'FeedbackRequest':
+            def __getitem__(self, i: int) -> 'FeedbackResponse':
                 return super().__getitem__(i)
         
         @classmethod
         @functools.lru_cache()
         def any_of(cls):
             # we need this here to make our import statements work
             # we must store _composed_schemas in here so the code is only run
             # when we invoke this method. If we kept this at the class
             # level we would get an error because the class level
             # code would be run when this module is imported, and these composed
             # classes don't exist yet because their module has not finished
             # loading
             return [
                 cls.any_of_0,
-                FeedbackRequest,
+                FeedbackResponse,
             ]
 
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'FeedbackSubmitRequest':
+    ) -> 'FeedbackSubmitResponse':
         return super().__new__(
             cls,
             *args,
             _configuration=_configuration,
             **kwargs,
         )
 
-from humanloop.model.feedback_request import FeedbackRequest
+from humanloop.model.feedback_response import FeedbackResponse
```

### Comparing `humanloop-0.4.6/humanloop/model/feedback_submit_response.py` & `humanloop-0.4.7/humanloop/model/logs_log_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class FeedbackSubmitResponse(
+class LogsLogResponse(
     schemas.ComposedSchema,
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
@@ -38,54 +38,54 @@
             schemas.ListSchema
         ):
         
         
             class MetaOapg:
                 
                 @staticmethod
-                def items() -> typing.Type['FeedbackResponse']:
-                    return FeedbackResponse
+                def items() -> typing.Type['CreateLogResponse']:
+                    return CreateLogResponse
         
             def __new__(
                 cls,
-                arg: typing.Union[typing.Tuple['FeedbackResponse'], typing.List['FeedbackResponse']],
+                arg: typing.Union[typing.Tuple['CreateLogResponse'], typing.List['CreateLogResponse']],
                 _configuration: typing.Optional[schemas.Configuration] = None,
             ) -> 'any_of_0':
                 return super().__new__(
                     cls,
                     arg,
                     _configuration=_configuration,
                 )
         
-            def __getitem__(self, i: int) -> 'FeedbackResponse':
+            def __getitem__(self, i: int) -> 'CreateLogResponse':
                 return super().__getitem__(i)
         
         @classmethod
         @functools.lru_cache()
         def any_of(cls):
             # we need this here to make our import statements work
             # we must store _composed_schemas in here so the code is only run
             # when we invoke this method. If we kept this at the class
             # level we would get an error because the class level
             # code would be run when this module is imported, and these composed
             # classes don't exist yet because their module has not finished
             # loading
             return [
                 cls.any_of_0,
-                FeedbackResponse,
+                CreateLogResponse,
             ]
 
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'FeedbackSubmitResponse':
+    ) -> 'LogsLogResponse':
         return super().__new__(
             cls,
             *args,
             _configuration=_configuration,
             **kwargs,
         )
 
-from humanloop.model.feedback_response import FeedbackResponse
+from humanloop.model.create_log_response import CreateLogResponse
```

### Comparing `humanloop-0.4.6/humanloop/model/feedback_submit_response.pyi` & `humanloop-0.4.7/humanloop/model/logs_log_response.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class FeedbackSubmitResponse(
+class LogsLogResponse(
     schemas.ComposedSchema,
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
@@ -38,54 +38,54 @@
             schemas.ListSchema
         ):
         
         
             class MetaOapg:
                 
                 @staticmethod
-                def items() -> typing.Type['FeedbackResponse']:
-                    return FeedbackResponse
+                def items() -> typing.Type['CreateLogResponse']:
+                    return CreateLogResponse
         
             def __new__(
                 cls,
-                arg: typing.Union[typing.Tuple['FeedbackResponse'], typing.List['FeedbackResponse']],
+                arg: typing.Union[typing.Tuple['CreateLogResponse'], typing.List['CreateLogResponse']],
                 _configuration: typing.Optional[schemas.Configuration] = None,
             ) -> 'any_of_0':
                 return super().__new__(
                     cls,
                     arg,
                     _configuration=_configuration,
                 )
         
-            def __getitem__(self, i: int) -> 'FeedbackResponse':
+            def __getitem__(self, i: int) -> 'CreateLogResponse':
                 return super().__getitem__(i)
         
         @classmethod
         @functools.lru_cache()
         def any_of(cls):
             # we need this here to make our import statements work
             # we must store _composed_schemas in here so the code is only run
             # when we invoke this method. If we kept this at the class
             # level we would get an error because the class level
             # code would be run when this module is imported, and these composed
             # classes don't exist yet because their module has not finished
             # loading
             return [
                 cls.any_of_0,
-                FeedbackResponse,
+                CreateLogResponse,
             ]
 
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'FeedbackSubmitResponse':
+    ) -> 'LogsLogResponse':
         return super().__new__(
             cls,
             *args,
             _configuration=_configuration,
             **kwargs,
         )
 
-from humanloop.model.feedback_response import FeedbackResponse
+from humanloop.model.create_log_response import CreateLogResponse
```

### Comparing `humanloop-0.4.6/humanloop/model/feedback_type.py` & `humanloop-0.4.7/humanloop/model/feedback_type.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback_type.pyi` & `humanloop-0.4.7/humanloop/model/feedback_type.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback_type_model.py` & `humanloop-0.4.7/humanloop/model/feedback_type_model.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback_type_model.pyi` & `humanloop-0.4.7/humanloop/model/feedback_type_model.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback_type_request.py` & `humanloop-0.4.7/humanloop/model/feedback_type_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback_type_request.pyi` & `humanloop-0.4.7/humanloop/model/feedback_type_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback_types.py` & `humanloop-0.4.7/humanloop/model/feedback_types.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/feedback_types.pyi` & `humanloop-0.4.7/humanloop/model/feedback_types.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/generic_config_request.py` & `humanloop-0.4.7/humanloop/model/generic_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/generic_config_request.pyi` & `humanloop-0.4.7/humanloop/model/generic_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/generic_config_response.py` & `humanloop-0.4.7/humanloop/model/update_project_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,144 +19,105 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class GenericConfigResponse(
+class UpdateProjectRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
-        required = {
-            "name",
-            "id",
-            "type",
-        }
         
         class properties:
-            id = schemas.StrSchema
+            active_experiment_id = schemas.StrSchema
+            active_config_id = schemas.StrSchema
             
             
-            class type(
-                schemas.ComposedSchema,
+            class positive_labels(
+                schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
-                    @classmethod
-                    @functools.lru_cache()
-                    def all_of(cls):
-                        # we need this here to make our import statements work
-                        # we must store _composed_schemas in here so the code is only run
-                        # when we invoke this method. If we kept this at the class
-                        # level we would get an error because the class level
-                        # code would be run when this module is imported, and these composed
-                        # classes don't exist yet because their module has not finished
-                        # loading
-                        return [
-                            ConfigType,
-                        ]
-            
+                    @staticmethod
+                    def items() -> typing.Type['PositiveLabel']:
+                        return PositiveLabel
             
                 def __new__(
                     cls,
-                    *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                    arg: typing.Union[typing.Tuple['PositiveLabel'], typing.List['PositiveLabel']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'type':
+                ) -> 'positive_labels':
                     return super().__new__(
                         cls,
-                        *args,
+                        arg,
                         _configuration=_configuration,
-                        **kwargs,
                     )
-            name = schemas.StrSchema
-            description = schemas.StrSchema
-            other = schemas.DictSchema
+            
+                def __getitem__(self, i: int) -> 'PositiveLabel':
+                    return super().__getitem__(i)
             __annotations__ = {
-                "id": id,
-                "type": type,
-                "name": name,
-                "description": description,
-                "other": other,
+                "active_experiment_id": active_experiment_id,
+                "active_config_id": active_config_id,
+                "positive_labels": positive_labels,
             }
     
-    name: MetaOapg.properties.name
-    id: MetaOapg.properties.id
-    type: MetaOapg.properties.type
-    
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def __getitem__(self, name: typing_extensions.Literal["active_experiment_id"]) -> MetaOapg.properties.active_experiment_id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
+    def __getitem__(self, name: typing_extensions.Literal["active_config_id"]) -> MetaOapg.properties.active_config_id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
+    def __getitem__(self, name: typing_extensions.Literal["positive_labels"]) -> MetaOapg.properties.positive_labels: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "description", "other", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["active_experiment_id", "active_config_id", "positive_labels", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["active_experiment_id"]) -> typing.Union[MetaOapg.properties.active_experiment_id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["active_config_id"]) -> typing.Union[MetaOapg.properties.active_config_id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["positive_labels"]) -> typing.Union[MetaOapg.properties.positive_labels, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "description", "other", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["active_experiment_id", "active_config_id", "positive_labels", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        name: typing.Union[MetaOapg.properties.name, str, ],
-        id: typing.Union[MetaOapg.properties.id, str, ],
-        type: typing.Union[MetaOapg.properties.type, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
-        other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        active_experiment_id: typing.Union[MetaOapg.properties.active_experiment_id, str, schemas.Unset] = schemas.unset,
+        active_config_id: typing.Union[MetaOapg.properties.active_config_id, str, schemas.Unset] = schemas.unset,
+        positive_labels: typing.Union[MetaOapg.properties.positive_labels, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'GenericConfigResponse':
+    ) -> 'UpdateProjectRequest':
         return super().__new__(
             cls,
             *args,
-            name=name,
-            id=id,
-            type=type,
-            description=description,
-            other=other,
+            active_experiment_id=active_experiment_id,
+            active_config_id=active_config_id,
+            positive_labels=positive_labels,
             _configuration=_configuration,
             **kwargs,
         )
 
-from humanloop.model.config_type import ConfigType
+from humanloop.model.positive_label import PositiveLabel
```

### Comparing `humanloop-0.4.6/humanloop/model/generic_config_response.pyi` & `humanloop-0.4.7/humanloop/model/update_project_request.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -19,144 +19,105 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class GenericConfigResponse(
+class UpdateProjectRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
-        required = {
-            "name",
-            "id",
-            "type",
-        }
         
         class properties:
-            id = schemas.StrSchema
+            active_experiment_id = schemas.StrSchema
+            active_config_id = schemas.StrSchema
             
             
-            class type(
-                schemas.ComposedSchema,
+            class positive_labels(
+                schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
-                    @classmethod
-                    @functools.lru_cache()
-                    def all_of(cls):
-                        # we need this here to make our import statements work
-                        # we must store _composed_schemas in here so the code is only run
-                        # when we invoke this method. If we kept this at the class
-                        # level we would get an error because the class level
-                        # code would be run when this module is imported, and these composed
-                        # classes don't exist yet because their module has not finished
-                        # loading
-                        return [
-                            ConfigType,
-                        ]
-            
+                    @staticmethod
+                    def items() -> typing.Type['PositiveLabel']:
+                        return PositiveLabel
             
                 def __new__(
                     cls,
-                    *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                    arg: typing.Union[typing.Tuple['PositiveLabel'], typing.List['PositiveLabel']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'type':
+                ) -> 'positive_labels':
                     return super().__new__(
                         cls,
-                        *args,
+                        arg,
                         _configuration=_configuration,
-                        **kwargs,
                     )
-            name = schemas.StrSchema
-            description = schemas.StrSchema
-            other = schemas.DictSchema
+            
+                def __getitem__(self, i: int) -> 'PositiveLabel':
+                    return super().__getitem__(i)
             __annotations__ = {
-                "id": id,
-                "type": type,
-                "name": name,
-                "description": description,
-                "other": other,
+                "active_experiment_id": active_experiment_id,
+                "active_config_id": active_config_id,
+                "positive_labels": positive_labels,
             }
     
-    name: MetaOapg.properties.name
-    id: MetaOapg.properties.id
-    type: MetaOapg.properties.type
-    
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def __getitem__(self, name: typing_extensions.Literal["active_experiment_id"]) -> MetaOapg.properties.active_experiment_id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
+    def __getitem__(self, name: typing_extensions.Literal["active_config_id"]) -> MetaOapg.properties.active_config_id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
+    def __getitem__(self, name: typing_extensions.Literal["positive_labels"]) -> MetaOapg.properties.positive_labels: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "description", "other", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["active_experiment_id", "active_config_id", "positive_labels", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["active_experiment_id"]) -> typing.Union[MetaOapg.properties.active_experiment_id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["active_config_id"]) -> typing.Union[MetaOapg.properties.active_config_id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["positive_labels"]) -> typing.Union[MetaOapg.properties.positive_labels, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "description", "other", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["active_experiment_id", "active_config_id", "positive_labels", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        name: typing.Union[MetaOapg.properties.name, str, ],
-        id: typing.Union[MetaOapg.properties.id, str, ],
-        type: typing.Union[MetaOapg.properties.type, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
-        other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        active_experiment_id: typing.Union[MetaOapg.properties.active_experiment_id, str, schemas.Unset] = schemas.unset,
+        active_config_id: typing.Union[MetaOapg.properties.active_config_id, str, schemas.Unset] = schemas.unset,
+        positive_labels: typing.Union[MetaOapg.properties.positive_labels, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'GenericConfigResponse':
+    ) -> 'UpdateProjectRequest':
         return super().__new__(
             cls,
             *args,
-            name=name,
-            id=id,
-            type=type,
-            description=description,
-            other=other,
+            active_experiment_id=active_experiment_id,
+            active_config_id=active_config_id,
+            positive_labels=positive_labels,
             _configuration=_configuration,
             **kwargs,
         )
 
-from humanloop.model.config_type import ConfigType
+from humanloop.model.positive_label import PositiveLabel
```

### Comparing `humanloop-0.4.6/humanloop/model/get_model_config_response.py` & `humanloop-0.4.7/humanloop/model/get_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/get_model_config_response.pyi` & `humanloop-0.4.7/humanloop/model/get_model_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/http_validation_error.py` & `humanloop-0.4.7/humanloop/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/http_validation_error.pyi` & `humanloop-0.4.7/humanloop/model/http_validation_error.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/label_sentiment.py` & `humanloop-0.4.7/humanloop/model/label_sentiment.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/label_sentiment.pyi` & `humanloop-0.4.7/humanloop/model/label_sentiment.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/log_datapoint_request.py` & `humanloop-0.4.7/humanloop/model/log_datapoint_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/log_datapoint_request.pyi` & `humanloop-0.4.7/humanloop/model/log_datapoint_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/log_model_config_request.py` & `humanloop-0.4.7/humanloop/model/log_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/log_model_config_request.pyi` & `humanloop-0.4.7/humanloop/model/log_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/log_request.py` & `humanloop-0.4.7/humanloop/model/log_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/log_request.pyi` & `humanloop-0.4.7/humanloop/model/log_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/log_response.py` & `humanloop-0.4.7/humanloop/model/log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/log_response.pyi` & `humanloop-0.4.7/humanloop/model/log_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/model_config_chat_request.py` & `humanloop-0.4.7/humanloop/model/model_config_chat_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/model_config_chat_request.pyi` & `humanloop-0.4.7/humanloop/model/model_config_chat_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/model_config_completion_request.py` & `humanloop-0.4.7/humanloop/model/model_config_completion_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/model_config_completion_request.pyi` & `humanloop-0.4.7/humanloop/model/model_config_completion_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/model_endpoints.py` & `humanloop-0.4.7/humanloop/model/model_endpoints.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/model_endpoints.pyi` & `humanloop-0.4.7/humanloop/model/model_endpoints.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/model_providers.py` & `humanloop-0.4.7/humanloop/model/model_providers.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/model_providers.pyi` & `humanloop-0.4.7/humanloop/model/model_providers.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/paginated_data_log_response.py` & `humanloop-0.4.7/humanloop/model/paginated_data_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/paginated_data_log_response.pyi` & `humanloop-0.4.7/humanloop/model/paginated_data_log_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/paginated_data_project_response.py` & `humanloop-0.4.7/humanloop/model/paginated_data_project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/paginated_data_project_response.pyi` & `humanloop-0.4.7/humanloop/model/paginated_data_project_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/paginated_data_session_response.py` & `humanloop-0.4.7/humanloop/model/paginated_data_session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/paginated_data_session_response.pyi` & `humanloop-0.4.7/humanloop/model/paginated_data_session_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/positive_label.py` & `humanloop-0.4.7/humanloop/model/positive_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/positive_label.pyi` & `humanloop-0.4.7/humanloop/model/positive_label.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/project_config_response.py` & `humanloop-0.4.7/humanloop/model/project_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/project_config_response.pyi` & `humanloop-0.4.7/humanloop/model/project_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/project_model_config_request.py` & `humanloop-0.4.7/humanloop/model/project_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/project_model_config_request.pyi` & `humanloop-0.4.7/humanloop/model/project_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/project_model_config_response.py` & `humanloop-0.4.7/humanloop/model/project_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/project_model_config_response.pyi` & `humanloop-0.4.7/humanloop/model/project_model_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/project_response.py` & `humanloop-0.4.7/humanloop/model/project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/project_response.pyi` & `humanloop-0.4.7/humanloop/model/project_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/project_sort_by.py` & `humanloop-0.4.7/humanloop/model/project_sort_by.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/project_sort_by.pyi` & `humanloop-0.4.7/humanloop/model/project_sort_by.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/project_user_response.py` & `humanloop-0.4.7/humanloop/model/project_user_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/project_user_response.pyi` & `humanloop-0.4.7/humanloop/model/project_user_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/projects_get_configs_response.py` & `humanloop-0.4.7/humanloop/model/projects_get_configs_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/projects_get_configs_response.pyi` & `humanloop-0.4.7/humanloop/model/projects_get_configs_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/projects_update_feedback_types_request.py` & `humanloop-0.4.7/humanloop/model/projects_update_feedback_types_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/projects_update_feedback_types_request.pyi` & `humanloop-0.4.7/humanloop/model/projects_update_feedback_types_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/provider_api_keys.py` & `humanloop-0.4.7/humanloop/model/provider_api_keys.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/provider_api_keys.pyi` & `humanloop-0.4.7/humanloop/model/provider_api_keys.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/session_project_response.py` & `humanloop-0.4.7/humanloop/model/session_project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/session_project_response.pyi` & `humanloop-0.4.7/humanloop/model/session_project_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/session_response.py` & `humanloop-0.4.7/humanloop/model/session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/session_response.pyi` & `humanloop-0.4.7/humanloop/model/session_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/sort_order.py` & `humanloop-0.4.7/humanloop/model/sort_order.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/sort_order.pyi` & `humanloop-0.4.7/humanloop/model/sort_order.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.py` & `humanloop-0.4.7/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.pyi` & `humanloop-0.4.7/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.7/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi` & `humanloop-0.4.7/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/src_external_app_models_v4_configs_model_config_response.py` & `humanloop-0.4.7/humanloop/model/src_external_app_models_v4_configs_model_config_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,47 +42,27 @@
         }
         
         class properties:
             id = schemas.StrSchema
             
             
             class type(
-                schemas.ComposedSchema,
+                schemas.EnumBase,
+                schemas.StrSchema
             ):
             
             
                 class MetaOapg:
-                    
-                    @classmethod
-                    @functools.lru_cache()
-                    def all_of(cls):
-                        # we need this here to make our import statements work
-                        # we must store _composed_schemas in here so the code is only run
-                        # when we invoke this method. If we kept this at the class
-                        # level we would get an error because the class level
-                        # code would be run when this module is imported, and these composed
-                        # classes don't exist yet because their module has not finished
-                        # loading
-                        return [
-                            ConfigType,
-                        ]
-            
-            
-                def __new__(
-                    cls,
-                    *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'type':
-                    return super().__new__(
-                        cls,
-                        *args,
-                        _configuration=_configuration,
-                        **kwargs,
-                    )
+                    enum_value_to_name = {
+                        "model": "MODEL",
+                    }
+                
+                @schemas.classproperty
+                def MODEL(cls):
+                    return cls("model")
             name = schemas.StrSchema
             model = schemas.StrSchema
             description = schemas.StrSchema
             other = schemas.DictSchema
             
             
             class provider(
@@ -385,15 +365,15 @@
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
         model: typing.Union[MetaOapg.properties.model, str, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
-        type: typing.Union[MetaOapg.properties.type, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        type: typing.Union[MetaOapg.properties.type, str, ],
         description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         provider: typing.Union[MetaOapg.properties.provider, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         max_tokens: typing.Union[MetaOapg.properties.max_tokens, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         temperature: typing.Union[MetaOapg.properties.temperature, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         top_p: typing.Union[MetaOapg.properties.top_p, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
@@ -425,10 +405,9 @@
             chat_template=chat_template,
             endpoint=endpoint,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.chat_message import ChatMessage
-from humanloop.model.config_type import ConfigType
 from humanloop.model.model_endpoints import ModelEndpoints
 from humanloop.model.model_providers import ModelProviders
```

### Comparing `humanloop-0.4.6/humanloop/model/src_external_app_models_v4_configs_model_config_response.pyi` & `humanloop-0.4.7/humanloop/model/src_external_app_models_v4_configs_model_config_response.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -42,47 +42,21 @@
         }
         
         class properties:
             id = schemas.StrSchema
             
             
             class type(
-                schemas.ComposedSchema,
+                schemas.EnumBase,
+                schemas.StrSchema
             ):
-            
-            
-                class MetaOapg:
-                    
-                    @classmethod
-                    @functools.lru_cache()
-                    def all_of(cls):
-                        # we need this here to make our import statements work
-                        # we must store _composed_schemas in here so the code is only run
-                        # when we invoke this method. If we kept this at the class
-                        # level we would get an error because the class level
-                        # code would be run when this module is imported, and these composed
-                        # classes don't exist yet because their module has not finished
-                        # loading
-                        return [
-                            ConfigType,
-                        ]
-            
-            
-                def __new__(
-                    cls,
-                    *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'type':
-                    return super().__new__(
-                        cls,
-                        *args,
-                        _configuration=_configuration,
-                        **kwargs,
-                    )
+                
+                @schemas.classproperty
+                def MODEL(cls):
+                    return cls("model")
             name = schemas.StrSchema
             model = schemas.StrSchema
             description = schemas.StrSchema
             other = schemas.DictSchema
             
             
             class provider(
@@ -385,15 +359,15 @@
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
         model: typing.Union[MetaOapg.properties.model, str, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
-        type: typing.Union[MetaOapg.properties.type, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        type: typing.Union[MetaOapg.properties.type, str, ],
         description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         provider: typing.Union[MetaOapg.properties.provider, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         max_tokens: typing.Union[MetaOapg.properties.max_tokens, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         temperature: typing.Union[MetaOapg.properties.temperature, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         top_p: typing.Union[MetaOapg.properties.top_p, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
@@ -425,10 +399,9 @@
             chat_template=chat_template,
             endpoint=endpoint,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.chat_message import ChatMessage
-from humanloop.model.config_type import ConfigType
 from humanloop.model.model_endpoints import ModelEndpoints
 from humanloop.model.model_providers import ModelProviders
```

### Comparing `humanloop-0.4.6/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.7/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.pyi` & `humanloop-0.4.7/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/tool_config_request.py` & `humanloop-0.4.7/humanloop/model/tool_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/tool_config_request.pyi` & `humanloop-0.4.7/humanloop/model/tool_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/tool_config_response.py` & `humanloop-0.4.7/humanloop/model/generic_config_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class ToolConfigResponse(
+class GenericConfigResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
@@ -39,58 +39,36 @@
         }
         
         class properties:
             id = schemas.StrSchema
             
             
             class type(
-                schemas.ComposedSchema,
+                schemas.EnumBase,
+                schemas.StrSchema
             ):
             
             
                 class MetaOapg:
-                    
-                    @classmethod
-                    @functools.lru_cache()
-                    def all_of(cls):
-                        # we need this here to make our import statements work
-                        # we must store _composed_schemas in here so the code is only run
-                        # when we invoke this method. If we kept this at the class
-                        # level we would get an error because the class level
-                        # code would be run when this module is imported, and these composed
-                        # classes don't exist yet because their module has not finished
-                        # loading
-                        return [
-                            ConfigType,
-                        ]
-            
-            
-                def __new__(
-                    cls,
-                    *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'type':
-                    return super().__new__(
-                        cls,
-                        *args,
-                        _configuration=_configuration,
-                        **kwargs,
-                    )
+                    enum_value_to_name = {
+                        "generic": "GENERIC",
+                    }
+                
+                @schemas.classproperty
+                def GENERIC(cls):
+                    return cls("generic")
             name = schemas.StrSchema
             description = schemas.StrSchema
             other = schemas.DictSchema
-            source = schemas.StrSchema
             __annotations__ = {
                 "id": id,
                 "type": type,
                 "name": name,
                 "description": description,
                 "other": other,
-                "source": source,
             }
     
     name: MetaOapg.properties.name
     id: MetaOapg.properties.id
     type: MetaOapg.properties.type
     
     @typing.overload
@@ -105,20 +83,17 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
-    
-    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "description", "other", "source", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "description", "other", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
@@ -131,42 +106,35 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "description", "other", "source", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "description", "other", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
-        type: typing.Union[MetaOapg.properties.type, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        type: typing.Union[MetaOapg.properties.type, str, ],
         description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
-        source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'ToolConfigResponse':
+    ) -> 'GenericConfigResponse':
         return super().__new__(
             cls,
             *args,
             name=name,
             id=id,
             type=type,
             description=description,
             other=other,
-            source=source,
             _configuration=_configuration,
             **kwargs,
         )
-
-from humanloop.model.config_type import ConfigType
```

### Comparing `humanloop-0.4.6/humanloop/model/tool_config_response.pyi` & `humanloop-0.4.7/humanloop/model/agent_config_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,34 +19,54 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class ToolConfigResponse(
+class AgentConfigResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
+            "model_config",
+            "agent_class",
             "name",
             "id",
             "type",
         }
         
         class properties:
             id = schemas.StrSchema
             
             
             class type(
+                schemas.EnumBase,
+                schemas.StrSchema
+            ):
+            
+            
+                class MetaOapg:
+                    enum_value_to_name = {
+                        "agent": "AGENT",
+                    }
+                
+                @schemas.classproperty
+                def AGENT(cls):
+                    return cls("agent")
+            name = schemas.StrSchema
+            agent_class = schemas.StrSchema
+            
+            
+            class model_config(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
@@ -56,117 +76,162 @@
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            ConfigType,
+                            LogModelConfigRequest,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'type':
+                ) -> 'model_config':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            name = schemas.StrSchema
             description = schemas.StrSchema
             other = schemas.DictSchema
-            source = schemas.StrSchema
+            
+            
+            class tools(
+                schemas.ListSchema
+            ):
+            
+            
+                class MetaOapg:
+                    
+                    @staticmethod
+                    def items() -> typing.Type['ToolConfigRequest']:
+                        return ToolConfigRequest
+            
+                def __new__(
+                    cls,
+                    arg: typing.Union[typing.Tuple['ToolConfigRequest'], typing.List['ToolConfigRequest']],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'tools':
+                    return super().__new__(
+                        cls,
+                        arg,
+                        _configuration=_configuration,
+                    )
+            
+                def __getitem__(self, i: int) -> 'ToolConfigRequest':
+                    return super().__getitem__(i)
             __annotations__ = {
                 "id": id,
                 "type": type,
                 "name": name,
+                "agent_class": agent_class,
+                "model_config": model_config,
                 "description": description,
                 "other": other,
-                "source": source,
+                "tools": tools,
             }
     
+    model_config: MetaOapg.properties.model_config
+    agent_class: MetaOapg.properties.agent_class
     name: MetaOapg.properties.name
     id: MetaOapg.properties.id
     type: MetaOapg.properties.type
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["agent_class"]) -> MetaOapg.properties.agent_class: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
+    def __getitem__(self, name: typing_extensions.Literal["tools"]) -> MetaOapg.properties.tools: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "description", "other", "source", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "agent_class", "model_config", "description", "other", "tools", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["agent_class"]) -> MetaOapg.properties.agent_class: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["tools"]) -> typing.Union[MetaOapg.properties.tools, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "description", "other", "source", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "agent_class", "model_config", "description", "other", "tools", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
+        model_config: typing.Union[MetaOapg.properties.model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        agent_class: typing.Union[MetaOapg.properties.agent_class, str, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
-        type: typing.Union[MetaOapg.properties.type, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        type: typing.Union[MetaOapg.properties.type, str, ],
         description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
-        source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
+        tools: typing.Union[MetaOapg.properties.tools, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'ToolConfigResponse':
+    ) -> 'AgentConfigResponse':
         return super().__new__(
             cls,
             *args,
+            model_config=model_config,
+            agent_class=agent_class,
             name=name,
             id=id,
             type=type,
             description=description,
             other=other,
-            source=source,
+            tools=tools,
             _configuration=_configuration,
             **kwargs,
         )
 
-from humanloop.model.config_type import ConfigType
+from humanloop.model.log_model_config_request import LogModelConfigRequest
+from humanloop.model.tool_config_request import ToolConfigRequest
```

### Comparing `humanloop-0.4.6/humanloop/model/tool_result_response.py` & `humanloop-0.4.7/humanloop/model/tool_result_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/tool_result_response.pyi` & `humanloop-0.4.7/humanloop/model/tool_result_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/trace_log_request.py` & `humanloop-0.4.7/humanloop/model/trace_model_config_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,263 +19,383 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class TraceLogRequest(
+class TraceModelConfigRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    Simplified version of LogRequest.
+    Model config request that supports both chat and completion.
 
-Changes:
-    - Renamed `project` to `function_name`. TODO: Allow either `function_name` or `function_id`.
+Implemented here with the full set of fields from both
+ChatModelConfigRequest and CompletionModelConfigRequest.
+
+Ideally we'd use `Union[ChatModelConfigRequest, CompletionModelConfigRequest]`
+but that seems to cause Pydantic errors, especially with the `type` discriminator.
+
+Validation is done to ensure that only one of `chat_template` and
+`prompt_template` is provided, and that the provided one properly
+corresponds to the endpoint.
+This defaults to `complete` endpoint.
     """
 
 
     class MetaOapg:
         required = {
-            "function_name",
+            "model",
+            "type",
         }
         
         class properties:
-            function_name = schemas.StrSchema
-            trial_id = schemas.StrSchema
-            inputs = schemas.DictSchema
+            model = schemas.StrSchema
             
             
-            class messages(
-                schemas.ListSchema
+            class type(
+                schemas.EnumBase,
+                schemas.StrSchema
+            ):
+            
+            
+                class MetaOapg:
+                    enum_value_to_name = {
+                        "model": "MODEL",
+                    }
+                
+                @schemas.classproperty
+                def MODEL(cls):
+                    return cls("model")
+            description = schemas.StrSchema
+            name = schemas.StrSchema
+            
+            
+            class provider(
+                schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
-                    @staticmethod
-                    def items() -> typing.Type['ChatMessage']:
-                        return ChatMessage
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            ModelProviders,
+                        ]
+            
             
                 def __new__(
                     cls,
-                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
+                    *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'messages':
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'provider':
                     return super().__new__(
                         cls,
-                        arg,
+                        *args,
                         _configuration=_configuration,
+                        **kwargs,
                     )
+            max_tokens = schemas.IntSchema
+            temperature = schemas.NumberSchema
+            top_p = schemas.NumberSchema
             
-                def __getitem__(self, i: int) -> 'ChatMessage':
-                    return super().__getitem__(i)
-            output = schemas.StrSchema
-            source = schemas.StrSchema
+            
+            class stop(
+                schemas.ComposedSchema,
+            ):
+            
+            
+                class MetaOapg:
+                    any_of_0 = schemas.StrSchema
+                    
+                    
+                    class any_of_1(
+                        schemas.ListSchema
+                    ):
+                    
+                    
+                        class MetaOapg:
+                            items = schemas.StrSchema
+                    
+                        def __new__(
+                            cls,
+                            arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
+                            _configuration: typing.Optional[schemas.Configuration] = None,
+                        ) -> 'any_of_1':
+                            return super().__new__(
+                                cls,
+                                arg,
+                                _configuration=_configuration,
+                            )
+                    
+                        def __getitem__(self, i: int) -> MetaOapg.items:
+                            return super().__getitem__(i)
+                    
+                    @classmethod
+                    @functools.lru_cache()
+                    def any_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            cls.any_of_0,
+                            cls.any_of_1,
+                        ]
             
             
-            class config(
+                def __new__(
+                    cls,
+                    *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'stop':
+                    return super().__new__(
+                        cls,
+                        *args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
+            presence_penalty = schemas.NumberSchema
+            frequency_penalty = schemas.NumberSchema
+            other = schemas.DictSchema
+            
+            
+            class endpoint(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
                     @functools.lru_cache()
-                    def one_of(cls):
+                    def all_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            TraceModelConfigRequest,
-                            ToolConfigRequest,
-                            GenericConfigRequest,
-                            AgentConfigRequest,
+                            ModelEndpoints,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'config':
+                ) -> 'endpoint':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            metadata = schemas.DictSchema
-            error = schemas.StrSchema
-            duration = schemas.NumberSchema
-            created_at = schemas.DateTimeSchema
+            prompt_template = schemas.StrSchema
             
             
-            class children(
+            class chat_template(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['TraceLogRequest']:
-                        return TraceLogRequest
+                    def items() -> typing.Type['ChatMessage']:
+                        return ChatMessage
             
                 def __new__(
                     cls,
-                    arg: typing.Union[typing.Tuple['TraceLogRequest'], typing.List['TraceLogRequest']],
+                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'children':
+                ) -> 'chat_template':
                     return super().__new__(
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'TraceLogRequest':
+                def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
             __annotations__ = {
-                "function_name": function_name,
-                "trial_id": trial_id,
-                "inputs": inputs,
-                "messages": messages,
-                "output": output,
-                "source": source,
-                "config": config,
-                "metadata": metadata,
-                "error": error,
-                "duration": duration,
-                "created_at": created_at,
-                "children": children,
+                "model": model,
+                "type": type,
+                "description": description,
+                "name": name,
+                "provider": provider,
+                "max_tokens": max_tokens,
+                "temperature": temperature,
+                "top_p": top_p,
+                "stop": stop,
+                "presence_penalty": presence_penalty,
+                "frequency_penalty": frequency_penalty,
+                "other": other,
+                "endpoint": endpoint,
+                "prompt_template": prompt_template,
+                "chat_template": chat_template,
             }
         additional_properties = schemas.NotAnyTypeSchema
     
-    function_name: MetaOapg.properties.function_name
+    model: MetaOapg.properties.model
+    type: MetaOapg.properties.type
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["function_name"]) -> MetaOapg.properties.function_name: ...
+    def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["trial_id"]) -> MetaOapg.properties.trial_id: ...
+    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
+    def __getitem__(self, name: typing_extensions.Literal["provider"]) -> MetaOapg.properties.provider: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+    def __getitem__(self, name: typing_extensions.Literal["max_tokens"]) -> MetaOapg.properties.max_tokens: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
+    def __getitem__(self, name: typing_extensions.Literal["temperature"]) -> MetaOapg.properties.temperature: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["config"]) -> MetaOapg.properties.config: ...
+    def __getitem__(self, name: typing_extensions.Literal["top_p"]) -> MetaOapg.properties.top_p: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
+    def __getitem__(self, name: typing_extensions.Literal["stop"]) -> MetaOapg.properties.stop: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["error"]) -> MetaOapg.properties.error: ...
+    def __getitem__(self, name: typing_extensions.Literal["presence_penalty"]) -> MetaOapg.properties.presence_penalty: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["duration"]) -> MetaOapg.properties.duration: ...
+    def __getitem__(self, name: typing_extensions.Literal["frequency_penalty"]) -> MetaOapg.properties.frequency_penalty: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
+    def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["children"]) -> MetaOapg.properties.children: ...
+    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["function_name"], typing_extensions.Literal["trial_id"], typing_extensions.Literal["inputs"], typing_extensions.Literal["messages"], typing_extensions.Literal["output"], typing_extensions.Literal["source"], typing_extensions.Literal["config"], typing_extensions.Literal["metadata"], typing_extensions.Literal["error"], typing_extensions.Literal["duration"], typing_extensions.Literal["created_at"], typing_extensions.Literal["children"], ]):
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["prompt_template"]) -> MetaOapg.properties.prompt_template: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["chat_template"]) -> MetaOapg.properties.chat_template: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model"], typing_extensions.Literal["type"], typing_extensions.Literal["description"], typing_extensions.Literal["name"], typing_extensions.Literal["provider"], typing_extensions.Literal["max_tokens"], typing_extensions.Literal["temperature"], typing_extensions.Literal["top_p"], typing_extensions.Literal["stop"], typing_extensions.Literal["presence_penalty"], typing_extensions.Literal["frequency_penalty"], typing_extensions.Literal["other"], typing_extensions.Literal["endpoint"], typing_extensions.Literal["prompt_template"], typing_extensions.Literal["chat_template"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["function_name"]) -> MetaOapg.properties.function_name: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["trial_id"]) -> typing.Union[MetaOapg.properties.trial_id, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["provider"]) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> typing.Union[MetaOapg.properties.inputs, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["max_tokens"]) -> typing.Union[MetaOapg.properties.max_tokens, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> typing.Union[MetaOapg.properties.messages, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["temperature"]) -> typing.Union[MetaOapg.properties.temperature, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> typing.Union[MetaOapg.properties.output, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["top_p"]) -> typing.Union[MetaOapg.properties.top_p, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["stop"]) -> typing.Union[MetaOapg.properties.stop, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["config"]) -> typing.Union[MetaOapg.properties.config, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["presence_penalty"]) -> typing.Union[MetaOapg.properties.presence_penalty, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["frequency_penalty"]) -> typing.Union[MetaOapg.properties.frequency_penalty, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["error"]) -> typing.Union[MetaOapg.properties.error, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["duration"]) -> typing.Union[MetaOapg.properties.duration, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> typing.Union[MetaOapg.properties.created_at, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["prompt_template"]) -> typing.Union[MetaOapg.properties.prompt_template, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["children"]) -> typing.Union[MetaOapg.properties.children, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["chat_template"]) -> typing.Union[MetaOapg.properties.chat_template, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["function_name"], typing_extensions.Literal["trial_id"], typing_extensions.Literal["inputs"], typing_extensions.Literal["messages"], typing_extensions.Literal["output"], typing_extensions.Literal["source"], typing_extensions.Literal["config"], typing_extensions.Literal["metadata"], typing_extensions.Literal["error"], typing_extensions.Literal["duration"], typing_extensions.Literal["created_at"], typing_extensions.Literal["children"], ]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model"], typing_extensions.Literal["type"], typing_extensions.Literal["description"], typing_extensions.Literal["name"], typing_extensions.Literal["provider"], typing_extensions.Literal["max_tokens"], typing_extensions.Literal["temperature"], typing_extensions.Literal["top_p"], typing_extensions.Literal["stop"], typing_extensions.Literal["presence_penalty"], typing_extensions.Literal["frequency_penalty"], typing_extensions.Literal["other"], typing_extensions.Literal["endpoint"], typing_extensions.Literal["prompt_template"], typing_extensions.Literal["chat_template"], ]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        function_name: typing.Union[MetaOapg.properties.function_name, str, ],
-        trial_id: typing.Union[MetaOapg.properties.trial_id, str, schemas.Unset] = schemas.unset,
-        inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
-        messages: typing.Union[MetaOapg.properties.messages, list, tuple, schemas.Unset] = schemas.unset,
-        output: typing.Union[MetaOapg.properties.output, str, schemas.Unset] = schemas.unset,
-        source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
-        config: typing.Union[MetaOapg.properties.config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
-        error: typing.Union[MetaOapg.properties.error, str, schemas.Unset] = schemas.unset,
-        duration: typing.Union[MetaOapg.properties.duration, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
-        created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, schemas.Unset] = schemas.unset,
-        children: typing.Union[MetaOapg.properties.children, list, tuple, schemas.Unset] = schemas.unset,
+        model: typing.Union[MetaOapg.properties.model, str, ],
+        type: typing.Union[MetaOapg.properties.type, str, ],
+        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
+        name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
+        provider: typing.Union[MetaOapg.properties.provider, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        max_tokens: typing.Union[MetaOapg.properties.max_tokens, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        temperature: typing.Union[MetaOapg.properties.temperature, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        top_p: typing.Union[MetaOapg.properties.top_p, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        presence_penalty: typing.Union[MetaOapg.properties.presence_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        frequency_penalty: typing.Union[MetaOapg.properties.frequency_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        prompt_template: typing.Union[MetaOapg.properties.prompt_template, str, schemas.Unset] = schemas.unset,
+        chat_template: typing.Union[MetaOapg.properties.chat_template, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> 'TraceLogRequest':
+    ) -> 'TraceModelConfigRequest':
         return super().__new__(
             cls,
             *args,
-            function_name=function_name,
-            trial_id=trial_id,
-            inputs=inputs,
-            messages=messages,
-            output=output,
-            source=source,
-            config=config,
-            metadata=metadata,
-            error=error,
-            duration=duration,
-            created_at=created_at,
-            children=children,
+            model=model,
+            type=type,
+            description=description,
+            name=name,
+            provider=provider,
+            max_tokens=max_tokens,
+            temperature=temperature,
+            top_p=top_p,
+            stop=stop,
+            presence_penalty=presence_penalty,
+            frequency_penalty=frequency_penalty,
+            other=other,
+            endpoint=endpoint,
+            prompt_template=prompt_template,
+            chat_template=chat_template,
             _configuration=_configuration,
         )
 
-from humanloop.model.agent_config_request import AgentConfigRequest
 from humanloop.model.chat_message import ChatMessage
-from humanloop.model.generic_config_request import GenericConfigRequest
-from humanloop.model.tool_config_request import ToolConfigRequest
-from humanloop.model.trace_model_config_request import TraceModelConfigRequest
+from humanloop.model.model_endpoints import ModelEndpoints
+from humanloop.model.model_providers import ModelProviders
```

### Comparing `humanloop-0.4.6/humanloop/model/trace_log_request.pyi` & `humanloop-0.4.7/humanloop/model/trace_model_config_request.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -19,263 +19,377 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class TraceLogRequest(
+class TraceModelConfigRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    Simplified version of LogRequest.
+    Model config request that supports both chat and completion.
 
-Changes:
-    - Renamed `project` to `function_name`. TODO: Allow either `function_name` or `function_id`.
+Implemented here with the full set of fields from both
+ChatModelConfigRequest and CompletionModelConfigRequest.
+
+Ideally we'd use `Union[ChatModelConfigRequest, CompletionModelConfigRequest]`
+but that seems to cause Pydantic errors, especially with the `type` discriminator.
+
+Validation is done to ensure that only one of `chat_template` and
+`prompt_template` is provided, and that the provided one properly
+corresponds to the endpoint.
+This defaults to `complete` endpoint.
     """
 
 
     class MetaOapg:
         required = {
-            "function_name",
+            "model",
+            "type",
         }
         
         class properties:
-            function_name = schemas.StrSchema
-            trial_id = schemas.StrSchema
-            inputs = schemas.DictSchema
+            model = schemas.StrSchema
             
             
-            class messages(
-                schemas.ListSchema
+            class type(
+                schemas.EnumBase,
+                schemas.StrSchema
+            ):
+                
+                @schemas.classproperty
+                def MODEL(cls):
+                    return cls("model")
+            description = schemas.StrSchema
+            name = schemas.StrSchema
+            
+            
+            class provider(
+                schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
-                    @staticmethod
-                    def items() -> typing.Type['ChatMessage']:
-                        return ChatMessage
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            ModelProviders,
+                        ]
+            
             
                 def __new__(
                     cls,
-                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
+                    *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'messages':
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'provider':
                     return super().__new__(
                         cls,
-                        arg,
+                        *args,
                         _configuration=_configuration,
+                        **kwargs,
                     )
+            max_tokens = schemas.IntSchema
+            temperature = schemas.NumberSchema
+            top_p = schemas.NumberSchema
             
-                def __getitem__(self, i: int) -> 'ChatMessage':
-                    return super().__getitem__(i)
-            output = schemas.StrSchema
-            source = schemas.StrSchema
             
+            class stop(
+                schemas.ComposedSchema,
+            ):
             
-            class config(
+            
+                class MetaOapg:
+                    any_of_0 = schemas.StrSchema
+                    
+                    
+                    class any_of_1(
+                        schemas.ListSchema
+                    ):
+                    
+                    
+                        class MetaOapg:
+                            items = schemas.StrSchema
+                    
+                        def __new__(
+                            cls,
+                            arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
+                            _configuration: typing.Optional[schemas.Configuration] = None,
+                        ) -> 'any_of_1':
+                            return super().__new__(
+                                cls,
+                                arg,
+                                _configuration=_configuration,
+                            )
+                    
+                        def __getitem__(self, i: int) -> MetaOapg.items:
+                            return super().__getitem__(i)
+                    
+                    @classmethod
+                    @functools.lru_cache()
+                    def any_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            cls.any_of_0,
+                            cls.any_of_1,
+                        ]
+            
+            
+                def __new__(
+                    cls,
+                    *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'stop':
+                    return super().__new__(
+                        cls,
+                        *args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
+            presence_penalty = schemas.NumberSchema
+            frequency_penalty = schemas.NumberSchema
+            other = schemas.DictSchema
+            
+            
+            class endpoint(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
                     @functools.lru_cache()
-                    def one_of(cls):
+                    def all_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            TraceModelConfigRequest,
-                            ToolConfigRequest,
-                            GenericConfigRequest,
-                            AgentConfigRequest,
+                            ModelEndpoints,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'config':
+                ) -> 'endpoint':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            metadata = schemas.DictSchema
-            error = schemas.StrSchema
-            duration = schemas.NumberSchema
-            created_at = schemas.DateTimeSchema
+            prompt_template = schemas.StrSchema
             
             
-            class children(
+            class chat_template(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['TraceLogRequest']:
-                        return TraceLogRequest
+                    def items() -> typing.Type['ChatMessage']:
+                        return ChatMessage
             
                 def __new__(
                     cls,
-                    arg: typing.Union[typing.Tuple['TraceLogRequest'], typing.List['TraceLogRequest']],
+                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'children':
+                ) -> 'chat_template':
                     return super().__new__(
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'TraceLogRequest':
+                def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
             __annotations__ = {
-                "function_name": function_name,
-                "trial_id": trial_id,
-                "inputs": inputs,
-                "messages": messages,
-                "output": output,
-                "source": source,
-                "config": config,
-                "metadata": metadata,
-                "error": error,
-                "duration": duration,
-                "created_at": created_at,
-                "children": children,
+                "model": model,
+                "type": type,
+                "description": description,
+                "name": name,
+                "provider": provider,
+                "max_tokens": max_tokens,
+                "temperature": temperature,
+                "top_p": top_p,
+                "stop": stop,
+                "presence_penalty": presence_penalty,
+                "frequency_penalty": frequency_penalty,
+                "other": other,
+                "endpoint": endpoint,
+                "prompt_template": prompt_template,
+                "chat_template": chat_template,
             }
         additional_properties = schemas.NotAnyTypeSchema
     
-    function_name: MetaOapg.properties.function_name
+    model: MetaOapg.properties.model
+    type: MetaOapg.properties.type
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["function_name"]) -> MetaOapg.properties.function_name: ...
+    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["trial_id"]) -> MetaOapg.properties.trial_id: ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
+    def __getitem__(self, name: typing_extensions.Literal["provider"]) -> MetaOapg.properties.provider: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
+    def __getitem__(self, name: typing_extensions.Literal["max_tokens"]) -> MetaOapg.properties.max_tokens: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+    def __getitem__(self, name: typing_extensions.Literal["temperature"]) -> MetaOapg.properties.temperature: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
+    def __getitem__(self, name: typing_extensions.Literal["top_p"]) -> MetaOapg.properties.top_p: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["config"]) -> MetaOapg.properties.config: ...
+    def __getitem__(self, name: typing_extensions.Literal["stop"]) -> MetaOapg.properties.stop: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
+    def __getitem__(self, name: typing_extensions.Literal["presence_penalty"]) -> MetaOapg.properties.presence_penalty: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["error"]) -> MetaOapg.properties.error: ...
+    def __getitem__(self, name: typing_extensions.Literal["frequency_penalty"]) -> MetaOapg.properties.frequency_penalty: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["duration"]) -> MetaOapg.properties.duration: ...
+    def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
+    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["children"]) -> MetaOapg.properties.children: ...
+    def __getitem__(self, name: typing_extensions.Literal["prompt_template"]) -> MetaOapg.properties.prompt_template: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["function_name"], typing_extensions.Literal["trial_id"], typing_extensions.Literal["inputs"], typing_extensions.Literal["messages"], typing_extensions.Literal["output"], typing_extensions.Literal["source"], typing_extensions.Literal["config"], typing_extensions.Literal["metadata"], typing_extensions.Literal["error"], typing_extensions.Literal["duration"], typing_extensions.Literal["created_at"], typing_extensions.Literal["children"], ]):
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["chat_template"]) -> MetaOapg.properties.chat_template: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model"], typing_extensions.Literal["type"], typing_extensions.Literal["description"], typing_extensions.Literal["name"], typing_extensions.Literal["provider"], typing_extensions.Literal["max_tokens"], typing_extensions.Literal["temperature"], typing_extensions.Literal["top_p"], typing_extensions.Literal["stop"], typing_extensions.Literal["presence_penalty"], typing_extensions.Literal["frequency_penalty"], typing_extensions.Literal["other"], typing_extensions.Literal["endpoint"], typing_extensions.Literal["prompt_template"], typing_extensions.Literal["chat_template"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["function_name"]) -> MetaOapg.properties.function_name: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["trial_id"]) -> typing.Union[MetaOapg.properties.trial_id, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["provider"]) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> typing.Union[MetaOapg.properties.inputs, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["max_tokens"]) -> typing.Union[MetaOapg.properties.max_tokens, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> typing.Union[MetaOapg.properties.messages, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["temperature"]) -> typing.Union[MetaOapg.properties.temperature, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> typing.Union[MetaOapg.properties.output, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["top_p"]) -> typing.Union[MetaOapg.properties.top_p, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["stop"]) -> typing.Union[MetaOapg.properties.stop, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["config"]) -> typing.Union[MetaOapg.properties.config, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["presence_penalty"]) -> typing.Union[MetaOapg.properties.presence_penalty, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["frequency_penalty"]) -> typing.Union[MetaOapg.properties.frequency_penalty, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["error"]) -> typing.Union[MetaOapg.properties.error, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["duration"]) -> typing.Union[MetaOapg.properties.duration, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> typing.Union[MetaOapg.properties.created_at, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["prompt_template"]) -> typing.Union[MetaOapg.properties.prompt_template, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["children"]) -> typing.Union[MetaOapg.properties.children, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["chat_template"]) -> typing.Union[MetaOapg.properties.chat_template, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["function_name"], typing_extensions.Literal["trial_id"], typing_extensions.Literal["inputs"], typing_extensions.Literal["messages"], typing_extensions.Literal["output"], typing_extensions.Literal["source"], typing_extensions.Literal["config"], typing_extensions.Literal["metadata"], typing_extensions.Literal["error"], typing_extensions.Literal["duration"], typing_extensions.Literal["created_at"], typing_extensions.Literal["children"], ]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model"], typing_extensions.Literal["type"], typing_extensions.Literal["description"], typing_extensions.Literal["name"], typing_extensions.Literal["provider"], typing_extensions.Literal["max_tokens"], typing_extensions.Literal["temperature"], typing_extensions.Literal["top_p"], typing_extensions.Literal["stop"], typing_extensions.Literal["presence_penalty"], typing_extensions.Literal["frequency_penalty"], typing_extensions.Literal["other"], typing_extensions.Literal["endpoint"], typing_extensions.Literal["prompt_template"], typing_extensions.Literal["chat_template"], ]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        function_name: typing.Union[MetaOapg.properties.function_name, str, ],
-        trial_id: typing.Union[MetaOapg.properties.trial_id, str, schemas.Unset] = schemas.unset,
-        inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
-        messages: typing.Union[MetaOapg.properties.messages, list, tuple, schemas.Unset] = schemas.unset,
-        output: typing.Union[MetaOapg.properties.output, str, schemas.Unset] = schemas.unset,
-        source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
-        config: typing.Union[MetaOapg.properties.config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
-        error: typing.Union[MetaOapg.properties.error, str, schemas.Unset] = schemas.unset,
-        duration: typing.Union[MetaOapg.properties.duration, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
-        created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, schemas.Unset] = schemas.unset,
-        children: typing.Union[MetaOapg.properties.children, list, tuple, schemas.Unset] = schemas.unset,
+        model: typing.Union[MetaOapg.properties.model, str, ],
+        type: typing.Union[MetaOapg.properties.type, str, ],
+        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
+        name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
+        provider: typing.Union[MetaOapg.properties.provider, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        max_tokens: typing.Union[MetaOapg.properties.max_tokens, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        temperature: typing.Union[MetaOapg.properties.temperature, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        top_p: typing.Union[MetaOapg.properties.top_p, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        presence_penalty: typing.Union[MetaOapg.properties.presence_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        frequency_penalty: typing.Union[MetaOapg.properties.frequency_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        prompt_template: typing.Union[MetaOapg.properties.prompt_template, str, schemas.Unset] = schemas.unset,
+        chat_template: typing.Union[MetaOapg.properties.chat_template, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> 'TraceLogRequest':
+    ) -> 'TraceModelConfigRequest':
         return super().__new__(
             cls,
             *args,
-            function_name=function_name,
-            trial_id=trial_id,
-            inputs=inputs,
-            messages=messages,
-            output=output,
-            source=source,
-            config=config,
-            metadata=metadata,
-            error=error,
-            duration=duration,
-            created_at=created_at,
-            children=children,
+            model=model,
+            type=type,
+            description=description,
+            name=name,
+            provider=provider,
+            max_tokens=max_tokens,
+            temperature=temperature,
+            top_p=top_p,
+            stop=stop,
+            presence_penalty=presence_penalty,
+            frequency_penalty=frequency_penalty,
+            other=other,
+            endpoint=endpoint,
+            prompt_template=prompt_template,
+            chat_template=chat_template,
             _configuration=_configuration,
         )
 
-from humanloop.model.agent_config_request import AgentConfigRequest
 from humanloop.model.chat_message import ChatMessage
-from humanloop.model.generic_config_request import GenericConfigRequest
-from humanloop.model.tool_config_request import ToolConfigRequest
-from humanloop.model.trace_model_config_request import TraceModelConfigRequest
+from humanloop.model.model_endpoints import ModelEndpoints
+from humanloop.model.model_providers import ModelProviders
```

### Comparing `humanloop-0.4.6/humanloop/model/update_experiment_request.py` & `humanloop-0.4.7/humanloop/model/update_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/update_experiment_request.pyi` & `humanloop-0.4.7/humanloop/model/update_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/update_log_request.py` & `humanloop-0.4.7/humanloop/model/update_log_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/update_log_request.pyi` & `humanloop-0.4.7/humanloop/model/update_log_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/usage.py` & `humanloop-0.4.7/humanloop/model/usage.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/usage.pyi` & `humanloop-0.4.7/humanloop/model/usage.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/validation_error.py` & `humanloop-0.4.7/humanloop/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/model/validation_error.pyi` & `humanloop-0.4.7/humanloop/model/validation_error.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/models/__init__.py` & `humanloop-0.4.7/humanloop/models/__init__.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/__init__.py` & `humanloop-0.4.7/humanloop/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/chat/post.py` & `humanloop-0.4.7/humanloop/paths/chat/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/chat/post.pyi` & `humanloop-0.4.7/humanloop/paths/chat/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/chat_deployed/post.py` & `humanloop-0.4.7/humanloop/paths/chat_deployed/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/chat_deployed/post.pyi` & `humanloop-0.4.7/humanloop/paths/chat_deployed/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/chat_experiment/post.py` & `humanloop-0.4.7/humanloop/paths/chat_experiment/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/chat_experiment/post.pyi` & `humanloop-0.4.7/humanloop/paths/chat_experiment/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/chat_model_config/post.py` & `humanloop-0.4.7/humanloop/paths/chat_model_config/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/chat_model_config/post.pyi` & `humanloop-0.4.7/humanloop/paths/chat_model_config/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/completion/post.py` & `humanloop-0.4.7/humanloop/paths/completion/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/completion/post.pyi` & `humanloop-0.4.7/humanloop/paths/completion/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/completion_deployed/post.py` & `humanloop-0.4.7/humanloop/paths/completion_deployed/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/completion_deployed/post.pyi` & `humanloop-0.4.7/humanloop/paths/completion_deployed/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/completion_experiment/post.py` & `humanloop-0.4.7/humanloop/paths/completion_experiment/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/completion_experiment/post.pyi` & `humanloop-0.4.7/humanloop/paths/completion_experiment/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/completion_model_config/post.py` & `humanloop-0.4.7/humanloop/paths/completion_model_config/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/completion_model_config/post.pyi` & `humanloop-0.4.7/humanloop/paths/completion_model_config/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/experiments_experiment_id/delete.py` & `humanloop-0.4.7/humanloop/paths/experiments_experiment_id/delete.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/experiments_experiment_id/delete.pyi` & `humanloop-0.4.7/humanloop/paths/experiments_experiment_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/experiments_experiment_id/patch.py` & `humanloop-0.4.7/humanloop/paths/experiments_experiment_id/patch.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/experiments_experiment_id/patch.pyi` & `humanloop-0.4.7/humanloop/paths/experiments_experiment_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/experiments_experiment_id_model_config/get.py` & `humanloop-0.4.7/humanloop/paths/experiments_experiment_id_model_config/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/experiments_experiment_id_model_config/get.pyi` & `humanloop-0.4.7/humanloop/paths/experiments_experiment_id_model_config/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/feedback/post.py` & `humanloop-0.4.7/humanloop/paths/feedback/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/feedback/post.pyi` & `humanloop-0.4.7/humanloop/paths/feedback/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/logs/patch.py` & `humanloop-0.4.7/humanloop/paths/logs/patch.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/logs/patch.pyi` & `humanloop-0.4.7/humanloop/paths/logs/patch.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/logs/post.py` & `humanloop-0.4.7/humanloop/paths/logs/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/logs/post.pyi` & `humanloop-0.4.7/humanloop/paths/logs/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/logs_id/patch.py` & `humanloop-0.4.7/humanloop/paths/logs_id/patch.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/logs_id/patch.pyi` & `humanloop-0.4.7/humanloop/paths/logs_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/model_configs/post.py` & `humanloop-0.4.7/humanloop/paths/model_configs/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/model_configs/post.pyi` & `humanloop-0.4.7/humanloop/paths/model_configs/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/model_configs_id/get.py` & `humanloop-0.4.7/humanloop/paths/model_configs_id/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/model_configs_id/get.pyi` & `humanloop-0.4.7/humanloop/paths/model_configs_id/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects/get.py` & `humanloop-0.4.7/humanloop/paths/projects/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects/get.pyi` & `humanloop-0.4.7/humanloop/paths/projects/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects/post.py` & `humanloop-0.4.7/humanloop/paths/projects/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects/post.pyi` & `humanloop-0.4.7/humanloop/paths/projects/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_id/get.py` & `humanloop-0.4.7/humanloop/paths/projects_id/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_id/get.pyi` & `humanloop-0.4.7/humanloop/paths/projects_id/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_id/patch.py` & `humanloop-0.4.7/humanloop/paths/projects_id/patch.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_id/patch.pyi` & `humanloop-0.4.7/humanloop/paths/projects_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_id_active_config/delete.py` & `humanloop-0.4.7/humanloop/paths/projects_id_active_config/delete.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_id_active_config/delete.pyi` & `humanloop-0.4.7/humanloop/paths/projects_id_active_config/delete.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_id_active_config/get.py` & `humanloop-0.4.7/humanloop/paths/projects_id_active_config/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_id_active_config/get.pyi` & `humanloop-0.4.7/humanloop/paths/projects_id_active_config/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_id_active_experiment/delete.py` & `humanloop-0.4.7/humanloop/paths/projects_id_active_experiment/delete.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_id_active_experiment/delete.pyi` & `humanloop-0.4.7/humanloop/paths/projects_id_active_experiment/delete.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_id_configs/get.py` & `humanloop-0.4.7/humanloop/paths/projects_id_configs/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_id_configs/get.pyi` & `humanloop-0.4.7/humanloop/paths/projects_id_configs/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_id_export/post.py` & `humanloop-0.4.7/humanloop/paths/projects_id_export/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_id_export/post.pyi` & `humanloop-0.4.7/humanloop/paths/projects_id_export/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_id_feedback_types/patch.py` & `humanloop-0.4.7/humanloop/paths/projects_id_feedback_types/patch.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_id_feedback_types/patch.pyi` & `humanloop-0.4.7/humanloop/paths/projects_id_feedback_types/patch.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_project_id_experiments/get.py` & `humanloop-0.4.7/humanloop/paths/projects_project_id_experiments/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_project_id_experiments/get.pyi` & `humanloop-0.4.7/humanloop/paths/projects_project_id_experiments/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_project_id_experiments/post.py` & `humanloop-0.4.7/humanloop/paths/projects_project_id_experiments/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/projects_project_id_experiments/post.pyi` & `humanloop-0.4.7/humanloop/paths/projects_project_id_experiments/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/sessions/get.py` & `humanloop-0.4.7/humanloop/paths/sessions/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/sessions/get.pyi` & `humanloop-0.4.7/humanloop/paths/sessions/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/sessions/post.py` & `humanloop-0.4.7/humanloop/paths/sessions/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/sessions/post.pyi` & `humanloop-0.4.7/humanloop/paths/sessions/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/sessions_id/get.py` & `humanloop-0.4.7/humanloop/paths/sessions_id/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/sessions_id/get.pyi` & `humanloop-0.4.7/humanloop/paths/sessions_id/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/traces/post.py` & `humanloop-0.4.7/humanloop/paths/traces/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/paths/traces/post.pyi` & `humanloop-0.4.7/humanloop/paths/traces/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/request_after_hook.py` & `humanloop-0.4.7/humanloop/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/request_before_hook.py` & `humanloop-0.4.7/humanloop/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/rest.py` & `humanloop-0.4.7/humanloop/rest.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/schemas.py` & `humanloop-0.4.7/humanloop/schemas.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/agent_config_request.py` & `humanloop-0.4.7/humanloop/type/agent_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/agent_config_response.py` & `humanloop-0.4.7/humanloop/type/agent_config_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,24 +10,22 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
-from humanloop.type.config_type import ConfigType
 from humanloop.type.log_model_config_request import LogModelConfigRequest
 from humanloop.type.tool_config_request import ToolConfigRequest
 
 class RequiredAgentConfigResponse(TypedDict):
     # String ID of config. Starts with `config_`.
     id: str
 
-    # Type of config.
-    type: ConfigType
+    type: str
 
     # Name of config.
     name: str
 
     # Class of the agent.
     agent_class: str
```

### Comparing `humanloop-0.4.6/humanloop/type/base_metric_response.py` & `humanloop-0.4.7/humanloop/type/base_metric_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/categorical_feedback_label.py` & `humanloop-0.4.7/humanloop/type/categorical_feedback_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/chat_data_response.py` & `humanloop-0.4.7/humanloop/type/chat_data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/chat_deployed_request.py` & `humanloop-0.4.7/humanloop/type/chat_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/chat_experiment_request.py` & `humanloop-0.4.7/humanloop/type/chat_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/chat_message.py` & `humanloop-0.4.7/humanloop/type/chat_message.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/chat_model_config_request.py` & `humanloop-0.4.7/humanloop/type/chat_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/chat_request.py` & `humanloop-0.4.7/humanloop/type/chat_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/chat_response.py` & `humanloop-0.4.7/humanloop/type/chat_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/chat_role.py` & `humanloop-0.4.7/humanloop/type/chat_role.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/completion_deployed_request.py` & `humanloop-0.4.7/humanloop/type/completion_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/completion_experiment_request.py` & `humanloop-0.4.7/humanloop/type/completion_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/completion_model_config_request.py` & `humanloop-0.4.7/humanloop/type/completion_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/completion_request.py` & `humanloop-0.4.7/humanloop/type/completion_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/completion_response.py` & `humanloop-0.4.7/humanloop/type/completion_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/config_response.py` & `humanloop-0.4.7/humanloop/type/config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/config_type.py` & `humanloop-0.4.7/humanloop/type/config_type.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/create_experiment_request.py` & `humanloop-0.4.7/humanloop/type/create_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/create_log_response.py` & `humanloop-0.4.7/humanloop/type/create_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/create_project_request.py` & `humanloop-0.4.7/humanloop/type/create_project_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/create_session_response.py` & `humanloop-0.4.7/humanloop/type/create_session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/create_trace_request.py` & `humanloop-0.4.7/humanloop/type/create_trace_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/create_trace_response.py` & `humanloop-0.4.7/humanloop/type/create_trace_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/data_response.py` & `humanloop-0.4.7/humanloop/type/data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/experiment_config_response.py` & `humanloop-0.4.7/humanloop/type/experiment_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/experiment_response.py` & `humanloop-0.4.7/humanloop/type/experiment_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/experiment_status.py` & `humanloop-0.4.7/humanloop/type/experiment_status.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/experiments_list_response.py` & `humanloop-0.4.7/humanloop/type/experiments_list_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/feedback.py` & `humanloop-0.4.7/humanloop/type/feedback.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/feedback_class.py` & `humanloop-0.4.7/humanloop/type/feedback_class.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/feedback_label_request.py` & `humanloop-0.4.7/humanloop/type/feedback_label_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/feedback_request.py` & `humanloop-0.4.7/humanloop/type/feedback_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/feedback_response.py` & `humanloop-0.4.7/humanloop/type/feedback_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/feedback_submit_request.py` & `humanloop-0.4.7/humanloop/type/feedback_submit_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/feedback_submit_response.py` & `humanloop-0.4.7/humanloop/type/feedback_submit_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/feedback_type.py` & `humanloop-0.4.7/humanloop/type/feedback_type.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/feedback_type_model.py` & `humanloop-0.4.7/humanloop/type/feedback_type_model.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/feedback_type_request.py` & `humanloop-0.4.7/humanloop/type/feedback_type_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/feedback_types.py` & `humanloop-0.4.7/humanloop/type/feedback_types.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/generic_config_request.py` & `humanloop-0.4.7/humanloop/type/generic_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/generic_config_response.py` & `humanloop-0.4.7/humanloop/type/generic_config_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,22 +10,20 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
-from humanloop.type.config_type import ConfigType
 
 class RequiredGenericConfigResponse(TypedDict):
     # String ID of config. Starts with `config_`.
     id: str
 
-    # Type of config.
-    type: ConfigType
+    type: str
 
     # Name of config.
     name: str
 
 class OptionalGenericConfigResponse(TypedDict, total=False):
     # Description of config.
     description: str
```

### Comparing `humanloop-0.4.6/humanloop/type/get_model_config_response.py` & `humanloop-0.4.7/humanloop/type/get_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/http_validation_error.py` & `humanloop-0.4.7/humanloop/type/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/label_sentiment.py` & `humanloop-0.4.7/humanloop/type/label_sentiment.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/log_datapoint_request.py` & `humanloop-0.4.7/humanloop/type/log_datapoint_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/log_model_config_request.py` & `humanloop-0.4.7/humanloop/type/log_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/log_request.py` & `humanloop-0.4.7/humanloop/type/log_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/log_response.py` & `humanloop-0.4.7/humanloop/type/log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/logs_log_response.py` & `humanloop-0.4.7/humanloop/type/logs_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/model_config_chat_request.py` & `humanloop-0.4.7/humanloop/type/model_config_chat_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/model_config_completion_request.py` & `humanloop-0.4.7/humanloop/type/model_config_completion_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/model_endpoints.py` & `humanloop-0.4.7/humanloop/type/model_endpoints.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/model_providers.py` & `humanloop-0.4.7/humanloop/type/model_providers.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/paginated_data_log_response.py` & `humanloop-0.4.7/humanloop/type/paginated_data_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/paginated_data_project_response.py` & `humanloop-0.4.7/humanloop/type/paginated_data_project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/paginated_data_session_response.py` & `humanloop-0.4.7/humanloop/type/paginated_data_session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/positive_label.py` & `humanloop-0.4.7/humanloop/type/positive_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/project_config_response.py` & `humanloop-0.4.7/humanloop/type/project_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/project_model_config_request.py` & `humanloop-0.4.7/humanloop/type/project_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/project_model_config_response.py` & `humanloop-0.4.7/humanloop/type/project_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/project_response.py` & `humanloop-0.4.7/humanloop/type/project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/project_sort_by.py` & `humanloop-0.4.7/humanloop/type/project_sort_by.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/project_user_response.py` & `humanloop-0.4.7/humanloop/type/project_user_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/projects_get_configs_response.py` & `humanloop-0.4.7/humanloop/type/projects_get_configs_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/projects_update_feedback_types_request.py` & `humanloop-0.4.7/humanloop/type/projects_update_feedback_types_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/provider_api_keys.py` & `humanloop-0.4.7/humanloop/type/provider_api_keys.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/session_project_response.py` & `humanloop-0.4.7/humanloop/type/session_project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/session_response.py` & `humanloop-0.4.7/humanloop/type/session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/sort_order.py` & `humanloop-0.4.7/humanloop/type/sort_order.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/src_external_app_models_v3_model_configs_model_config_response.py` & `humanloop-0.4.7/humanloop/type/src_external_app_models_v3_model_configs_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.7/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/src_external_app_models_v4_configs_model_config_response.py` & `humanloop-0.4.7/humanloop/type/src_external_app_models_v4_configs_model_config_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,24 +11,22 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.chat_message import ChatMessage
-from humanloop.type.config_type import ConfigType
 from humanloop.type.model_endpoints import ModelEndpoints
 from humanloop.type.model_providers import ModelProviders
 
 class RequiredSrcExternalAppModelsV4ConfigsModelConfigResponse(TypedDict):
     # String ID of config. Starts with `config_`.
     id: str
 
-    # Type of config.
-    type: ConfigType
+    type: str
 
     # Name of config.
     name: str
 
     # The model instance used. E.g. text-davinci-002.
     model: str
```

### Comparing `humanloop-0.4.6/humanloop/type/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.7/humanloop/type/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/tool_config_request.py` & `humanloop-0.4.7/humanloop/type/tool_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/tool_config_response.py` & `humanloop-0.4.7/humanloop/type/tool_config_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,22 +10,20 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
-from humanloop.type.config_type import ConfigType
 
 class RequiredToolConfigResponse(TypedDict):
     # String ID of config. Starts with `config_`.
     id: str
 
-    # Type of config.
-    type: ConfigType
+    type: str
 
     # Name of config.
     name: str
 
 class OptionalToolConfigResponse(TypedDict, total=False):
     # Description of config.
     description: str
```

### Comparing `humanloop-0.4.6/humanloop/type/tool_result_response.py` & `humanloop-0.4.7/humanloop/type/tool_result_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/trace_log_request.py` & `humanloop-0.4.7/humanloop/type/trace_log_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/trace_model_config_request.py` & `humanloop-0.4.7/humanloop/type/trace_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/update_experiment_request.py` & `humanloop-0.4.7/humanloop/type/update_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/update_log_request.py` & `humanloop-0.4.7/humanloop/type/update_log_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/update_project_request.py` & `humanloop-0.4.7/humanloop/type/update_project_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/usage.py` & `humanloop-0.4.7/humanloop/type/usage.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type/validation_error.py` & `humanloop-0.4.7/humanloop/type/validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/type_util.py` & `humanloop-0.4.7/humanloop/type_util.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/humanloop/validation_metadata.py` & `humanloop-0.4.7/humanloop/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.6/pyproject.toml` & `humanloop-0.4.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "humanloop"
-version = "0.4.6"
+version = "0.4.7"
 description = "Client for Humanloop API"
 authors = ["Konfig <engineering@konfigthis.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "humanloop"}]
 
 [tool.poetry.dependencies]
```

### Comparing `humanloop-0.4.6/PKG-INFO` & `humanloop-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humanloop
-Version: 0.4.6
+Version: 0.4.7
 Summary: Client for Humanloop API
 License: MIT
 Author: Konfig
 Author-email: engineering@konfigthis.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,25 +18,25 @@
 Requires-Dist: frozendict (>=2.3.4,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.7,<2.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
-# humanloop@0.4.6
+# humanloop@0.4.7
 
 
 ## Requirements
 
 Python >=3.7
 
 ## Installing
 
 ```sh
-pip install humanloop==0.4.6
+pip install humanloop==0.4.7
 ```
 
 ## Getting Started
 
 ```python
 from pprint import pprint
 from humanloop import Humanloop, ApiException
```

