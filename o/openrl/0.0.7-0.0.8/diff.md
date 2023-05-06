# Comparing `tmp/openrl-0.0.7.tar.gz` & `tmp/openrl-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrl-0.0.7.tar", last modified: Thu May  4 10:36:38 2023, max compression
+gzip compressed data, was "openrl-0.0.8.tar", last modified: Sat May  6 12:05:19 2023, max compression
```

## Comparing `openrl-0.0.7.tar` & `openrl-0.0.8.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.431155 openrl-0.0.7/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-04-28 07:15:42.000000 openrl-0.0.7/LICENSE
--rw-r--r--   0 4paradigm   (501) staff       (20)    11342 2023-03-23 09:43:52.000000 openrl-0.0.7/LICENSE.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)    11973 2023-05-04 10:36:38.428981 openrl-0.0.7/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)    10888 2023-05-04 10:32:54.000000 openrl-0.0.7/README.md
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.383222 openrl-0.0.7/openrl/
--rw-r--r--   0 4paradigm   (501) staff       (20)      194 2023-05-04 10:35:02.000000 openrl-0.0.7/openrl/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.385693 openrl-0.0.7/openrl/algorithms/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/algorithms/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2916 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/algorithms/base_algorithm.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    16410 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/algorithms/ppo.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.386699 openrl-0.0.7/openrl/buffers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      726 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/buffers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3100 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/buffers/normal_buffer.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    54804 2023-04-28 09:05:05.000000 openrl-0.0.7/openrl/buffers/replay_data.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.387857 openrl-0.0.7/openrl/buffers/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/buffers/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1938 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/buffers/utils/obs_data.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3153 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/buffers/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.388436 openrl-0.0.7/openrl/cli/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/cli/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2551 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/cli/cli.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1579 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/cli/train.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.388715 openrl-0.0.7/openrl/configs/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/configs/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    31231 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/configs/config.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.389502 openrl-0.0.7/openrl/drivers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/drivers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      238 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/drivers/base_driver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9929 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/drivers/onpolicy_driver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      841 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/drivers/rl_driver.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.389661 openrl-0.0.7/openrl/envs/
--rw-r--r--   0 4paradigm   (501) staff       (20)       79 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.390182 openrl-0.0.7/openrl/envs/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)      739 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1621 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/common/build_envs.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3305 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/envs/common/registration.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.390327 openrl-0.0.7/openrl/envs/gymnasium/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1425 2023-04-28 09:05:04.000000 openrl-0.0.7/openrl/envs/gymnasium/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.391733 openrl-0.0.7/openrl/envs/mpe/
--rw-r--r--   0 4paradigm   (501) staff       (20)      628 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    14285 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/core.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      615 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/mpe_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2488 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/multi_discrete.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    19199 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/multiagent_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11650 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/rendering.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      343 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/scenario.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.392297 openrl-0.0.7/openrl/envs/mpe/scenarios/
--rw-r--r--   0 4paradigm   (501) staff       (20)      145 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/scenarios/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4405 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/mpe/scenarios/simple_spread.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.392932 openrl-0.0.7/openrl/envs/nlp/
--rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7514 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/envs/nlp/daily_dialog_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      347 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/nlp_env.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.394245 openrl-0.0.7/openrl/envs/nlp/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2765 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/custom_text_generation_pools.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4515 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/distribution.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1823 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/evaluation_utils.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.394627 openrl-0.0.7/openrl/envs/nlp/utils/metrics/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/metrics/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7088 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/metrics/meteor.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7201 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/observation.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1363 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/sampler.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1233 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/nlp/utils/text_generation_pool.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.395372 openrl-0.0.7/openrl/envs/vec_env/
--rw-r--r--   0 4paradigm   (501) staff       (20)      348 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/envs/vec_env/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    30978 2023-04-28 09:05:05.000000 openrl-0.0.7/openrl/envs/vec_env/async_venv.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7845 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/vec_env/base_venv.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11100 2023-04-28 09:05:05.000000 openrl-0.0.7/openrl/envs/vec_env/sync_venv.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.396500 openrl-0.0.7/openrl/envs/vec_env/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/vec_env/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6518 2023-04-28 09:05:05.000000 openrl-0.0.7/openrl/envs/vec_env/utils/numpy_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7902 2023-04-28 09:05:05.000000 openrl-0.0.7/openrl/envs/vec_env/utils/share_memory.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1909 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/vec_env/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.397307 openrl-0.0.7/openrl/envs/vec_env/vec_info/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1058 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/envs/vec_env/vec_info/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      585 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/envs/vec_env/vec_info/base_vec_info.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2323 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/envs/vec_env/vec_info/nlp_vec_info.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1221 2023-05-04 10:32:54.000000 openrl-0.0.7/openrl/envs/vec_env/vec_info/simple_vec_info.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.398342 openrl-0.0.7/openrl/envs/vec_env/wrappers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/vec_env/wrappers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9266 2023-04-28 09:05:05.000000 openrl-0.0.7/openrl/envs/vec_env/wrappers/base_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2227 2023-05-04 10:32:54.000000 openrl-0.0.7/openrl/envs/vec_env/wrappers/reward_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1544 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.399772 openrl-0.0.7/openrl/envs/wrappers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      372 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/wrappers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1612 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/envs/wrappers/base_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2454 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/wrappers/extra_wrappers.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2533 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/wrappers/multiagent_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1188 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/envs/wrappers/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.400999 openrl-0.0.7/openrl/modules/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1540 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/base_module.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.401662 openrl-0.0.7/openrl/modules/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)       57 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      738 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/common/base_net.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3441 2023-04-28 09:15:51.000000 openrl-0.0.7/openrl/modules/common/ppo_net.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1210 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/model_config.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.403369 openrl-0.0.7/openrl/modules/networks/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1227 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/base_policy_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1191 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/base_value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     8075 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/policy_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6445 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/policy_value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3991 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/modules/networks/policy_value_network_gpt.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.406198 openrl-0.0.7/openrl/modules/networks/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7389 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/act.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9343 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/attention.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2270 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/cnn.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      805 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/distributed_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3551 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/distributions.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    10432 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/mix.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5904 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/mlp.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.407541 openrl-0.0.7/openrl/modules/networks/utils/nlp/
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/nlp/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11814 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/nlp/base_policy.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    10986 2023-04-28 09:05:05.000000 openrl-0.0.7/openrl/modules/networks/utils/nlp/causal_policy.py
--rw-r--r--   0 4paradigm   (501) staff       (20)   188639 2023-04-28 09:05:05.000000 openrl-0.0.7/openrl/modules/networks/utils/nlp/hf_generation_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3973 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/popart.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3515 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/rnn.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3344 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/transformer_act.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      317 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/utils/util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4602 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/networks/value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7053 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/ppo_module.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5206 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/rl_module.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.409066 openrl-0.0.7/openrl/modules/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      631 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/utils/util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3599 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/modules/utils/valuenorm.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.411385 openrl-0.0.7/openrl/rewards/
--rw-r--r--   0 4paradigm   (501) staff       (20)      919 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/rewards/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      588 2023-05-04 10:32:54.000000 openrl-0.0.7/openrl/rewards/base_reward.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3467 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/rewards/nlp_reward.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.411672 openrl-0.0.7/openrl/runners/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/runners/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.414173 openrl-0.0.7/openrl/runners/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)      156 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/runners/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1263 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/runners/common/base_agent.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3185 2023-04-28 09:15:51.000000 openrl-0.0.7/openrl/runners/common/chat_agent.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6083 2023-04-28 09:44:16.000000 openrl-0.0.7/openrl/runners/common/ppo_agent.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.415883 openrl-0.0.7/openrl/supports/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/supports/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.416110 openrl-0.0.7/openrl/supports/opendata/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/supports/opendata/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.418315 openrl-0.0.7/openrl/supports/opendata/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/supports/opendata/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2132 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/supports/opendata/utils/opendata_utils.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.421928 openrl-0.0.7/openrl/supports/opengpu/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/supports/opengpu/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4184 2023-05-04 10:32:54.000000 openrl-0.0.7/openrl/supports/opengpu/gpu_info.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7113 2023-05-04 10:32:54.000000 openrl-0.0.7/openrl/supports/opengpu/manager.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.422781 openrl-0.0.7/openrl/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5744 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/utils/logger.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1482 2023-04-28 07:15:42.000000 openrl-0.0.7/openrl/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.384760 openrl-0.0.7/openrl.egg-info/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11973 2023-05-04 10:36:38.000000 openrl-0.0.7/openrl.egg-info/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)     4554 2023-05-04 10:36:38.000000 openrl-0.0.7/openrl.egg-info/SOURCES.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-05-04 10:36:38.000000 openrl-0.0.7/openrl.egg-info/dependency_links.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-05-04 10:36:38.000000 openrl-0.0.7/openrl.egg-info/entry_points.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)      292 2023-05-04 10:36:38.000000 openrl-0.0.7/openrl.egg-info/requires.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       13 2023-05-04 10:36:38.000000 openrl-0.0.7/openrl.egg-info/top_level.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-05-04 10:36:38.431210 openrl-0.0.7/setup.cfg
--rw-r--r--   0 4paradigm   (501) staff       (20)     3089 2023-05-04 10:32:55.000000 openrl-0.0.7/setup.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.422927 openrl-0.0.7/tests/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/tests/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.424859 openrl-0.0.7/tests/project/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/tests/project/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      972 2023-04-28 07:15:42.000000 openrl-0.0.7/tests/project/test_version.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-04 10:36:38.428701 openrl-0.0.7/tests/test_buffer/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.7/tests/test_buffer/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1803 2023-04-28 07:15:42.000000 openrl-0.0.7/tests/test_buffer/test_buffer.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.866665 openrl-0.0.8/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-04-28 07:15:42.000000 openrl-0.0.8/LICENSE
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11342 2023-03-23 09:43:52.000000 openrl-0.0.8/LICENSE.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)    13317 2023-05-06 12:05:19.866443 openrl-0.0.8/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)    12168 2023-05-06 12:04:43.000000 openrl-0.0.8/README.md
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.838034 openrl-0.0.8/openrl/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      371 2023-05-06 12:04:43.000000 openrl-0.0.8/openrl/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.839690 openrl-0.0.8/openrl/algorithms/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/algorithms/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2916 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/algorithms/base_algorithm.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    16410 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/algorithms/ppo.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.840782 openrl-0.0.8/openrl/buffers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      726 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/buffers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3100 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/buffers/normal_buffer.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    54804 2023-04-28 09:05:05.000000 openrl-0.0.8/openrl/buffers/replay_data.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.842390 openrl-0.0.8/openrl/buffers/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/buffers/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1938 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/buffers/utils/obs_data.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3153 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/buffers/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.843063 openrl-0.0.8/openrl/cli/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/cli/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2551 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/cli/cli.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1579 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/cli/train.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.843432 openrl-0.0.8/openrl/configs/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/configs/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    31231 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/configs/config.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.844701 openrl-0.0.8/openrl/drivers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/drivers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      238 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/drivers/base_driver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9929 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/drivers/onpolicy_driver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      841 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/drivers/rl_driver.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.844985 openrl-0.0.8/openrl/envs/
+-rw-r--r--   0 4paradigm   (501) staff       (20)       79 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.845518 openrl-0.0.8/openrl/envs/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      739 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1621 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/common/build_envs.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3305 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/envs/common/registration.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.845755 openrl-0.0.8/openrl/envs/gymnasium/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1425 2023-04-28 09:05:04.000000 openrl-0.0.8/openrl/envs/gymnasium/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.847878 openrl-0.0.8/openrl/envs/mpe/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      628 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    14285 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/core.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      615 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/mpe_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2488 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/multi_discrete.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    19199 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/multiagent_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11650 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/rendering.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      343 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/scenario.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.848290 openrl-0.0.8/openrl/envs/mpe/scenarios/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      145 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/scenarios/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4405 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/mpe/scenarios/simple_spread.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.848965 openrl-0.0.8/openrl/envs/nlp/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7514 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/envs/nlp/daily_dialog_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      347 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/nlp_env.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.850316 openrl-0.0.8/openrl/envs/nlp/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2765 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/custom_text_generation_pools.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4515 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/distribution.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1823 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/evaluation_utils.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.850624 openrl-0.0.8/openrl/envs/nlp/utils/metrics/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/metrics/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7088 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/metrics/meteor.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7201 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/observation.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1363 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/sampler.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1233 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/nlp/utils/text_generation_pool.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.851426 openrl-0.0.8/openrl/envs/vec_env/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      348 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/envs/vec_env/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    30978 2023-04-28 09:05:05.000000 openrl-0.0.8/openrl/envs/vec_env/async_venv.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7845 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/vec_env/base_venv.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11100 2023-04-28 09:05:05.000000 openrl-0.0.8/openrl/envs/vec_env/sync_venv.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.852262 openrl-0.0.8/openrl/envs/vec_env/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/vec_env/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6518 2023-04-28 09:05:05.000000 openrl-0.0.8/openrl/envs/vec_env/utils/numpy_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7902 2023-04-28 09:05:05.000000 openrl-0.0.8/openrl/envs/vec_env/utils/share_memory.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1909 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/vec_env/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.852982 openrl-0.0.8/openrl/envs/vec_env/vec_info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1058 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/envs/vec_env/vec_info/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      585 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/envs/vec_env/vec_info/base_vec_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2323 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/envs/vec_env/vec_info/nlp_vec_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1221 2023-05-04 10:32:54.000000 openrl-0.0.8/openrl/envs/vec_env/vec_info/simple_vec_info.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.853959 openrl-0.0.8/openrl/envs/vec_env/wrappers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/vec_env/wrappers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9266 2023-04-28 09:05:05.000000 openrl-0.0.8/openrl/envs/vec_env/wrappers/base_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2227 2023-05-04 10:32:54.000000 openrl-0.0.8/openrl/envs/vec_env/wrappers/reward_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1544 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.854802 openrl-0.0.8/openrl/envs/wrappers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      372 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/wrappers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1612 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/envs/wrappers/base_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2454 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/wrappers/extra_wrappers.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2533 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/wrappers/multiagent_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1188 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/envs/wrappers/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.855783 openrl-0.0.8/openrl/modules/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1540 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/base_module.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.856353 openrl-0.0.8/openrl/modules/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)       57 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      738 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/common/base_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3441 2023-04-28 09:15:51.000000 openrl-0.0.8/openrl/modules/common/ppo_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1210 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/model_config.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.857615 openrl-0.0.8/openrl/modules/networks/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1227 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/base_policy_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1191 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/base_value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     8075 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/policy_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6445 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/policy_value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3991 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/modules/networks/policy_value_network_gpt.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.859879 openrl-0.0.8/openrl/modules/networks/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7389 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/act.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9343 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/attention.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2270 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/cnn.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      805 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/distributed_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3551 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/distributions.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10432 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/mix.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5904 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/mlp.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.860560 openrl-0.0.8/openrl/modules/networks/utils/nlp/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/nlp/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11814 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/nlp/base_policy.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10986 2023-04-28 09:05:05.000000 openrl-0.0.8/openrl/modules/networks/utils/nlp/causal_policy.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)   188639 2023-04-28 09:05:05.000000 openrl-0.0.8/openrl/modules/networks/utils/nlp/hf_generation_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3973 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/popart.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3515 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/rnn.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3344 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/transformer_act.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      317 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/utils/util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4602 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/networks/value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7053 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/ppo_module.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5206 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/rl_module.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.862167 openrl-0.0.8/openrl/modules/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      631 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/utils/util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3599 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/modules/utils/valuenorm.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.862761 openrl-0.0.8/openrl/rewards/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      919 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/rewards/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      570 2023-05-06 12:04:43.000000 openrl-0.0.8/openrl/rewards/base_reward.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3467 2023-04-28 09:44:16.000000 openrl-0.0.8/openrl/rewards/nlp_reward.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.863041 openrl-0.0.8/openrl/runners/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/runners/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.863805 openrl-0.0.8/openrl/runners/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      188 2023-05-06 12:04:43.000000 openrl-0.0.8/openrl/runners/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1263 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/runners/common/base_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4024 2023-05-06 12:04:43.000000 openrl-0.0.8/openrl/runners/common/chat_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6067 2023-05-06 12:04:43.000000 openrl-0.0.8/openrl/runners/common/ppo_agent.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.864040 openrl-0.0.8/openrl/supports/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/supports/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.864175 openrl-0.0.8/openrl/supports/opendata/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/supports/opendata/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.864457 openrl-0.0.8/openrl/supports/opendata/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/supports/opendata/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2132 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/supports/opendata/utils/opendata_utils.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.864980 openrl-0.0.8/openrl/supports/opengpu/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/supports/opengpu/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4184 2023-05-04 10:32:54.000000 openrl-0.0.8/openrl/supports/opengpu/gpu_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7114 2023-05-06 12:04:43.000000 openrl-0.0.8/openrl/supports/opengpu/manager.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.865417 openrl-0.0.8/openrl/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5744 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/utils/logger.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1482 2023-04-28 07:15:42.000000 openrl-0.0.8/openrl/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.839014 openrl-0.0.8/openrl.egg-info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    13317 2023-05-06 12:05:19.000000 openrl-0.0.8/openrl.egg-info/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4554 2023-05-06 12:05:19.000000 openrl-0.0.8/openrl.egg-info/SOURCES.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-05-06 12:05:19.000000 openrl-0.0.8/openrl.egg-info/dependency_links.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-05-06 12:05:19.000000 openrl-0.0.8/openrl.egg-info/entry_points.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)      278 2023-05-06 12:05:19.000000 openrl-0.0.8/openrl.egg-info/requires.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       13 2023-05-06 12:05:19.000000 openrl-0.0.8/openrl.egg-info/top_level.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-05-06 12:05:19.866704 openrl-0.0.8/setup.cfg
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3149 2023-05-06 12:04:43.000000 openrl-0.0.8/setup.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.865592 openrl-0.0.8/tests/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/tests/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.865898 openrl-0.0.8/tests/project/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/tests/project/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      972 2023-04-28 07:15:42.000000 openrl-0.0.8/tests/project/test_version.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-06 12:05:19.866200 openrl-0.0.8/tests/test_buffer/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.8/tests/test_buffer/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1803 2023-04-28 07:15:42.000000 openrl-0.0.8/tests/test_buffer/test_buffer.py
```

### Comparing `openrl-0.0.7/LICENSE` & `openrl-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/LICENSE.txt` & `openrl-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/PKG-INFO` & `openrl-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: openrl
-Version: 0.0.7
-Summary: unified reinforcement learning framework
-Home-page: https://github.com/OpenRL-Lab/openrl
-Author: openrl contributors
-Author-email: huangsy1314@163.com
-Project-URL: Code, https://github.com/OpenRL-Lab/openrl
-Project-URL: Documentation, https://openrl-docs.readthedocs.io/zh/latest/
-Keywords: reinforcement-learning multi-agent reinforcement-learning-algorithms pytorch machine-learning baselines toolbox python data-science gym gymnasium
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: mpe
-Provides-Extra: nlp
-License-File: LICENSE
-License-File: LICENSE.txt
-
 <div align="center">
     <a href="https://openrl-docs.readthedocs.io/zh/latest/index.html"><img width="450px" height="auto" src="./docs/images/openrl_text.png"></a>
 </div>
 
 ---
 [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/openrl/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openrl)
