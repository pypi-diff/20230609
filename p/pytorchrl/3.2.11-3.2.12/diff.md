# Comparing `tmp/pytorchrl-3.2.11.tar.gz` & `tmp/pytorchrl-3.2.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorchrl-3.2.11.tar", last modified: Thu Apr  6 10:22:24 2023, max compression
+gzip compressed data, was "pytorchrl-3.2.12.tar", last modified: Fri Jun  9 11:41:53 2023, max compression
```

## Comparing `pytorchrl-3.2.11.tar` & `pytorchrl-3.2.12.tar`

### file list

```diff
@@ -1,212 +1,212 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.763457 pytorchrl-3.2.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-06 10:22:07.000000 pytorchrl-3.2.11/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-06 10:22:07.000000 pytorchrl-3.2.11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-06 10:22:24.763457 pytorchrl-3.2.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-06 10:22:07.000000 pytorchrl-3.2.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.735458 pytorchrl-3.2.11/pytorchrl/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.735458 pytorchrl-3.2.11/pytorchrl/agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.735458 pytorchrl-3.2.11/pytorchrl/agent/actors/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.735458 pytorchrl-3.2.11/pytorchrl/agent/actors/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/distributions/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/distributions/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/distributions/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/distributions/squashed_gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.739457 pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/dictnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/ensemble_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/fixup_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.739457 pytorchrl-3.2.11/pytorchrl/agent/actors/memory_networks/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/memory_networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/memory_networks/gru_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    15468 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/memory_networks/lstm_encoder_decoder_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/memory_networks/lstm_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/model_based_planner_actor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.739457 pytorchrl-3.2.11/pytorchrl/agent/actors/noise/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/noise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/noise/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/noise/nonoise.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/noise/ou.py
--rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/off_policy_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18095 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/on_policy_actor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.739457 pytorchrl-3.2.11/pytorchrl/agent/actors/reward_functions/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/reward_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/reward_functions/gym_reward_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/reward_functions/pybullet_reward_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.739457 pytorchrl-3.2.11/pytorchrl/agent/actors/world_models/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/world_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/world_models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/actors/world_models/world_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.739457 pytorchrl-3.2.11/pytorchrl/agent/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.739457 pytorchrl-3.2.11/pytorchrl/agent/algorithms/model_based/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/model_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17244 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/model_based/mpc_cem.py
--rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/model_based/mpc_pddm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/model_based/mpc_rs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.743457 pytorchrl-3.2.11/pytorchrl/agent/algorithms/off_policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/off_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/off_policy/ddpg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/off_policy/ddqn.py
--rw-r--r--   0 runner    (1001) docker     (123)    32877 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/off_policy/mpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    24981 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/off_policy/sac.py
--rw-r--r--   0 runner    (1001) docker     (123)    20412 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/off_policy/td3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.743457 pytorchrl-3.2.11/pytorchrl/agent/algorithms/on_policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/on_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/on_policy/a2c.py
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/on_policy/ppo.py
--rw-r--r--   0 runner    (1001) docker     (123)    24792 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/on_policy/rnd_ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.743457 pytorchrl-3.2.11/pytorchrl/agent/algorithms/policy_loss_addons/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/policy_loss_addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/policy_loss_addons/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/policy_loss_addons/kv_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/policy_loss_addons/return_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/policy_loss_addons/reward_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/algorithms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.743457 pytorchrl-3.2.11/pytorchrl/agent/env/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/env/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.743457 pytorchrl-3.2.11/pytorchrl/agent/env/base_envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/env/base_envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/env/base_envs/batched_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/env/base_envs/env_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.747457 pytorchrl-3.2.11/pytorchrl/agent/env/vec_envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/env/vec_envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/env/vec_envs/parallel_vec_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/env/vec_envs/sequential_vec_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/env/vec_envs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/env/vec_envs/vec_env_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/env/vec_envs/vec_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/env/vec_envs/vector_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.747457 pytorchrl-3.2.11/pytorchrl/agent/storages/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/storages/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.747457 pytorchrl-3.2.11/pytorchrl/agent/storages/model_based/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/storages/model_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/storages/model_based/mb_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.747457 pytorchrl-3.2.11/pytorchrl/agent/storages/off_policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/storages/off_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/storages/off_policy/ere_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/storages/off_policy/her_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/storages/off_policy/nstep_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/storages/off_policy/per_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/storages/off_policy/replay_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.747457 pytorchrl-3.2.11/pytorchrl/agent/storages/on_policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/storages/on_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/storages/on_policy/gae_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    36542 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/storages/on_policy/ppod2_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19127 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/storages/on_policy/ppod2rebel_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28310 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/storages/on_policy/ppod_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16763 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/storages/on_policy/vanilla_on_policy_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/agent/storages/on_policy/vtrace_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.747457 pytorchrl-3.2.11/pytorchrl/envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.751457 pytorchrl-3.2.11/pytorchrl/envs/animal_olympics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/animal_olympics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/animal_olympics/animal_olympics_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/animal_olympics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/animal_olympics/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.751457 pytorchrl-3.2.11/pytorchrl/envs/atari/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/atari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/atari/atari_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/atari/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/atari/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.751457 pytorchrl-3.2.11/pytorchrl/envs/causal_world/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/causal_world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/causal_world/causal_world_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.751457 pytorchrl-3.2.11/pytorchrl/envs/crafter/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/crafter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/crafter/crafter_env_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.751457 pytorchrl-3.2.11/pytorchrl/envs/dm_control/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/dm_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/dm_control/dmcontrol_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/dm_control/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.751457 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.751457 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/diversity_filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/diversity_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/diversity_filter/base_diversity_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/diversity_filter/diversity_filter_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/diversity_filter/no_filter_with_penalty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.755457 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/libinvent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/libinvent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/libinvent/batched_rnn_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/libinvent/generative_chemistry_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/libinvent/rnn_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/libinvent/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.755457 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/reinvent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/reinvent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/reinvent/generative_chemistry_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/reinvent/rnn_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/reinvent/transformer_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.755457 pytorchrl-3.2.11/pytorchrl/envs/habitat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/habitat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/habitat/habitat_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/habitat/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/habitat/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.755457 pytorchrl-3.2.11/pytorchrl/envs/minigrid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/minigrid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.759457 pytorchrl-3.2.11/pytorchrl/envs/minigrid/custom_environments/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/minigrid/custom_environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/minigrid/custom_environments/deceiving_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/minigrid/custom_environments/multiple_deceiving_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/minigrid/minigrid_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/minigrid/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.759457 pytorchrl-3.2.11/pytorchrl/envs/mujoco/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/mujoco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/mujoco/mujoco_env_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.759457 pytorchrl-3.2.11/pytorchrl/envs/obstacle_tower/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/obstacle_tower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/obstacle_tower/obstacle_tower_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/obstacle_tower/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/obstacle_tower/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.759457 pytorchrl-3.2.11/pytorchrl/envs/pybullet/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/pybullet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/pybullet/pybullet_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/envs/pybullet/sparse_reacher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.759457 pytorchrl-3.2.11/pytorchrl/scheme/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/scheme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.763457 pytorchrl-3.2.11/pytorchrl/scheme/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/scheme/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/scheme/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/scheme/base/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/scheme/base/worker_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.763457 pytorchrl-3.2.11/pytorchrl/scheme/collection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/scheme/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/scheme/collection/c_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/scheme/collection/c_worker_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.763457 pytorchrl-3.2.11/pytorchrl/scheme/gradients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/scheme/gradients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20972 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/scheme/gradients/g_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/scheme/gradients/g_worker_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/scheme/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.763457 pytorchrl-3.2.11/pytorchrl/scheme/updates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/scheme/updates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14506 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/scheme/updates/u_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/scheme/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/pytorchrl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:22:24.735458 pytorchrl-3.2.11/pytorchrl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-06 10:22:24.000000 pytorchrl-3.2.11/pytorchrl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-04-06 10:22:24.000000 pytorchrl-3.2.11/pytorchrl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 10:22:24.000000 pytorchrl-3.2.11/pytorchrl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-06 10:22:24.000000 pytorchrl-3.2.11/pytorchrl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-06 10:22:24.000000 pytorchrl-3.2.11/pytorchrl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 10:22:24.763457 pytorchrl-3.2.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-06 10:22:08.000000 pytorchrl-3.2.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.101385 pytorchrl-3.2.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-09 11:41:40.000000 pytorchrl-3.2.12/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-09 11:41:40.000000 pytorchrl-3.2.12/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-09 11:41:53.101385 pytorchrl-3.2.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-09 11:41:40.000000 pytorchrl-3.2.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.085384 pytorchrl-3.2.12/pytorchrl/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.085384 pytorchrl-3.2.12/pytorchrl/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.089385 pytorchrl-3.2.12/pytorchrl/agent/actors/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.089385 pytorchrl-3.2.12/pytorchrl/agent/actors/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/distributions/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/distributions/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/distributions/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/distributions/squashed_gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.089385 pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/dictnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/ensemble_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/fixup_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.089385 pytorchrl-3.2.12/pytorchrl/agent/actors/memory_networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/memory_networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/memory_networks/gru_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15468 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/memory_networks/lstm_encoder_decoder_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/memory_networks/lstm_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/model_based_planner_actor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.089385 pytorchrl-3.2.12/pytorchrl/agent/actors/noise/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/noise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/noise/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/noise/nonoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/noise/ou.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/off_policy_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18095 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/on_policy_actor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.089385 pytorchrl-3.2.12/pytorchrl/agent/actors/reward_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/reward_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/reward_functions/gym_reward_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/reward_functions/pybullet_reward_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.089385 pytorchrl-3.2.12/pytorchrl/agent/actors/world_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/world_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/world_models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/actors/world_models/world_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.089385 pytorchrl-3.2.12/pytorchrl/agent/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.093385 pytorchrl-3.2.12/pytorchrl/agent/algorithms/model_based/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/model_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17244 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/model_based/mpc_cem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/model_based/mpc_pddm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/model_based/mpc_rs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.093385 pytorchrl-3.2.12/pytorchrl/agent/algorithms/off_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/off_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/off_policy/ddpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/off_policy/ddqn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32877 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/off_policy/mpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24981 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/off_policy/sac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20412 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/off_policy/td3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.093385 pytorchrl-3.2.12/pytorchrl/agent/algorithms/on_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/on_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/on_policy/a2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/on_policy/ppo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24792 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/on_policy/rnd_ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.093385 pytorchrl-3.2.12/pytorchrl/agent/algorithms/policy_loss_addons/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/policy_loss_addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/policy_loss_addons/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/policy_loss_addons/kv_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/policy_loss_addons/return_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/policy_loss_addons/reward_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/algorithms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.093385 pytorchrl-3.2.12/pytorchrl/agent/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/env/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.093385 pytorchrl-3.2.12/pytorchrl/agent/env/base_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/env/base_envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/env/base_envs/batched_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/env/base_envs/env_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.093385 pytorchrl-3.2.12/pytorchrl/agent/env/vec_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/env/vec_envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/env/vec_envs/parallel_vec_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/env/vec_envs/sequential_vec_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/env/vec_envs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/env/vec_envs/vec_env_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/env/vec_envs/vec_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/env/vec_envs/vector_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.093385 pytorchrl-3.2.12/pytorchrl/agent/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/storages/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.093385 pytorchrl-3.2.12/pytorchrl/agent/storages/model_based/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/storages/model_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/storages/model_based/mb_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.093385 pytorchrl-3.2.12/pytorchrl/agent/storages/off_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/storages/off_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/storages/off_policy/ere_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/storages/off_policy/her_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/storages/off_policy/nstep_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/storages/off_policy/per_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/storages/off_policy/replay_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.097385 pytorchrl-3.2.12/pytorchrl/agent/storages/on_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/storages/on_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/storages/on_policy/gae_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36542 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/storages/on_policy/ppod2_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19127 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/storages/on_policy/ppod2rebel_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28310 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/storages/on_policy/ppod_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16763 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/storages/on_policy/vanilla_on_policy_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/agent/storages/on_policy/vtrace_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.097385 pytorchrl-3.2.12/pytorchrl/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.097385 pytorchrl-3.2.12/pytorchrl/envs/animal_olympics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/animal_olympics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/animal_olympics/animal_olympics_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/animal_olympics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/animal_olympics/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.097385 pytorchrl-3.2.12/pytorchrl/envs/atari/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/atari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/atari/atari_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/atari/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/atari/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.097385 pytorchrl-3.2.12/pytorchrl/envs/causal_world/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/causal_world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/causal_world/causal_world_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.097385 pytorchrl-3.2.12/pytorchrl/envs/crafter/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/crafter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/crafter/crafter_env_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.097385 pytorchrl-3.2.12/pytorchrl/envs/dm_control/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/dm_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/dm_control/dmcontrol_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/dm_control/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.097385 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.097385 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/diversity_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/diversity_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/diversity_filter/base_diversity_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/diversity_filter/diversity_filter_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/diversity_filter/no_filter_with_penalty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.097385 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/libinvent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/libinvent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/libinvent/batched_rnn_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/libinvent/generative_chemistry_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/libinvent/rnn_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/libinvent/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.097385 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/reinvent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/reinvent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/reinvent/generative_chemistry_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/reinvent/rnn_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/reinvent/transformer_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.097385 pytorchrl-3.2.12/pytorchrl/envs/habitat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/habitat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/habitat/habitat_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/habitat/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/habitat/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.101385 pytorchrl-3.2.12/pytorchrl/envs/minigrid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/minigrid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.101385 pytorchrl-3.2.12/pytorchrl/envs/minigrid/custom_environments/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/minigrid/custom_environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/minigrid/custom_environments/deceiving_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/minigrid/custom_environments/multiple_deceiving_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/minigrid/minigrid_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/minigrid/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.101385 pytorchrl-3.2.12/pytorchrl/envs/mujoco/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/mujoco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/mujoco/mujoco_env_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.101385 pytorchrl-3.2.12/pytorchrl/envs/obstacle_tower/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/obstacle_tower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/obstacle_tower/obstacle_tower_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/obstacle_tower/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/obstacle_tower/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.101385 pytorchrl-3.2.12/pytorchrl/envs/pybullet/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/pybullet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/pybullet/pybullet_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/envs/pybullet/sparse_reacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.101385 pytorchrl-3.2.12/pytorchrl/scheme/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/scheme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.101385 pytorchrl-3.2.12/pytorchrl/scheme/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/scheme/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/scheme/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/scheme/base/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/scheme/base/worker_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.101385 pytorchrl-3.2.12/pytorchrl/scheme/collection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/scheme/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/scheme/collection/c_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/scheme/collection/c_worker_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.101385 pytorchrl-3.2.12/pytorchrl/scheme/gradients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/scheme/gradients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21056 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/scheme/gradients/g_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/scheme/gradients/g_worker_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/scheme/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.101385 pytorchrl-3.2.12/pytorchrl/scheme/updates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/scheme/updates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/scheme/updates/u_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/scheme/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/pytorchrl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:41:53.085384 pytorchrl-3.2.12/pytorchrl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-09 11:41:53.000000 pytorchrl-3.2.12/pytorchrl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-09 11:41:53.000000 pytorchrl-3.2.12/pytorchrl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:41:53.000000 pytorchrl-3.2.12/pytorchrl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-09 11:41:53.000000 pytorchrl-3.2.12/pytorchrl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-09 11:41:53.000000 pytorchrl-3.2.12/pytorchrl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 11:41:53.101385 pytorchrl-3.2.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-09 11:41:41.000000 pytorchrl-3.2.12/setup.py
```

### Comparing `pytorchrl-3.2.11/LICENCE` & `pytorchrl-3.2.12/LICENCE`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/PKG-INFO` & `pytorchrl-3.2.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: pytorchrl
-Version: 3.2.11
+Version: 3.2.12
 Summary: Disributed RL implementations with ray and pytorch.
 Home-page: https://github.com/PyTorchRL/pytorchrl/
 Author: albertbou92
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 ## PyTorchRL: A PyTorch library for reinforcement learning
 
-Deep Reinforcement learning (DRL) has been very successful in recent years but current methods still require vast amounts of data to solve non-trivial environments.  Scaling to solve more complex tasks requires frameworks that are flexible enough to allow prototyping and testing of new ideas, yet avoiding the impractically slow experimental turnaround times associated to single-threaded implementations.  PyTorchRL is a pytorch-based library for DRL that allows to easily assemble RL agents using a set of core reusable and easily extendable sub-modules as building blocks.  To reduce training times, PyTorchRL allows scaling agents with a parameterizable component called Scheme, that permits to define distributed architectures with great flexibility by specifying which operations should be decoupled, which should be parallelized, and how parallel tasks should be synchronized.
+Deep Reinforcement learning (DRL) has been very successful in recent years but current methods still require vast amounts of data to solve non-trivial environments. Scaling to solve more complex tasks requires frameworks that are flexible enough to allow prototyping and testing of new ideas, yet avoiding the impractically slow experimental turnaround times associated to single-threaded implementations. PyTorchRL is a pytorch-based library for DRL that allows to easily assemble RL agents using a set of core reusable and easily extendable sub-modules as building blocks. To reduce training times, PyTorchRL allows scaling agents with a parameterizable component called Scheme, that permits to define distributed architectures with great flexibility by specifying which operations should be decoupled, which should be parallelized, and how parallel tasks should be synchronized.
 
 ### Installation
 
 ```
     conda create -y -n pytorchrl
     conda activate pytorchrl
 
     conda install pytorch torchvision cudatoolkit -c pytorch
