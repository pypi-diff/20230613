# Comparing `tmp/rlgym-1.2.0.tar.gz` & `tmp/rlgym-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rlgym-1.2.0.tar", last modified: Mon May 16 18:15:21 2022, max compression
+gzip compressed data, was "dist/rlgym-1.2.1.tar", last modified: Mon Jun 12 22:11:29 2023, max compression
```

## Comparing `rlgym-1.2.0.tar` & `rlgym-1.2.1.tar`

### file list

```diff
@@ -1,94 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)    10756 2022-05-16 18:15:15.000000 rlgym-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-05-16 18:15:15.000000 rlgym-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-05-16 18:15:21.000000 rlgym-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-05-16 18:15:15.000000 rlgym-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym/communication/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/communication/communication_exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     5499 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/communication/communication_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     2518 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/communication/message.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym/envs/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/envs/environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     6374 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/envs/match.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym/gamelaunch/
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/gamelaunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5834 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/gamelaunch/epic_launch.py
--rw-r--r--   0 runner    (1001) docker     (121)     4670 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/gamelaunch/launch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/gamelaunch/minimize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/gamelaunch/paging.py
--rw-r--r--   0 runner    (1001) docker     (121)     9280 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/gym.py
--rw-r--r--   0 runner    (1001) docker     (121)     4427 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/make.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym/plugin/
--rw-r--r--   0 runner    (1001) docker     (121)   252928 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/plugin/RLGym.dll
--rw-r--r--   0 runner    (1001) docker     (121)    23040 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/plugin/RLMultiInjector.exe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym/utils/action_parsers/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/action_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/action_parsers/action_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/action_parsers/continuous_act.py
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/action_parsers/default_act.py
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/action_parsers/discrete_act.py
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/common_values.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym/utils/gamestates/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/gamestates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5139 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/gamestates/game_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     3920 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/gamestates/physics_object.py
--rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/gamestates/player_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     4143 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/math.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym/utils/obs_builders/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/obs_builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/obs_builders/advanced_obs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2674 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/obs_builders/default_obs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2268 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/obs_builders/obs_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2971 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/obs_builders/rhobot_obs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym/utils/reward_functions/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/reward_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3587 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/reward_functions/combined_reward.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym/utils/reward_functions/common_rewards/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/reward_functions/common_rewards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2979 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/reward_functions/common_rewards/ball_goal_rewards.py
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/reward_functions/common_rewards/conditional_rewards.py
--rw-r--r--   0 runner    (1001) docker     (121)     4600 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/reward_functions/common_rewards/misc_rewards.py
--rw-r--r--   0 runner    (1001) docker     (121)     2618 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/reward_functions/common_rewards/player_ball_rewards.py
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/reward_functions/default_reward.py
--rw-r--r--   0 runner    (1001) docker     (121)     2341 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/reward_functions/reward_function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym/utils/state_setters/
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/state_setters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1993 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/state_setters/default_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     3797 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/state_setters/random_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/state_setters/state_setter.py
--rw-r--r--   0 runner    (1001) docker     (121)     7156 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/state_setters/state_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym/utils/state_setters/wrappers/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/state_setters/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/state_setters/wrappers/car_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2856 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/state_setters/wrappers/physics_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2687 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/state_setters/wrappers/state_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym/utils/terminal_conditions/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/terminal_conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/terminal_conditions/common_conditions.py
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/utils/terminal_conditions/terminal_condition.py
--rw-r--r--   0 runner    (1001) docker     (121)     5186 2022-05-16 18:15:15.000000 rlgym-1.2.0/rlgym/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-05-16 18:15:21.000000 rlgym-1.2.0/rlgym.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-16 18:15:21.000000 rlgym-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2700 2022-05-16 18:15:15.000000 rlgym-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:15.000000 rlgym-1.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/tests/cases/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:15.000000 rlgym-1.2.0/tests/cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-05-16 18:15:15.000000 rlgym-1.2.0/tests/cases/boost_pad_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1427 2022-05-16 18:15:15.000000 rlgym-1.2.0/tests/run_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:21.000000 rlgym-1.2.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-16 18:15:15.000000 rlgym-1.2.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-05-16 18:15:15.000000 rlgym-1.2.0/tests/utils/base_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-05-16 18:15:15.000000 rlgym-1.2.0/tests/utils/setter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-05-16 18:15:15.000000 rlgym-1.2.0/tests/utils/state_obs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-06-12 22:11:22.000000 rlgym-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 22:11:22.000000 rlgym-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-12 22:11:29.000000 rlgym-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-12 22:11:22.000000 rlgym-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/communication/communication_exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/communication/communication_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/communication/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/envs/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/envs/match.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/gamelaunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/gamelaunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/gamelaunch/epic_launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/gamelaunch/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/gamelaunch/minimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/gamelaunch/paging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/make.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)   252928 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/plugin/RLGym.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/plugin/RLMultiInjector.exe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/action_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/action_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/action_parsers/action_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/action_parsers/continuous_act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/action_parsers/default_act.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/action_parsers/discrete_act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/common_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/gamestates/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/gamestates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/gamestates/game_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/gamestates/physics_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/gamestates/player_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/obs_builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/obs_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/obs_builders/advanced_obs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/obs_builders/default_obs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/obs_builders/obs_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/reward_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/combined_reward.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/ball_goal_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/conditional_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/misc_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/player_ball_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/default_reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/reward_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/state_setters/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/default_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/random_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/state_setter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/state_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/state_setters/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/wrappers/car_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/wrappers/physics_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/wrappers/state_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/terminal_conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/terminal_conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/terminal_conditions/common_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/terminal_conditions/terminal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 22:11:29.000000 rlgym-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-12 22:11:22.000000 rlgym-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:22.000000 rlgym-1.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/tests/cases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:22.000000 rlgym-1.2.1/tests/cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-12 22:11:22.000000 rlgym-1.2.1/tests/cases/boost_pad_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-12 22:11:22.000000 rlgym-1.2.1/tests/run_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:22.000000 rlgym-1.2.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-12 22:11:22.000000 rlgym-1.2.1/tests/utils/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-12 22:11:22.000000 rlgym-1.2.1/tests/utils/setter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-12 22:11:22.000000 rlgym-1.2.1/tests/utils/state_obs.py
```

### Comparing `rlgym-1.2.0/LICENSE` & `rlgym-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/PKG-INFO` & `rlgym-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlgym
-Version: 1.2.0
+Version: 1.2.1
 Summary: A python API that can be used to treat the game Rocket League as an Openai Gym-like environment for Reinforcement Learning projects.
 Home-page: https://github.com/lucas-emery/rocket-league-gym
 Author: Lucas Emery and Matthew Allen
 License: Apache 2.0
 Description: # The Rocket League Gym
         This is a python API that can be used to treat the game [Rocket League](https://www.rocketleague.com) as though it were an [OpenAI Gym](https://gym.openai.com)-style environment for Reinforcement Learning projects. This API must be used with the accompanying Bakkesmod plugin.
         
@@ -29,9 +29,9 @@
         
 Keywords: rocket-league,gym,reinforcement-learning
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
+Requires-Python: >=3.7,<=3.9
 Description-Content-Type: text/markdown
```

### Comparing `rlgym-1.2.0/README.md` & `rlgym-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/communication/communication_exception_handler.py` & `rlgym-1.2.1/rlgym/communication/communication_exception_handler.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/communication/communication_handler.py` & `rlgym-1.2.1/rlgym/communication/communication_handler.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/communication/message.py` & `rlgym-1.2.1/rlgym/communication/message.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/envs/environment.py` & `rlgym-1.2.1/rlgym/envs/environment.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/envs/match.py` & `rlgym-1.2.1/rlgym/envs/match.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/gamelaunch/epic_launch.py` & `rlgym-1.2.1/rlgym/gamelaunch/epic_launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Copied from https://github.com/RLBot/RLBot/blob/master/src/main/python/rlbot/gamelaunch/epic_launch.py
 
 def launch_with_epic_simple(ideal_args: List[str]) -> Optional[subprocess.Popen]:
     try:
         # Try launch via Epic Games
         epic_rl_exe_path = locate_epic_games_launcher_rocket_league_binary()
         if epic_rl_exe_path is not None:
-            exe_and_args = [str(epic_rl_exe_path)] + ideal_args + ['-EpicPortal']
+            exe_and_args = [str(epic_rl_exe_path)] + ideal_args + ['-EpicPortal', '-AUTH_PASSWORD=0']
             # print(f'Launching Rocket League with: {exe_and_args}')
             try:
                 return subprocess.Popen(exe_and_args)
             except Exception as e:
                 print(f'Unable to launch via Epic due to: {e}')
     except:
         print('Unable to launch via Epic.')
```

### Comparing `rlgym-1.2.0/rlgym/gamelaunch/launch.py` & `rlgym-1.2.1/rlgym/gamelaunch/launch.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/gamelaunch/minimize.py` & `rlgym-1.2.1/rlgym/gamelaunch/minimize.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/gamelaunch/paging.py` & `rlgym-1.2.1/rlgym/gamelaunch/paging.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/gym.py` & `rlgym-1.2.1/rlgym/gym.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/make.py` & `rlgym-1.2.1/rlgym/make.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/plugin/RLGym.dll` & `rlgym-1.2.1/rlgym/plugin/RLGym.dll`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/plugin/RLMultiInjector.exe` & `rlgym-1.2.1/rlgym/plugin/RLMultiInjector.exe`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/action_parsers/action_parser.py` & `rlgym-1.2.1/rlgym/utils/action_parsers/action_parser.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/action_parsers/continuous_act.py` & `rlgym-1.2.1/rlgym/utils/action_parsers/continuous_act.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/action_parsers/default_act.py` & `rlgym-1.2.1/rlgym/utils/action_parsers/default_act.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/action_parsers/discrete_act.py` & `rlgym-1.2.1/rlgym/utils/action_parsers/discrete_act.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/common_values.py` & `rlgym-1.2.1/rlgym/utils/common_values.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/gamestates/game_state.py` & `rlgym-1.2.1/rlgym/utils/gamestates/game_state.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/gamestates/physics_object.py` & `rlgym-1.2.1/rlgym/utils/gamestates/physics_object.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/gamestates/player_data.py` & `rlgym-1.2.1/rlgym/utils/gamestates/player_data.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/math.py` & `rlgym-1.2.1/rlgym/utils/math.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/obs_builders/advanced_obs.py` & `rlgym-1.2.1/rlgym/utils/obs_builders/advanced_obs.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/obs_builders/default_obs.py` & `rlgym-1.2.1/rlgym/utils/obs_builders/default_obs.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/obs_builders/obs_builder.py` & `rlgym-1.2.1/rlgym/utils/obs_builders/obs_builder.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/reward_functions/combined_reward.py` & `rlgym-1.2.1/rlgym/utils/reward_functions/combined_reward.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/reward_functions/common_rewards/ball_goal_rewards.py` & `rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/ball_goal_rewards.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/reward_functions/common_rewards/conditional_rewards.py` & `rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/conditional_rewards.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/reward_functions/common_rewards/misc_rewards.py` & `rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/misc_rewards.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/reward_functions/common_rewards/player_ball_rewards.py` & `rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/player_ball_rewards.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/reward_functions/default_reward.py` & `rlgym-1.2.1/rlgym/utils/reward_functions/default_reward.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,11 +10,11 @@
         super().__init__()
         self.last_touch = None
 
     def reset(self, initial_state: GameState):
         self.last_touch = initial_state.last_touch
 
     def get_reward(self, player: PlayerData, state: GameState, previous_action: np.ndarray) -> float:
-        return - math.vecmag(player.car_data.angular_velocity) / 100
+        return - math.vecmag(player.car_data.linear_velocity) / 100
 
     def get_final_reward(self, player: PlayerData, state: GameState, previous_action: np.ndarray) -> float:
         return self.get_reward(player, state, previous_action)
```

### Comparing `rlgym-1.2.0/rlgym/utils/reward_functions/reward_function.py` & `rlgym-1.2.1/rlgym/utils/reward_functions/reward_function.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/state_setters/default_state.py` & `rlgym-1.2.1/rlgym/utils/state_setters/default_state.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/state_setters/random_state.py` & `rlgym-1.2.1/rlgym/utils/state_setters/random_state.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/state_setters/state_setter.py` & `rlgym-1.2.1/rlgym/utils/state_setters/state_setter.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/state_setters/state_wrapper.py` & `rlgym-1.2.1/rlgym/utils/state_setters/state_wrapper.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/state_setters/wrappers/car_wrapper.py` & `rlgym-1.2.1/rlgym/utils/state_setters/wrappers/car_wrapper.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/state_setters/wrappers/physics_wrapper.py` & `rlgym-1.2.1/rlgym/utils/state_setters/wrappers/physics_wrapper.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/state_setters/wrappers/state_wrapper.py` & `rlgym-1.2.1/rlgym/utils/state_setters/wrappers/state_wrapper.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/terminal_conditions/common_conditions.py` & `rlgym-1.2.1/rlgym/utils/terminal_conditions/common_conditions.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/utils/terminal_conditions/terminal_condition.py` & `rlgym-1.2.1/rlgym/utils/terminal_conditions/terminal_condition.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/rlgym/version.py` & `rlgym-1.2.1/rlgym/version.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 # From https://github.com/RLBot/RLBot/blob/master/src/main/python/rlbot/version.py
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
 # https://stackoverflow.com/questions/458550/standard-way-to-embed-version-into-python-package
 
-__version__ = '1.2.0'
+__version__ = '1.2.1'
 
 release_notes = {
     'beta':
     """
     - This version contains numerous untested and potentially breaking changes. Run at your own risk.
     """,
+    '1.2.1':
+    """
+    - Fixed epic version crashing instantly - Bakkes
+    - Added max python version
+    - Added ActionParser to utils submodule
+    - Updated default reward, it now minimizes linear velocity instead of angular
+    - RIP RhobotObs
+    """,
     '1.2.0': """
     - Deprecated self_play flag, playing against Psyonix agents is no longer supported
     - Added has_jump to PlayerData, which is useful to detect when a flip won't run out
     - Added pre_step() function to ObsBuilder and RewardFunction, useful for pre-calculating stuff each step
     - Added support for changing gamemode without restarting RLGym, see StateSetter.build_wrapper()
     - Added gravity and boost_consumption configuration to rlgym.make()
     - Added update_settings() method to gym, for updating some parts of the config without restarting
```

### Comparing `rlgym-1.2.0/rlgym.egg-info/PKG-INFO` & `rlgym-1.2.1/rlgym.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlgym
-Version: 1.2.0
+Version: 1.2.1
 Summary: A python API that can be used to treat the game Rocket League as an Openai Gym-like environment for Reinforcement Learning projects.
 Home-page: https://github.com/lucas-emery/rocket-league-gym
 Author: Lucas Emery and Matthew Allen
 License: Apache 2.0
 Description: # The Rocket League Gym
         This is a python API that can be used to treat the game [Rocket League](https://www.rocketleague.com) as though it were an [OpenAI Gym](https://gym.openai.com)-style environment for Reinforcement Learning projects. This API must be used with the accompanying Bakkesmod plugin.
         
@@ -29,9 +29,9 @@
         
 Keywords: rocket-league,gym,reinforcement-learning
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
+Requires-Python: >=3.7,<=3.9
 Description-Content-Type: text/markdown
```

### Comparing `rlgym-1.2.0/rlgym.egg-info/SOURCES.txt` & `rlgym-1.2.1/rlgym.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 rlgym/utils/gamestates/game_state.py
 rlgym/utils/gamestates/physics_object.py
 rlgym/utils/gamestates/player_data.py
 rlgym/utils/obs_builders/__init__.py
 rlgym/utils/obs_builders/advanced_obs.py
 rlgym/utils/obs_builders/default_obs.py
 rlgym/utils/obs_builders/obs_builder.py
-rlgym/utils/obs_builders/rhobot_obs.py
 rlgym/utils/reward_functions/__init__.py
 rlgym/utils/reward_functions/combined_reward.py
 rlgym/utils/reward_functions/default_reward.py
 rlgym/utils/reward_functions/reward_function.py
 rlgym/utils/reward_functions/common_rewards/__init__.py
 rlgym/utils/reward_functions/common_rewards/ball_goal_rewards.py
 rlgym/utils/reward_functions/common_rewards/conditional_rewards.py
```

### Comparing `rlgym-1.2.0/setup.py` & `rlgym-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     install_requires=[
         'gym>=0.17',
         'numpy>=1.19',
         'pywin32==228',
         'pywinauto==0.6.8',
         'psutil>=5.8',
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.7,<=3.9',
     cmdclass={'install': CustomInstall},
     license='Apache 2.0',
     license_file='LICENSE',
     keywords=['rocket-league', 'gym', 'reinforcement-learning'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `rlgym-1.2.0/tests/cases/boost_pad_test.py` & `rlgym-1.2.1/tests/cases/boost_pad_test.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.0/tests/run_tests.py` & `rlgym-1.2.1/tests/run_tests.py`

 * *Files identical despite different names*