@@ -48,15 +22,17 @@
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl)
 [![GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls)
 [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/blob/master/LICENSE)
 
-OpenRL-v0.0.7 is updated on April 29, 2023 
+OpenRL-v0.0.8 is updated on May 4, 2023 
+
+The main branch is the latest version of OpenRL, which is under active development. If you just want to have a try with OpenRL, you can switch to the stable branch.
 
 ## 欢迎来到OpenRL
 
 [English](./README_en.md) | [中文文档](https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-docs.readthedocs.io/en/latest/)
 
 OpenRL是一个开源的通用强化学习研究框架，支持单智能体、多智能体、自然语言等多种任务的训练。 OpenRL基于PyTorch进行开发，目标是为强化学习研究社区提供一个简单易用、灵活高效、可持续扩展的平台。
 目前，OpenRL支持的特性包括：
@@ -80,20 +56,22 @@
 关于OpenRL的更多信息，请参考[文档](https://openrl-docs.readthedocs.io/zh/latest/)。
 
 ## 目录
 
 - [欢迎来到OpenRL](#欢迎来到openrl)
 - [目录](#目录)
 - [安装](#安装)
+- [使用Docker](#使用docker)
 - [快速上手](#快速上手)
 - [Gallery](#Gallery)
 - [使用OpenRL的项目](#使用OpenRL的项目)
 - [反馈和贡献](#反馈和贡献)
 - [维护人员](#维护人员)
 - [支持者](#支持者)
+  - [&#8627; Contributors](#-contributors)  
   - [&#8627; Stargazers](#-stargazers)
   - [&#8627; Forkers](#-forkers)
 - [Citing OpenRL](#citing-openrl)
 - [License](#license)
 - [Acknowledgments](#acknowledgments)
 
 ## 安装
@@ -104,25 +82,55 @@
 ```
 
 如果用户使用了Anaconda或者Miniconda，也可以通过conda安装OpenRL:
 ```bash
 conda install -c openrl openrl
 ```
 
-用户也可以从源码安装OpenRL:
+想要修改源码的用户也可以从源码安装OpenRL:
 ```bash
-git clone https://github.com/OpenRL-Lab/openrl && cd openrl
+git clone https://github.com/OpenRL-Lab/openrl.git && cd openrl
 pip install -e .
 ```
 
 安装完成后，用户可以直接通过命令行查看OpenRL的版本：
 ```bash
 openrl --version
 ```
 
+## 使用Docker
+
+OpenRL目前也提供了包含显卡支持和非显卡支持的Docker镜像。
+如果用户的电脑上没有英伟达显卡，则可以通过以下命令获取不包含显卡插件的镜像：
+```bash
+sudo docker pull openrllab/openrl-cpu
+```
+
+如果用户想要通过显卡加速训练，则可以通过以下命令获取：
+```bash
+sudo docker pull openrllab/openrl
+```
+
+镜像拉取成功后，用户可以通过以下命令运行OpenRL的Docker镜像：
+```bash
+# 不带显卡加速
+sudo docker run -it openrllab/openrl-cpu
+# 带显卡加速
+sudo docker run -it --gpus all --net host openrllab/openrl
+```
+
+进入Docker镜像后，用户可以通过以下命令查看OpenRL的版本然后运行测例：
+```bash
+# 查看Docker镜像中OpenRL的版本
+openrl --version
+# 运行测例
+openrl --mode train --env CartPole-v1
+```
+
+
 ## 快速上手
 
 OpenRL为强化学习入门用户提供了简单易用的接口，
 下面是一个使用PPO算法训练`CartPole`环境的例子：
 ```python
 # train_ppo.py
 from openrl.envs.common import make
@@ -211,14 +219,20 @@
 - [Shiyu Huang](https://huangshiyu13.github.io/)([@huangshiyu13](https://github.com/huangshiyu13))
 - Wenze Chen([@Chen001117](https://github.com/Chen001117))
 
 欢迎更多的贡献者加入我们的维护团队 (发送邮件到[huangshiyu@4paradigm.com](huangshiyu@4paradigm.com)申请加入OpenRL团队)。
 
 ## 支持者
 
+### &#8627; Contributors
+
+<a href="https://github.com/OpenRL-Lab/openrl/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=OpenRL-Lab/openrl" />
+</a>
+
 ### &#8627; Stargazers
 
 [![Stargazers repo roster for @OpenRL-Lab/openrl](https://reporoster.com/stars/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/stargazers)
 
 ### &#8627; Forkers
 
 [![Forkers repo roster for @OpenRL-Lab/openrl](https://reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network/members)
```

#### html2text {}

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1 Name: openrl Version: 0.0.7 Summary: unified
-reinforcement learning framework Home-page: https://github.com/OpenRL-Lab/
-openrl Author: openrl contributors Author-email: huangsy1314@163.com Project-
-URL: Code, https://github.com/OpenRL-Lab/openrl Project-URL: Documentation,
-https://openrl-docs.readthedocs.io/zh/latest/ Keywords: reinforcement-learning
-multi-agent reinforcement-learning-algorithms pytorch machine-learning
-baselines toolbox python data-science gym gymnasium Classifier: Development
-Status :: 3 - Alpha Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
-Provides-Extra: test Provides-Extra: dev Provides-Extra: mpe Provides-Extra:
-nlp License-File: LICENSE License-File: LICENSE.txt
                         [./docs/images/openrl_text.png]
 --- [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/
 openrl/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 openrl) [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/
 version.svg)](https://anaconda.org/openrl/openrl) [![Anaconda-Server Badge]
 (https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://
 anaconda.org/openrl/openrl) [![Anaconda-Server Badge](https://anaconda.org/
@@ -39,18 +24,20 @@
 img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [![GitHub issues]
 (https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/
 OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/github/
 issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls) [!
 [Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)]
 (https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub license]
 (https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/
-OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.7 is updated on April 29,
-2023 ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£](https://
-openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-
-docs.readthedocs.io/en/latest/
+OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.8 is updated on May 4, 2023
+The main branch is the latest version of OpenRL, which is under active
+development. If you just want to have a try with OpenRL, you can switch to the
+stable branch. ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£]
+(https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://
+openrl-docs.readthedocs.io/en/latest/
 )
 OpenRLæ¯ä¸ä¸ªå¼æºçéç¨å¼ºåå­¦ä¹ ç ç©¶æ¡æ¶ï¼æ¯æåæºè½ä½ãå¤æºè½ä½ãèªç¶è¯­è¨ç­å¤ç§ä»»å¡çè®­ç»ã
 OpenRLåºäºPyTorchè¿è¡å¼åï¼ç®æ æ¯ä¸ºå¼ºåå­¦ä¹ ç ç©¶ç¤¾åºæä¾ä¸ä¸ªç®åæç¨ãçµæ´»é«æãå¯æç»­æ©å±çå¹³å°ã
 ç®åï¼OpenRLæ¯æçç¹æ§åæ¬ï¼ -
 ç®åæç¨ä¸æ¯æåæºè½ä½ãå¤æºè½ä½è®­ç»çéç¨æ¥å£ -
 æ¯æèªç¶è¯­è¨ä»»å¡ï¼å¦å¯¹è¯ä»»å¡ï¼çå¼ºåå­¦ä¹ è®­ç» - æ¯æä»
 [Hugging Face](https://huggingface.co/)ä¸å¯¼å¥æ¨¡ååæ°æ® -
@@ -66,27 +53,39 @@
 Styleåç±»åæ£æ¥ è¯¥æ¡æ¶ç»è¿äº[OpenRL-Lab](https://github.com/OpenRL-
 Lab)çå¤æ¬¡è¿­ä»£å¹¶åºç¨äºå­¦æ¯ç ç©¶ï¼ç®åå·²ç»æä¸ºäºä¸ä¸ªæççå¼ºåå­¦ä¹ æ¡æ¶ã
 OpenRL-Labå°æç»­ç»´æ¤åæ´æ°OpenRLï¼æ¬¢è¿å¤§å®¶å å¥æä»¬ç
 [å¼æºç¤¾åº](./
 CONTRIBUTING.md)ï¼ä¸èµ·ä¸ºå¼ºåå­¦ä¹ çåå±ååºè´¡ç®ã
 å³äºOpenRLçæ´å¤ä¿¡æ¯ï¼è¯·åè[ææ¡£](https://openrl-
 docs.readthedocs.io/zh/latest/)ã ## ç®å½ - [æ¬¢è¿æ¥å°OpenRL]
-(#æ¬¢è¿æ¥å°openrl) - [ç®å½](#ç®å½) - [å®è£](#å®è£) - [å¿«éä¸æ]
-(#å¿«éä¸æ) - [Gallery](#Gallery) - [ä½¿ç¨OpenRLçé¡¹ç®]
-(#ä½¿ç¨OpenRLçé¡¹ç®) - [åé¦åè´¡ç®](#åé¦åè´¡ç®) - [ç»´æ¤äººå]
-(#ç»´æ¤äººå) - [æ¯æè](#æ¯æè) - [↳ Stargazers](#-stargazers) - [↳
-Forkers](#-forkers) - [Citing OpenRL](#citing-openrl) - [License](#license) -
+(#æ¬¢è¿æ¥å°openrl) - [ç®å½](#ç®å½) - [å®è£](#å®è£) - [ä½¿ç¨Docker]
+(#ä½¿ç¨docker) - [å¿«éä¸æ](#å¿«éä¸æ) - [Gallery](#Gallery) -
+[ä½¿ç¨OpenRLçé¡¹ç®](#ä½¿ç¨OpenRLçé¡¹ç®) - [åé¦åè´¡ç®]
+(#åé¦åè´¡ç®) - [ç»´æ¤äººå](#ç»´æ¤äººå) - [æ¯æè](#æ¯æè) -
+[↳ Contributors](#-contributors) - [↳ Stargazers](#-stargazers) - [↳ Forkers]
+(#-forkers) - [Citing OpenRL](#citing-openrl) - [License](#license) -
 [Acknowledgments](#acknowledgments) ## å®è£
 ç¨æ·å¯ä»¥ç´æ¥éè¿pipå®è£OpenRL: ```bash pip install openrl ```
 å¦æç¨æ·ä½¿ç¨äºAnacondaæèMinicondaï¼ä¹å¯ä»¥éè¿condaå®è£OpenRL:
 ```bash conda install -c openrl openrl ```
-ç¨æ·ä¹å¯ä»¥ä»æºç å®è£OpenRL: ```bash git clone https://github.com/
-OpenRL-Lab/openrl && cd openrl pip install -e . ```
+æ³è¦ä¿®æ¹æºç çç¨æ·ä¹å¯ä»¥ä»æºç å®è£OpenRL: ```bash git clone
+https://github.com/OpenRL-Lab/openrl.git && cd openrl pip install -e . ```
 å®è£å®æåï¼ç¨æ·å¯ä»¥ç´æ¥éè¿å½ä»¤è¡æ¥çOpenRLççæ¬ï¼
-```bash openrl --version ``` ## å¿«éä¸æ
+```bash openrl --version ``` ## ä½¿ç¨Docker
+OpenRLç®åä¹æä¾äºåå«æ¾å¡æ¯æåéæ¾å¡æ¯æçDockeréåã
+å¦æç¨æ·ççµèä¸æ²¡æè±ä¼è¾¾æ¾å¡ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åä¸åå«æ¾å¡æä»¶çéåï¼
+```bash sudo docker pull openrllab/openrl-cpu ```
+å¦æç¨æ·æ³è¦éè¿æ¾å¡å éè®­ç»ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åï¼
+```bash sudo docker pull openrllab/openrl ```
+éåæåæååï¼ç¨æ·å¯ä»¥éè¿ä»¥ä¸å½ä»¤è¿è¡OpenRLçDockeréåï¼
+```bash # ä¸å¸¦æ¾å¡å é sudo docker run -it openrllab/openrl-cpu #
+å¸¦æ¾å¡å é sudo docker run -it --gpus all --net host openrllab/openrl ```
+è¿å¥Dockeréååï¼ç¨æ·å¯ä»¥éè¿ä»¥ä¸å½ä»¤æ¥çOpenRLççæ¬ç¶åè¿è¡æµä¾ï¼
+```bash # æ¥çDockeréåä¸­OpenRLççæ¬ openrl --version # è¿è¡æµä¾
+openrl --mode train --env CartPole-v1 ``` ## å¿«éä¸æ
 OpenRLä¸ºå¼ºåå­¦ä¹ å¥é¨ç¨æ·æä¾äºç®åæç¨çæ¥å£ï¼
 ä¸é¢æ¯ä¸ä¸ªä½¿ç¨PPOç®æ³è®­ç»`CartPole`ç¯å¢çä¾å­ï¼ ```python #
 train_ppo.py from openrl.envs.common import make from openrl.modules.common
 import PPONet as Net from openrl.runners.common import PPOAgent as Agent env =
 make("CartPole-v1", env_num=9) # åå»ºç¯å¢ï¼å¹¶è®¾ç½®ç¯å¢å¹¶è¡æ°ä¸º9
 net = Net(env) # åå»ºç¥ç»ç½ç» agent = Agent(net) # åå§åæºè½ä½
 agent.train(total_time_steps=20000) #
@@ -142,14 +141,15 @@
 [OpenRLå¼åè®¡å](https://github.com/OpenRL-Lab/openrl/issues/2) ##
 ç»´æ¤äººå ç®åï¼OpenRLç±ä»¥ä¸ç»´æ¤äººåç»´æ¤ï¼ - [Shiyu Huang]
 (https://huangshiyu13.github.io/)([@huangshiyu13](https://github.com/
 huangshiyu13)) - Wenze Chen([@Chen001117](https://github.com/Chen001117))
 æ¬¢è¿æ´å¤çè´¡ç®èå å¥æä»¬çç»´æ¤å¢é (åéé®ä»¶å°
 [huangshiyu@4paradigm.com]
 (huangshiyu@4paradigm.com)ç³è¯·å å¥OpenRLå¢é)ã ## æ¯æè ### ↳
+Contributors [https://contrib.rocks/image?repo=OpenRL-Lab/openrl] ### ↳
 Stargazers [![Stargazers repo roster for @OpenRL-Lab/openrl](https://
 reporoster.com/stars/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/
 stargazers) ### ↳ Forkers [![Forkers repo roster for @OpenRL-Lab/openrl](https:
 //reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/
 openrl/network/members) ## Citing OpenRL
 å¦ææä»¬çå·¥ä½å¯¹ä½ æå¸®å©ï¼æ¬¢è¿å¼ç¨æä»¬: ```latex @misc
 {openrl2023, title={OpenRL}, author={OpenRL Contributors}, publisher =
```

### Comparing `openrl-0.0.7/README.md` & `openrl-0.0.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: openrl
+Version: 0.0.8
+Summary: unified reinforcement learning framework
+Home-page: https://github.com/OpenRL-Lab/openrl
+Author: openrl contributors
+Author-email: huangsy1314@163.com
+Project-URL: Code, https://github.com/OpenRL-Lab/openrl
+Project-URL: Documentation, https://openrl-docs.readthedocs.io/zh/latest/
+Keywords: reinforcement-learning multi-agent reinforcement-learning-algorithms pytorch machine-learning baselines toolbox python data-science gym gymnasium
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: mpe
+Provides-Extra: nlp
+License-File: LICENSE
+License-File: LICENSE.txt
+
 <div align="center">
     <a href="https://openrl-docs.readthedocs.io/zh/latest/index.html"><img width="450px" height="auto" src="./docs/images/openrl_text.png"></a>
 </div>
 
 ---
 [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/openrl/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openrl)
@@ -22,15 +49,17 @@
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl)
 [![GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls)
 [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/blob/master/LICENSE)
 
-OpenRL-v0.0.7 is updated on April 29, 2023 
+OpenRL-v0.0.8 is updated on May 4, 2023 
+
+The main branch is the latest version of OpenRL, which is under active development. If you just want to have a try with OpenRL, you can switch to the stable branch.
 
 ## 欢迎来到OpenRL
 
 [English](./README_en.md) | [中文文档](https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-docs.readthedocs.io/en/latest/)
 
 OpenRL是一个开源的通用强化学习研究框架，支持单智能体、多智能体、自然语言等多种任务的训练。 OpenRL基于PyTorch进行开发，目标是为强化学习研究社区提供一个简单易用、灵活高效、可持续扩展的平台。
 目前，OpenRL支持的特性包括：
@@ -54,20 +83,22 @@
 关于OpenRL的更多信息，请参考[文档](https://openrl-docs.readthedocs.io/zh/latest/)。
 
 ## 目录
 
 - [欢迎来到OpenRL](#欢迎来到openrl)
 - [目录](#目录)
 - [安装](#安装)
+- [使用Docker](#使用docker)
 - [快速上手](#快速上手)
 - [Gallery](#Gallery)
 - [使用OpenRL的项目](#使用OpenRL的项目)
 - [反馈和贡献](#反馈和贡献)
 - [维护人员](#维护人员)
 - [支持者](#支持者)
+  - [&#8627; Contributors](#-contributors)  
   - [&#8627; Stargazers](#-stargazers)
   - [&#8627; Forkers](#-forkers)
 - [Citing OpenRL](#citing-openrl)
 - [License](#license)
 - [Acknowledgments](#acknowledgments)
 
 ## 安装
@@ -78,25 +109,55 @@
 ```
 
 如果用户使用了Anaconda或者Miniconda，也可以通过conda安装OpenRL:
 ```bash
 conda install -c openrl openrl
 ```
 
-用户也可以从源码安装OpenRL:
+想要修改源码的用户也可以从源码安装OpenRL:
 ```bash
-git clone https://github.com/OpenRL-Lab/openrl && cd openrl
+git clone https://github.com/OpenRL-Lab/openrl.git && cd openrl
 pip install -e .
 ```
 
 安装完成后，用户可以直接通过命令行查看OpenRL的版本：
 ```bash
 openrl --version
 ```
 
+## 使用Docker
+
+OpenRL目前也提供了包含显卡支持和非显卡支持的Docker镜像。
+如果用户的电脑上没有英伟达显卡，则可以通过以下命令获取不包含显卡插件的镜像：
+```bash
+sudo docker pull openrllab/openrl-cpu
+```
+
+如果用户想要通过显卡加速训练，则可以通过以下命令获取：
+```bash
+sudo docker pull openrllab/openrl
+```
+
+镜像拉取成功后，用户可以通过以下命令运行OpenRL的Docker镜像：
+```bash
+# 不带显卡加速
+sudo docker run -it openrllab/openrl-cpu
+# 带显卡加速
+sudo docker run -it --gpus all --net host openrllab/openrl
+```
+
+进入Docker镜像后，用户可以通过以下命令查看OpenRL的版本然后运行测例：
+```bash
+# 查看Docker镜像中OpenRL的版本
+openrl --version
+# 运行测例
+openrl --mode train --env CartPole-v1
+```
+
+
 ## 快速上手
 
 OpenRL为强化学习入门用户提供了简单易用的接口，
 下面是一个使用PPO算法训练`CartPole`环境的例子：
 ```python
 # train_ppo.py
 from openrl.envs.common import make
@@ -185,14 +246,20 @@
 - [Shiyu Huang](https://huangshiyu13.github.io/)([@huangshiyu13](https://github.com/huangshiyu13))
 - Wenze Chen([@Chen001117](https://github.com/Chen001117))
 
 欢迎更多的贡献者加入我们的维护团队 (发送邮件到[huangshiyu@4paradigm.com](huangshiyu@4paradigm.com)申请加入OpenRL团队)。
 
 ## 支持者
 
+### &#8627; Contributors
+
+<a href="https://github.com/OpenRL-Lab/openrl/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=OpenRL-Lab/openrl" />
+</a>
+
 ### &#8627; Stargazers
 
 [![Stargazers repo roster for @OpenRL-Lab/openrl](https://reporoster.com/stars/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/stargazers)
 
 ### &#8627; Forkers
 
 [![Forkers repo roster for @OpenRL-Lab/openrl](https://reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network/members)
```

#### html2text {}

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1 Name: openrl Version: 0.0.8 Summary: unified
+reinforcement learning framework Home-page: https://github.com/OpenRL-Lab/
+openrl Author: openrl contributors Author-email: huangsy1314@163.com Project-
+URL: Code, https://github.com/OpenRL-Lab/openrl Project-URL: Documentation,
+https://openrl-docs.readthedocs.io/zh/latest/ Keywords: reinforcement-learning
+multi-agent reinforcement-learning-algorithms pytorch machine-learning
+baselines toolbox python data-science gym gymnasium Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Science/
+Research Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Operating System :: OS Independent Requires-
+Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: test
+Provides-Extra: dev Provides-Extra: mpe Provides-Extra: nlp License-File:
+LICENSE License-File: LICENSE.txt
                         [./docs/images/openrl_text.png]
 --- [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/
 openrl/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 openrl) [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/
 version.svg)](https://anaconda.org/openrl/openrl) [![Anaconda-Server Badge]
 (https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://
 anaconda.org/openrl/openrl) [![Anaconda-Server Badge](https://anaconda.org/
@@ -24,18 +40,20 @@
 img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [![GitHub issues]
 (https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/
 OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/github/
 issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls) [!
 [Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)]
 (https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub license]
 (https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/
-OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.7 is updated on April 29,
-2023 ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£](https://
-openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-
-docs.readthedocs.io/en/latest/
+OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.8 is updated on May 4, 2023
+The main branch is the latest version of OpenRL, which is under active
+development. If you just want to have a try with OpenRL, you can switch to the
+stable branch. ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£]
+(https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://
+openrl-docs.readthedocs.io/en/latest/
 )
 OpenRLæ¯ä¸ä¸ªå¼æºçéç¨å¼ºåå­¦ä¹ ç ç©¶æ¡æ¶ï¼æ¯æåæºè½ä½ãå¤æºè½ä½ãèªç¶è¯­è¨ç­å¤ç§ä»»å¡çè®­ç»ã
 OpenRLåºäºPyTorchè¿è¡å¼åï¼ç®æ æ¯ä¸ºå¼ºåå­¦ä¹ ç ç©¶ç¤¾åºæä¾ä¸ä¸ªç®åæç¨ãçµæ´»é«æãå¯æç»­æ©å±çå¹³å°ã
 ç®åï¼OpenRLæ¯æçç¹æ§åæ¬ï¼ -
 ç®åæç¨ä¸æ¯æåæºè½ä½ãå¤æºè½ä½è®­ç»çéç¨æ¥å£ -
 æ¯æèªç¶è¯­è¨ä»»å¡ï¼å¦å¯¹è¯ä»»å¡ï¼çå¼ºåå­¦ä¹ è®­ç» - æ¯æä»
 [Hugging Face](https://huggingface.co/)ä¸å¯¼å¥æ¨¡ååæ°æ® -
@@ -51,27 +69,39 @@
 Styleåç±»åæ£æ¥ è¯¥æ¡æ¶ç»è¿äº[OpenRL-Lab](https://github.com/OpenRL-
 Lab)çå¤æ¬¡è¿­ä»£å¹¶åºç¨äºå­¦æ¯ç ç©¶ï¼ç®åå·²ç»æä¸ºäºä¸ä¸ªæççå¼ºåå­¦ä¹ æ¡æ¶ã
 OpenRL-Labå°æç»­ç»´æ¤åæ´æ°OpenRLï¼æ¬¢è¿å¤§å®¶å å¥æä»¬ç
 [å¼æºç¤¾åº](./
 CONTRIBUTING.md)ï¼ä¸èµ·ä¸ºå¼ºåå­¦ä¹ çåå±ååºè´¡ç®ã
 å³äºOpenRLçæ´å¤ä¿¡æ¯ï¼è¯·åè[ææ¡£](https://openrl-
 docs.readthedocs.io/zh/latest/)ã ## ç®å½ - [æ¬¢è¿æ¥å°OpenRL]
-(#æ¬¢è¿æ¥å°openrl) - [ç®å½](#ç®å½) - [å®è£](#å®è£) - [å¿«éä¸æ]
-(#å¿«éä¸æ) - [Gallery](#Gallery) - [ä½¿ç¨OpenRLçé¡¹ç®]
-(#ä½¿ç¨OpenRLçé¡¹ç®) - [åé¦åè´¡ç®](#åé¦åè´¡ç®) - [ç»´æ¤äººå]
-(#ç»´æ¤äººå) - [æ¯æè](#æ¯æè) - [↳ Stargazers](#-stargazers) - [↳
-Forkers](#-forkers) - [Citing OpenRL](#citing-openrl) - [License](#license) -
+(#æ¬¢è¿æ¥å°openrl) - [ç®å½](#ç®å½) - [å®è£](#å®è£) - [ä½¿ç¨Docker]
+(#ä½¿ç¨docker) - [å¿«éä¸æ](#å¿«éä¸æ) - [Gallery](#Gallery) -
+[ä½¿ç¨OpenRLçé¡¹ç®](#ä½¿ç¨OpenRLçé¡¹ç®) - [åé¦åè´¡ç®]
+(#åé¦åè´¡ç®) - [ç»´æ¤äººå](#ç»´æ¤äººå) - [æ¯æè](#æ¯æè) -
+[↳ Contributors](#-contributors) - [↳ Stargazers](#-stargazers) - [↳ Forkers]
+(#-forkers) - [Citing OpenRL](#citing-openrl) - [License](#license) -
 [Acknowledgments](#acknowledgments) ## å®è£
 ç¨æ·å¯ä»¥ç´æ¥éè¿pipå®è£OpenRL: ```bash pip install openrl ```
 å¦æç¨æ·ä½¿ç¨äºAnacondaæèMinicondaï¼ä¹å¯ä»¥éè¿condaå®è£OpenRL:
 ```bash conda install -c openrl openrl ```
-ç¨æ·ä¹å¯ä»¥ä»æºç å®è£OpenRL: ```bash git clone https://github.com/
-OpenRL-Lab/openrl && cd openrl pip install -e . ```
+æ³è¦ä¿®æ¹æºç çç¨æ·ä¹å¯ä»¥ä»æºç å®è£OpenRL: ```bash git clone
+https://github.com/OpenRL-Lab/openrl.git && cd openrl pip install -e . ```
 å®è£å®æåï¼ç¨æ·å¯ä»¥ç´æ¥éè¿å½ä»¤è¡æ¥çOpenRLççæ¬ï¼
-```bash openrl --version ``` ## å¿«éä¸æ
+```bash openrl --version ``` ## ä½¿ç¨Docker
+OpenRLç®åä¹æä¾äºåå«æ¾å¡æ¯æåéæ¾å¡æ¯æçDockeréåã
+å¦æç¨æ·ççµèä¸æ²¡æè±ä¼è¾¾æ¾å¡ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åä¸åå«æ¾å¡æä»¶çéåï¼
+```bash sudo docker pull openrllab/openrl-cpu ```
+å¦æç¨æ·æ³è¦éè¿æ¾å¡å éè®­ç»ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åï¼
+```bash sudo docker pull openrllab/openrl ```
+éåæåæååï¼ç¨æ·å¯ä»¥éè¿ä»¥ä¸å½ä»¤è¿è¡OpenRLçDockeréåï¼
+```bash # ä¸å¸¦æ¾å¡å é sudo docker run -it openrllab/openrl-cpu #
+å¸¦æ¾å¡å é sudo docker run -it --gpus all --net host openrllab/openrl ```
+è¿å¥Dockeréååï¼ç¨æ·å¯ä»¥éè¿ä»¥ä¸å½ä»¤æ¥çOpenRLççæ¬ç¶åè¿è¡æµä¾ï¼
+```bash # æ¥çDockeréåä¸­OpenRLççæ¬ openrl --version # è¿è¡æµä¾
+openrl --mode train --env CartPole-v1 ``` ## å¿«éä¸æ
 OpenRLä¸ºå¼ºåå­¦ä¹ å¥é¨ç¨æ·æä¾äºç®åæç¨çæ¥å£ï¼
 ä¸é¢æ¯ä¸ä¸ªä½¿ç¨PPOç®æ³è®­ç»`CartPole`ç¯å¢çä¾å­ï¼ ```python #
 train_ppo.py from openrl.envs.common import make from openrl.modules.common
 import PPONet as Net from openrl.runners.common import PPOAgent as Agent env =
 make("CartPole-v1", env_num=9) # åå»ºç¯å¢ï¼å¹¶è®¾ç½®ç¯å¢å¹¶è¡æ°ä¸º9
 net = Net(env) # åå»ºç¥ç»ç½ç» agent = Agent(net) # åå§åæºè½ä½
 agent.train(total_time_steps=20000) #
@@ -127,14 +157,15 @@
 [OpenRLå¼åè®¡å](https://github.com/OpenRL-Lab/openrl/issues/2) ##
 ç»´æ¤äººå ç®åï¼OpenRLç±ä»¥ä¸ç»´æ¤äººåç»´æ¤ï¼ - [Shiyu Huang]
 (https://huangshiyu13.github.io/)([@huangshiyu13](https://github.com/
 huangshiyu13)) - Wenze Chen([@Chen001117](https://github.com/Chen001117))
 æ¬¢è¿æ´å¤çè´¡ç®èå å¥æä»¬çç»´æ¤å¢é (åéé®ä»¶å°
 [huangshiyu@4paradigm.com]
 (huangshiyu@4paradigm.com)ç³è¯·å å¥OpenRLå¢é)ã ## æ¯æè ### ↳
+Contributors [https://contrib.rocks/image?repo=OpenRL-Lab/openrl] ### ↳
 Stargazers [![Stargazers repo roster for @OpenRL-Lab/openrl](https://
 reporoster.com/stars/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/
 stargazers) ### ↳ Forkers [![Forkers repo roster for @OpenRL-Lab/openrl](https:
 //reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/
 openrl/network/members) ## Citing OpenRL
 å¦ææä»¬çå·¥ä½å¯¹ä½ æå¸®å©ï¼æ¬¢è¿å¼ç¨æä»¬: ```latex @misc
 {openrl2023, title={OpenRL}, author={OpenRL Contributors}, publisher =
```

### Comparing `openrl-0.0.7/openrl/algorithms/__init__.py` & `openrl-0.0.8/openrl/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/algorithms/base_algorithm.py` & `openrl-0.0.8/openrl/algorithms/base_algorithm.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/algorithms/ppo.py` & `openrl-0.0.8/openrl/algorithms/ppo.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/buffers/__init__.py` & `openrl-0.0.8/openrl/buffers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/buffers/normal_buffer.py` & `openrl-0.0.8/openrl/buffers/normal_buffer.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/buffers/replay_data.py` & `openrl-0.0.8/openrl/buffers/replay_data.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/buffers/utils/__init__.py` & `openrl-0.0.8/openrl/buffers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/buffers/utils/obs_data.py` & `openrl-0.0.8/openrl/buffers/utils/obs_data.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/buffers/utils/util.py` & `openrl-0.0.8/openrl/buffers/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/cli/__init__.py` & `openrl-0.0.8/openrl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/cli/cli.py` & `openrl-0.0.8/openrl/cli/cli.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/cli/train.py` & `openrl-0.0.8/openrl/cli/train.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/configs/__init__.py` & `openrl-0.0.8/openrl/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/configs/config.py` & `openrl-0.0.8/openrl/configs/config.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/drivers/__init__.py` & `openrl-0.0.8/openrl/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/drivers/onpolicy_driver.py` & `openrl-0.0.8/openrl/drivers/onpolicy_driver.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/drivers/rl_driver.py` & `openrl-0.0.8/openrl/drivers/rl_driver.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/common/__init__.py` & `openrl-0.0.8/openrl/envs/common/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/common/build_envs.py` & `openrl-0.0.8/openrl/envs/common/build_envs.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/common/registration.py` & `openrl-0.0.8/openrl/envs/common/registration.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/gymnasium/__init__.py` & `openrl-0.0.8/openrl/envs/gymnasium/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/mpe/__init__.py` & `openrl-0.0.8/openrl/envs/mpe/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/mpe/core.py` & `openrl-0.0.8/openrl/envs/mpe/core.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/mpe/mpe_env.py` & `openrl-0.0.8/openrl/envs/mpe/mpe_env.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/mpe/multi_discrete.py` & `openrl-0.0.8/openrl/envs/mpe/multi_discrete.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/mpe/multiagent_env.py` & `openrl-0.0.8/openrl/envs/mpe/multiagent_env.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/mpe/rendering.py` & `openrl-0.0.8/openrl/envs/mpe/rendering.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/mpe/scenarios/simple_spread.py` & `openrl-0.0.8/openrl/envs/mpe/scenarios/simple_spread.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/nlp/__init__.py` & `openrl-0.0.8/openrl/envs/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/nlp/daily_dialog_env.py` & `openrl-0.0.8/openrl/envs/nlp/daily_dialog_env.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/nlp/utils/custom_text_generation_pools.py` & `openrl-0.0.8/openrl/envs/nlp/utils/custom_text_generation_pools.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/nlp/utils/distribution.py` & `openrl-0.0.8/openrl/envs/nlp/utils/distribution.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/nlp/utils/evaluation_utils.py` & `openrl-0.0.8/openrl/envs/nlp/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/nlp/utils/metrics/__init__.py` & `openrl-0.0.8/openrl/envs/nlp/utils/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/nlp/utils/metrics/meteor.py` & `openrl-0.0.8/openrl/envs/nlp/utils/metrics/meteor.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/nlp/utils/observation.py` & `openrl-0.0.8/openrl/envs/nlp/utils/observation.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/nlp/utils/sampler.py` & `openrl-0.0.8/openrl/envs/nlp/utils/sampler.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/nlp/utils/text_generation_pool.py` & `openrl-0.0.8/openrl/envs/nlp/utils/text_generation_pool.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/vec_env/async_venv.py` & `openrl-0.0.8/openrl/envs/vec_env/async_venv.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/vec_env/base_venv.py` & `openrl-0.0.8/openrl/envs/vec_env/base_venv.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/vec_env/sync_venv.py` & `openrl-0.0.8/openrl/envs/vec_env/sync_venv.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/vec_env/utils/__init__.py` & `openrl-0.0.8/openrl/envs/vec_env/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/vec_env/utils/numpy_utils.py` & `openrl-0.0.8/openrl/envs/vec_env/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/vec_env/utils/share_memory.py` & `openrl-0.0.8/openrl/envs/vec_env/utils/share_memory.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/vec_env/utils/util.py` & `openrl-0.0.8/openrl/envs/vec_env/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/vec_env/vec_info/__init__.py` & `openrl-0.0.8/openrl/envs/vec_env/vec_info/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/vec_env/vec_info/base_vec_info.py` & `openrl-0.0.8/openrl/envs/vec_env/vec_info/base_vec_info.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/vec_env/vec_info/nlp_vec_info.py` & `openrl-0.0.8/openrl/envs/vec_env/vec_info/nlp_vec_info.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/vec_env/vec_info/simple_vec_info.py` & `openrl-0.0.8/openrl/envs/vec_env/vec_info/simple_vec_info.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/vec_env/wrappers/__init__.py` & `openrl-0.0.8/openrl/envs/vec_env/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/vec_env/wrappers/base_wrapper.py` & `openrl-0.0.8/openrl/envs/vec_env/wrappers/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/vec_env/wrappers/reward_wrapper.py` & `openrl-0.0.8/openrl/envs/vec_env/wrappers/reward_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py` & `openrl-0.0.8/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/wrappers/base_wrapper.py` & `openrl-0.0.8/openrl/envs/wrappers/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/wrappers/extra_wrappers.py` & `openrl-0.0.8/openrl/envs/wrappers/extra_wrappers.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/wrappers/multiagent_wrapper.py` & `openrl-0.0.8/openrl/envs/wrappers/multiagent_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/envs/wrappers/util.py` & `openrl-0.0.8/openrl/envs/wrappers/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/__init__.py` & `openrl-0.0.8/openrl/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/base_module.py` & `openrl-0.0.8/openrl/modules/base_module.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/common/base_net.py` & `openrl-0.0.8/openrl/modules/common/base_net.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/common/ppo_net.py` & `openrl-0.0.8/openrl/modules/common/ppo_net.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/model_config.py` & `openrl-0.0.8/openrl/modules/model_config.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/__init__.py` & `openrl-0.0.8/openrl/modules/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/base_policy_network.py` & `openrl-0.0.8/openrl/modules/networks/base_policy_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/base_value_network.py` & `openrl-0.0.8/openrl/modules/networks/base_value_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/policy_network.py` & `openrl-0.0.8/openrl/modules/networks/policy_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/policy_value_network.py` & `openrl-0.0.8/openrl/modules/networks/policy_value_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/policy_value_network_gpt.py` & `openrl-0.0.8/openrl/modules/networks/policy_value_network_gpt.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/utils/act.py` & `openrl-0.0.8/openrl/modules/networks/utils/act.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/utils/attention.py` & `openrl-0.0.8/openrl/modules/networks/utils/attention.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/utils/cnn.py` & `openrl-0.0.8/openrl/modules/networks/utils/cnn.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/utils/distributed_utils.py` & `openrl-0.0.8/openrl/modules/networks/utils/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/utils/distributions.py` & `openrl-0.0.8/openrl/modules/networks/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/utils/mix.py` & `openrl-0.0.8/openrl/modules/networks/utils/mix.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/utils/mlp.py` & `openrl-0.0.8/openrl/modules/networks/utils/mlp.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/utils/nlp/base_policy.py` & `openrl-0.0.8/openrl/modules/networks/utils/nlp/base_policy.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/utils/nlp/causal_policy.py` & `openrl-0.0.8/openrl/modules/networks/utils/nlp/causal_policy.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/utils/nlp/hf_generation_utils.py` & `openrl-0.0.8/openrl/modules/networks/utils/nlp/hf_generation_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/utils/popart.py` & `openrl-0.0.8/openrl/modules/networks/utils/popart.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/utils/rnn.py` & `openrl-0.0.8/openrl/modules/networks/utils/rnn.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/utils/transformer_act.py` & `openrl-0.0.8/openrl/modules/networks/utils/transformer_act.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/networks/value_network.py` & `openrl-0.0.8/openrl/modules/networks/value_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/ppo_module.py` & `openrl-0.0.8/openrl/modules/ppo_module.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/rl_module.py` & `openrl-0.0.8/openrl/modules/rl_module.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/utils/__init__.py` & `openrl-0.0.8/openrl/modules/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/utils/util.py` & `openrl-0.0.8/openrl/modules/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/modules/utils/valuenorm.py` & `openrl-0.0.8/openrl/modules/utils/valuenorm.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/rewards/__init__.py` & `openrl-0.0.8/openrl/rewards/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/rewards/base_reward.py` & `openrl-0.0.8/openrl/rewards/base_reward.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,16 @@
         self.step_reward_fn = dict()
         self.inner_reward_fn = dict()
         self.batch_reward_fn = dict()
 
     def step_reward(
         self, data: Dict[str, Any]
     ) -> Union[np.ndarray, List[Dict[str, Any]]]:
-        
         rewards = data["rewards"].copy()
         infos = [dict() for _ in range(rewards.shape[0])]
 
         return rewards, infos
 
     def batch_rewards(self, buffer: Any) -> Dict[str, Any]:
-        
         infos = dict()
 
         return infos
```

### Comparing `openrl-0.0.7/openrl/rewards/nlp_reward.py` & `openrl-0.0.8/openrl/rewards/nlp_reward.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/runners/__init__.py` & `openrl-0.0.8/openrl/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/runners/common/base_agent.py` & `openrl-0.0.8/openrl/runners/common/base_agent.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/runners/common/chat_agent.py` & `openrl-0.0.8/openrl/runners/common/chat_agent.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import io
 import pathlib
 from typing import List, Optional, Type, Union
 
+import numpy as np
 import torch
 
 from openrl.runners.common.base_agent import BaseAgent, SelfAgent
 
 
 class ChatAgent(BaseAgent):
     def __init__(self, model, tokenizer, device=None):
@@ -94,7 +95,33 @@
         return response
 
     def save(
         self,
         path: Union[str, pathlib.Path, io.BufferedIOBase],
     ) -> None:
         pass
+
+
+class Chat6BAgent(ChatAgent):
+    @classmethod
+    def load(
+        cls: Type[SelfAgent],
+        agent_path: Union[str, pathlib.Path, io.BufferedIOBase],
+        device="cuda:0",
+    ) -> SelfAgent:
+        from transformers import AutoModel, AutoTokenizer
+
+        tokenizer = AutoTokenizer.from_pretrained(agent_path, trust_remote_code=True)
+        model = (
+            AutoModel.from_pretrained(agent_path, trust_remote_code=True)
+            .half()
+            .cuda(device)
+        )
+        model.eval()
+        return cls(model, tokenizer, device)
+
+    def chat(self, input: str, history: List[str]):
+        new_history = np.reshape(history, (-1, 2)).tolist()
+        response, _ = self.model.chat(
+            self.tokenizer, input, history=new_history, do_sample=False
+        )
+        return response
```

### Comparing `openrl-0.0.7/openrl/runners/common/ppo_agent.py` & `openrl-0.0.8/openrl/runners/common/ppo_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,16 @@
         if run_dir is None:
             self.run_dir = self._cfg.run_dir
         else:
             self.run_dir = run_dir
 
         if self.run_dir is None:
             assert (not self._use_wandb) and (not self._use_tensorboard), (
-                "log_path must be set when using wandb or tensorboard.Please set"
-                " log_path in PPOAgent or in the config file or pass run_dir in the"
+                "run_dir must be set when using wandb or tensorboard. Please set"
+                " run_dir in the config file or pass run_dir in the"
                 " command line."
             )
 
         if self._cfg.experiment_name == "":
             self.exp_name = "ppo"
         else:
             self.exp_name = self._cfg.experiment_name
```

### Comparing `openrl-0.0.7/openrl/supports/__init__.py` & `openrl-0.0.8/openrl/supports/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/supports/opendata/__init__.py` & `openrl-0.0.8/openrl/supports/opendata/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/supports/opendata/utils/__init__.py` & `openrl-0.0.8/openrl/supports/opendata/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/supports/opendata/utils/opendata_utils.py` & `openrl-0.0.8/openrl/supports/opendata/utils/opendata_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/supports/opengpu/__init__.py` & `openrl-0.0.8/openrl/supports/opengpu/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/supports/opengpu/gpu_info.py` & `openrl-0.0.8/openrl/supports/opengpu/gpu_info.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/supports/opengpu/manager.py` & `openrl-0.0.8/openrl/supports/opengpu/manager.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -190,8 +190,8 @@
             return None
 
     def log_info(self):
         if self.args and self.args.disable_cuda:
             return
 
         for gpu in self.gpus:
-            print(gpu)
+            print(gpu)
```

### Comparing `openrl-0.0.7/openrl/utils/__init__.py` & `openrl-0.0.8/openrl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/utils/logger.py` & `openrl-0.0.8/openrl/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl/utils/util.py` & `openrl-0.0.8/openrl/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/openrl.egg-info/PKG-INFO` & `openrl-0.0.8/openrl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: openrl
-Version: 0.0.7
+Version: 0.0.8
 Summary: unified reinforcement learning framework
 Home-page: https://github.com/OpenRL-Lab/openrl
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openrl
 Project-URL: Documentation, https://openrl-docs.readthedocs.io/zh/latest/
 Keywords: reinforcement-learning multi-agent reinforcement-learning-algorithms pytorch machine-learning baselines toolbox python data-science gym gymnasium
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: mpe
@@ -48,15 +49,17 @@
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl)
 [![GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls)
 [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/blob/master/LICENSE)
 
-OpenRL-v0.0.7 is updated on April 29, 2023 
+OpenRL-v0.0.8 is updated on May 4, 2023 
+
+The main branch is the latest version of OpenRL, which is under active development. If you just want to have a try with OpenRL, you can switch to the stable branch.
 
 ## 欢迎来到OpenRL
 
 [English](./README_en.md) | [中文文档](https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-docs.readthedocs.io/en/latest/)
 
 OpenRL是一个开源的通用强化学习研究框架，支持单智能体、多智能体、自然语言等多种任务的训练。 OpenRL基于PyTorch进行开发，目标是为强化学习研究社区提供一个简单易用、灵活高效、可持续扩展的平台。
 目前，OpenRL支持的特性包括：
@@ -80,20 +83,22 @@
 关于OpenRL的更多信息，请参考[文档](https://openrl-docs.readthedocs.io/zh/latest/)。
 
 ## 目录
 
 - [欢迎来到OpenRL](#欢迎来到openrl)
 - [目录](#目录)
 - [安装](#安装)
+- [使用Docker](#使用docker)
 - [快速上手](#快速上手)
 - [Gallery](#Gallery)
 - [使用OpenRL的项目](#使用OpenRL的项目)
 - [反馈和贡献](#反馈和贡献)
 - [维护人员](#维护人员)
 - [支持者](#支持者)
+  - [&#8627; Contributors](#-contributors)  
   - [&#8627; Stargazers](#-stargazers)
   - [&#8627; Forkers](#-forkers)
 - [Citing OpenRL](#citing-openrl)
 - [License](#license)
 - [Acknowledgments](#acknowledgments)
 
 ## 安装
@@ -104,25 +109,55 @@
 ```
 
 如果用户使用了Anaconda或者Miniconda，也可以通过conda安装OpenRL:
 ```bash
 conda install -c openrl openrl
 ```
 
-用户也可以从源码安装OpenRL:
+想要修改源码的用户也可以从源码安装OpenRL:
 ```bash
-git clone https://github.com/OpenRL-Lab/openrl && cd openrl
+git clone https://github.com/OpenRL-Lab/openrl.git && cd openrl
 pip install -e .
 ```
 
 安装完成后，用户可以直接通过命令行查看OpenRL的版本：
 ```bash
 openrl --version
 ```
 
+## 使用Docker
+
+OpenRL目前也提供了包含显卡支持和非显卡支持的Docker镜像。
+如果用户的电脑上没有英伟达显卡，则可以通过以下命令获取不包含显卡插件的镜像：
+```bash
+sudo docker pull openrllab/openrl-cpu
+```
+
+如果用户想要通过显卡加速训练，则可以通过以下命令获取：
+```bash
+sudo docker pull openrllab/openrl
+```
+
+镜像拉取成功后，用户可以通过以下命令运行OpenRL的Docker镜像：
+```bash
+# 不带显卡加速
+sudo docker run -it openrllab/openrl-cpu
+# 带显卡加速
+sudo docker run -it --gpus all --net host openrllab/openrl
+```
+
+进入Docker镜像后，用户可以通过以下命令查看OpenRL的版本然后运行测例：
+```bash
+# 查看Docker镜像中OpenRL的版本
+openrl --version
+# 运行测例
+openrl --mode train --env CartPole-v1
+```
+
+
 ## 快速上手
 
 OpenRL为强化学习入门用户提供了简单易用的接口，
 下面是一个使用PPO算法训练`CartPole`环境的例子：
 ```python
 # train_ppo.py
 from openrl.envs.common import make
@@ -211,14 +246,20 @@
 - [Shiyu Huang](https://huangshiyu13.github.io/)([@huangshiyu13](https://github.com/huangshiyu13))
 - Wenze Chen([@Chen001117](https://github.com/Chen001117))
 
 欢迎更多的贡献者加入我们的维护团队 (发送邮件到[huangshiyu@4paradigm.com](huangshiyu@4paradigm.com)申请加入OpenRL团队)。
 
 ## 支持者
 
+### &#8627; Contributors
+
+<a href="https://github.com/OpenRL-Lab/openrl/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=OpenRL-Lab/openrl" />
+</a>
+
 ### &#8627; Stargazers
 
 [![Stargazers repo roster for @OpenRL-Lab/openrl](https://reporoster.com/stars/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/stargazers)
 
 ### &#8627; Forkers
 
 [![Forkers repo roster for @OpenRL-Lab/openrl](https://reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network/members)
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: openrl Version: 0.0.7 Summary: unified
+Metadata-Version: 2.1 Name: openrl Version: 0.0.8 Summary: unified
 reinforcement learning framework Home-page: https://github.com/OpenRL-Lab/
 openrl Author: openrl contributors Author-email: huangsy1314@163.com Project-
 URL: Code, https://github.com/OpenRL-Lab/openrl Project-URL: Documentation,
 https://openrl-docs.readthedocs.io/zh/latest/ Keywords: reinforcement-learning
 multi-agent reinforcement-learning-algorithms pytorch machine-learning
 baselines toolbox python data-science gym gymnasium Classifier: Development
-Status :: 3 - Alpha Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Science/
+Research Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
-Provides-Extra: test Provides-Extra: dev Provides-Extra: mpe Provides-Extra:
-nlp License-File: LICENSE License-File: LICENSE.txt
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Operating System :: OS Independent Requires-
+Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: test
+Provides-Extra: dev Provides-Extra: mpe Provides-Extra: nlp License-File:
+LICENSE License-File: LICENSE.txt
                         [./docs/images/openrl_text.png]
 --- [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/
 openrl/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 openrl) [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/
 version.svg)](https://anaconda.org/openrl/openrl) [![Anaconda-Server Badge]
 (https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://
 anaconda.org/openrl/openrl) [![Anaconda-Server Badge](https://anaconda.org/
@@ -39,18 +40,20 @@
 img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [![GitHub issues]
 (https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/
 OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/github/
 issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls) [!
 [Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)]
 (https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub license]
 (https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/
-OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.7 is updated on April 29,
-2023 ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£](https://
-openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-
-docs.readthedocs.io/en/latest/
+OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.8 is updated on May 4, 2023
+The main branch is the latest version of OpenRL, which is under active
+development. If you just want to have a try with OpenRL, you can switch to the
+stable branch. ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£]
+(https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://
+openrl-docs.readthedocs.io/en/latest/
 )
 OpenRLæ¯ä¸ä¸ªå¼æºçéç¨å¼ºåå­¦ä¹ ç ç©¶æ¡æ¶ï¼æ¯æåæºè½ä½ãå¤æºè½ä½ãèªç¶è¯­è¨ç­å¤ç§ä»»å¡çè®­ç»ã
 OpenRLåºäºPyTorchè¿è¡å¼åï¼ç®æ æ¯ä¸ºå¼ºåå­¦ä¹ ç ç©¶ç¤¾åºæä¾ä¸ä¸ªç®åæç¨ãçµæ´»é«æãå¯æç»­æ©å±çå¹³å°ã
 ç®åï¼OpenRLæ¯æçç¹æ§åæ¬ï¼ -
 ç®åæç¨ä¸æ¯æåæºè½ä½ãå¤æºè½ä½è®­ç»çéç¨æ¥å£ -
 æ¯æèªç¶è¯­è¨ä»»å¡ï¼å¦å¯¹è¯ä»»å¡ï¼çå¼ºåå­¦ä¹ è®­ç» - æ¯æä»
 [Hugging Face](https://huggingface.co/)ä¸å¯¼å¥æ¨¡ååæ°æ® -
@@ -66,27 +69,39 @@
 Styleåç±»åæ£æ¥ è¯¥æ¡æ¶ç»è¿äº[OpenRL-Lab](https://github.com/OpenRL-
 Lab)çå¤æ¬¡è¿­ä»£å¹¶åºç¨äºå­¦æ¯ç ç©¶ï¼ç®åå·²ç»æä¸ºäºä¸ä¸ªæççå¼ºåå­¦ä¹ æ¡æ¶ã
 OpenRL-Labå°æç»­ç»´æ¤åæ´æ°OpenRLï¼æ¬¢è¿å¤§å®¶å å¥æä»¬ç
 [å¼æºç¤¾åº](./
 CONTRIBUTING.md)ï¼ä¸èµ·ä¸ºå¼ºåå­¦ä¹ çåå±ååºè´¡ç®ã
 å³äºOpenRLçæ´å¤ä¿¡æ¯ï¼è¯·åè[ææ¡£](https://openrl-
 docs.readthedocs.io/zh/latest/)ã ## ç®å½ - [æ¬¢è¿æ¥å°OpenRL]
-(#æ¬¢è¿æ¥å°openrl) - [ç®å½](#ç®å½) - [å®è£](#å®è£) - [å¿«éä¸æ]
-(#å¿«éä¸æ) - [Gallery](#Gallery) - [ä½¿ç¨OpenRLçé¡¹ç®]
-(#ä½¿ç¨OpenRLçé¡¹ç®) - [åé¦åè´¡ç®](#åé¦åè´¡ç®) - [ç»´æ¤äººå]
-(#ç»´æ¤äººå) - [æ¯æè](#æ¯æè) - [↳ Stargazers](#-stargazers) - [↳
-Forkers](#-forkers) - [Citing OpenRL](#citing-openrl) - [License](#license) -
+(#æ¬¢è¿æ¥å°openrl) - [ç®å½](#ç®å½) - [å®è£](#å®è£) - [ä½¿ç¨Docker]
+(#ä½¿ç¨docker) - [å¿«éä¸æ](#å¿«éä¸æ) - [Gallery](#Gallery) -
+[ä½¿ç¨OpenRLçé¡¹ç®](#ä½¿ç¨OpenRLçé¡¹ç®) - [åé¦åè´¡ç®]
+(#åé¦åè´¡ç®) - [ç»´æ¤äººå](#ç»´æ¤äººå) - [æ¯æè](#æ¯æè) -
+[↳ Contributors](#-contributors) - [↳ Stargazers](#-stargazers) - [↳ Forkers]
+(#-forkers) - [Citing OpenRL](#citing-openrl) - [License](#license) -
 [Acknowledgments](#acknowledgments) ## å®è£
 ç¨æ·å¯ä»¥ç´æ¥éè¿pipå®è£OpenRL: ```bash pip install openrl ```
 å¦æç¨æ·ä½¿ç¨äºAnacondaæèMinicondaï¼ä¹å¯ä»¥éè¿condaå®è£OpenRL:
 ```bash conda install -c openrl openrl ```
-ç¨æ·ä¹å¯ä»¥ä»æºç å®è£OpenRL: ```bash git clone https://github.com/
-OpenRL-Lab/openrl && cd openrl pip install -e . ```
+æ³è¦ä¿®æ¹æºç çç¨æ·ä¹å¯ä»¥ä»æºç å®è£OpenRL: ```bash git clone
+https://github.com/OpenRL-Lab/openrl.git && cd openrl pip install -e . ```
 å®è£å®æåï¼ç¨æ·å¯ä»¥ç´æ¥éè¿å½ä»¤è¡æ¥çOpenRLççæ¬ï¼
-```bash openrl --version ``` ## å¿«éä¸æ
+```bash openrl --version ``` ## ä½¿ç¨Docker
+OpenRLç®åä¹æä¾äºåå«æ¾å¡æ¯æåéæ¾å¡æ¯æçDockeréåã
+å¦æç¨æ·ççµèä¸æ²¡æè±ä¼è¾¾æ¾å¡ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åä¸åå«æ¾å¡æä»¶çéåï¼
+```bash sudo docker pull openrllab/openrl-cpu ```
+å¦æç¨æ·æ³è¦éè¿æ¾å¡å éè®­ç»ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åï¼
+```bash sudo docker pull openrllab/openrl ```
+éåæåæååï¼ç¨æ·å¯ä»¥éè¿ä»¥ä¸å½ä»¤è¿è¡OpenRLçDockeréåï¼
+```bash # ä¸å¸¦æ¾å¡å é sudo docker run -it openrllab/openrl-cpu #
+å¸¦æ¾å¡å é sudo docker run -it --gpus all --net host openrllab/openrl ```
+è¿å¥Dockeréååï¼ç¨æ·å¯ä»¥éè¿ä»¥ä¸å½ä»¤æ¥çOpenRLççæ¬ç¶åè¿è¡æµä¾ï¼
+```bash # æ¥çDockeréåä¸­OpenRLççæ¬ openrl --version # è¿è¡æµä¾
+openrl --mode train --env CartPole-v1 ``` ## å¿«éä¸æ
 OpenRLä¸ºå¼ºåå­¦ä¹ å¥é¨ç¨æ·æä¾äºç®åæç¨çæ¥å£ï¼
 ä¸é¢æ¯ä¸ä¸ªä½¿ç¨PPOç®æ³è®­ç»`CartPole`ç¯å¢çä¾å­ï¼ ```python #
 train_ppo.py from openrl.envs.common import make from openrl.modules.common
 import PPONet as Net from openrl.runners.common import PPOAgent as Agent env =
 make("CartPole-v1", env_num=9) # åå»ºç¯å¢ï¼å¹¶è®¾ç½®ç¯å¢å¹¶è¡æ°ä¸º9
 net = Net(env) # åå»ºç¥ç»ç½ç» agent = Agent(net) # åå§åæºè½ä½
 agent.train(total_time_steps=20000) #
@@ -142,14 +157,15 @@
 [OpenRLå¼åè®¡å](https://github.com/OpenRL-Lab/openrl/issues/2) ##
 ç»´æ¤äººå ç®åï¼OpenRLç±ä»¥ä¸ç»´æ¤äººåç»´æ¤ï¼ - [Shiyu Huang]
 (https://huangshiyu13.github.io/)([@huangshiyu13](https://github.com/
 huangshiyu13)) - Wenze Chen([@Chen001117](https://github.com/Chen001117))
 æ¬¢è¿æ´å¤çè´¡ç®èå å¥æä»¬çç»´æ¤å¢é (åéé®ä»¶å°
 [huangshiyu@4paradigm.com]
 (huangshiyu@4paradigm.com)ç³è¯·å å¥OpenRLå¢é)ã ## æ¯æè ### ↳
+Contributors [https://contrib.rocks/image?repo=OpenRL-Lab/openrl] ### ↳
 Stargazers [![Stargazers repo roster for @OpenRL-Lab/openrl](https://
 reporoster.com/stars/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/
 stargazers) ### ↳ Forkers [![Forkers repo roster for @OpenRL-Lab/openrl](https:
 //reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/
 openrl/network/members) ## Citing OpenRL
 å¦ææä»¬çå·¥ä½å¯¹ä½ æå¸®å©ï¼æ¬¢è¿å¼ç¨æä»¬: ```latex @misc
 {openrl2023, title={OpenRL}, author={OpenRL Contributors}, publisher =
```

### Comparing `openrl-0.0.7/openrl.egg-info/SOURCES.txt` & `openrl-0.0.8/openrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/setup.py` & `openrl-0.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,27 +20,28 @@
 
 import setuptools
 from setuptools import setup
 
 
 def get_install_requires() -> list:
     return [
-        "setuptools>=50.0",
+        "setuptools>=67.0",
         "gymnasium",
         "click",
         "termcolor",
         "gym",
         "torch",
         "treevalue",
         "rich",
         "wandb",
         "seaborn",
         "jsonargparse",
         "imageio",
         "opencv-python",
+        "pygame",
     ]
 
 
 def get_extra_requires() -> dict:
     req = {
         "test": [
             "pytest",
@@ -50,19 +51,19 @@
             "black",
             "ruff",
             "gpustat",
         ],
         "dev": ["build", "twine"],
         "mpe": ["pyglet==1.5.27"],
         "nlp": [
-            "stable-baselines3==1.5.1a5",
             "transformers==4.18.0",
             "datasets",
             "nltk",
             "evaluate",
+            "icetk",
         ],
     }
     return req
 
 
 def get_version() -> str:
     # https://packaging.python.org/guides/single-sourcing-package-version/
@@ -82,19 +83,20 @@
     packages=setuptools.find_packages(),
     entry_points={"console_scripts": ["openrl=openrl.cli.cli:run"]},
     project_urls={
         "Code": "https://github.com/OpenRL-Lab/openrl",
         "Documentation": "https://openrl-docs.readthedocs.io/zh/latest/",
     },
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development :: Libraries :: Python Modules",
-        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     keywords=(
         "reinforcement-learning multi-agent "
         "reinforcement-learning-algorithms pytorch machine-learning "
         "baselines toolbox python data-science gym gymnasium"
```

### Comparing `openrl-0.0.7/tests/__init__.py` & `openrl-0.0.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/tests/project/__init__.py` & `openrl-0.0.8/tests/project/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/tests/project/test_version.py` & `openrl-0.0.8/tests/project/test_version.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/tests/test_buffer/__init__.py` & `openrl-0.0.8/tests/test_buffer/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.7/tests/test_buffer/test_buffer.py` & `openrl-0.0.8/tests/test_buffer/test_buffer.py`

 * *Files identical despite different names*