-    
-    pip install pytorchrl
+
+    pip install pytorchrl gym[atari,accept-rom-license]==0.19.0 wandb opencv-python hydra-core
 ```
 
 ### Documentation
 
 PyTorchRL documentation can be found [here](https://pytorchrl.readthedocs.io/en/latest/).
 
 ### Citing PyTorchRL
+
 Here is the [paper](https://arxiv.org/abs/2007.02622)
 
 ```
 @misc{bou2021pytorchrl,
-      title={PyTorchRL: Modular and Distributed Reinforcement Learning in PyTorch}, 
+      title={PyTorchRL: Modular and Distributed Reinforcement Learning in PyTorch},
       author={Albert Bou and Gianni De Fabritiis},
       year={2021},
       eprint={2007.02622},
       archivePrefix={arXiv},
       primaryClass={cs.CV}
 }
 ```
```

### Comparing `pytorchrl-3.2.11/README.md` & `pytorchrl-3.2.12/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 ## PyTorchRL: A PyTorch library for reinforcement learning
 
-Deep Reinforcement learning (DRL) has been very successful in recent years but current methods still require vast amounts of data to solve non-trivial environments.  Scaling to solve more complex tasks requires frameworks that are flexible enough to allow prototyping and testing of new ideas, yet avoiding the impractically slow experimental turnaround times associated to single-threaded implementations.  PyTorchRL is a pytorch-based library for DRL that allows to easily assemble RL agents using a set of core reusable and easily extendable sub-modules as building blocks.  To reduce training times, PyTorchRL allows scaling agents with a parameterizable component called Scheme, that permits to define distributed architectures with great flexibility by specifying which operations should be decoupled, which should be parallelized, and how parallel tasks should be synchronized.
+Deep Reinforcement learning (DRL) has been very successful in recent years but current methods still require vast amounts of data to solve non-trivial environments. Scaling to solve more complex tasks requires frameworks that are flexible enough to allow prototyping and testing of new ideas, yet avoiding the impractically slow experimental turnaround times associated to single-threaded implementations. PyTorchRL is a pytorch-based library for DRL that allows to easily assemble RL agents using a set of core reusable and easily extendable sub-modules as building blocks. To reduce training times, PyTorchRL allows scaling agents with a parameterizable component called Scheme, that permits to define distributed architectures with great flexibility by specifying which operations should be decoupled, which should be parallelized, and how parallel tasks should be synchronized.
 
 ### Installation
 
 ```
     conda create -y -n pytorchrl
     conda activate pytorchrl
 
     conda install pytorch torchvision cudatoolkit -c pytorch
-    
-    pip install pytorchrl
+
+    pip install pytorchrl gym[atari,accept-rom-license]==0.19.0 wandb opencv-python hydra-core
 ```
 
 ### Documentation
 
 PyTorchRL documentation can be found [here](https://pytorchrl.readthedocs.io/en/latest/).
 
 ### Citing PyTorchRL
+
 Here is the [paper](https://arxiv.org/abs/2007.02622)
 
 ```
 @misc{bou2021pytorchrl,
-      title={PyTorchRL: Modular and Distributed Reinforcement Learning in PyTorch}, 
+      title={PyTorchRL: Modular and Distributed Reinforcement Learning in PyTorch},
       author={Albert Bou and Gianni De Fabritiis},
       year={2021},
       eprint={2007.02622},
       archivePrefix={arXiv},
       primaryClass={cs.CV}
 }
 ```
```

### Comparing `pytorchrl-3.2.11/pytorchrl/__init__.py` & `pytorchrl-3.2.12/pytorchrl/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/base.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/base.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/distributions/__init__.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/distributions/categorical.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/distributions/categorical.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/distributions/deterministic.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/distributions/deterministic.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/distributions/gaussian.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/distributions/gaussian.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/distributions/squashed_gaussian.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/distributions/squashed_gaussian.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/__init__.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/cnn.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/cnn.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/dictnet.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/dictnet.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/embedding.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/embedding.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/ensemble_layer.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/ensemble_layer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/fixup_cnn.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/fixup_cnn.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/gpt.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/gpt.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/feature_extractors/mlp.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/feature_extractors/mlp.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/memory_networks/__init__.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/memory_networks/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/memory_networks/gru_net.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/memory_networks/gru_net.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/memory_networks/lstm_encoder_decoder_net.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/memory_networks/lstm_encoder_decoder_net.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/memory_networks/lstm_net.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/memory_networks/lstm_net.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/model_based_planner_actor.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/model_based_planner_actor.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/noise/ou.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/noise/ou.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/off_policy_actor.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/off_policy_actor.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/on_policy_actor.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/on_policy_actor.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/reward_functions/__init__.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/reward_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/reward_functions/gym_reward_functions.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/reward_functions/gym_reward_functions.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/reward_functions/pybullet_reward_functions.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/reward_functions/pybullet_reward_functions.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/utils.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/world_models/utils.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/world_models/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/actors/world_models/world_model.py` & `pytorchrl-3.2.12/pytorchrl/agent/actors/world_models/world_model.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/algorithms/__init__.py` & `pytorchrl-3.2.12/pytorchrl/agent/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/algorithms/base.py` & `pytorchrl-3.2.12/pytorchrl/agent/algorithms/base.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/algorithms/model_based/mpc_cem.py` & `pytorchrl-3.2.12/pytorchrl/agent/algorithms/model_based/mpc_cem.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/algorithms/model_based/mpc_pddm.py` & `pytorchrl-3.2.12/pytorchrl/agent/algorithms/model_based/mpc_pddm.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/algorithms/model_based/mpc_rs.py` & `pytorchrl-3.2.12/pytorchrl/agent/algorithms/model_based/mpc_rs.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/algorithms/off_policy/ddpg.py` & `pytorchrl-3.2.12/pytorchrl/agent/algorithms/off_policy/ddpg.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/algorithms/off_policy/ddqn.py` & `pytorchrl-3.2.12/pytorchrl/agent/algorithms/off_policy/ddqn.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/algorithms/off_policy/mpo.py` & `pytorchrl-3.2.12/pytorchrl/agent/algorithms/off_policy/mpo.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/algorithms/off_policy/sac.py` & `pytorchrl-3.2.12/pytorchrl/agent/algorithms/off_policy/sac.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/algorithms/off_policy/td3.py` & `pytorchrl-3.2.12/pytorchrl/agent/algorithms/off_policy/td3.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/algorithms/on_policy/a2c.py` & `pytorchrl-3.2.12/pytorchrl/agent/algorithms/on_policy/a2c.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/algorithms/on_policy/ppo.py` & `pytorchrl-3.2.12/pytorchrl/agent/algorithms/on_policy/ppo.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/algorithms/on_policy/rnd_ppo.py` & `pytorchrl-3.2.12/pytorchrl/agent/algorithms/on_policy/rnd_ppo.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/algorithms/policy_loss_addons/kv_similarity.py` & `pytorchrl-3.2.12/pytorchrl/agent/algorithms/policy_loss_addons/kv_similarity.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/algorithms/policy_loss_addons/return_predictor.py` & `pytorchrl-3.2.12/pytorchrl/agent/algorithms/policy_loss_addons/return_predictor.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/algorithms/policy_loss_addons/reward_predictor.py` & `pytorchrl-3.2.12/pytorchrl/agent/algorithms/policy_loss_addons/reward_predictor.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/algorithms/utils.py` & `pytorchrl-3.2.12/pytorchrl/agent/algorithms/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/env/base_envs/batched_env.py` & `pytorchrl-3.2.12/pytorchrl/agent/env/base_envs/batched_env.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/env/base_envs/env_wrappers.py` & `pytorchrl-3.2.12/pytorchrl/agent/env/base_envs/env_wrappers.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/env/vec_envs/parallel_vec_env.py` & `pytorchrl-3.2.12/pytorchrl/agent/env/vec_envs/parallel_vec_env.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/env/vec_envs/sequential_vec_env.py` & `pytorchrl-3.2.12/pytorchrl/agent/env/vec_envs/sequential_vec_env.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/env/vec_envs/util.py` & `pytorchrl-3.2.12/pytorchrl/agent/env/vec_envs/util.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/env/vec_envs/vec_env_base.py` & `pytorchrl-3.2.12/pytorchrl/agent/env/vec_envs/vec_env_base.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/env/vec_envs/vec_env_factory.py` & `pytorchrl-3.2.12/pytorchrl/agent/env/vec_envs/vec_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/env/vec_envs/vector_wrappers.py` & `pytorchrl-3.2.12/pytorchrl/agent/env/vec_envs/vector_wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     device : torch.device
         CPU or specific GPU where obs, reward's and done's are placed after
         being transformed into pytorch tensors.
     num_envs : int
         Size of vector environment.
 
     """
-    def __init__(self, venv, device):
+    def __init__(self, venv, device=torch.device('cpu')):
         super(VecPyTorch, self).__init__(venv)
         self.venv = venv
         self.device = device
         self.num_envs = venv.num_envs
 
     def reset(self):
         """New vec env reset function"""
```

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/storages/__init__.py` & `pytorchrl-3.2.12/pytorchrl/agent/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/storages/base.py` & `pytorchrl-3.2.12/pytorchrl/agent/storages/base.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/storages/model_based/mb_buffer.py` & `pytorchrl-3.2.12/pytorchrl/agent/storages/model_based/mb_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/storages/off_policy/ere_buffer.py` & `pytorchrl-3.2.12/pytorchrl/agent/storages/off_policy/ere_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/storages/off_policy/her_buffer.py` & `pytorchrl-3.2.12/pytorchrl/agent/storages/off_policy/her_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/storages/off_policy/nstep_buffer.py` & `pytorchrl-3.2.12/pytorchrl/agent/storages/off_policy/nstep_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/storages/off_policy/per_buffer.py` & `pytorchrl-3.2.12/pytorchrl/agent/storages/off_policy/per_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/storages/off_policy/replay_buffer.py` & `pytorchrl-3.2.12/pytorchrl/agent/storages/off_policy/replay_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/storages/on_policy/gae_buffer.py` & `pytorchrl-3.2.12/pytorchrl/agent/storages/on_policy/gae_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/storages/on_policy/ppod2_buffer.py` & `pytorchrl-3.2.12/pytorchrl/agent/storages/on_policy/ppod2_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/storages/on_policy/ppod2rebel_buffer.py` & `pytorchrl-3.2.12/pytorchrl/agent/storages/on_policy/ppod2rebel_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/storages/on_policy/ppod_buffer.py` & `pytorchrl-3.2.12/pytorchrl/agent/storages/on_policy/ppod_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/storages/on_policy/vanilla_on_policy_buffer.py` & `pytorchrl-3.2.12/pytorchrl/agent/storages/on_policy/vanilla_on_policy_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/agent/storages/on_policy/vtrace_buffer.py` & `pytorchrl-3.2.12/pytorchrl/agent/storages/on_policy/vtrace_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/animal_olympics/animal_olympics_env_factory.py` & `pytorchrl-3.2.12/pytorchrl/envs/animal_olympics/animal_olympics_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/animal_olympics/utils.py` & `pytorchrl-3.2.12/pytorchrl/envs/animal_olympics/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/animal_olympics/wrappers.py` & `pytorchrl-3.2.12/pytorchrl/envs/animal_olympics/wrappers.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/atari/atari_env_factory.py` & `pytorchrl-3.2.12/pytorchrl/envs/atari/atari_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/atari/wrappers.py` & `pytorchrl-3.2.12/pytorchrl/envs/atari/wrappers.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/causal_world/causal_world_env_factory.py` & `pytorchrl-3.2.12/pytorchrl/envs/causal_world/causal_world_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/common.py` & `pytorchrl-3.2.12/pytorchrl/envs/common.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/crafter/crafter_env_factory.py` & `pytorchrl-3.2.12/pytorchrl/envs/crafter/crafter_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/dm_control/dmcontrol_env_factory.py` & `pytorchrl-3.2.12/pytorchrl/envs/dm_control/dmcontrol_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/dm_control/utils.py` & `pytorchrl-3.2.12/pytorchrl/envs/dm_control/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/diversity_filter/base_diversity_filter.py` & `pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/diversity_filter/base_diversity_filter.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/diversity_filter/diversity_filter_memory.py` & `pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/diversity_filter/diversity_filter_memory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/diversity_filter/no_filter_with_penalty.py` & `pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/diversity_filter/no_filter_with_penalty.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/libinvent/batched_rnn_environment.py` & `pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/libinvent/batched_rnn_environment.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/libinvent/generative_chemistry_env_factory.py` & `pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/libinvent/generative_chemistry_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/libinvent/rnn_environment.py` & `pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/libinvent/rnn_environment.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/libinvent/utils.py` & `pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/libinvent/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/reinvent/generative_chemistry_env_factory.py` & `pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/reinvent/generative_chemistry_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/reinvent/rnn_environment.py` & `pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/reinvent/rnn_environment.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/reinvent/transformer_environment.py` & `pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/reinvent/transformer_environment.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/utils.py` & `pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/generative_chemistry/vocabulary.py` & `pytorchrl-3.2.12/pytorchrl/envs/generative_chemistry/vocabulary.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/habitat/habitat_env_factory.py` & `pytorchrl-3.2.12/pytorchrl/envs/habitat/habitat_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/habitat/utils.py` & `pytorchrl-3.2.12/pytorchrl/envs/habitat/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/habitat/wrappers.py` & `pytorchrl-3.2.12/pytorchrl/envs/habitat/wrappers.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/minigrid/custom_environments/__init__.py` & `pytorchrl-3.2.12/pytorchrl/envs/minigrid/custom_environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/minigrid/custom_environments/deceiving_rewards.py` & `pytorchrl-3.2.12/pytorchrl/envs/minigrid/custom_environments/deceiving_rewards.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/minigrid/custom_environments/multiple_deceiving_rewards.py` & `pytorchrl-3.2.12/pytorchrl/envs/minigrid/custom_environments/multiple_deceiving_rewards.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/minigrid/minigrid_env_factory.py` & `pytorchrl-3.2.12/pytorchrl/envs/minigrid/minigrid_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/minigrid/wrappers.py` & `pytorchrl-3.2.12/pytorchrl/envs/minigrid/wrappers.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/mujoco/mujoco_env_factory.py` & `pytorchrl-3.2.12/pytorchrl/envs/mujoco/mujoco_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/obstacle_tower/obstacle_tower_env_factory.py` & `pytorchrl-3.2.12/pytorchrl/envs/obstacle_tower/obstacle_tower_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/obstacle_tower/utils.py` & `pytorchrl-3.2.12/pytorchrl/envs/obstacle_tower/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/obstacle_tower/wrappers.py` & `pytorchrl-3.2.12/pytorchrl/envs/obstacle_tower/wrappers.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/pybullet/pybullet_env_factory.py` & `pytorchrl-3.2.12/pytorchrl/envs/pybullet/pybullet_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/envs/pybullet/sparse_reacher.py` & `pytorchrl-3.2.12/pytorchrl/envs/pybullet/sparse_reacher.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/learner.py` & `pytorchrl-3.2.12/pytorchrl/learner.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/scheme/base/worker.py` & `pytorchrl-3.2.12/pytorchrl/scheme/base/worker.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/scheme/base/worker_set.py` & `pytorchrl-3.2.12/pytorchrl/scheme/base/worker_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,33 +52,33 @@
         if add_local_worker:
 
             local_params = worker_params.copy()
             local_params.update(
                 {"device": local_device, "initial_weights": initial_weights})
 
             # If multiple grad workers the collection workers of grad worker with index 0 should not collect
-            if worker.__name__ == "CWorker" and total_parent_workers > 0 and index_parent_worker == 0:
+            if worker.__name__ == "CWorker" and total_parent_workers and total_parent_workers > 0 and index_parent_worker == 0:
                 self.num_workers = 0
                 _ = local_params.pop("test_envs_factory")
                 _ = local_params.pop("train_envs_factory")
 
             # If multiple col workers, local collection workers don't need to collect
-            elif worker.__name__ == "CWorker" and num_workers > 0:
+            elif worker.__name__ == "CWorker" and num_workers > 1:
                 _ = local_params.pop("test_envs_factory")
                 _ = local_params.pop("train_envs_factory")
 
             self._local_worker = self._make_worker(
                 self.worker_class, index_worker=0,
                 worker_params=local_params)
 
         else:
             self._local_worker = None
 
         self._remote_workers = []
-        if self.num_workers > 0:
+        if self.num_workers > 1:
             self.add_workers(self.num_workers)
 
     @staticmethod
     def _make_worker(cls, index_worker, worker_params):
         """
         Create a single worker.
```

### Comparing `pytorchrl-3.2.11/pytorchrl/scheme/collection/c_worker.py` & `pytorchrl-3.2.12/pytorchrl/scheme/collection/c_worker.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/scheme/collection/c_worker_set.py` & `pytorchrl-3.2.12/pytorchrl/scheme/collection/c_worker_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
                  total_parent_workers=0,
                  compress_data_to_send=False,
                  train_envs_factory=lambda x, y, z: None,
                  test_envs_factory=lambda v, x, y, c: None,
                  worker_remote_config=default_remote_config):
 
         self.worker_class = CWorker
+        self.fraction_samples = fraction_samples
         default_remote_config.update(worker_remote_config)
         self.remote_config = default_remote_config
         self.worker_params = {
             "index_parent": index_parent,
             "algo_factory": algo_factory,
             "actor_factory": actor_factory,
             "storage_factory": storage_factory,
```

### Comparing `pytorchrl-3.2.11/pytorchrl/scheme/gradients/g_worker.py` & `pytorchrl-3.2.12/pytorchrl/scheme/gradients/g_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,18 +32,14 @@
         A function that creates a set of data collection workers.
     col_communication : str
         Communication coordination pattern for data collection.
     compress_grads_to_send : bool
         Whether or not to compress gradients before sending then to the update worker.
     col_execution : str
         Execution patterns for data collection.
-    col_fraction_workers : float
-        Minimum fraction of samples required to stop if collection is
-        synchronously coordinated and most workers have finished their
-        collection task.
     device : str
         "cpu" or specific GPU "cuda:number`" to use for computation.
     initial_weights : ray object ID
         Initial model weights.
 
     Attributes
     ----------
@@ -53,14 +49,18 @@
         Number of times gradients have been computed and sent.
     col_communication : str
         Communication coordination pattern for data collection.
     compress_grads_to_send : bool
         Whether or not to compress gradients before sending then to the update worker.
     col_workers : CWorkerSet
         A CWorkerSet class instance.
+    col_fraction_workers : float
+        Minimum fraction of samples required to stop if collection is
+        synchronously coordinated and most workers have finished their
+        collection task.
     local_worker : CWorker
         col_workers local worker.
     remote_workers : List of CWorker's
         col_workers remote data collection workers.
     actor : Actor
         An actor class instance.
     algo : Algo
@@ -75,16 +75,14 @@
     """
 
     def __init__(self,
                  index_worker,
                  col_workers_factory,
                  col_communication=prl.SYNC,
                  compress_grads_to_send=False,
-                 col_execution=prl.CENTRAL,
-                 col_fraction_workers=1.0,
                  initial_weights=None,
                  device=None):
 
         self.index_worker = index_worker
         super(GWorker, self).__init__(index_worker)
 
         # Define counters and other attributes
@@ -94,18 +92,20 @@
         self.processing_time_start = None
 
         # Computation device
         dev = device or "cuda" if torch.cuda.is_available() else "cpu"
 
         # Create CWorkerSet instance
         self.col_workers = col_workers_factory(dev, initial_weights, index_worker)
+        self.col_fraction_workers = self.col_workers.fraction_samples
         self.local_worker = self.col_workers.local_worker()
         self.remote_workers = self.col_workers.remote_workers()
         self.num_remote_workers = len(self.remote_workers)
         self.num_collection_workers = 1 if self.num_remote_workers == 0 else self.num_remote_workers
+        self.col_execution = prl.CENTRAL if self.num_remote_workers == 0 else prl.PARALLEL
 
         # Get Actor Critic instance
         self.actor = self.local_worker.actor
 
         # Get Algorithm instance
         self.algo = self.local_worker.algo
 
@@ -141,16 +141,16 @@
 
             # Create CollectorThread
             self.collector = CollectorThread(
                 index_worker=index_worker,
                 local_worker=self.local_worker,
                 remote_workers=self.remote_workers,
                 col_communication=col_communication,
-                col_fraction_workers=col_fraction_workers,
-                col_execution=col_execution,
+                col_fraction_workers=self.col_fraction_workers,
+                col_execution=self.col_execution,
                 broadcast_interval=1)
 
             # Print worker information
             self.print_worker_info()
 
     @property
     def actor_version(self):
```

### Comparing `pytorchrl-3.2.11/pytorchrl/scheme/gradients/g_worker_set.py` & `pytorchrl-3.2.12/pytorchrl/scheme/gradients/g_worker_set.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,18 +58,16 @@
 
         self.worker_class = GWorker
         self.num_workers = num_workers
         default_remote_config.update(grad_worker_resources)
         self.remote_config = default_remote_config
 
         self.worker_params = {
-            "col_execution": col_execution,
             "col_communication": col_communication,
             "col_workers_factory": col_workers_factory,
-            "col_fraction_workers": col_fraction_workers,
             "compress_grads_to_send": compress_grads_to_send,
         }
 
         super(GWorkerSet, self).__init__(
             worker=self.worker_class,
             local_device=local_device,
             num_workers=self.num_workers,
```

### Comparing `pytorchrl-3.2.11/pytorchrl/scheme/scheme.py` & `pytorchrl-3.2.12/pytorchrl/scheme/scheme.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,60 +74,44 @@
 
         assert col_workers_communication in (prl.SYNC, prl.ASYNC),\
             "col_workers_communication can only be `prl.SYNC` or `prl.ASYNC`"
 
         assert grad_workers_communication in (prl.SYNC, prl.ASYNC),\
             "grad_workers_communication can only be `prl.SYNC` or `prl.ASYNC`"
 
-        col_execution = prl.PARALLEL if num_col_workers > 1 else prl.CENTRAL
-        grad_execution = prl.PARALLEL if num_grad_workers > 1 else prl.CENTRAL
-
         col_workers_factory = CWorkerSet.create_factory(
-
             # core modules
             algo_factory=algo_factory,
             actor_factory=actor_factory,
             storage_factory=storage_factory,
             test_envs_factory=test_envs_factory,
             train_envs_factory=train_envs_factory,
-
             # col specs
             num_workers=num_col_workers - 1 if num_col_workers == 1 else num_col_workers,
             col_worker_resources=col_workers_resources,
             col_fraction_samples=col_preemption_thresholds.get("fraction_samples"),
             compress_data_to_send=col_compress_data,
-
             # grad specs
             total_parent_workers=num_grad_workers - 1 if num_grad_workers == 1 else num_grad_workers,
         )
 
         grad_workers_factory = GWorkerSet.create_factory(
-
             # col specs
-            col_execution=col_execution,
             col_communication=col_workers_communication,
             col_workers_factory=col_workers_factory,
-            col_fraction_workers=col_preemption_thresholds.get("fraction_workers"),
-
             # grad_specs
             num_workers=num_grad_workers - 1 if num_grad_workers == 1 else num_grad_workers,
             grad_worker_resources=grad_workers_resources,
             compress_grads_to_send=grad_compress_data,
         )
 
         self._update_worker = UWorker(
-
-           # col specs
-            col_fraction_workers=col_preemption_thresholds.get("fraction_workers"),
-
             # grad specs
-            grad_execution=grad_execution,
             grad_communication=grad_workers_communication,
             grad_workers_factory=grad_workers_factory,
-
             # update specs
             local_device=local_device,
             decentralized_update_execution=decentralized_update_execution,
         )
 
         logger.warning("Created training scheme.")
```

### Comparing `pytorchrl-3.2.11/pytorchrl/scheme/updates/u_worker.py` & `pytorchrl-3.2.12/pytorchrl/scheme/updates/u_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,14 @@
         A function that creates a set of gradientc omputation workers.
     index_worker : int
         Worker index.
     col_fraction_workers : float
         Minimum fraction of samples required to stop if collection is
         synchronously coordinated and most workers have finished their
         collection task.
-    grad_execution : str
-        Execution patterns for gradients computation.
     grad_communication : str
         Communication coordination pattern for gradient computation workers.
     decentralized_update_execution : bool
         Whether the gradients are applied in the update workers (central update)
         or broadcasted to all gradient workers for a decentralized update.
     local_device : str
         "cpu" or specific GPU "cuda:number`" to use for computation.
@@ -57,50 +55,47 @@
         performing update steps and placing update information into the
         output queue `outqueue`.
     """
 
     def __init__(self,
                  grad_workers_factory,
                  index_worker=0,
-                 col_fraction_workers=1.0,
-                 grad_execution=prl.CENTRAL,
                  grad_communication=prl.SYNC,
                  decentralized_update_execution=False,
                  local_device=None):
 
         super(UWorker, self).__init__(index_worker)
 
-        self.grad_execution = grad_execution
-        self.grad_communication = grad_communication
-
         # Computation device
         dev = local_device or "cuda" if torch.cuda.is_available() else "cpu"
 
         self.grad_workers = grad_workers_factory(dev, index_worker)
         self.local_worker = self.grad_workers.local_worker()
         self.remote_workers = self.grad_workers.remote_workers()
         self.num_workers = len(self.grad_workers.remote_workers())
 
+        self.grad_execution = prl.PARALLEL if self.num_workers > 1 else prl.CENTRAL
+        self.grad_communication = grad_communication
+
         # Create CWorkerSet instance
         if decentralized_update_execution:
             # Setup the distributed processes for gradient averaging
             ip = ray.get(self.remote_workers[0].get_node_ip.remote())
             port = ray.get(self.remote_workers[0].find_free_port.remote())
             address = "tcp://{ip}:{port}".format(ip=ip, port=port)
             ray.get([worker.setup_torch_data_parallel.remote(
                 address, i, len(self.remote_workers), "nccl")
                      for i, worker in enumerate(self.remote_workers)])
 
         # Create UpdaterThread
         self.updater = UpdaterThread(
             local_worker=self.local_worker,
             remote_workers=self.remote_workers,
-            col_fraction_workers=col_fraction_workers,
+            col_fraction_workers=self.local_worker.col_fraction_workers,
             grad_communication=grad_communication,
-            grad_execution=grad_execution,
             decentralized_update_execution=decentralized_update_execution,
         )
 
         # Print worker information
         self.print_worker_info()
 
     @property
@@ -173,18 +168,14 @@
     ----------
     local_worker : GWorker
         Local GWorker that acts as a parameter server.
     remote_workers : List
         grad_workers remote data collection workers.
     decentralized_update_execution : bool
         Whether decentralized execution pattern for update steps is enabled or not.
-    col_fraction_workers : float
-        Minimum fraction of samples required to stop if collection is
-        synchronously coordinated and most workers have finished their
-        collection task.
     grad_execution : str
         Execution patterns for gradients computation.
     grad_communication : str
         Communication coordination pattern for gradient computation workers.
 
     Attributes
     ----------
```

### Comparing `pytorchrl-3.2.11/pytorchrl/scheme/utils.py` & `pytorchrl-3.2.12/pytorchrl/scheme/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/trainer.py` & `pytorchrl-3.2.12/pytorchrl/trainer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl/utils.py` & `pytorchrl-3.2.12/pytorchrl/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/pytorchrl.egg-info/PKG-INFO` & `pytorchrl-3.2.12/pytorchrl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: pytorchrl
-Version: 3.2.11
+Version: 3.2.12
 Summary: Disributed RL implementations with ray and pytorch.
 Home-page: https://github.com/PyTorchRL/pytorchrl/
 Author: albertbou92
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 ## PyTorchRL: A PyTorch library for reinforcement learning
 
-Deep Reinforcement learning (DRL) has been very successful in recent years but current methods still require vast amounts of data to solve non-trivial environments.  Scaling to solve more complex tasks requires frameworks that are flexible enough to allow prototyping and testing of new ideas, yet avoiding the impractically slow experimental turnaround times associated to single-threaded implementations.  PyTorchRL is a pytorch-based library for DRL that allows to easily assemble RL agents using a set of core reusable and easily extendable sub-modules as building blocks.  To reduce training times, PyTorchRL allows scaling agents with a parameterizable component called Scheme, that permits to define distributed architectures with great flexibility by specifying which operations should be decoupled, which should be parallelized, and how parallel tasks should be synchronized.
+Deep Reinforcement learning (DRL) has been very successful in recent years but current methods still require vast amounts of data to solve non-trivial environments. Scaling to solve more complex tasks requires frameworks that are flexible enough to allow prototyping and testing of new ideas, yet avoiding the impractically slow experimental turnaround times associated to single-threaded implementations. PyTorchRL is a pytorch-based library for DRL that allows to easily assemble RL agents using a set of core reusable and easily extendable sub-modules as building blocks. To reduce training times, PyTorchRL allows scaling agents with a parameterizable component called Scheme, that permits to define distributed architectures with great flexibility by specifying which operations should be decoupled, which should be parallelized, and how parallel tasks should be synchronized.
 
 ### Installation
 
 ```
     conda create -y -n pytorchrl
     conda activate pytorchrl
 
     conda install pytorch torchvision cudatoolkit -c pytorch
-    
-    pip install pytorchrl
+
+    pip install pytorchrl gym[atari,accept-rom-license]==0.19.0 wandb opencv-python hydra-core
 ```
 
 ### Documentation
 
 PyTorchRL documentation can be found [here](https://pytorchrl.readthedocs.io/en/latest/).
 
 ### Citing PyTorchRL
+
 Here is the [paper](https://arxiv.org/abs/2007.02622)
 
 ```
 @misc{bou2021pytorchrl,
-      title={PyTorchRL: Modular and Distributed Reinforcement Learning in PyTorch}, 
+      title={PyTorchRL: Modular and Distributed Reinforcement Learning in PyTorch},
       author={Albert Bou and Gianni De Fabritiis},
       year={2021},
       eprint={2007.02622},
       archivePrefix={arXiv},
       primaryClass={cs.CV}
 }
 ```
```

### Comparing `pytorchrl-3.2.11/pytorchrl.egg-info/SOURCES.txt` & `pytorchrl-3.2.12/pytorchrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.11/setup.py` & `pytorchrl-3.2.12/setup.py`

 * *Files identical despite different names*

