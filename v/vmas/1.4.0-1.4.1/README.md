# Comparing `tmp/vmas-1.4.0.tar.gz` & `tmp/vmas-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmas-1.4.0.tar", last modified: Wed Feb  7 10:28:18 2024, max compression
+gzip compressed data, was "vmas-1.4.1.tar", last modified: Mon May 20 13:37:28 2024, max compression
```

## Comparing `vmas-1.4.0.tar` & `vmas-1.4.1.tar`

### file list

```diff
@@ -1,93 +1,97 @@
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-02-07 10:28:18.172450 vmas-1.4.0/
--rw-r--r--   0 Matteo     (501) staff       (20)    35149 2022-11-19 11:21:06.000000 vmas-1.4.0/LICENSE
--rw-r--r--   0 Matteo     (501) staff       (20)       35 2023-05-25 09:41:38.000000 vmas-1.4.0/MANIFEST.in
--rw-r--r--   0 Matteo     (501) staff       (20)      254 2024-02-07 10:28:18.172520 vmas-1.4.0/PKG-INFO
--rw-r--r--   0 Matteo     (501) staff       (20)    70355 2024-02-06 17:06:34.000000 vmas-1.4.0/README.md
--rw-r--r--   0 Matteo     (501) staff       (20)      103 2024-02-07 10:28:18.172729 vmas-1.4.0/setup.cfg
--rw-r--r--   0 Matteo     (501) staff       (20)      533 2024-02-07 10:28:16.000000 vmas-1.4.0/setup.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-02-07 10:28:18.151613 vmas-1.4.0/vmas/
--rw-r--r--   0 Matteo     (501) staff       (20)     1472 2023-12-11 07:42:35.000000 vmas-1.4.0/vmas/__init__.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-02-07 10:28:18.157296 vmas-1.4.0/vmas/examples/
--rw-r--r--   0 Matteo     (501) staff       (20)       89 2023-01-23 16:01:21.000000 vmas-1.4.0/vmas/examples/__init__.py
--rw-r--r--   0 Matteo     (501) staff       (20)     5731 2023-05-23 13:24:52.000000 vmas-1.4.0/vmas/examples/rllib.py
--rw-r--r--   0 Matteo     (501) staff       (20)     2374 2024-01-02 08:41:25.000000 vmas-1.4.0/vmas/examples/run_heuristic.py
--rw-r--r--   0 Matteo     (501) staff       (20)     5105 2024-02-06 17:51:55.000000 vmas-1.4.0/vmas/examples/use_vmas_env.py
--rw-r--r--   0 Matteo     (501) staff       (20)    12145 2024-01-10 08:50:22.000000 vmas-1.4.0/vmas/interactive_rendering.py
--rw-r--r--   0 Matteo     (501) staff       (20)     2740 2024-02-05 17:40:51.000000 vmas-1.4.0/vmas/make_env.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-02-07 10:28:18.162912 vmas-1.4.0/vmas/scenarios/
--rw-r--r--   0 Matteo     (501) staff       (20)      752 2023-10-18 07:42:00.000000 vmas-1.4.0/vmas/scenarios/__init__.py
--rw-r--r--   0 Matteo     (501) staff       (20)     9618 2024-02-06 12:13:53.000000 vmas-1.4.0/vmas/scenarios/balance.py
--rw-r--r--   0 Matteo     (501) staff       (20)    13748 2024-02-06 12:13:58.000000 vmas-1.4.0/vmas/scenarios/ball_passage.py
--rw-r--r--   0 Matteo     (501) staff       (20)     7899 2024-02-06 12:14:03.000000 vmas-1.4.0/vmas/scenarios/ball_trajectory.py
--rw-r--r--   0 Matteo     (501) staff       (20)     9999 2023-10-31 18:19:12.000000 vmas-1.4.0/vmas/scenarios/buzz_wire.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-02-07 10:28:18.165137 vmas-1.4.0/vmas/scenarios/debug/
--rw-r--r--   0 Matteo     (501) staff       (20)       89 2023-01-23 16:01:21.000000 vmas-1.4.0/vmas/scenarios/debug/__init__.py
--rw-r--r--   0 Matteo     (501) staff       (20)    10055 2023-05-10 08:13:21.000000 vmas-1.4.0/vmas/scenarios/debug/asym_joint.py
--rw-r--r--   0 Matteo     (501) staff       (20)     7087 2023-12-11 07:42:35.000000 vmas-1.4.0/vmas/scenarios/debug/circle_trajectory.py
--rw-r--r--   0 Matteo     (501) staff       (20)     3350 2024-02-06 17:06:34.000000 vmas-1.4.0/vmas/scenarios/debug/diff_drive.py
--rw-r--r--   0 Matteo     (501) staff       (20)     8888 2023-05-23 13:24:35.000000 vmas-1.4.0/vmas/scenarios/debug/goal.py
--rw-r--r--   0 Matteo     (501) staff       (20)     3773 2023-05-10 08:13:21.000000 vmas-1.4.0/vmas/scenarios/debug/het_mass.py
--rw-r--r--   0 Matteo     (501) staff       (20)     4012 2024-02-06 14:44:20.000000 vmas-1.4.0/vmas/scenarios/debug/kinematic_bicycle.py
--rw-r--r--   0 Matteo     (501) staff       (20)     4636 2023-10-31 18:19:12.000000 vmas-1.4.0/vmas/scenarios/debug/line_trajectory.py
--rw-r--r--   0 Matteo     (501) staff       (20)     2861 2023-12-11 07:42:35.000000 vmas-1.4.0/vmas/scenarios/debug/pollock.py
--rw-r--r--   0 Matteo     (501) staff       (20)     5521 2023-05-19 16:58:04.000000 vmas-1.4.0/vmas/scenarios/debug/vel_control.py
--rw-r--r--   0 Matteo     (501) staff       (20)     5169 2024-02-06 12:16:51.000000 vmas-1.4.0/vmas/scenarios/debug/waterfall.py
--rw-r--r--   0 Matteo     (501) staff       (20)    13458 2023-05-10 08:13:21.000000 vmas-1.4.0/vmas/scenarios/discovery.py
--rw-r--r--   0 Matteo     (501) staff       (20)     5562 2024-02-01 15:33:37.000000 vmas-1.4.0/vmas/scenarios/dispersion.py
--rw-r--r--   0 Matteo     (501) staff       (20)     5522 2024-01-17 10:42:22.000000 vmas-1.4.0/vmas/scenarios/dropout.py
--rw-r--r--   0 Matteo     (501) staff       (20)     8930 2023-12-11 07:42:35.000000 vmas-1.4.0/vmas/scenarios/flocking.py
--rw-r--r--   0 Matteo     (501) staff       (20)    64456 2023-10-31 18:19:12.000000 vmas-1.4.0/vmas/scenarios/football.py
--rw-r--r--   0 Matteo     (501) staff       (20)    19815 2024-01-17 10:42:22.000000 vmas-1.4.0/vmas/scenarios/give_way.py
--rw-r--r--   0 Matteo     (501) staff       (20)    27851 2023-10-31 18:19:12.000000 vmas-1.4.0/vmas/scenarios/joint_passage.py
--rw-r--r--   0 Matteo     (501) staff       (20)    27978 2023-10-31 18:19:12.000000 vmas-1.4.0/vmas/scenarios/joint_passage_size.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-02-07 10:28:18.166968 vmas-1.4.0/vmas/scenarios/mpe/
--rw-r--r--   0 Matteo     (501) staff       (20)       89 2022-11-19 11:21:06.000000 vmas-1.4.0/vmas/scenarios/mpe/__init__.py
--rwxr-xr-x   0 Matteo     (501) staff       (20)     2480 2023-10-31 18:19:12.000000 vmas-1.4.0/vmas/scenarios/mpe/simple.py
--rw-r--r--   0 Matteo     (501) staff       (20)     8305 2023-10-31 18:19:12.000000 vmas-1.4.0/vmas/scenarios/mpe/simple_adversary.py
--rw-r--r--   0 Matteo     (501) staff       (20)     6318 2024-01-04 13:25:08.000000 vmas-1.4.0/vmas/scenarios/mpe/simple_crypto.py
--rw-r--r--   0 Matteo     (501) staff       (20)     5831 2023-10-31 18:19:12.000000 vmas-1.4.0/vmas/scenarios/mpe/simple_push.py
--rwxr-xr-x   0 Matteo     (501) staff       (20)     4993 2023-10-31 18:19:12.000000 vmas-1.4.0/vmas/scenarios/mpe/simple_reference.py
--rwxr-xr-x   0 Matteo     (501) staff       (20)     5160 2023-10-31 18:19:12.000000 vmas-1.4.0/vmas/scenarios/mpe/simple_speaker_listener.py
--rw-r--r--   0 Matteo     (501) staff       (20)     4301 2023-10-31 18:19:12.000000 vmas-1.4.0/vmas/scenarios/mpe/simple_spread.py
--rw-r--r--   0 Matteo     (501) staff       (20)     9916 2024-01-17 10:42:22.000000 vmas-1.4.0/vmas/scenarios/mpe/simple_tag.py
--rw-r--r--   0 Matteo     (501) staff       (20)    13021 2023-10-31 18:19:12.000000 vmas-1.4.0/vmas/scenarios/mpe/simple_world_comm.py
--rw-r--r--   0 Matteo     (501) staff       (20)    15651 2023-10-31 18:19:12.000000 vmas-1.4.0/vmas/scenarios/multi_give_way.py
--rw-r--r--   0 Matteo     (501) staff       (20)    13911 2024-02-06 17:51:55.000000 vmas-1.4.0/vmas/scenarios/navigation.py
--rw-r--r--   0 Matteo     (501) staff       (20)    11444 2023-12-16 15:14:39.000000 vmas-1.4.0/vmas/scenarios/passage.py
--rw-r--r--   0 Matteo     (501) staff       (20)     6589 2024-01-17 10:42:22.000000 vmas-1.4.0/vmas/scenarios/reverse_transport.py
--rw-r--r--   0 Matteo     (501) staff       (20)    13418 2024-02-01 15:33:37.000000 vmas-1.4.0/vmas/scenarios/sampling.py
--rw-r--r--   0 Matteo     (501) staff       (20)    12548 2024-01-17 09:24:24.000000 vmas-1.4.0/vmas/scenarios/transport.py
--rw-r--r--   0 Matteo     (501) staff       (20)     4540 2023-12-11 07:42:35.000000 vmas-1.4.0/vmas/scenarios/wheel.py
--rw-r--r--   0 Matteo     (501) staff       (20)    15286 2024-01-17 10:42:22.000000 vmas-1.4.0/vmas/scenarios/wind_flocking.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-02-07 10:28:18.169345 vmas-1.4.0/vmas/simulator/
--rw-r--r--   0 Matteo     (501) staff       (20)       89 2022-11-19 11:21:06.000000 vmas-1.4.0/vmas/simulator/__init__.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-02-07 10:28:18.169815 vmas-1.4.0/vmas/simulator/controllers/
--rw-r--r--   0 Matteo     (501) staff       (20)       89 2023-05-19 16:58:04.000000 vmas-1.4.0/vmas/simulator/controllers/__init__.py
--rw-r--r--   0 Matteo     (501) staff       (20)     4701 2023-05-19 16:58:04.000000 vmas-1.4.0/vmas/simulator/controllers/velocity_controller.py
--rw-r--r--   0 Matteo     (501) staff       (20)    81142 2024-02-06 17:52:23.000000 vmas-1.4.0/vmas/simulator/core.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-02-07 10:28:18.171200 vmas-1.4.0/vmas/simulator/dynamics/
--rw-r--r--   0 Matteo     (501) staff       (20)       89 2023-05-19 16:58:04.000000 vmas-1.4.0/vmas/simulator/dynamics/__init__.py
--rw-r--r--   0 Matteo     (501) staff       (20)     1194 2024-01-10 08:50:22.000000 vmas-1.4.0/vmas/simulator/dynamics/common.py
--rw-r--r--   0 Matteo     (501) staff       (20)     2604 2024-02-06 17:06:34.000000 vmas-1.4.0/vmas/simulator/dynamics/diff_drive.py
--rw-r--r--   0 Matteo     (501) staff       (20)      362 2024-01-10 08:50:22.000000 vmas-1.4.0/vmas/simulator/dynamics/holonomic.py
--rw-r--r--   0 Matteo     (501) staff       (20)      425 2024-01-10 08:50:22.000000 vmas-1.4.0/vmas/simulator/dynamics/holonomic_with_rot.py
--rw-r--r--   0 Matteo     (501) staff       (20)     4401 2024-02-06 17:06:34.000000 vmas-1.4.0/vmas/simulator/dynamics/kinematic_bicycle.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-02-07 10:28:18.172237 vmas-1.4.0/vmas/simulator/environment/
--rw-r--r--   0 Matteo     (501) staff       (20)      546 2023-01-23 16:01:21.000000 vmas-1.4.0/vmas/simulator/environment/__init__.py
--rw-r--r--   0 Matteo     (501) staff       (20)    28427 2024-02-06 12:16:41.000000 vmas-1.4.0/vmas/simulator/environment/environment.py
--rw-r--r--   0 Matteo     (501) staff       (20)     3815 2023-05-23 16:48:23.000000 vmas-1.4.0/vmas/simulator/environment/gym.py
--rw-r--r--   0 Matteo     (501) staff       (20)     9502 2023-05-23 16:48:23.000000 vmas-1.4.0/vmas/simulator/environment/rllib.py
--rw-r--r--   0 Matteo     (501) staff       (20)      658 2023-01-23 16:01:21.000000 vmas-1.4.0/vmas/simulator/heuristic_policy.py
--rw-r--r--   0 Matteo     (501) staff       (20)     6810 2024-02-06 12:16:30.000000 vmas-1.4.0/vmas/simulator/joints.py
--rw-r--r--   0 Matteo     (501) staff       (20)    14069 2024-02-06 10:41:43.000000 vmas-1.4.0/vmas/simulator/physics.py
--rw-r--r--   0 Matteo     (501) staff       (20)    14755 2023-12-11 07:42:35.000000 vmas-1.4.0/vmas/simulator/rendering.py
--rw-r--r--   0 Matteo     (501) staff       (20)    11610 2024-01-10 08:50:22.000000 vmas-1.4.0/vmas/simulator/scenario.py
--rw-r--r--   0 Matteo     (501) staff       (20)     7780 2023-05-25 09:41:18.000000 vmas-1.4.0/vmas/simulator/secrcode.ttf
--rw-r--r--   0 Matteo     (501) staff       (20)     4097 2023-04-13 14:11:26.000000 vmas-1.4.0/vmas/simulator/sensors.py
--rw-r--r--   0 Matteo     (501) staff       (20)     8683 2024-02-06 12:16:51.000000 vmas-1.4.0/vmas/simulator/utils.py
-drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-02-07 10:28:18.152262 vmas-1.4.0/vmas.egg-info/
--rw-r--r--   0 Matteo     (501) staff       (20)      254 2024-02-07 10:28:18.000000 vmas-1.4.0/vmas.egg-info/PKG-INFO
--rw-r--r--   0 Matteo     (501) staff       (20)     2474 2024-02-07 10:28:18.000000 vmas-1.4.0/vmas.egg-info/SOURCES.txt
--rw-r--r--   0 Matteo     (501) staff       (20)        1 2024-02-07 10:28:18.000000 vmas-1.4.0/vmas.egg-info/dependency_links.txt
--rw-r--r--   0 Matteo     (501) staff       (20)       35 2024-02-07 10:28:18.000000 vmas-1.4.0/vmas.egg-info/requires.txt
--rw-r--r--   0 Matteo     (501) staff       (20)        5 2024-02-07 10:28:18.000000 vmas-1.4.0/vmas.egg-info/top_level.txt
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-05-20 13:37:28.225696 vmas-1.4.1/
+-rw-r--r--   0 Matteo     (501) staff       (20)    35149 2022-11-19 11:21:06.000000 vmas-1.4.1/LICENSE
+-rw-r--r--   0 Matteo     (501) staff       (20)       36 2024-05-03 15:58:49.000000 vmas-1.4.1/MANIFEST.in
+-rw-r--r--   0 Matteo     (501) staff       (20)      364 2024-05-20 13:37:28.225623 vmas-1.4.1/PKG-INFO
+-rw-r--r--   0 Matteo     (501) staff       (20)    71906 2024-05-03 15:58:49.000000 vmas-1.4.1/README.md
+-rw-r--r--   0 Matteo     (501) staff       (20)      456 2024-05-20 13:37:28.226235 vmas-1.4.1/setup.cfg
+-rw-r--r--   0 Matteo     (501) staff       (20)      932 2024-05-03 15:58:49.000000 vmas-1.4.1/setup.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-05-20 13:37:28.210764 vmas-1.4.1/tests/
+-rw-r--r--   0 Matteo     (501) staff       (20)     2690 2024-05-03 15:58:49.000000 vmas-1.4.1/tests/test_vmas.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-05-20 13:37:28.211470 vmas-1.4.1/vmas/
+-rw-r--r--   0 Matteo     (501) staff       (20)     1635 2024-05-20 13:36:48.000000 vmas-1.4.1/vmas/__init__.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-05-20 13:37:28.212716 vmas-1.4.1/vmas/examples/
+-rw-r--r--   0 Matteo     (501) staff       (20)       94 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/examples/__init__.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     5769 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/examples/rllib.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     2427 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/examples/run_heuristic.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     3946 2024-05-13 16:12:19.000000 vmas-1.4.1/vmas/examples/use_vmas_env.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    13360 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/interactive_rendering.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     4159 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/make_env.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-05-20 13:37:28.216454 vmas-1.4.1/vmas/scenarios/
+-rw-r--r--   0 Matteo     (501) staff       (20)      750 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/__init__.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     9763 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/balance.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    13895 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/ball_passage.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     7939 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/ball_trajectory.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    10112 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/buzz_wire.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-05-20 13:37:28.218482 vmas-1.4.1/vmas/scenarios/debug/
+-rw-r--r--   0 Matteo     (501) staff       (20)       94 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/debug/__init__.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    10063 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/debug/asym_joint.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     7139 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/debug/circle_trajectory.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     3351 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/debug/diff_drive.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     3570 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/debug/drone.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     9118 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/debug/goal.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     3829 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/debug/het_mass.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     4012 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/debug/kinematic_bicycle.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     4590 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/debug/line_trajectory.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     2861 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/debug/pollock.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     5529 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/debug/vel_control.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     5301 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/debug/waterfall.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    13621 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/discovery.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     5696 2024-05-20 13:36:10.000000 vmas-1.4.1/vmas/scenarios/dispersion.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     5610 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/dropout.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     8971 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/flocking.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    65313 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/football.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    19930 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/give_way.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    28059 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/joint_passage.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    28231 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/joint_passage_size.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-05-20 13:37:28.220198 vmas-1.4.1/vmas/scenarios/mpe/
+-rw-r--r--   0 Matteo     (501) staff       (20)       94 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/mpe/__init__.py
+-rwxr-xr-x   0 Matteo     (501) staff       (20)     2605 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/mpe/simple.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     8898 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/mpe/simple_adversary.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     6464 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/mpe/simple_crypto.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     6094 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/mpe/simple_push.py
+-rwxr-xr-x   0 Matteo     (501) staff       (20)     5256 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/mpe/simple_reference.py
+-rwxr-xr-x   0 Matteo     (501) staff       (20)     5456 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/mpe/simple_speaker_listener.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     4446 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/mpe/simple_spread.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    10156 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/mpe/simple_tag.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    13418 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/mpe/simple_world_comm.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    15788 2024-05-20 13:36:10.000000 vmas-1.4.1/vmas/scenarios/multi_give_way.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    14076 2024-05-20 13:36:10.000000 vmas-1.4.1/vmas/scenarios/navigation.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    12063 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/passage.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     7003 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/reverse_transport.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    13844 2024-05-20 13:36:10.000000 vmas-1.4.1/vmas/scenarios/sampling.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    12685 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/transport.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     4596 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/scenarios/wheel.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    15433 2024-05-20 13:36:10.000000 vmas-1.4.1/vmas/scenarios/wind_flocking.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-05-20 13:37:28.222784 vmas-1.4.1/vmas/simulator/
+-rw-r--r--   0 Matteo     (501) staff       (20)       94 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/__init__.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-05-20 13:37:28.223075 vmas-1.4.1/vmas/simulator/controllers/
+-rw-r--r--   0 Matteo     (501) staff       (20)       94 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/controllers/__init__.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     4606 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/controllers/velocity_controller.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    82990 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/core.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-05-20 13:37:28.224446 vmas-1.4.1/vmas/simulator/dynamics/
+-rw-r--r--   0 Matteo     (501) staff       (20)       94 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/dynamics/__init__.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     1341 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/dynamics/common.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     2594 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/dynamics/diff_drive.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     5321 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/dynamics/drone.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      362 2024-02-29 10:15:20.000000 vmas-1.4.1/vmas/simulator/dynamics/holonomic.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      425 2024-01-10 08:50:22.000000 vmas-1.4.1/vmas/simulator/dynamics/holonomic_with_rot.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     4377 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/dynamics/kinematic_bicycle.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-05-20 13:37:28.225129 vmas-1.4.1/vmas/simulator/environment/
+-rw-r--r--   0 Matteo     (501) staff       (20)      551 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/environment/__init__.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    31544 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/environment/environment.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     3806 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/environment/gym.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     8642 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/environment/rllib.py
+-rw-r--r--   0 Matteo     (501) staff       (20)      663 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/heuristic_policy.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     6869 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/joints.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    14228 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/physics.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    14787 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/rendering.py
+-rw-r--r--   0 Matteo     (501) staff       (20)    16655 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/scenario.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     7780 2023-05-25 09:41:18.000000 vmas-1.4.1/vmas/simulator/secrcode.ttf
+-rw-r--r--   0 Matteo     (501) staff       (20)     4097 2024-05-03 15:58:49.000000 vmas-1.4.1/vmas/simulator/sensors.py
+-rw-r--r--   0 Matteo     (501) staff       (20)     8932 2024-05-20 13:36:10.000000 vmas-1.4.1/vmas/simulator/utils.py
+drwxr-xr-x   0 Matteo     (501) staff       (20)        0 2024-05-20 13:37:28.225345 vmas-1.4.1/vmas.egg-info/
+-rw-r--r--   0 Matteo     (501) staff       (20)      364 2024-05-20 13:37:28.000000 vmas-1.4.1/vmas.egg-info/PKG-INFO
+-rw-r--r--   0 Matteo     (501) staff       (20)     2556 2024-05-20 13:37:28.000000 vmas-1.4.1/vmas.egg-info/SOURCES.txt
+-rw-r--r--   0 Matteo     (501) staff       (20)        1 2024-05-20 13:37:28.000000 vmas-1.4.1/vmas.egg-info/dependency_links.txt
+-rw-r--r--   0 Matteo     (501) staff       (20)       35 2024-05-20 13:37:28.000000 vmas-1.4.1/vmas.egg-info/requires.txt
+-rw-r--r--   0 Matteo     (501) staff       (20)        5 2024-05-20 13:37:28.000000 vmas-1.4.1/vmas.egg-info/top_level.txt
```

### Comparing `vmas-1.4.0/LICENSE` & `vmas-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vmas-1.4.0/README.md` & `vmas-1.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # VectorizedMultiAgentSimulator (VMAS)
 <a href="https://pypi.org/project/vmas"><img src="https://img.shields.io/pypi/v/vmas" alt="pypi version"></a>
 [![Downloads](https://static.pepy.tech/personalized-badge/vmas?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/vmas)
-![tests](https://github.com/proroklab/VectorizedMultiAgentSimulator/actions/workflows/python-app.yml/badge.svg)
-[![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://www.python.org/downloads/)
+![tests](https://github.com/proroklab/VectorizedMultiAgentSimulator/actions/workflows/tests-linux.yml/badge.svg)
+[![codecov](https://codecov.io/github/proroklab/VectorizedMultiAgentSimulator/coverage.svg?branch=main)](https://codecov.io/gh/proroklab/VectorizedMultiAgentSimulator)
+[![Documentation Status](https://readthedocs.org/projects/vmas/badge/?version=latest)](https://vmas.readthedocs.io/en/latest/?badge=latest)
+[![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://www.python.org/downloads/)
 [![GitHub license](https://img.shields.io/badge/license-GPLv3.0-blue.svg)](https://github.com/proroklab/VectorizedMultiAgentSimulator/blob/main/LICENSE)
+[![arXiv](https://img.shields.io/badge/arXiv-2207.03530-b31b1b.svg)](https://arxiv.org/abs/2207.03530)
+
 
 <p align="center">
 <img src="https://github.com/matteobettini/vmas-media/blob/main/media/VMAS_scenarios.gif?raw=true" alt="drawing"/>  
 </p>
 
 > [!NOTE]  
 > We have just released [BenchMARL](https://github.com/facebookresearch/BenchMARL), a benchmarking library where you 
@@ -86,17 +90,18 @@
   * [TODOS](#todos)
 
 
 ## How to use
 ### Notebooks
 -  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/proroklab/VectorizedMultiAgentSimulator/blob/main/notebooks/VMAS_Use_vmas_environment.ipynb) &ensp; **Using a VMAS environment**.
  Here is a simple notebook that you can run to create, step and render any scenario in VMAS. It reproduces the `use_vmas_env.py` script in the `examples` folder.
-- [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/facebookresearch/BenchMARL/blob/main/notebooks/run.ipynb) &ensp;  **Using VMAS in BenchMARL (suggested)**.  In this notebook, we show how to use VMAS in [BenchMARL](https://github.com/facebookresearch/BenchMARL), TorchRL's MARL training library.
-- [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pytorch/rl/blob/gh-pages/_downloads/a977047786179278d12b52546e1c0da8/multiagent_ppo.ipynb)  &ensp;  **Using VMAS in TorchRL**.  In this notebook, [available in the TorchRL docs](https://pytorch.org/rl/tutorials/multiagent_ppo.html), we show how to use any VMAS scenario in TorchRL. It will guide you through the full pipeline needed to train agents using MAPPO/IPPO.
-- [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/proroklab/VectorizedMultiAgentSimulator/blob/main/notebooks/VMAS_RLlib.ipynb)  &ensp;  **Using VMAS in RLlib**.  In this notebook, we show how to use any VMAS scenario in RLlib. It reproduces the `rllib.py` script in the `examples` folder.
+- [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/facebookresearch/BenchMARL/blob/main/notebooks/run.ipynb) &ensp;  **Training VMAS in BenchMARL (suggested)**.  In this notebook, we show how to use VMAS in [BenchMARL](https://github.com/facebookresearch/BenchMARL), TorchRL's MARL training library.
+- [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pytorch/rl/blob/gh-pages/_downloads/a977047786179278d12b52546e1c0da8/multiagent_ppo.ipynb)  &ensp;  **Training VMAS in TorchRL**.  In this notebook, [available in the TorchRL docs](https://pytorch.org/rl/tutorials/multiagent_ppo.html), we show how to use any VMAS scenario in TorchRL. It will guide you through the full pipeline needed to train agents using MAPPO/IPPO.
+- [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pytorch/rl/blob/gh-pages/_downloads/d30bb6552cc07dec0f1da33382d3fa02/multiagent_competitive_ddpg.py)  &ensp;  **Training competitive VMAS MPE in TorchRL**.  In this notebook, [available in the TorchRL docs](https://pytorch.org/rl/main/tutorials/multiagent_competitive_ddpg.html), we show how to solve a Competitive Multi-Agent Reinforcement Learning (MARL) problem using MADDPG/IDDPG.
+- [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/proroklab/VectorizedMultiAgentSimulator/blob/main/notebooks/VMAS_RLlib.ipynb)  &ensp;  **Training VMAS in RLlib**.  In this notebook, we show how to use any VMAS scenario in RLlib. It reproduces the `rllib.py` script in the `examples` folder.
 
 
 
 ### Install
 
 To install the simulator, you can use pip to get the latest release:
 ```bash
@@ -113,16 +118,16 @@
 # Training
 pip install "ray[rllib]"==2.1.0 # We support versions "ray[rllib]<=2.2,>=1.13"
 pip install torchrl
 
 # Logging
 pip installl wandb 
 
-# Save renders
-pip install opencv-python moviepy
+# Rendering
+pip install opencv-python moviepy matplotlib
 
 # Tests
 pip install pytest pyyaml pytest-instafail tqdm
 ```
 
 ### Run 
 
@@ -160,15 +165,15 @@
 VMAS is supported by [TorchRL](https://github.com/pytorch/rl) and its MARL training library [BenchMARL](https://github.com/facebookresearch/BenchMARL).
 
 Check out how simple it is to use VMAS in [BenchMARL](https://github.com/facebookresearch/BenchMARL) with this [notebook](https://colab.research.google.com/github/facebookresearch/BenchMARL/blob/main/notebooks/run.ipynb).
 
 We provide a [notebook](https://pytorch.org/rl/tutorials/multiagent_ppo.html) which guides you through a full
 multi-agent reinforcement learning pipeline for training VMAS scenarios in TorchRL using MAPPO/IPPO.
 
-You can find **example scripts** in the TorchRL repo [here](https://github.com/pytorch/rl/tree/main/examples/multiagent)
+You can find **example scripts** in the TorchRL repo [here](https://github.com/pytorch/rl/tree/main/sota-implementations/multiagent)
 on how to run MAPPO-IPPO-MADDPG-QMIX-VDN using the [VMAS wrapper](https://github.com/pytorch/rl/blob/main/torchrl/envs/libs/vmas.py).
 
 
 
 ### Input and output spaces
 
 VMAS uses gym spaces for input and output spaces. 
@@ -242,15 +247,15 @@
 - **Non-differentiable communication**: Scenarios can require agents to perform discrete or continuous communication actions.
 - **Gravity**: VMAS supports customizable gravity.
 - **Sensors**: Our simulator implements ray casting, which can be used to simulate a wide range of distance-based sensors that can be added to agents. We currently support LIDARs. To see available sensors, have a look at the `sensors` script.
 - **Joints**: Our simulator supports joints. Joints are constraints that keep entities at a specified distance. The user can specify the anchor points on the two objects, the distance (including 0), the thickness of the joint, if the joint is allowed to rotate at either anchor point, and if he wants the joint to be collidable. Have a look at the waterfall scenario to see how you can use joints. See the `waterfall` and `joint_passage` scenarios for an example.
 - **Agent actions**: Agents' physical actions are 2D forces for holonomic motion. Agent rotation can also be controlled through a torque action (activated by setting `agent.action.u_rot_range` at agent creation time). Agents can also be equipped with continuous or discrete communication actions.
 - **Action preprocessing**: By implementing the `process_action` function of a scenario, you can modify the agents' actions before they are passed to the simulator. This is used in `controllers` (where we provide different types of controllers to use) and `dynamics` (where we provide custom robot dynamic models).
 - **Controllers**: Controllers are components that can be appended to the neural network policy or replace it completely.  We provide a `VelocityController` which can be used to treat input actions as velocities (instead of default vmas input forces). This PID controller takes velocities and outputs the forces which are fed to the simulator. See the `vel_control` debug scenario for an example.
-- **Dynamic models**: VMAS simulates holonomic dynamics models by default. Custom dynamics can be chosen at agent creation time. Implementations now include `DiffDriveDynamics` for differential drive robots and `KinematicBicycleDynamics` for kinematic bicycle model. See `diff_drive` and `kinematic_bicycle` debug scenarios for examples.
+- **Dynamic models**: VMAS simulates holonomic dynamics models by default. Custom dynamics can be chosen at agent creation time. Implementations now include `DiffDriveDynamics` for differential drive robots, `KinematicBicycleDynamics` for kinematic bicycle model, and `Drone` for quadcopter dynamics. See `diff_drive`, `kinematic_bicycle` and `drone` debug scenarios for examples.
 - **Differentiable**: By setting `grad_enabled=True` when creating an environment, the simulator will be differentiable, allowing gradients flowing through any of its function.
 
 ## Creating a new scenario
 
 To create a new scenario, just extend the `BaseScenario` class in `scenario.py`.
 
 You will need to implement at least `make_world`, `reset_world_at`, `observation`, and `reward`. Optionally, you can also implement `done`, `info`, `process_action`, and `extra_render`.
@@ -376,14 +381,15 @@
 | `vel_control.py`       | Example scenario where three agents have velocity controllers with different acceleration constraints                                                                                                                                                                                                                                                                                   | <img src="https://github.com/matteobettini/vmas-media/blob/main/media/scenarios/vel_control.gif?raw=true" alt="drawing" width="300"/>       |
 | `goal.py`              | An agent with a velocity controller is spawned at random in the workspace. It is rewarded for moving to a randomly initialised goal while consuming the least energy. The agent observes its velocity and the relative position to the goal.                                                                                                                                            | <img src="https://github.com/matteobettini/vmas-media/blob/main/media/scenarios/goal.gif?raw=true" alt="drawing" width="300"/>              | 
 | `het_mass.py`          | Two agents with different masses are spawned randomly in the workspace. They are rewarded for maximising the team maximum speed while minimizing the team energy expenditure. The optimal policy requires the heavy agent to stay still while the light agent moves at maximum speed.                                                                                                   | <img src="https://github.com/matteobettini/vmas-media/blob/main/media/scenarios/het_mass.gif?raw=true" alt="drawing" width="300"/>          |
 | `line_trajectory.py`   | One agent is rewarded to move in a line trajectory.                                                                                                                                                                                                                                                                                                                                     | <img src="https://github.com/matteobettini/vmas-media/blob/main/media/scenarios/line_trajectory.gif?raw=true" alt="drawing" width="300"/>   |
 | `circle_trajectory.py` | One agent is rewarded to move in a circle trajectory at the `desired_radius`.                                                                                                                                                                                                                                                                                                           | <img src="https://github.com/matteobettini/vmas-media/blob/main/media/scenarios/circle_trajectory.gif?raw=true" alt="drawing" width="300"/> |
 | `diff_drive.py`        | An example of the `diff_drive` dynamic model constraint. Both agents have rotational actions which can be controlled interactively.  The first agent has differential drive dynamics. The second agent has standard vmas holonomic dynamics.                                                                                                                                            | <img src="https://github.com/matteobettini/vmas-media/blob/main/media/scenarios/diff_drive.gif?raw=true" alt="drawing" width="300"/>        |
 | `kinematic_bicycle.py` | An example of `kinematic_bicycle` dynamic model constraint. Both agents have rotational actions which can be controlled interactively.  The first agent has kinematic bicycle model dynamics. The second agent has standard vmas holonomic dynamics.                                                                                                                                    | <img src="https://github.com/matteobettini/vmas-media/blob/main/media/scenarios/kinematic_bicycle.gif?raw=true" alt="drawing" width="300"/> |
+| `drone.py`             | An example of the `drone` dynamic model.                                                                                                                                                                                                                                                                                                                                                | <img src="https://github.com/matteobettini/vmas-media/blob/main/media/scenarios/drone.gif?raw=true" alt="drawing" width="300"/>             |
 
 ### [MPE](https://github.com/openai/multiagent-particle-envs)
 
 | Env name in code (name in paper)                         | Communication? | Competitive? | Notes                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 |----------------------------------------------------------|----------------|--------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `simple.py`                                              | N              | N            | Single agent sees landmark position, rewarded based on how close it gets to landmark. Not a multi-agent environment -- used for debugging policies.                                                                                                                                                                                                                                                                                                                                                                                                               |
 | `simple_adversary.py` (Physical deception)               | N              | Y            | 1 adversary (red), N good agents (green), N landmarks (usually N=2). All agents observe position of landmarks and other agents. One landmark is the ‘target landmark’ (colored green). Good agents rewarded based on how close one of them is to the target landmark, but negatively rewarded if the adversary is close to target landmark. Adversary is rewarded based on how close it is to the target, but it doesn’t know which landmark is the target landmark. So good agents have to learn to ‘split up’ and cover all landmarks to deceive the adversary. |
@@ -401,18 +407,18 @@
 - [HetGPPO](https://matteobettini.github.io/publication/heterogeneous-multi-robot-reinforcement-learning/) features training of `het_mass`, `give_way`, `joint_passage`, `joint_passage_size`
 - [SND](https://matteobettini.github.io/publication/system-neural-diversity-measuring-behavioral-heterogeneity-in-multi-agent-learning/) features training of `navigation`, `joint_passage`, `joint_passage_size`, `wind`
 - [TorchRL](https://matteobettini.com/publication/torchrl-a-data-driven-decision-making-library-for-pytorch/) features training of `navigation`, `sampling`, `balance`
 
 ## TODOS
 
 - [ ] Reset any number of dimensions
-- [ ] Improve test efficiency and add new tests
 - [ ] Implement 1D camera sensor
 - [ ] Implement 2D birds eye view camera sensor
-- [ ] Implement 2D drone dynamics
+- [X] Improve test efficiency and add new tests
+- [X] Implement 2D drone dynamics
 - [X] Allow any number of actions
 - [X] Improve VMAS performance
 - [X] Dict obs support in torchrl
 - [X] Make TextLine a Geom usable in a scenario
 - [X] Notebook on how to use torch rl with vmas
 - [X] Allow dict obs spaces and multidim obs
 - [X] Talk about action preprocessing and velocity controller
@@ -426,8 +432,8 @@
   - [x] simple_adversary
   - [X] simple_crypto
   - [X] simple_push
   - [X] simple_reference
   - [X] simple_speaker_listener
   - [X] simple_spread
   - [X] simple_tag
-  - [X] simple_world_comm
+  - [X] simple_world_comm
```

#### html2text {}

```diff
@@ -1,16 +1,23 @@
 # VectorizedMultiAgentSimulator (VMAS) _[_p_y_p_i_ _v_e_r_s_i_o_n_][![Downloads](https://
 static.pepy.tech/personalized-badge/
 vmas?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)]
 (https://pepy.tech/project/vmas) ![tests](https://github.com/proroklab/
-VectorizedMultiAgentSimulator/actions/workflows/python-app.yml/badge.svg) [!
-[Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-
-blue.svg)](https://www.python.org/downloads/) [![GitHub license](https://
-img.shields.io/badge/license-GPLv3.0-blue.svg)](https://github.com/proroklab/
-VectorizedMultiAgentSimulator/blob/main/LICENSE)
+VectorizedMultiAgentSimulator/actions/workflows/tests-linux.yml/badge.svg) [!
+[codecov](https://codecov.io/github/proroklab/VectorizedMultiAgentSimulator/
+coverage.svg?branch=main)](https://codecov.io/gh/proroklab/
+VectorizedMultiAgentSimulator) [![Documentation Status](https://
+readthedocs.org/projects/vmas/badge/?version=latest)](https://
+vmas.readthedocs.io/en/latest/?badge=latest) [![Python](https://img.shields.io/
+badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://
+www.python.org/downloads/) [![GitHub license](https://img.shields.io/badge/
+license-GPLv3.0-blue.svg)](https://github.com/proroklab/
+VectorizedMultiAgentSimulator/blob/main/LICENSE) [![arXiv](https://
+img.shields.io/badge/arXiv-2207.03530-b31b1b.svg)](https://arxiv.org/abs/
+2207.03530)
                                    [drawing]
 > [!NOTE] > We have just released [BenchMARL](https://github.com/
 facebookresearch/BenchMARL), a benchmarking library where you > can train VMAS
 tasks using TorchRL! > Check out [how easy it is to use it.](https://
 colab.research.google.com/github/facebookresearch/BenchMARL/blob/main/
 notebooks/run.ipynb) ## Welcome to VMAS! This repository contains the code for
 the Vectorized Multi-Agent Simulator (VMAS). VMAS is a vectorized
@@ -61,46 +68,53 @@
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/proroklab/VectorizedMultiAgentSimulator/blob/
 main/notebooks/VMAS_Use_vmas_environment.ipynb)   **Using a VMAS environment**.
 Here is a simple notebook that you can run to create, step and render any
 scenario in VMAS. It reproduces the `use_vmas_env.py` script in the `examples`
 folder. - [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/facebookresearch/
-BenchMARL/blob/main/notebooks/run.ipynb)   **Using VMAS in BenchMARL
+BenchMARL/blob/main/notebooks/run.ipynb)   **Training VMAS in BenchMARL
 (suggested)**. In this notebook, we show how to use VMAS in [BenchMARL](https:/
 /github.com/facebookresearch/BenchMARL), TorchRL's MARL training library. - [!
 [Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/github/pytorch/rl/blob/gh-pages/_downloads/
-a977047786179278d12b52546e1c0da8/multiagent_ppo.ipynb)   **Using VMAS in
+a977047786179278d12b52546e1c0da8/multiagent_ppo.ipynb)   **Training VMAS in
 TorchRL**. In this notebook, [available in the TorchRL docs](https://
 pytorch.org/rl/tutorials/multiagent_ppo.html), we show how to use any VMAS
 scenario in TorchRL. It will guide you through the full pipeline needed to
 train agents using MAPPO/IPPO. - [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/pytorch/rl/blob/gh-pages/_downloads/
+d30bb6552cc07dec0f1da33382d3fa02/multiagent_competitive_ddpg.py)   **Training
+competitive VMAS MPE in TorchRL**. In this notebook, [available in the TorchRL
+docs](https://pytorch.org/rl/main/tutorials/multiagent_competitive_ddpg.html),
+we show how to solve a Competitive Multi-Agent Reinforcement Learning (MARL)
+problem using MADDPG/IDDPG. - [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/proroklab/VectorizedMultiAgentSimulator/blob/
-main/notebooks/VMAS_RLlib.ipynb)   **Using VMAS in RLlib**. In this notebook,
-we show how to use any VMAS scenario in RLlib. It reproduces the `rllib.py`
-script in the `examples` folder. ### Install To install the simulator, you can
-use pip to get the latest release: ```bash pip install vmas ``` If you want to
-install the current master version (more up to date than latest release), you
-can do: ```bash git clone https://github.com/proroklab/
+main/notebooks/VMAS_RLlib.ipynb)   **Training VMAS in RLlib**. In this
+notebook, we show how to use any VMAS scenario in RLlib. It reproduces the
+`rllib.py` script in the `examples` folder. ### Install To install the
+simulator, you can use pip to get the latest release: ```bash pip install vmas
+``` If you want to install the current master version (more up to date than
+latest release), you can do: ```bash git clone https://github.com/proroklab/
 VectorizedMultiAgentSimulator.git cd VectorizedMultiAgentSimulator pip install
 -e . ``` By default, vmas has only the core requirements. Here are some
 optional packages you may want to install: ```bash # Training pip install "ray
 [rllib]"==2.1.0 # We support versions "ray[rllib]<=2.2,>=1.13" pip install
-torchrl # Logging pip installl wandb # Save renders pip install opencv-python
-moviepy # Tests pip install pytest pyyaml pytest-instafail tqdm ``` ### Run To
-use the simulator, simply create an environment by passing the name of the
-scenario you want (from the `scenarios` folder) to the `make_env` function. The
-function arguments are explained in the documentation. The function returns an
-environment object with the OpenAI gym interface: Here is an example: ```python
-env = vmas.make_env( scenario="waterfall", # can be scenario name or
-BaseScenario class num_envs=32, device="cpu", # Or "cuda" for GPU
-continuous_actions=True, wrapper=None, # One of: None, vmas.Wrapper.RLLIB, and
-vmas.Wrapper.GYM max_steps=None, # Defines the horizon. None is infinite
+torchrl # Logging pip installl wandb # Rendering pip install opencv-python
+moviepy matplotlib # Tests pip install pytest pyyaml pytest-instafail tqdm ```
+### Run To use the simulator, simply create an environment by passing the name
+of the scenario you want (from the `scenarios` folder) to the `make_env`
+function. The function arguments are explained in the documentation. The
+function returns an environment object with the OpenAI gym interface: Here is
+an example: ```python env = vmas.make_env( scenario="waterfall", # can be
+scenario name or BaseScenario class num_envs=32, device="cpu", # Or "cuda" for
+GPU continuous_actions=True, wrapper=None, # One of: None, vmas.Wrapper.RLLIB,
+and vmas.Wrapper.GYM max_steps=None, # Defines the horizon. None is infinite
 horizon. seed=None, # Seed of the environment dict_spaces=False, # By default
 tuple spaces are used with each element in the tuple being an agent. # If
 dict_spaces=True, the spaces will become Dict with each key being the agent's
 name grad_enabled=False, # If grad_enabled the simulator is differentiable and
 gradients can flow from output to input **kwargs # Additional arguments you
 want to pass to the scenario initialization ) ``` A further example that you
 can run is contained in `use_vmas_env.py` in the `examples` directory. ####
@@ -112,24 +126,24 @@
 how simple it is to use VMAS in [BenchMARL](https://github.com/
 facebookresearch/BenchMARL) with this [notebook](https://
 colab.research.google.com/github/facebookresearch/BenchMARL/blob/main/
 notebooks/run.ipynb). We provide a [notebook](https://pytorch.org/rl/tutorials/
 multiagent_ppo.html) which guides you through a full multi-agent reinforcement
 learning pipeline for training VMAS scenarios in TorchRL using MAPPO/IPPO. You
 can find **example scripts** in the TorchRL repo [here](https://github.com/
-pytorch/rl/tree/main/examples/multiagent) on how to run MAPPO-IPPO-MADDPG-QMIX-
-VDN using the [VMAS wrapper](https://github.com/pytorch/rl/blob/main/torchrl/
-envs/libs/vmas.py). ### Input and output spaces VMAS uses gym spaces for input
-and output spaces. By default, action and observation spaces are tuples:
-```python spaces.Tuple( [agent_space for agent in agents] ) ``` When creating
-the environment, by setting `dict_spaces=True`, tuples can be changed to
-dictionaries: ```python spaces.Dict( {agent.name: agent_space for agent in
-agents} ) ``` #### Output spaces If `dict_spaces=False`, observations, infos,
-and rewards returned by the environment will be a list with each element being
-the value for that agent. If `dict_spaces=True`, observations, infos, and
+pytorch/rl/tree/main/sota-implementations/multiagent) on how to run MAPPO-IPPO-
+MADDPG-QMIX-VDN using the [VMAS wrapper](https://github.com/pytorch/rl/blob/
+main/torchrl/envs/libs/vmas.py). ### Input and output spaces VMAS uses gym
+spaces for input and output spaces. By default, action and observation spaces
+are tuples: ```python spaces.Tuple( [agent_space for agent in agents] ) ```
+When creating the environment, by setting `dict_spaces=True`, tuples can be
+changed to dictionaries: ```python spaces.Dict( {agent.name: agent_space for
+agent in agents} ) ``` #### Output spaces If `dict_spaces=False`, observations,
+infos, and rewards returned by the environment will be a list with each element
+being the value for that agent. If `dict_spaces=True`, observations, infos, and
 rewards returned by the environment will be a dictionary with each element
 having key = agent_name and value being the value for that agent. Each agent
 **observation** in either of these structures is either (depending on how you
 implement the scenario): - a tensor with shape `[num_envs, observation_size]`,
 where `observation_size` is the size of the agent's observation. ```python def
 observation(self, agent: Agent): return torch.cat([agent.state.pos,
 agent.state.vel], dim=-1) ``` - a dictionary of such tensors ```python def
@@ -205,38 +219,39 @@
 **Controllers**: Controllers are components that can be appended to the neural
 network policy or replace it completely. We provide a `VelocityController`
 which can be used to treat input actions as velocities (instead of default vmas
 input forces). This PID controller takes velocities and outputs the forces
 which are fed to the simulator. See the `vel_control` debug scenario for an
 example. - **Dynamic models**: VMAS simulates holonomic dynamics models by
 default. Custom dynamics can be chosen at agent creation time. Implementations
-now include `DiffDriveDynamics` for differential drive robots and
-`KinematicBicycleDynamics` for kinematic bicycle model. See `diff_drive` and
-`kinematic_bicycle` debug scenarios for examples. - **Differentiable**: By
-setting `grad_enabled=True` when creating an environment, the simulator will be
-differentiable, allowing gradients flowing through any of its function. ##
-Creating a new scenario To create a new scenario, just extend the
-`BaseScenario` class in `scenario.py`. You will need to implement at least
-`make_world`, `reset_world_at`, `observation`, and `reward`. Optionally, you
-can also implement `done`, `info`, `process_action`, and `extra_render`. You
-can also change the viewer size, zoom, and enable a background rendered grid by
-changing these inherited attributes in the `make_world` function. To know how,
-just read the documentation of `BaseScenario` in `scenario.py` and look at the
-implemented scenarios. ## Play a scenario You can play with a scenario
-interactively! **Just execute its script!** Just use the `render_interactively`
-function in the `interactive_rendering.py` script. Relevant values will be
-plotted to screen. Move the agent with the arrow keys and switch agents with
-TAB. You can reset the environment by pressing R. If you have more than 1
-agent, you can control another one with W,A,S,D and switch the second agent
-using LSHIFT. To do this, just set `control_two_agents=True`. If the agents
-also have rotational actions, you can control them with M,N for the first agent
-and with Q,E (for example in the `diff_drive` scenario). On the screen you will
-see some data from the agent controlled with arrow keys. This data includes:
-name, current obs, current reward, total reward so far and environment done
-flag. Here is an overview of what it looks like:
+now include `DiffDriveDynamics` for differential drive robots,
+`KinematicBicycleDynamics` for kinematic bicycle model, and `Drone` for
+quadcopter dynamics. See `diff_drive`, `kinematic_bicycle` and `drone` debug
+scenarios for examples. - **Differentiable**: By setting `grad_enabled=True`
+when creating an environment, the simulator will be differentiable, allowing
+gradients flowing through any of its function. ## Creating a new scenario To
+create a new scenario, just extend the `BaseScenario` class in `scenario.py`.
+You will need to implement at least `make_world`, `reset_world_at`,
+`observation`, and `reward`. Optionally, you can also implement `done`, `info`,
+`process_action`, and `extra_render`. You can also change the viewer size,
+zoom, and enable a background rendered grid by changing these inherited
+attributes in the `make_world` function. To know how, just read the
+documentation of `BaseScenario` in `scenario.py` and look at the implemented
+scenarios. ## Play a scenario You can play with a scenario interactively!
+**Just execute its script!** Just use the `render_interactively` function in
+the `interactive_rendering.py` script. Relevant values will be plotted to
+screen. Move the agent with the arrow keys and switch agents with TAB. You can
+reset the environment by pressing R. If you have more than 1 agent, you can
+control another one with W,A,S,D and switch the second agent using LSHIFT. To
+do this, just set `control_two_agents=True`. If the agents also have rotational
+actions, you can control them with M,N for the first agent and with Q,E (for
+example in the `diff_drive` scenario). On the screen you will see some data
+from the agent controlled with arrow keys. This data includes: name, current
+obs, current reward, total reward so far and environment done flag. Here is an
+overview of what it looks like:
                                    [drawing]
 ## Rendering To render the environment, just call the `render` or the
 `try_render_at` functions (depending on environment wrapping). Example: ```
 env.render( mode="rgb_array", # "rgb_array" returns image, "human" renders in
 display agent_index_focus=4, # If None keep all agents in camera, else focus
 camera on specific agent index=0, # Index of batched environment to render
 visualize_when_rgb: bool = False, # Also run human visualization when
@@ -568,15 +583,16 @@
 [drawing]| | `diff_drive.py` | An example of the `diff_drive` dynamic model
 constraint. Both agents have rotational actions which can be controlled
 interactively. The first agent has differential drive dynamics. The second
 agent has standard vmas holonomic dynamics. | [drawing]| |
 `kinematic_bicycle.py` | An example of `kinematic_bicycle` dynamic model
 constraint. Both agents have rotational actions which can be controlled
 interactively. The first agent has kinematic bicycle model dynamics. The second
-agent has standard vmas holonomic dynamics. | [drawing]| ### [MPE](https://
+agent has standard vmas holonomic dynamics. | [drawing]| | `drone.py` | An
+example of the `drone` dynamic model. | [drawing]| ### [MPE](https://
 github.com/openai/multiagent-particle-envs) | Env name in code (name in paper)
 | Communication? | Competitive? | Notes | |------------------------------------
 ----------------------|----------------|--------------|------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
@@ -631,17 +647,17 @@
 publication/heterogeneous-multi-robot-reinforcement-learning/) features
 training of `het_mass`, `give_way`, `joint_passage`, `joint_passage_size` -
 [SND](https://matteobettini.github.io/publication/system-neural-diversity-
 measuring-behavioral-heterogeneity-in-multi-agent-learning/) features training
 of `navigation`, `joint_passage`, `joint_passage_size`, `wind` - [TorchRL]
 (https://matteobettini.com/publication/torchrl-a-data-driven-decision-making-
 library-for-pytorch/) features training of `navigation`, `sampling`, `balance`
-## TODOS - [ ] Reset any number of dimensions - [ ] Improve test efficiency and
-add new tests - [ ] Implement 1D camera sensor - [ ] Implement 2D birds eye
-view camera sensor - [ ] Implement 2D drone dynamics - [X] Allow any number of
+## TODOS - [ ] Reset any number of dimensions - [ ] Implement 1D camera sensor
+- [ ] Implement 2D birds eye view camera sensor - [X] Improve test efficiency
+and add new tests - [X] Implement 2D drone dynamics - [X] Allow any number of
 actions - [X] Improve VMAS performance - [X] Dict obs support in torchrl - [X]
 Make TextLine a Geom usable in a scenario - [X] Notebook on how to use torch rl
 with vmas - [X] Allow dict obs spaces and multidim obs - [X] Talk about action
 preprocessing and velocity controller - [X] New envs from joint project with
 their descriptions - [X] Talk about navigation / multi_goal - [X] Link video of
 experiments - [X] Add LIDAR section - [X] Implement LIDAR - [X] Rewrite all MPE
 scenarios - [X] simple - [x] simple_adversary - [X] simple_crypto - [X]
```

### Comparing `vmas-1.4.0/vmas/__init__.py` & `vmas-1.4.1/vmas/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 from vmas.interactive_rendering import render_interactively
 from vmas.make_env import make_env
 from vmas.simulator.environment import Wrapper
 
 from vmas.simulator.utils import _init_pyglet_device
 
 _init_pyglet_device()
 
 __all__ = [
     "make_env",
     "render_interactively",
-    "Wrapper",
     "scenarios",
     "debug_scenarios",
     "mpe_scenarios",
 ]
 
+__version__ = "1.4.1"
+
 scenarios = sorted(
     [
         "dropout",
         "dispersion",
         "transport",
         "reverse_transport",
         "give_way",
@@ -39,36 +40,41 @@
         "buzz_wire",
         "multi_give_way",
         "navigation",
         "sampling",
         "wind_flocking",
     ]
 )
+"""List of the vmas scenarios (excluding MPE and debug)"""
 
 debug_scenarios = sorted(
     [
         "asym_joint",
         "circle_trajectory",
         "goal",
         "het_mass",
         "line_trajectory",
         "vel_control",
         "waterfall",
         "diff_drive",
         "kinematic_bicycle",
         "pollock",
+        "drone",
     ]
 )
+"""List of the vmas debug scenarios """
+
 
 mpe_scenarios = sorted(
     [
         "simple",
         "simple_adversary",
         "simple_crypto",
         "simple_push",
         "simple_reference",
         "simple_speaker_listener",
         "simple_spread",
         "simple_tag",
         "simple_world_comm",
     ]
 )
+"""List of the vmas MPE scenarios """
```

### Comparing `vmas-1.4.0/vmas/examples/rllib.py` & `vmas-1.4.1/vmas/examples/rllib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 import os
 from typing import Dict, Optional
 
 import numpy as np
@@ -12,15 +12,17 @@
 from ray.rllib import BaseEnv, Policy, RolloutWorker
 from ray.rllib.agents.ppo import PPOTrainer
 from ray.rllib.algorithms.callbacks import DefaultCallbacks, MultiCallbacks
 from ray.rllib.evaluation import Episode, MultiAgentEpisode
 from ray.rllib.utils.typing import PolicyID
 from ray.tune import register_env
 from ray.tune.integration.wandb import WandbLoggerCallback
-from vmas import make_env, Wrapper
+
+from vmas import make_env
+from vmas.simulator.environment import Wrapper
 
 scenario_name = "balance"
 
 # Scenario specific variables.
 # When modifying this also modify env_config and env_creator
 n_agents = 4
 
@@ -114,15 +116,14 @@
         episode.media["rendering"] = wandb.Video(
             vid, fps=1 / base_env.vector_env.env.world.dt, format="mp4"
         )
         self.frames = []
 
 
 def train():
-
     RLLIB_NUM_GPUS = int(os.environ.get("RLLIB_NUM_GPUS", "0"))
     num_gpus = 0.001 if RLLIB_NUM_GPUS > 0 else 0  # Driver GPU
     num_gpus_per_worker = (
         (RLLIB_NUM_GPUS - num_gpus) / (num_workers + 1) if vmas_device == "cuda" else 0
     )
 
     tune.run(
```

### Comparing `vmas-1.4.0/vmas/examples/run_heuristic.py` & `vmas-1.4.1/vmas/examples/run_heuristic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 import time
 from typing import Type
 
 import torch
+
 from vmas import make_env
 from vmas.simulator.heuristic_policy import BaseHeuristicPolicy, RandomPolicy
 from vmas.simulator.utils import save_video
 
 
 def run_heuristic(
     scenario_name: str,
     heuristic: Type[BaseHeuristicPolicy] = RandomPolicy,
     n_steps: int = 200,
     n_envs: int = 32,
-    env_kwargs: dict = {},
+    env_kwargs: dict = None,
     render: bool = False,
     save_render: bool = False,
     device: str = "cpu",
 ):
-
     assert not (save_render and not render), "To save the video you have to render it"
+    if env_kwargs is None:
+        env_kwargs = {}
 
     # Scenario specific variables
     policy = heuristic(continuous_action=True)
 
     env = make_env(
         scenario=scenario_name,
         num_envs=n_envs,
@@ -37,15 +39,15 @@
     )
 
     frame_list = []  # For creating a gif
     init_time = time.time()
     step = 0
     obs = env.reset()
     total_reward = 0
-    for s in range(n_steps):
+    for _ in range(n_steps):
         step += 1
         actions = [None] * len(obs)
         for i in range(len(obs)):
             actions[i] = policy.compute_action(obs[i], u_range=env.agents[i].u_range)
         obs, rews, dones, info = env.step(actions)
         rewards = torch.stack(rews, dim=1)
         global_reward = rewards.mean(dim=1)
```

### Comparing `vmas-1.4.0/vmas/examples/use_vmas_env.py` & `vmas-1.4.1/vmas/examples/use_vmas_env.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,87 +7,51 @@
 import torch
 
 from vmas import make_env
 from vmas.simulator.core import Agent
 from vmas.simulator.utils import save_video
 
 
-def _get_random_action(agent: Agent, continuous: bool, env):
-    if continuous:
-        actions = []
-        for action_index in range(agent.action_size):
-            actions.append(
-                torch.zeros(
-                    agent.batch_dim,
-                    device=agent.device,
-                    dtype=torch.float32,
-                ).uniform_(
-                    -agent.action.u_range_tensor[action_index],
-                    agent.action.u_range_tensor[action_index],
-                )
-            )
-        if env.world.dim_c != 0 and not agent.silent:
-            # If the agent needs to communicate
-            for _ in range(env.world.dim_c):
-                actions.append(
-                    torch.zeros(
-                        agent.batch_dim,
-                        device=agent.device,
-                        dtype=torch.float32,
-                    ).uniform_(
-                        0,
-                        1,
-                    )
-                )
-        action = torch.stack(actions, dim=-1)
-    else:
-        action = torch.randint(
-            low=0,
-            high=env.get_agent_action_space(agent).n,
-            size=(agent.batch_dim,),
-            device=agent.device,
-        )
-    return action
-
-
 def _get_deterministic_action(agent: Agent, continuous: bool, env):
     if continuous:
         action = -agent.action.u_range_tensor.expand(env.batch_dim, agent.action_size)
     else:
         action = (
             torch.tensor([1], device=env.device, dtype=torch.long)
             .unsqueeze(-1)
             .expand(env.batch_dim, 1)
         )
-    return action
+    return action.clone()
 
 
 def use_vmas_env(
     render: bool = False,
     save_render: bool = False,
     num_envs: int = 32,
     n_steps: int = 100,
     random_action: bool = False,
     device: str = "cpu",
     scenario_name: str = "waterfall",
     n_agents: int = 4,
     continuous_actions: bool = True,
+    visualize_render: bool = True,
 ):
     """Example function to use a vmas environment
 
     Args:
         continuous_actions (bool): Whether the agents have continuous or discrete actions
         n_agents (int): Number of agents
         scenario_name (str): Name of scenario
         device (str): Torch device to use
         render (bool): Whether to render the scenario
         save_render (bool):  Whether to save render of the scenario
         num_envs (int): Number of vectorized environments
         n_steps (int): Number of steps before returning done
         random_action (bool): Use random actions or have all agents perform the down action
+        visualize_render (bool, optional): Whether to visualize the render. Defaults to ``True``.
 
     Returns:
 
     """
     assert not (save_render and not render), "To save the video you have to render it"
 
     dict_spaces = True  # Weather to return obs, rewards, and infos as dictionaries with agent names
@@ -105,41 +69,41 @@
         n_agents=n_agents,
     )
 
     frame_list = []  # For creating a gif
     init_time = time.time()
     step = 0
 
-    for s in range(n_steps):
+    for _ in range(n_steps):
         step += 1
         print(f"Step {step}")
 
         # VMAS actions can be either a list of tensors (one per agent)
         # or a dict of tensors (one entry per agent with its name as key)
         # Both action inputs can be used independently of what type of space its chosen
         dict_actions = random.choice([True, False])
 
         actions = {} if dict_actions else []
-        for i, agent in enumerate(env.agents):
+        for agent in env.agents:
             if not random_action:
                 action = _get_deterministic_action(agent, continuous_actions, env)
             else:
-                action = _get_random_action(agent, continuous_actions, env)
+                action = env.get_random_action(agent)
             if dict_actions:
                 actions.update({agent.name: action})
             else:
                 actions.append(action)
 
         obs, rews, dones, info = env.step(actions)
 
         if render:
             frame = env.render(
-                mode="rgb_array" if save_render else "human",
+                mode="rgb_array",
                 agent_index_focus=None,  # Can give the camera an agent index to focus on
-                visualize_when_rgb=True,
+                visualize_when_rgb=visualize_render,
             )
             if save_render:
                 frame_list.append(frame)
 
     total_time = time.time() - init_time
     print(
         f"It took: {total_time}s for {n_steps} steps of {num_envs} parallel environments on device {device} "
```

### Comparing `vmas-1.4.0/vmas/interactive_rendering.py` & `vmas-1.4.1/vmas/interactive_rendering.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 You can change agent by pressing TAB
 You can reset the environment by pressing R
 You can move agents with the arrow keys
 If you have more than 1 agent, you can control another one with W,A,S,D
 and switch the agent with these controls using LSHIFT
 """
 from operator import add
-from typing import Union, Dict
+from typing import Dict, Union
 
 import numpy as np
 from torch import Tensor
 
 from vmas.make_env import make_env
 from vmas.simulator.environment import Wrapper
 from vmas.simulator.environment.gym import GymWrapper
@@ -27,16 +27,16 @@
 
 class InteractiveEnv:
     """
     Use this script to interactively play with scenarios
 
     You can change agent by pressing TAB
     You can reset the environment by pressing R
-    You can move agents with the arrow keys and if the agent has a rotational action you can control it with M, N
-    If you have more than 1 agent, you can control another one with W,A,S,D and Q,E for eventual rotational actions
+    You can control agent actions with the arrow keys and M/N (left/right control the first action, up/down control the second, M/N controls the third)
+    If you have more than 1 agent, you can control another one with W,A,S,D and Q,E in the same way.
     and switch the agent with these controls using LSHIFT
     """
 
     def __init__(
         self,
         env: GymWrapper,
         control_two_agents: bool = False,
@@ -296,22 +296,42 @@
 def render_interactively(
     scenario: Union[str, BaseScenario],
     control_two_agents: bool = False,
     display_info: bool = True,
     save_render: bool = False,
     **kwargs,
 ):
-    """
-    Use this script to interactively play with scenarios
+    """Executes a scenario and renders it so that you can debug and control agents interactively.
+
+    You can change the agent to control by pressing TAB.
+    You can reset the environment by pressing R.
+    You can control agent actions with the arrow keys and M/N (left/right control the first action, up/down control the second, M/N controls the third)
+
+    If you have more than 1 agent, you can control another one with W,A,S,D and Q,E in the same way.
+    and switch the agent using LSHIFT.
+
+    Args:
+        scenario (Union[str, BaseScenario]): Scenario to load.
+            Can be the name of a file in `vmas.scenarios` folder or a :class:`~vmas.simulator.scenario.BaseScenario` class
+        control_two_agents (bool, optional): Whether to control two agents or just one. Defaults to ``False``.
+        display_info (bool, optional): Whether to display on the screen the following info from the first controlled agent:
+            name, reward, total reward, done, and observation. Defaults to ``True``.
+        save_render (bool, optional): Whether to save a video of the render up to the first reset.
+            The video will be saved in the directory of this file with the name ``{scenario}_interactive``.
+            Defaults to ``False``.
+
+    Examples:
+        >>> from vmas import render_interactively
+        >>> render_interactively(
+        ...     "waterfall",
+        ...     control_two_agents=True,
+        ...     save_render=False,
+        ...     display_info=True,
+        ... )
 
-    You can change agent by pressing TAB
-    You can reset the environment by pressing R
-    You can move agents with the arrow keys and if the agent has a rotational action you can control it with M, N
-    If you have more than 1 agent, you can control another one with W,A,S,D and Q,E for eventual rotational actions
-    and switch the agent with these controls using LSHIFT
     """
 
     InteractiveEnv(
         make_env(
             scenario=scenario,
             num_envs=1,
             device="cpu",
@@ -320,27 +340,32 @@
             seed=0,
             # Environment specific variables
             **kwargs,
         ),
         control_two_agents=control_two_agents,
         display_info=display_info,
         save_render=save_render,
-        render_name=f"{scenario}",
+        render_name=f"{scenario}_interactive"
+        if isinstance(scenario, str)
+        else "interactive",
     )
 
 
 if __name__ == "__main__":
     # Use this script to interactively play with scenarios
     #
     # You can change agent by pressing TAB
     # You can reset the environment by pressing R
-    # You can move agents with the arrow keys and if the agent has a rotational action you can control it with M, N
-    # If you have more than 1 agent, you can control another one with W,A,S,D and Q,E for eventual rotational actions
+    # You can control agent actions with the arrow keys and M/N (left/right control the first action, up/down control the second, M/N controls the third)
+    # If you have more than 1 agent, you can control another one with W,A,S,D and Q,E in the same way.
     # and switch the agent with these controls using LSHIFT
 
     scenario_name = "waterfall"
 
     # Scenario specific variables
 
     render_interactively(
-        scenario_name, control_two_agents=True, save_render=False, display_info=True
+        scenario_name,
+        control_two_agents=True,
+        save_render=False,
+        display_info=True,
     )
```

### Comparing `vmas-1.4.0/vmas/make_env.py` & `vmas-1.4.1/vmas/make_env.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,73 @@
 #  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 from typing import Optional, Union
 
 from vmas import scenarios
-from vmas.simulator.environment import Environment
-from vmas.simulator.environment import Wrapper
+from vmas.simulator.environment import Environment, Wrapper
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import DEVICE_TYPING
 
 
 def make_env(
     scenario: Union[str, BaseScenario],
-    num_envs: int = 32,
+    num_envs: int,
     device: DEVICE_TYPING = "cpu",
     continuous_actions: bool = True,
     wrapper: Optional[
         Wrapper
     ] = None,  # One of: None, vmas.Wrapper.RLLIB, and vmas.Wrapper.GYM
     max_steps: Optional[int] = None,
     seed: Optional[int] = None,
     dict_spaces: bool = False,
     multidiscrete_actions: bool = False,
     clamp_actions: bool = False,
     grad_enabled: bool = False,
     **kwargs,
 ):
-    """
-    Create a vmas environment
+    """Create a vmas environment.
+
     Args:
-        scenario: Scenario to load. Can be the name of a file in the "scenarios" folder or a `BaseScenario` class.
-        num_envs: Number of vectorized simulation environments.
-        device: Device for simulation
-        continuous_actions: Weather to use continuous actions.
-        wrapper: Wrapper class to use. For example can be Wrapper.RLLIB.
-        max_steps: Maximum number of steps in each vectorized environment after which done is returned
-        seed: seed
-        dict_spaces:  Weather to use dictionary i/o spaces with format {agent_name: tensor}
-            for obs, rewards, and info instead of tuples.
-        multidiscrete_actions (bool): Whether to use multidiscrete_actions action spaces when continuous_actions=False.
-            Otherwise, (default) the action space will be Discrete, and it will be the cartesian product of the
-            action spaces of an agent.
-        clamp_actions: Weather to clamp input actions to the range instead of throwing
-            an error when continuous_actions is True and actions are out of bounds
-        grad_enabled: (bool): Whether the simulator will keep track of gradients in the output. Default is ``False``.
-        **kwargs ():
+        scenario (Union[str, BaseScenario]): Scenario to load.
+            Can be the name of a file in `vmas.scenarios` folder or a :class:`~vmas.simulator.scenario.BaseScenario` class,
+        num_envs (int): Number of vectorized simulation environments. VMAS performs vectorized simulations using PyTorch.
+            This argument indicates the number of vectorized environments that should be simulated in a batch. It will also
+            determine the batch size of the environment.
+        device (Union[str, int, torch.device], optional): Device for simulation. All the tensors created by VMAS
+            will be placed on this device. Default is ``"cpu"``,
+        continuous_actions (bool, optional): Whether to use continuous actions. If ``False``, actions
+            will be discrete. The number of actions and their size will depend on the chosen scenario. Default is ``True``,
+        wrapper (:class:`~vmas.simulator.environment.Wrapper`, optional): Wrapper class to use. For example can be Wrapper.RLLIB.
+            Default is ``None``,
+        max_steps (int, optional): Horizon of the task. Defaults to ``None`` (infinite horizon). Each VMAS scenario can
+            be terminating or not. If ``max_steps`` is specified,
+            the scenario is also terminated whenever this horizon is reached,
+        seed (int, optional): Seed for the environment. Defaults to ``None``,
+        dict_spaces (bool, optional):  Weather to use dictionaries spaces with format ``{"agent_name": tensor, ...}``
+            for obs, rewards, and info instead of tuples. Defaults to ``False``: obs, rewards, info are tuples with length number of agents,
+        multidiscrete_actions (bool, optional): Whether to use multidiscrete action spaces when ``continuous_actions=False``.
+            Default is ``False``: the action space will be ``Discrete``, and it will be the cartesian product of the
+            discrete action spaces available to an agent,
+        clamp_actions (bool, optional): Weather to clamp input actions to their range instead of throwing
+            an error when ``continuous_actions==True`` and actions are out of bounds,
+        grad_enabled (bool, optional): If ``True`` the simulator will not call ``detach()`` on input actions and gradients can
+            be taken from the simulator output. Default is ``False``.
+        **kwargs (dict, optional): Keyword arguments to pass to the :class:`~vmas.simulator.scenario.BaseScenario` class.
+
+    Examples:
+        >>> from vmas import make_env
+        >>> env = make_env(
+        ...     "waterfall",
+        ...     num_envs=3,
+        ...     num_agents=2,
+        ... )
+        >>> print(env.reset())
 
-    Returns:
 
     """
 
     # load scenario from script
     if isinstance(scenario, str):
         if not scenario.endswith(".py"):
             scenario += ".py"
```

### Comparing `vmas-1.4.0/vmas/scenarios/__init__.py` & `vmas-1.4.1/vmas/scenarios/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-#  Copyright (c) 2022.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 import importlib
 import os
 import os.path as osp
 from pathlib import Path
 
 
 def load(name: str):
     pathname = None
-    for dirpath, dirnames, filenames in os.walk(osp.dirname(__file__)):
+    for dirpath, _, filenames in os.walk(osp.dirname(__file__)):
         if pathname is None:
             for filename in filenames:
                 if name == filename or name == str(Path(dirpath) / Path(filename)):
                     pathname = os.path.join(dirpath, filename)
                     break
     assert pathname is not None, f"{name} scenario not found."
```

### Comparing `vmas-1.4.0/vmas/scenarios/balance.py` & `vmas-1.4.1/vmas/scenarios/balance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 import torch
 
 from vmas import render_interactively
-from vmas.simulator.core import Agent, Landmark, Sphere, World, Line, Box
+from vmas.simulator.core import Agent, Box, Landmark, Line, Sphere, World
 from vmas.simulator.heuristic_policy import BaseHeuristicPolicy
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color, Y
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
@@ -26,15 +26,17 @@
         self.fall_reward = -10
 
         # Make world
         world = World(batch_dim, device, gravity=(0.0, -0.05), y_semidim=1)
         # Add agents
         for i in range(self.n_agents):
             agent = Agent(
-                name=f"agent_{i}", shape=Sphere(self.agent_radius), u_multiplier=0.7
+                name=f"agent_{i}",
+                shape=Sphere(self.agent_radius),
+                u_multiplier=0.7,
             )
             world.add_agent(agent)
 
         goal = Landmark(
             name="goal",
             collide=False,
             shape=Sphere(),
@@ -121,20 +123,24 @@
         package_rel_pos = torch.cat(
             [
                 torch.zeros(
                     (1, 1) if env_index is not None else (self.world.batch_dim, 1),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
-                    -self.line_length / 2 + self.package.shape.radius
-                    if self.random_package_pos_on_line
-                    else 0.0,
-                    self.line_length / 2 - self.package.shape.radius
-                    if self.random_package_pos_on_line
-                    else 0.0,
+                    (
+                        -self.line_length / 2 + self.package.shape.radius
+                        if self.random_package_pos_on_line
+                        else 0.0
+                    ),
+                    (
+                        self.line_length / 2 - self.package.shape.radius
+                        if self.random_package_pos_on_line
+                        else 0.0
+                    ),
                 ),
                 torch.full(
                     (1, 1) if env_index is not None else (self.world.batch_dim, 1),
                     self.package.shape.radius,
                     device=self.world.device,
                     dtype=torch.float32,
                 ),
```

### Comparing `vmas-1.4.0/vmas/scenarios/ball_passage.py` & `vmas-1.4.1/vmas/scenarios/ball_passage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 from typing import Dict
 
 import torch
 from torch import Tensor
 
 from vmas import render_interactively
-from vmas.simulator.core import Agent, Box, Landmark, Sphere, World, Line
+from vmas.simulator.core import Agent, Box, Landmark, Line, Sphere, World
 from vmas.simulator.scenario import BaseScenario
-from vmas.simulator.utils import Color, Y, X
+from vmas.simulator.utils import Color, X, Y
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         self.n_passages = kwargs.get("n_passages", 1)
         self.fixed_passage = kwargs.get("fixed_passage", False)
         self.random_start_angle = kwargs.get("random_start_angle", True)
@@ -209,15 +209,17 @@
             )
 
     def reward(self, agent: Agent):
         is_first = agent == self.world.agents[0]
 
         if is_first:
             self.rew = torch.zeros(
-                self.world.batch_dim, device=self.world.device, dtype=torch.float32
+                self.world.batch_dim,
+                device=self.world.device,
+                dtype=torch.float32,
             )
             self.pos_rew[:] = 0
             self.collision_rew[:] = 0
 
             ball_passed = self.ball.state.pos[:, Y] > 0
 
             # Pos shaping
@@ -250,15 +252,15 @@
                 for passage in self.passages:
                     if passage.collide:
                         self.collision_rew[
                             self.world.is_overlapping(a, passage)
                         ] += self.collision_reward
 
             # Ball collisions
-            for i, p in enumerate(self.passages):
+            for p in self.passages:
                 if p.collide:
                     self.collision_rew[
                         self.world.is_overlapping(p, self.ball)
                     ] += self.collision_reward
 
             self.rew = self.pos_rew + self.collision_rew
 
@@ -369,27 +371,31 @@
         # Perimeter
         for i in range(4):
             geom = Line(length=2 + self.agent_radius * 2).get_geometry()
             xform = rendering.Transform()
             geom.add_attr(xform)
 
             xform.set_translation(
-                0.0
-                if i % 2
-                else (
-                    self.world.x_semidim + self.agent_radius
-                    if i == 0
-                    else -self.world.x_semidim - self.agent_radius
+                (
+                    0.0
+                    if i % 2
+                    else (
+                        self.world.x_semidim + self.agent_radius
+                        if i == 0
+                        else -self.world.x_semidim - self.agent_radius
+                    )
                 ),
-                0.0
-                if not i % 2
-                else (
-                    self.world.x_semidim + self.agent_radius
-                    if i == 1
-                    else -self.world.x_semidim - self.agent_radius
+                (
+                    0.0
+                    if not i % 2
+                    else (
+                        self.world.x_semidim + self.agent_radius
+                        if i == 1
+                        else -self.world.x_semidim - self.agent_radius
+                    )
                 ),
             )
             xform.set_rotation(torch.pi / 2 if not i % 2 else 0.0)
             color = Color.BLACK.value
             if isinstance(color, torch.Tensor) and len(color.shape) > 1:
                 color = color[env_index]
             geom.set_color(*color)
```

### Comparing `vmas-1.4.0/vmas/scenarios/ball_trajectory.py` & `vmas-1.4.1/vmas/scenarios/ball_trajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 from typing import Dict
 
 import torch
 from torch import Tensor
 
 from vmas import render_interactively
 from vmas.simulator.core import Agent, Landmark, Sphere, World
 from vmas.simulator.joints import Joint
 from vmas.simulator.scenario import BaseScenario
-from vmas.simulator.utils import X, Color, JOINT_FORCE
+from vmas.simulator.utils import Color, JOINT_FORCE, X
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         self.pos_shaping_factor = kwargs.get("pos_shaping_factor", 0)
         self.speed_shaping_factor = kwargs.get("speed_shaping_factor", 1)
         self.dist_shaping_factor = kwargs.get("dist_shaping_factor", 0)
@@ -76,17 +76,19 @@
         self.speed_rew = self.pos_rew.clone()
         self.dist_rew = self.pos_rew.clone()
 
         return world
 
     def reset_world_at(self, env_index: int = None):
         ball_pos = torch.zeros(
-            (1, self.world.dim_p)
-            if env_index is not None
-            else (self.world.batch_dim, self.world.dim_p),
+            (
+                (1, self.world.dim_p)
+                if env_index is not None
+                else (self.world.batch_dim, self.world.dim_p)
+            ),
             device=self.world.device,
             dtype=torch.float32,
         ).uniform_(
             -self.desired_radius,
             self.desired_radius,
         )
```

### Comparing `vmas-1.4.0/vmas/scenarios/buzz_wire.py` & `vmas-1.4.1/vmas/scenarios/buzz_wire.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 from typing import Dict
 
 import torch
 from torch import Tensor
 
 from vmas import render_interactively
-from vmas.simulator.core import Agent, Landmark, Sphere, World, Line
+from vmas.simulator.core import Agent, Landmark, Line, Sphere, World
 from vmas.simulator.joints import Joint
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
@@ -177,15 +177,16 @@
                 + (
                     (torch.cat([start_delta_x, start_delta_y], dim=1) / 2)
                     * (-1 if i == 0 else 1)
                 ),
                 batch_index=env_index,
             )
             joint.landmark.set_rot(
-                start_angle + (torch.pi if i == 1 else 0), batch_index=env_index
+                start_angle + (torch.pi if i == 1 else 0),
+                batch_index=env_index,
             )
 
         self.spawn_path_line(env_index)
         if env_index is None:
             self.pos_shaping = (
                 torch.linalg.vector_norm(
                     self.ball.state.pos - self.goal.state.pos, dim=1
@@ -203,15 +204,17 @@
             self.collided[env_index] = False
 
     def reward(self, agent: Agent):
         is_first = agent == self.world.agents[0]
 
         if is_first:
             self.rew = torch.zeros(
-                self.world.batch_dim, device=self.world.device, dtype=torch.float32
+                self.world.batch_dim,
+                device=self.world.device,
+                dtype=torch.float32,
             )
             self.pos_rew[:] = 0
             self.collision_rew[:] = 0
             self.collided[:] = False
 
             dist_to_goal = torch.linalg.vector_norm(
                 self.ball.state.pos - self.goal.state.pos,
@@ -230,15 +233,19 @@
 
             self.rew = self.pos_rew + self.collision_rew
 
         return self.rew
 
     def observation(self, agent: Agent):
         return torch.cat(
-            [agent.state.pos, agent.state.vel, agent.state.pos - self.goal.state.pos],
+            [
+                agent.state.pos,
+                agent.state.vel,
+                agent.state.pos - self.goal.state.pos,
+            ],
             dim=-1,
         )
 
     def done(self):
         return (
             torch.linalg.vector_norm(self.ball.state.pos - self.goal.state.pos, dim=1)
             <= 0.01
```

### Comparing `vmas-1.4.0/vmas/scenarios/debug/asym_joint.py` & `vmas-1.4.1/vmas/scenarios/debug/asym_joint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 import math
 import typing
 from typing import Dict, List
 
 import torch
@@ -31,15 +31,16 @@
 
 def get_line_angle_dist_0_180(angle, goal):
     angle = get_line_angle_0_180(angle)
     goal = get_line_angle_0_180(goal)
     return torch.minimum(
         (angle - goal).abs(),
         torch.minimum(
-            (angle - (goal - torch.pi)).abs(), ((angle - torch.pi) - goal).abs()
+            (angle - (goal - torch.pi)).abs(),
+            ((angle - torch.pi) - goal).abs(),
         ),
     ).squeeze(-1)
 
 
 def angle_to_vector(angle):
     return torch.cat([torch.cos(angle), torch.sin(angle)], dim=1)
 
@@ -252,32 +253,31 @@
         return self.rew
 
     def observation(self, agent: Agent):
         if self.observe_joint_angle:
             joint_angle = self.joint.landmark.state.rot
             angle_noise = (
                 torch.randn(
-                    *joint_angle.shape, device=self.world.device, dtype=torch.float32
+                    *joint_angle.shape,
+                    device=self.world.device,
+                    dtype=torch.float32,
                 )
                 * self.joint_angle_obs_noise
                 if self.joint_angle_obs_noise
                 else 0.0
             )
             joint_angle += angle_noise
 
         observations = [
             agent.state.pos,
             agent.state.vel,
         ] + ([angle_to_vector(joint_angle)] if self.observe_joint_angle else [])
 
         for i, obs in enumerate(observations):
-            noise = torch.zeros(
-                *obs.shape,
-                device=self.world.device,
-            ).uniform_(
+            noise = torch.zeros(*obs.shape, device=self.world.device,).uniform_(
                 -self.obs_noise,
                 self.obs_noise,
             )
             observations[i] = obs.clone() + noise
         return torch.cat(
             observations,
             dim=-1,
```

### Comparing `vmas-1.4.0/vmas/scenarios/debug/circle_trajectory.py` & `vmas-1.4.1/vmas/scenarios/debug/circle_trajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 from typing import Dict
 
 import torch
 from torch import Tensor
+
 from vmas import render_interactively
+from vmas.simulator.controllers.velocity_controller import VelocityController
 from vmas.simulator.core import Agent, Sphere, World
 from vmas.simulator.scenario import BaseScenario
-from vmas.simulator.utils import Color, X, Y, TorchUtils
-from vmas.simulator.controllers.velocity_controller import VelocityController
+from vmas.simulator.utils import Color, TorchUtils, X, Y
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         self.u_range = kwargs.get("u_range", 1)
         self.a_range = kwargs.get("a_range", 1)
         self.obs_noise = kwargs.get("obs_noise", 0.0)
@@ -24,15 +25,19 @@
         self.agent_radius = 0.16
         self.desired_radius = 1.5
 
         self.viewer_zoom = 2
 
         # Make world
         world = World(
-            batch_dim, device, linear_friction=self.linear_friction, dt=0.05, drag=0
+            batch_dim,
+            device,
+            linear_friction=self.linear_friction,
+            dt=0.05,
+            drag=0,
         )
 
         controller_params = [2, 6, 0.002]
 
         self.f_range = self.a_range + self.linear_friction
 
         null_action = torch.zeros(world.batch_dim, world.dim_p, device=world.device)
@@ -72,17 +77,19 @@
         agent.vel_action = agent.action.u.clone()
         agent.controller.process_force()
 
     def reset_world_at(self, env_index: int = None):
         self.agent.controller.reset(env_index)
         self.agent.set_pos(
             torch.zeros(
-                (1, self.world.dim_p)
-                if env_index is not None
-                else (self.world.batch_dim, self.world.dim_p),
+                (
+                    (1, self.world.dim_p)
+                    if env_index is not None
+                    else (self.world.batch_dim, self.world.dim_p)
+                ),
                 device=self.world.device,
                 dtype=torch.float32,
             ).uniform_(
                 -self.desired_radius,
                 self.desired_radius,
             ),
             batch_index=env_index,
@@ -146,18 +153,15 @@
         ).unsqueeze(-1)
         angle = torch.nan_to_num(angle)
         return angle
 
     def observation(self, agent: Agent):
         observations = [agent.state.pos, agent.state.vel, agent.state.pos]
         for i, obs in enumerate(observations):
-            noise = torch.zeros(
-                *obs.shape,
-                device=self.world.device,
-            ).uniform_(
+            noise = torch.zeros(*obs.shape, device=self.world.device,).uniform_(
                 -self.obs_noise,
                 self.obs_noise,
             )
             observations[i] = obs + noise
         return torch.cat(
             observations,
             dim=-1,
```

### Comparing `vmas-1.4.0/vmas/scenarios/debug/diff_drive.py` & `vmas-1.4.1/vmas/scenarios/debug/diff_drive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 import typing
 from typing import List
 
 import torch
+
 from vmas import render_interactively
 from vmas.simulator.core import Agent, World
 from vmas.simulator.dynamics.diff_drive import DiffDrive
 from vmas.simulator.dynamics.holonomic_with_rot import HolonomicWithRotation
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color, ScenarioUtils
```

### Comparing `vmas-1.4.0/vmas/scenarios/debug/goal.py` & `vmas-1.4.1/vmas/scenarios/debug/goal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 import math
 from typing import Dict
 
 import torch
 from torch import Tensor
 
 from vmas import render_interactively
-from vmas.simulator.core import Agent, World, Landmark, Sphere
+from vmas.simulator.controllers.velocity_controller import VelocityController
+from vmas.simulator.core import Agent, Landmark, Sphere, World
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color, TorchUtils
-from vmas.simulator.controllers.velocity_controller import VelocityController
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         self.u_range = kwargs.get("u_range", 1)
         self.a_range = kwargs.get("a_range", 1)
         self.obs_noise = kwargs.get("obs_noise", 0.0)
@@ -88,27 +88,31 @@
     def reset_world_at(self, env_index: int = None):
         for agent in self.world.agents:
             agent.controller.reset(env_index)
             agent.set_pos(
                 torch.cat(
                     [
                         torch.zeros(
-                            (1, 1)
-                            if env_index is not None
-                            else (self.world.batch_dim, 1),
+                            (
+                                (1, 1)
+                                if env_index is not None
+                                else (self.world.batch_dim, 1)
+                            ),
                             device=self.world.device,
                             dtype=torch.float32,
                         ).uniform_(
                             -self.lab_length / 2,
                             self.lab_length / 2,
                         ),
                         torch.zeros(
-                            (1, 1)
-                            if env_index is not None
-                            else (self.world.batch_dim, 1),
+                            (
+                                (1, 1)
+                                if env_index is not None
+                                else (self.world.batch_dim, 1)
+                            ),
                             device=self.world.device,
                             dtype=torch.float32,
                         ).uniform_(
                             -self.lab_width / 2,
                             self.lab_width / 2,
                         ),
                     ],
@@ -119,27 +123,31 @@
 
         for landmark in self.world.landmarks:
             # Random pos between -1 and 1
             landmark.set_pos(
                 torch.cat(
                     [
                         torch.zeros(
-                            (1, 1)
-                            if env_index is not None
-                            else (self.world.batch_dim, 1),
+                            (
+                                (1, 1)
+                                if env_index is not None
+                                else (self.world.batch_dim, 1)
+                            ),
                             device=self.world.device,
                             dtype=torch.float32,
                         ).uniform_(
                             -self.lab_length / 2,
                             self.lab_length / 2,
                         ),
                         torch.zeros(
-                            (1, 1)
-                            if env_index is not None
-                            else (self.world.batch_dim, 1),
+                            (
+                                (1, 1)
+                                if env_index is not None
+                                else (self.world.batch_dim, 1)
+                            ),
                             device=self.world.device,
                             dtype=torch.float32,
                         ).uniform_(
                             -self.lab_width / 2,
                             self.lab_width / 2,
                         ),
                     ],
@@ -232,18 +240,15 @@
             agent.state.pos,
             agent.state.vel,
             agent.state.pos - self.goal.state.pos,
         ]
 
         if self.obs_noise > 0:
             for i, obs in enumerate(observations):
-                noise = torch.zeros(
-                    *obs.shape,
-                    device=self.world.device,
-                ).uniform_(
+                noise = torch.zeros(*obs.shape, device=self.world.device,).uniform_(
                     -self.obs_noise,
                     self.obs_noise,
                 )
                 observations[i] = obs + noise
         return torch.cat(
             observations,
             dim=-1,
```

### Comparing `vmas-1.4.0/vmas/scenarios/debug/het_mass.py` & `vmas-1.4.1/vmas/scenarios/debug/het_mass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 import math
 from typing import Dict
 
 import numpy as np
 import torch
@@ -51,17 +51,19 @@
         self.green_agent.mass = self.green_mass + np.random.uniform(
             -self.mass_noise, self.mass_noise
         )
 
         for agent in self.world.agents:
             agent.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(-1, 1),
                 batch_index=env_index,
             )
 
     def process_action(self, agent: Agent):
```

### Comparing `vmas-1.4.0/vmas/scenarios/debug/kinematic_bicycle.py` & `vmas-1.4.1/vmas/scenarios/debug/kinematic_bicycle.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import typing
 from typing import List
 
 import torch
 
 from vmas import render_interactively
-from vmas.simulator.core import Agent, World, Box
+from vmas.simulator.core import Agent, Box, World
 from vmas.simulator.dynamics.holonomic_with_rot import HolonomicWithRotation
 from vmas.simulator.dynamics.kinematic_bicycle import KinematicBicycle
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color, ScenarioUtils
 
 if typing.TYPE_CHECKING:
     from vmas.simulator.rendering import Geom
```

### Comparing `vmas-1.4.0/vmas/scenarios/debug/line_trajectory.py` & `vmas-1.4.1/vmas/scenarios/debug/line_trajectory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 from typing import Dict
 
 import torch
 from torch import Tensor
 
 from vmas import render_interactively
+from vmas.simulator.controllers.velocity_controller import VelocityController
 from vmas.simulator.core import Agent, Sphere, World
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color, X, Y
-from vmas.simulator.controllers.velocity_controller import VelocityController
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         self.obs_noise = kwargs.get("obs_noise", 0)
 
         self.agent_radius = 0.03
@@ -100,18 +100,15 @@
         )
 
         return self.pos_rew + self.dot_product + self.steady_rew
 
     def observation(self, agent: Agent):
         observations = [agent.state.pos, agent.state.vel, agent.state.pos]
         for i, obs in enumerate(observations):
-            noise = torch.zeros(
-                *obs.shape,
-                device=self.world.device,
-            ).uniform_(
+            noise = torch.zeros(*obs.shape, device=self.world.device,).uniform_(
                 -self.obs_noise,
                 self.obs_noise,
             )
             observations[i] = obs + noise
         return torch.cat(
             observations,
             dim=-1,
```

### Comparing `vmas-1.4.0/vmas/scenarios/debug/pollock.py` & `vmas-1.4.1/vmas/scenarios/debug/pollock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 import torch
 
 from vmas import render_interactively
-from vmas.simulator.core import Agent, World, Sphere, Landmark, Line, Box
+from vmas.simulator.core import Agent, Box, Landmark, Line, Sphere, World
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color, ScenarioUtils
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         self.n_agents = kwargs.get("n_agents", 15)
```

### Comparing `vmas-1.4.0/vmas/scenarios/debug/vel_control.py` & `vmas-1.4.1/vmas/scenarios/debug/vel_control.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 from typing import Dict
 
 import torch
 from torch import Tensor
 
 from vmas import render_interactively
-from vmas.simulator.core import Agent, World, Landmark
-from vmas.simulator.scenario import BaseScenario
-from vmas.simulator.utils import Color, X, TorchUtils
 from vmas.simulator.controllers.velocity_controller import VelocityController
+from vmas.simulator.core import Agent, Landmark, World
+from vmas.simulator.scenario import BaseScenario
+from vmas.simulator.utils import Color, TorchUtils, X
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         self.green_mass = kwargs.get("green_mass", 1)
         self.plot_grid = True
 
@@ -91,44 +91,44 @@
     def reset_world_at(self, env_index: int = None):
         for agent in self.world.agents:
             agent.controller.reset(env_index)
             agent.set_pos(
                 torch.cat(
                     [
                         torch.zeros(
-                            (1, 1)
-                            if env_index is not None
-                            else (self.world.batch_dim, 1),
+                            (
+                                (1, 1)
+                                if env_index is not None
+                                else (self.world.batch_dim, 1)
+                            ),
                             device=self.world.device,
                             dtype=torch.float32,
                         ).uniform_(
                             -1,
                             -1,
                         ),
                         torch.zeros(
-                            (1, 1)
-                            if env_index is not None
-                            else (self.world.batch_dim, 1),
+                            (
+                                (1, 1)
+                                if env_index is not None
+                                else (self.world.batch_dim, 1)
+                            ),
                             device=self.world.device,
                             dtype=torch.float32,
                         ).uniform_(
                             0,
                             0,
                         ),
                     ],
                     dim=1,
                 ),
                 batch_index=env_index,
             )
 
     def process_action(self, agent: Agent):
-        # Use queue for delay
-        self.input_queue.append(agent.action.u.clone())
-        agent.action.u = self.input_queue.pop(0)
-
         # Clamp square to circle
         agent.action.u = TorchUtils.clamp_with_norm(agent.action.u, agent.u_range)
 
         # Zero small input
         action_norm = torch.linalg.vector_norm(agent.action.u, dim=1)
         agent.action.u[action_norm < 0.08] = 0
```

### Comparing `vmas-1.4.0/vmas/scenarios/debug/waterfall.py` & `vmas-1.4.1/vmas/scenarios/debug/waterfall.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 import torch
 
 from vmas import render_interactively
-from vmas.simulator.core import Agent, World, Sphere, Landmark, Box, Line
+from vmas.simulator.core import Agent, Box, Landmark, Line, Sphere, World
 from vmas.simulator.joints import Joint
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
@@ -17,15 +17,20 @@
         self.with_joints = kwargs.get("joints", True)
 
         self.agent_dist = 0.1
         self.agent_radius = 0.04
 
         # Make world
         world = World(
-            batch_dim, device, dt=0.1, drag=0.25, substeps=5, collision_force=500
+            batch_dim,
+            device,
+            dt=0.1,
+            drag=0.25,
+            substeps=5,
+            collision_force=500,
         )
         # Add agents
         for i in range(self.n_agents):
             agent = Agent(
                 name=f"agent_{i}",
                 shape=Sphere(radius=self.agent_radius),
                 u_multiplier=0.7,
@@ -98,15 +103,18 @@
 
     def reset_world_at(self, env_index: int = None):
         for i, agent in enumerate(
             self.world.agents + [self.world.landmarks[self.n_agents - 1]]
         ):
             agent.set_pos(
                 torch.tensor(
-                    [-0.2 + (self.agent_dist + 2 * self.agent_radius) * i, 1.0],
+                    [
+                        -0.2 + (self.agent_dist + 2 * self.agent_radius) * i,
+                        1.0,
+                    ],
                     dtype=torch.float32,
                     device=self.world.device,
                 ),
                 batch_index=env_index,
             )
         for i, landmark in enumerate(
             self.world.landmarks[(self.n_agents + 1) if self.with_joints else 0 : -1]
```

### Comparing `vmas-1.4.0/vmas/scenarios/discovery.py` & `vmas-1.4.1/vmas/scenarios/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 import typing
-from typing import Dict, Callable, List
+from typing import Callable, Dict, List
 
 import torch
 from torch import Tensor
 
 from vmas import render_interactively
-from vmas.simulator.core import Agent, Landmark, Sphere, World, Entity
+from vmas.simulator.core import Agent, Entity, Landmark, Sphere, World
 from vmas.simulator.heuristic_policy import BaseHeuristicPolicy
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.sensors import Lidar
-from vmas.simulator.utils import Color, X, Y, ScenarioUtils
+from vmas.simulator.utils import Color, ScenarioUtils, X, Y
 
 if typing.TYPE_CHECKING:
     from vmas.simulator.rendering import Geom
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
@@ -50,17 +50,17 @@
             y_semidim=1,
             collision_force=500,
             substeps=2,
             drag=0.25,
         )
 
         # Add agents
-        entity_filter_agents: Callable[[Entity], bool] = lambda e: e.name.startswith(
-            "agent"
-        )
+        # entity_filter_agents: Callable[[Entity], bool] = lambda e: e.name.startswith(
+        #     "agent"
+        # )
         entity_filter_targets: Callable[[Entity], bool] = lambda e: e.name.startswith(
             "target"
         )
         for i in range(self.n_agents):
             # Constraint: all agents have same action range and multiplier
             agent = Agent(
                 name=f"agent_{i}",
@@ -106,15 +106,17 @@
 
         return world
 
     def reset_world_at(self, env_index: int = None):
         placable_entities = self._targets[: self.n_targets] + self.world.agents
         if env_index is None:
             self.all_time_covered_targets = torch.full(
-                (self.world.batch_dim, self.n_targets), False, device=self.world.device
+                (self.world.batch_dim, self.n_targets),
+                False,
+                device=self.world.device,
             )
         else:
             self.all_time_covered_targets[env_index] = False
         ScenarioUtils.spawn_entities_randomly(
             entities=placable_entities,
             world=self.world,
             env_index=env_index,
@@ -127,15 +129,17 @@
 
     def reward(self, agent: Agent):
         is_first = agent == self.world.agents[0]
         is_last = agent == self.world.agents[-1]
 
         if is_first:
             self.time_rew = torch.full(
-                (self.world.batch_dim,), self.time_penalty, device=self.world.device
+                (self.world.batch_dim,),
+                self.time_penalty,
+                device=self.world.device,
             )
             self.agents_pos = torch.stack(
                 [a.state.pos for a in self.world.agents], dim=1
             )
             self.targets_pos = torch.stack([t.state.pos for t in self._targets], dim=1)
             self.agents_targets_dists = torch.cdist(self.agents_pos, self.targets_pos)
             self.agents_per_target = torch.sum(
@@ -163,15 +167,16 @@
                 for i, target in enumerate(self._targets):
                     occupied_positions_targets = [
                         o.state.pos.unsqueeze(1)
                         for o in self._targets
                         if o is not target
                     ]
                     occupied_positions = torch.cat(
-                        occupied_positions_agents + occupied_positions_targets, dim=1
+                        occupied_positions_agents + occupied_positions_targets,
+                        dim=1,
                     )
                     pos = ScenarioUtils.find_random_pos_for_entity(
                         occupied_positions,
                         env_index=None,
                         world=self.world,
                         min_dist_between_entities=self._min_dist_between_entities,
                         x_bounds=(-self.world.x_semidim, self.world.x_semidim),
@@ -193,17 +198,19 @@
             else self.shared_covering_rew
         )
 
         return agent.collision_rew + covering_rew + self.time_rew
 
     def get_outside_pos(self, env_index):
         return torch.empty(
-            (1, self.world.dim_p)
-            if env_index is not None
-            else (self.world.batch_dim, self.world.dim_p),
+            (
+                (1, self.world.dim_p)
+                if env_index is not None
+                else (self.world.batch_dim, self.world.dim_p)
+            ),
             device=self.world.device,
         ).uniform_(-1000 * self.world.x_semidim, -10 * self.world.x_semidim)
 
     def agent_reward(self, agent):
         agent_index = self.world.agents.index(agent)
 
         agent.covering_reward[:] = 0
@@ -230,31 +237,33 @@
                 # lidar_2_measures,
             ],
             dim=-1,
         )
 
     def info(self, agent: Agent) -> Dict[str, Tensor]:
         info = {
-            "covering_reward": agent.covering_reward
-            if not self.shared_reward
-            else self.shared_covering_rew,
+            "covering_reward": (
+                agent.covering_reward
+                if not self.shared_reward
+                else self.shared_covering_rew
+            ),
             "collision_rew": agent.collision_rew,
             "targets_covered": self.covered_targets.sum(-1),
         }
         return info
 
     def done(self):
         return self.all_time_covered_targets.all(dim=-1)
 
     def extra_render(self, env_index: int = 0) -> "List[Geom]":
         from vmas.simulator import rendering
 
         geoms: List[Geom] = []
         # Target ranges
-        for i, target in enumerate(self._targets):
+        for target in self._targets:
             range_circle = rendering.make_circle(self._covering_range, filled=False)
             xform = rendering.Transform()
             xform.set_translation(*target.state.pos[env_index])
             range_circle.add_attr(xform)
             range_circle.set_color(*self.target_color.value)
             geoms.append(range_circle)
         # Communication lines
```

### Comparing `vmas-1.4.0/vmas/scenarios/dispersion.py` & `vmas-1.4.1/vmas/scenarios/dispersion.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,18 @@
         self.penalise_by_time = kwargs.get("penalise_by_time", False)
         self.food_radius = kwargs.get("food_radius", 0.05)
         self.pos_range = kwargs.get("pos_range", 1.0)
         n_food = kwargs.get("n_food", n_agents)
 
         # Make world
         world = World(
-            batch_dim, device, x_semidim=self.pos_range, y_semidim=self.pos_range
+            batch_dim,
+            device,
+            x_semidim=self.pos_range,
+            y_semidim=self.pos_range,
         )
         # Add agents
         for i in range(n_agents):
             # Constraint: all agents have same action range and multiplier
             agent = Agent(
                 name=f"agent_{i}",
                 collide=False,
@@ -44,24 +47,28 @@
 
         return world
 
     def reset_world_at(self, env_index: int = None):
         for agent in self.world.agents:
             agent.set_pos(
                 torch.zeros(
-                    self.world.dim_p, device=self.world.device, dtype=torch.float32
+                    self.world.dim_p,
+                    device=self.world.device,
+                    dtype=torch.float32,
                 ),
                 batch_index=env_index,
             )
         for landmark in self.world.landmarks:
             landmark.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -self.pos_range,
                     self.pos_range,
                 ),
                 batch_index=env_index,
```

### Comparing `vmas-1.4.0/vmas/scenarios/dropout.py` & `vmas-1.4.1/vmas/scenarios/dropout.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 import math
 from typing import Dict
 
 import torch
 from torch import Tensor
+
 from vmas import render_interactively
 from vmas.simulator.core import Agent, Landmark, Sphere, World
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color, ScenarioUtils
 
 DEFAULT_ENERGY_COEFF = 0.02
 
@@ -26,15 +27,17 @@
 
         # Make world
         world = World(batch_dim, device)
         # Add agents
         for i in range(n_agents):
             # Constraint: all agents have same action range and multiplier
             agent = Agent(
-                name=f"agent_{i}", collide=False, shape=Sphere(radius=self.agent_radius)
+                name=f"agent_{i}",
+                collide=False,
+                shape=Sphere(radius=self.agent_radius),
             )
             world.add_agent(agent)
         # Add landmarks
         goal = Landmark(
             name="goal",
             collide=False,
             shape=Sphere(radius=self.goal_radius),
@@ -101,15 +104,16 @@
         is_last = agent == self.world.agents[-1]
 
         if is_first:
             self.any_eaten = self._done = torch.any(
                 torch.stack(
                     [
                         torch.linalg.vector_norm(
-                            a.state.pos - self.world.landmarks[0].state.pos, dim=1
+                            a.state.pos - self.world.landmarks[0].state.pos,
+                            dim=1,
                         )
                         < a.shape.radius + self.world.landmarks[0].shape.radius
                         for a in self.world.agents
                     ],
                     dim=1,
                 ),
                 dim=-1,
@@ -154,9 +158,12 @@
 
     def done(self):
         return self._done
 
 
 if __name__ == "__main__":
     render_interactively(
-        __file__, control_two_agents=True, n_agents=4, energy_coeff=DEFAULT_ENERGY_COEFF
+        __file__,
+        control_two_agents=True,
+        n_agents=4,
+        energy_coeff=DEFAULT_ENERGY_COEFF,
     )
```

### Comparing `vmas-1.4.0/vmas/scenarios/flocking.py` & `vmas-1.4.1/vmas/scenarios/flocking.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 from typing import Callable, Dict
 
 import torch
 from torch import Tensor
+
 from vmas import render_interactively
-from vmas.simulator.core import Agent, Landmark, Sphere, World, Entity
+from vmas.simulator.core import Agent, Entity, Landmark, Sphere, World
 from vmas.simulator.heuristic_policy import BaseHeuristicPolicy
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.sensors import Lidar
-from vmas.simulator.utils import Color, X, Y, ScenarioUtils
+from vmas.simulator.utils import Color, ScenarioUtils, X, Y
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         n_agents = kwargs.get("n_agents", 4)
         n_obstacles = kwargs.get("n_obstacles", 5)
         self._min_dist_between_entities = kwargs.get("min_dist_between_entities", 0.15)
@@ -81,17 +82,19 @@
             t = self.t / 30
             agent.action.u = torch.stack([torch.cos(t), torch.sin(t)], dim=1)
 
         return action_script
 
     def reset_world_at(self, env_index: int = None):
         target_pos = torch.zeros(
-            (1, self.world.dim_p)
-            if env_index is not None
-            else (self.world.batch_dim, self.world.dim_p),
+            (
+                (1, self.world.dim_p)
+                if env_index is not None
+                else (self.world.batch_dim, self.world.dim_p)
+            ),
             device=self.world.device,
             dtype=torch.float32,
         )
 
         target_pos[:, Y] = -self.y_dim
         self._target.set_pos(target_pos, batch_index=env_index)
         ScenarioUtils.spawn_entities_randomly(
```

### Comparing `vmas-1.4.0/vmas/scenarios/football.py` & `vmas-1.4.1/vmas/scenarios/football.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 import math
 import operator
 from functools import reduce
 
 import torch
 
 from vmas import render_interactively
-from vmas.simulator.core import Agent, World, Landmark, Sphere, Box, Line
+from vmas.simulator.core import Agent, Box, Landmark, Line, Sphere, World
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color, X, Y
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         self.init_params(**kwargs)
@@ -111,42 +111,48 @@
         world.red_agents = red_agents
         world.blue_agents = blue_agents
 
     def reset_agents(self, env_index: int = None):
         for agent in self.blue_agents:
             agent.set_pos(
                 torch.rand(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                 )
                 * torch.tensor(
-                    [self.pitch_length / 2, self.pitch_width], device=self.world.device
+                    [self.pitch_length / 2, self.pitch_width],
+                    device=self.world.device,
                 )
                 + torch.tensor(
                     [-self.pitch_length / 2, -self.pitch_width / 2],
                     device=self.world.device,
                 ),
                 batch_index=env_index,
             )
             agent.set_vel(
                 torch.zeros(2, device=self.world.device),
                 batch_index=env_index,
             )
         for agent in self.red_agents:
             agent.set_pos(
                 torch.rand(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                 )
                 * torch.tensor(
-                    [self.pitch_length / 2, self.pitch_width], device=self.world.device
+                    [self.pitch_length / 2, self.pitch_width],
+                    device=self.world.device,
                 )
                 + torch.tensor([0.0, -self.pitch_width / 2], device=self.world.device),
                 batch_index=env_index,
             )
             agent.set_vel(
                 torch.zeros(2, device=self.world.device),
                 batch_index=env_index,
@@ -261,45 +267,51 @@
         world.add_landmark(bottom_line)
 
     def reset_background(self, env_index: int = None):
         for landmark in self.world.landmarks:
             if landmark.name == "Centre Line":
                 landmark.set_rot(
                     torch.tensor(
-                        [torch.pi / 2], dtype=torch.float32, device=self.world.device
+                        [torch.pi / 2],
+                        dtype=torch.float32,
+                        device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
             elif landmark.name == "Right Line":
                 landmark.set_pos(
                     torch.tensor(
                         [self.pitch_length / 2 - self.agent_size, 0.0],
                         dtype=torch.float32,
                         device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
                 landmark.set_rot(
                     torch.tensor(
-                        [torch.pi / 2], dtype=torch.float32, device=self.world.device
+                        [torch.pi / 2],
+                        dtype=torch.float32,
+                        device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
             elif landmark.name == "Left Line":
                 landmark.set_pos(
                     torch.tensor(
                         [-self.pitch_length / 2 + self.agent_size, 0.0],
                         dtype=torch.float32,
                         device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
                 landmark.set_rot(
                     torch.tensor(
-                        [torch.pi / 2], dtype=torch.float32, device=self.world.device
+                        [torch.pi / 2],
+                        dtype=torch.float32,
+                        device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
             elif landmark.name == "Top Line":
                 landmark.set_pos(
                     torch.tensor(
                         [0.0, self.pitch_width / 2 - self.agent_size],
@@ -375,15 +387,17 @@
                         dtype=torch.float32,
                         device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
                 landmark.set_rot(
                     torch.tensor(
-                        [torch.pi / 2], dtype=torch.float32, device=self.world.device
+                        [torch.pi / 2],
+                        dtype=torch.float32,
+                        device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
 
             elif landmark.name == "Left Bottom Wall":
                 landmark.set_pos(
                     torch.tensor(
@@ -394,15 +408,17 @@
                         dtype=torch.float32,
                         device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
                 landmark.set_rot(
                     torch.tensor(
-                        [torch.pi / 2], dtype=torch.float32, device=self.world.device
+                        [torch.pi / 2],
+                        dtype=torch.float32,
+                        device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
 
             elif landmark.name == "Right Top Wall":
                 landmark.set_pos(
                     torch.tensor(
@@ -413,15 +429,17 @@
                         dtype=torch.float32,
                         device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
                 landmark.set_rot(
                     torch.tensor(
-                        [torch.pi / 2], dtype=torch.float32, device=self.world.device
+                        [torch.pi / 2],
+                        dtype=torch.float32,
+                        device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
             elif landmark.name == "Right Bottom Wall":
                 landmark.set_pos(
                     torch.tensor(
                         [
@@ -431,15 +449,17 @@
                         dtype=torch.float32,
                         device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
                 landmark.set_rot(
                     torch.tensor(
-                        [torch.pi / 2], dtype=torch.float32, device=self.world.device
+                        [torch.pi / 2],
+                        dtype=torch.float32,
+                        device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
 
     def init_goals(self, world):
         right_goal_back = Landmark(
             name="Right Goal Back",
@@ -530,15 +550,17 @@
                         dtype=torch.float32,
                         device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
                 landmark.set_rot(
                     torch.tensor(
-                        [torch.pi / 2], dtype=torch.float32, device=self.world.device
+                        [torch.pi / 2],
+                        dtype=torch.float32,
+                        device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
             elif landmark.name == "Right Goal Back":
                 landmark.set_pos(
                     torch.tensor(
                         [
@@ -548,15 +570,17 @@
                         dtype=torch.float32,
                         device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
                 landmark.set_rot(
                     torch.tensor(
-                        [torch.pi / 2], dtype=torch.float32, device=self.world.device
+                        [torch.pi / 2],
+                        dtype=torch.float32,
+                        device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
             elif landmark.name == "Left Goal Top":
                 landmark.set_pos(
                     torch.tensor(
                         [
@@ -711,15 +735,15 @@
 
     def done(self):
         if self.ai_blue_agents and self.ai_red_agents:
             self.reward(None)
         return self._done
 
 
-""" Ball Physics """
+# Ball Physics
 
 
 def ball_action_script(ball, world):
     # Avoid getting stuck against the wall
     dist_thres = world.agent_size * 2
     vel_thres = 0.1
     impulse = 0.01
@@ -777,15 +801,15 @@
     goal_mask = (ball.state.pos[:, 1] < world.goal_size / 2) * (
         ball.state.pos[:, 1] > -world.goal_size / 2
     )
     actions[goal_mask, 0] = 0
     ball.action.u = actions
 
 
-""" Agent Policy """
+# Agent Policy
 
 
 class AgentPolicy:
     def __init__(self, team="Red"):
         self.team_name = team
         self.otherteam_name = "Blue" if (self.team_name == "Red") else "Red"
 
@@ -895,15 +919,15 @@
 
         if len(self.teammates) == 1:
             self.role = {self.teammates[0]: 1.0}
         else:
             roles = torch.linspace(0.5, 1, len(self.teammates), device=world.device)
             self.role = {agent: roles[i] for i, agent in enumerate(self.teammates)}
 
-    def reset(self, env_index=slice(None)):
+    def reset(self, env_index=Ellipsis):
         for agent in self.teammates:
             self.actions[agent]["dribbling"][env_index] = False
             self.actions[agent]["shooting"][env_index] = False
             self.actions[agent]["pre-shooting"][env_index] = False
             self.objectives[agent]["target_pos"][env_index] = torch.zeros(
                 self.world.dim_p, device=self.world.device
             )
@@ -955,57 +979,62 @@
                 move_mask.sum(), self.world.dim_p, device=self.world.device
             ),
             env_index=move_mask,
         )
         # Dribble with the ball
         self.dribble_to_goal(agent, env_index=dribble_mask)
         # If other agent is passing/shooting, stay still
-        other_agent_shooting_mask = self.combine_or(
-            [
-                self.actions[otheragent]["pre-shooting"]
-                | self.actions[otheragent]["shooting"]
-                for otheragent in self.teammates
-                if (otheragent != agent)
-            ]
+        other_agents_shooting = [
+            self.actions[otheragent]["pre-shooting"]
+            | self.actions[otheragent]["shooting"]
+            for otheragent in self.teammates
+            if (otheragent != agent)
+        ]
+        other_agent_shooting_mask = (
+            self.combine_or(other_agents_shooting)
+            if len(other_agents_shooting)
+            else False
         )
         stay_still_mask = other_agent_shooting_mask & ~shooting_mask  # hmm
         self.go_to(
             agent,
             pos=agent.state.pos[stay_still_mask],
             vel=torch.zeros(
-                stay_still_mask.sum(), self.world.dim_p, device=self.world.device
+                stay_still_mask.sum(),
+                self.world.dim_p,
+                device=self.world.device,
             ),
             env_index=stay_still_mask,
         )
 
     def run(self, agent, world):
         self.check_possession()
         self.policy(agent)
         control = self.get_action(agent)
         control = torch.clamp(control, min=-agent.u_range, max=agent.u_range)
         agent.action.u = control * agent.u_multiplier
 
-    def dribble_to_goal(self, agent, env_index=slice(None)):
+    def dribble_to_goal(self, agent, env_index=Ellipsis):
         self.dribble(agent, self.target_net.state.pos[env_index], env_index=env_index)
 
-    def shoot_on_goal(self, agent, env_index=slice(None)):
+    def shoot_on_goal(self, agent, env_index=Ellipsis):
         goal_front = self.target_net.state.pos[env_index].clone()
         left_goal_mask = goal_front[:, X] < 0
         goal_front[:, X] += self.world.goal_depth / 2 * (left_goal_mask.float() * 2 - 1)
         agent_pos = agent.state.pos[env_index]
         shoot_dir = goal_front - agent_pos
         shoot_dir = shoot_dir / shoot_dir.norm(dim=-1)[:, None]
         shoot_pos = goal_front + shoot_dir * self.shoot_on_goal_dist
         self.shoot(agent, shoot_pos, env_index=env_index)
-        # self.shoot(agent, torch.tensor([-0.6, 0.]).unsqueeze(0), env_index=slice(None))
+        # self.shoot(agent, torch.tensor([-0.6, 0.]).unsqueeze(0), env_index=Ellipsis)
 
-    def passto(self, agent, agent_dest, env_index=slice(None)):
+    def passto(self, agent, agent_dest, env_index=Ellipsis):
         self.shoot(agent, agent_dest.state.pos[env_index], env_index=env_index)
 
-    def shoot(self, agent, pos, env_index=slice(None)):
+    def shoot(self, agent, pos, env_index=Ellipsis):
         if isinstance(env_index, int):
             env_index = [env_index]
         self.actions[agent]["dribbling"][env_index] = False
 
         ball_curr_pos = self.ball.state.pos[env_index]
         agent_curr_pos = agent.state.pos[env_index]
         agent_curr_vel = agent.state.vel[env_index]
@@ -1104,15 +1133,15 @@
         self.actions[agent]["shooting"][reached_goal_mask] = False
         self.actions[agent]["pre-shooting"][reached_goal_mask] = False
 
         max_time_mask = self.shooting_timer[agent] > self.max_shoot_time
         self.actions[agent]["shooting"][max_time_mask] = False
         self.actions[agent]["pre-shooting"][max_time_mask] = False
 
-    def dribble(self, agent, pos, env_index=slice(None)):
+    def dribble(self, agent, pos, env_index=Ellipsis):
         if isinstance(env_index, int):
             env_index = [env_index]
         self.actions[agent]["dribbling"][env_index] = True
         dist = (pos - self.ball.state.pos[env_index]).norm(dim=-1)
         reached_goal_mask = self.combine_mask(env_index, dist <= self.ball_pos_eps)
         self.actions[agent]["dribbling"][reached_goal_mask] = False
         dribble_mask = self.actions[agent]["dribbling"][env_index]
@@ -1127,15 +1156,15 @@
             agent,
             pos=pos[dribble_mask],
             env_index=self.combine_mask(
                 env_index, self.actions[agent]["dribbling"][env_index]
             ),
         )
 
-    def update_dribble(self, agent, pos, env_index=slice(None)):
+    def update_dribble(self, agent, pos, env_index=Ellipsis):
         agent_pos = agent.state.pos[env_index]
         ball_pos = self.ball.state.pos[env_index]
         ball_disp = pos - ball_pos
         ball_dist = ball_disp.norm(dim=-1)
         direction = ball_disp / ball_dist[:, None]
         hit_pos = ball_pos - direction * (self.ball.shape.radius + agent.shape.radius)
         hit_vel = direction * self.dribble_speed
@@ -1145,15 +1174,15 @@
         hit_vel[slowdown_mask, :] *= (
             ball_dist[slowdown_mask, None] / self.dribble_slowdown_dist
         )
         # start_vel[slowdown_mask,:] *= ball_dist[slowdown_mask,None] / self.dribble_slowdown_dist
 
         self.go_to(agent, hit_pos, hit_vel, start_vel=start_vel, env_index=env_index)
 
-    def go_to(self, agent, pos, vel, start_vel=None, env_index=slice(None)):
+    def go_to(self, agent, pos, vel, start_vel=None, env_index=Ellipsis):
         start_pos = agent.state.pos[env_index]
         if start_vel is None:
             start_vel = self.get_start_vel(pos, vel, start_pos, self.start_vel_mag)
         self.objectives[agent]["target_pos"][env_index] = pos
         self.objectives[agent]["target_vel"][env_index] = vel
         self.objectives[agent]["start_pos"][env_index] = start_pos
         self.objectives[agent]["start_vel"][env_index] = start_vel
@@ -1173,15 +1202,15 @@
         target_disp = target_pos - start_pos
         target_dist = target_disp.norm(dim=1)
         start_vel_aug_dir = target_disp
         start_vel_aug_dir[target_dist > 0] /= target_dist[target_dist > 0, None]
         start_vel = start_vel_aug_dir * start_vel_mag[:, None]
         return start_vel
 
-    def get_action(self, agent, env_index=slice(None)):
+    def get_action(self, agent, env_index=Ellipsis):
         curr_pos = agent.state.pos[env_index, :]
         curr_vel = agent.state.vel[env_index, :]
         u_start = torch.zeros(curr_pos.shape[0], device=self.world.device)
         des_curr_pos = self.hermite(
             self.objectives[agent]["start_pos"][env_index, :],
             self.objectives[agent]["target_pos"][env_index, :],
             self.objectives[agent]["start_vel"][env_index, :],
@@ -1246,21 +1275,22 @@
                 self.objectives[agent]["start_pos"][env_index, :],
                 self.objectives[agent]["target_pos"][env_index, :],
                 self.objectives[agent]["start_vel"][env_index, :],
                 self.objectives[agent]["target_vel"][env_index, :],
                 u=torch.tensor([u] * num_envs, device=self.world.device),
                 deriv=0,
             )
-            if env_index == slice(None) or (
+            if env_index == Ellipsis or (
                 isinstance(env_index, torch.Tensor)
                 and env_index.dtype == torch.bool
                 and torch.all(env_index)
             ):
                 pointi.set_pos(
-                    torch.as_tensor(posi, device=self.world.device), batch_index=None
+                    torch.as_tensor(posi, device=self.world.device),
+                    batch_index=None,
                 )
             elif isinstance(env_index, int):
                 pointi.set_pos(
                     torch.as_tensor(posi, device=self.world.device),
                     batch_index=env_index,
                 )
             elif isinstance(env_index, list):
@@ -1313,29 +1343,29 @@
         return reduce(
             operator.or_,
             seq,
             torch.zeros(seq[0].shape, device=self.world.device).bool(),
         )
 
     def combine_mask(self, env_index, mask):
-        if env_index == slice(None):
+        if env_index == Ellipsis:
             return mask
         elif isinstance(env_index, torch.Tensor) and env_index.dtype == torch.bool:
             if isinstance(mask, torch.Tensor) and mask.dtype == torch.bool:
                 new_env_index = env_index.clone()
                 new_env_index[env_index] = mask
                 return new_env_index
             else:
                 return torch.arange(env_index.shape[0], device=self.world.device)[mask]
         elif isinstance(env_index, torch.Tensor) and env_index.dtype == torch.int:
             return env_index[mask]
         elif isinstance(env_index, list):
             return torch.tensor(env_index, device=self.world.device)[mask]
 
-    def check_possession(self, env_index=slice(None)):
+    def check_possession(self, env_index=Ellipsis):
         agents_pos = torch.stack(
             [agent.state.pos[env_index] for agent in self.teammates + self.opposition],
             dim=1,
         )
         agents_vel = torch.stack(
             [agent.state.vel[env_index] for agent in self.teammates + self.opposition],
             dim=1,
@@ -1347,15 +1377,15 @@
         dists = (disps + relvels * self.possession_lookahead).norm(dim=-1)
         mindist_agent = torch.argmin(dists[:, : len(self.teammates)], dim=-1)
         mindist_team = torch.argmin(dists, dim=-1) < len(self.teammates)
         for i, agent in enumerate(self.teammates):
             self.agent_possession[agent][env_index] = mindist_agent == i
         self.team_possession[env_index] = mindist_team
 
-    def check_better_positions(self, agent, role, env_index=slice(None)):
+    def check_better_positions(self, agent, role, env_index=Ellipsis):
         curr_pos = agent.state.pos[env_index]
         curr_target = self.objectives[agent]["target_pos"]
         samples = (
             torch.randn(
                 self.nsamples,
                 curr_pos.shape[0],
                 self.world.dim_p,
@@ -1387,17 +1417,15 @@
             dim=0,
             index=highest_value.unsqueeze(0)
             .unsqueeze(-1)
             .expand(-1, -1, self.world.dim_p),
         )
         return best_pos[0, :, :]
 
-    def get_angle_interval(
-        self, pos, obj, objpos=None, beams=128, env_index=slice(None)
-    ):
+    def get_angle_interval(self, pos, obj, objpos=None, beams=128, env_index=Ellipsis):
         # agent_pos = agent.state.pos[env_index]
         if objpos is not None:
             obj_pos = objpos
         else:
             obj_pos = obj.state.pos[env_index]
         if obj == self.target_net or obj == self.own_net:
             left_goal_mask = obj_pos[:, X] < 0
@@ -1448,15 +1476,15 @@
     def get_separations(
         self,
         pos,
         agent=None,
         teammate=True,
         wall=True,
         opposition=False,
-        env_index=slice(None),
+        env_index=Ellipsis,
     ):
         disps = []
         if wall:
             top_wall_dist = -pos[:, Y] + self.world.pitch_width / 2
             bottom_wall_dist = pos[:, Y] + self.world.pitch_width / 2
             left_wall_dist = pos[:, X] + self.world.pitch_length / 2
             right_wall_dist = -pos[:, X] + self.world.pitch_length / 2
@@ -1476,15 +1504,15 @@
         if opposition:
             for otheragent in self.opposition:
                 if otheragent != agent:
                     agent_disp = otheragent.state.pos[env_index] - pos
                     disps.append(agent_disp)
         return disps
 
-    def get_lane_value(self, pos, agent, opposition=False, env_index=slice(None)):
+    def get_lane_value(self, pos, agent, opposition=False, env_index=Ellipsis):
         if not opposition:
             ball_angles, lidar_angles = self.get_angle_interval(pos, self.ball)
             goal_angles, _ = self.get_angle_interval(
                 pos, self.target_net, env_index=env_index
             )
             blocking_angles_list = [
                 self.get_angle_interval(pos, otheragent, env_index=env_index)[0]
@@ -1504,75 +1532,83 @@
             for opp_agent in self.opposition:
                 opp_agent_pos = opp_agent.state.pos[env_index]
                 opp_desired_angles = self.get_angle_interval(
                     opp_agent_pos, self.own_net, env_index=env_index
                 )[0]
                 opp_blocking_angles_list = [
                     self.get_angle_interval(
-                        opp_agent_pos, otheragent, objpos=pos, env_index=env_index
+                        opp_agent_pos,
+                        otheragent,
+                        objpos=pos,
+                        env_index=env_index,
                     )[0]
                     for otheragent in self.teammates
                 ]
                 opp_unblocked_angles = opp_desired_angles & ~self.combine_or(
                     opp_blocking_angles_list
                 )
                 opp_unblocked_angle_ratio = opp_unblocked_angles.sum(
                     dim=-1
                 ) / opp_desired_angles.sum(dim=-1)
                 opp_lane_value += -opp_unblocked_angle_ratio
             opp_lane_value /= len(self.opposition)
             return opp_lane_value
 
-    def get_pos_value(self, pos, role=0.5, agent=None, env_index=slice(None)):
+    def get_pos_value(self, pos, role=0.5, agent=None, env_index=Ellipsis):
         # The value of a position for movement
         # Single agent's sight on goal and the ball, blocked by teammates and opposition
         lane_value = self.get_lane_value(
             pos, agent, opposition=False, env_index=env_index
         )
         # Agent Separations
-        disps = self.get_separations(pos, agent, env_index=env_index)
-        dists = torch.stack(list(map(lambda x: x.norm(dim=-1), disps)), dim=-1)
+        dists = self.get_separations(pos, agent, env_index=env_index)
+        dists = torch.stack([dist.norm(dim=-1) for dist in dists], dim=-1)
         inv_sq_dists = dists ** (-2)
         separation_value = -inv_sq_dists.sum(dim=-1)
         # Entire opposition's sight on goal, blocked by all teammates (shared value for all teammates)
         opp_lane_value = self.get_lane_value(
             pos, agent, opposition=True, env_index=env_index
         )
         # Value Calculation
         values = (
             self.separation_weight * separation_value
             + self.lane_weight * role * lane_value
             + self.lane_weight * (1 - role) * opp_lane_value
         )
         return values
 
-    def get_attack_value(self, agent, env_index=slice(None)):
+    def get_attack_value(self, agent, env_index=Ellipsis):
         # The value of a position for attacking purposes
         agent_pos = agent.state.pos[env_index]
         lane_value = self.attack_lane_weight * self.get_lane_value(
-            agent.state.pos[env_index], agent, opposition=False, env_index=env_index
+            agent.state.pos[env_index],
+            agent,
+            opposition=False,
+            env_index=env_index,
         )
 
         goal_dist = (agent_pos - self.target_net.state.pos[env_index]).norm(dim=-1)
         goal_dist_value = self.attack_goal_dist_weight * -goal_dist
 
-        opp_disps = self.get_separations(
+        opp_dists = self.get_separations(
             agent_pos,
             agent,
             teammate=False,
             wall=False,
             opposition=True,
             env_index=env_index,
         )
-        opp_dists = torch.stack(list(map(lambda x: x.norm(dim=-1), opp_disps)), dim=-1)
+        opp_dists = torch.stack(
+            [opp_dist.norm(dim=-1) for opp_dist in opp_dists], dim=-1
+        )
         opp_dist = torch.min(opp_dists, dim=-1)[0]
         opp_dist_value = self.attack_defender_dist_weight * opp_dist
         return lane_value + goal_dist_value + opp_dist_value
 
-    def can_shoot(self, agent, env_index=slice(None)):
+    def can_shoot(self, agent, env_index=Ellipsis):
         # Distance
         ball_pos = self.ball.state.pos[env_index]
         goal_dist = (ball_pos - self.target_net.state.pos[env_index]).norm(dim=-1)
         within_range_mask = goal_dist < self.shooting_dist
         # Angle
         beams = 128
         goal_angles, lidar_angles = self.get_angle_interval(
@@ -1592,31 +1628,31 @@
             unblocked_angles[:, :-1].int() - unblocked_angles[:, 1:].int()
         )
         indicesx = indicesxy[0].view(-1, 2)[:, 0]
         indicesy = indicesxy[1].view(-1, 2)
         n = (
             torch.zeros(unblocked_angles.shape[0], device=self.world.device)
             .int()
-            .scatter(
+            .scatter_reduce(
                 index=indicesx,
                 src=(indicesy[:, 1] - indicesy[:, 0]).int(),
                 dim=0,
-                reduce="add",
+                reduce="sum",
             )
         )
         midpt = (
             torch.zeros(unblocked_angles.shape[0], device=self.world.device)
             .float()
-            .scatter(
+            .scatter_reduce(
                 index=indicesx,
                 src=(indicesy[:, 1] + indicesy[:, 0])
                 / 2
                 * (indicesy[:, 1] - indicesy[:, 0]),
                 dim=0,
-                reduce="add",
+                reduce="sum",
             )
             / n
             + 0.5
         )
         midpt[torch.isnan(midpt)] = 0
         within_angle_mask = n * (2 * torch.pi / beams) >= self.shooting_angle
         # Result
@@ -1629,15 +1665,15 @@
             [torch.sin(shoot_angle), torch.cos(shoot_angle)], dim=-1
         )
         shoot_pos = ball_pos + shoot_dir * (
             goal_dist[:, None] + self.shoot_on_goal_dist
         )
         return can_shoot_mask, shoot_pos
 
-    def can_pass(self, agent_dest, env_index=slice(None)):
+    def can_pass(self, agent_dest, env_index=Ellipsis):
         # Distance
         ball_pos = self.ball.state.pos[env_index]
         agent_pos = agent_dest.state.pos[env_index]
         agent_dist = (ball_pos - agent_pos).norm(dim=-1)
         within_range_mask = agent_dist <= self.shooting_dist
         # Angle
         beams = 128
@@ -1654,17 +1690,19 @@
         unblocked_angles = goal_angles & ~self.combine_or(blocking_angles_list)
         passing_angle = unblocked_angles.sum(dim=-1) * (2 * torch.pi / beams)
         within_angle_mask = passing_angle >= self.passing_angle
         can_pass_mask = within_range_mask & within_angle_mask
         return can_pass_mask
 
 
-""" Run """
+# Run
 if __name__ == "__main__":
     render_interactively(
         __file__,
         control_two_agents=True,
         continuous=True,
-        n_blue_agents=3,
-        n_red_agents=3,
+        n_blue_agents=2,
+        n_red_agents=2,
+        ai_red_agents=True,
+        ai_blue_agents=False,
         dense_reward_ratio=0.001,
     )
```

### Comparing `vmas-1.4.0/vmas/scenarios/give_way.py` & `vmas-1.4.1/vmas/scenarios/give_way.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 import math
 
 import torch
+
 from vmas import render_interactively
-from vmas.simulator.core import Agent, World, Landmark, Sphere, Line, Box
+from vmas.simulator.controllers.velocity_controller import VelocityController
+from vmas.simulator.core import Agent, Box, Landmark, Line, Sphere, World
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color, TorchUtils
-from vmas.simulator.controllers.velocity_controller import VelocityController
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         self.v_range = kwargs.get("v_range", 0.5)
         self.a_range = kwargs.get("a_range", 1)
         self.obs_noise = kwargs.get("obs_noise", 0)
@@ -62,17 +63,19 @@
         self.min_collision_distance = 0.005
 
         # Add agents
         blue_agent = Agent(
             name="agent_0",
             rotatable=False,
             linear_friction=self.linear_friction,
-            shape=Sphere(radius=self.agent_radius)
-            if not self.box_agents
-            else Box(length=self.agent_box_length, width=self.agent_box_width),
+            shape=(
+                Sphere(radius=self.agent_radius)
+                if not self.box_agents
+                else Box(length=self.agent_box_length, width=self.agent_box_width)
+            ),
             u_range=self.u_range,
             f_range=self.f_range,
             v_range=self.v_range,
             render_action=True,
         )
         if self.use_velocity_controller:
             blue_agent.controller = VelocityController(
@@ -88,17 +91,19 @@
         world.add_agent(blue_agent)
         world.add_landmark(blue_goal)
 
         green_agent = Agent(
             name="agent_1",
             color=Color.GREEN,
             linear_friction=self.linear_friction,
-            shape=Sphere(radius=self.agent_radius)
-            if not self.box_agents
-            else Box(length=self.agent_box_length, width=self.agent_box_width),
+            shape=(
+                Sphere(radius=self.agent_radius)
+                if not self.box_agents
+                else Box(length=self.agent_box_length, width=self.agent_box_width)
+            ),
             rotatable=False,
             u_range=self.u_range,
             f_range=self.f_range,
             v_range=self.v_range,
             render_action=True,
         )
         if self.use_velocity_controller:
@@ -135,18 +140,15 @@
     def reset_world_at(self, env_index: int = None):
         self.world.agents[0].set_pos(
             torch.tensor(
                 [-(self.scenario_length / 2 - self.agent_dist_from_wall), 0.0],
                 dtype=torch.float32,
                 device=self.world.device,
             )
-            + torch.zeros(
-                self.world.dim_p,
-                device=self.world.device,
-            ).uniform_(
+            + torch.zeros(self.world.dim_p, device=self.world.device,).uniform_(
                 -self.spawn_pos_noise,
                 self.spawn_pos_noise,
             ),
             batch_index=env_index,
         )
         if self.use_velocity_controller:
             self.world.agents[0].controller.reset(env_index)
@@ -160,18 +162,15 @@
         )
         self.world.agents[1].set_pos(
             torch.tensor(
                 [self.scenario_length / 2 - self.agent_dist_from_wall, 0.0],
                 dtype=torch.float32,
                 device=self.world.device,
             )
-            + torch.zeros(
-                self.world.dim_p,
-                device=self.world.device,
-            ).uniform_(
+            + torch.zeros(self.world.dim_p, device=self.world.device,).uniform_(
                 -self.spawn_pos_noise,
                 self.spawn_pos_noise,
             ),
             batch_index=env_index,
         )
         if self.use_velocity_controller:
             self.world.agents[1].controller.reset(env_index)
@@ -268,26 +267,27 @@
         agent.agent_collision_rew[:] = 0
         agent.obstacle_collision_rew[:] = 0
         for a in self.world.agents:
             if a != agent:
                 agent.agent_collision_rew[
                     self.world.get_distance(agent, a) <= self.min_collision_distance
                 ] += self.agent_collision_penalty
-        for l in self.world.landmarks:
-            if self.world.collides(agent, l):
-                if l in (
+        for landmark in self.world.landmarks:
+            if self.world.collides(agent, landmark):
+                if landmark in (
                     [*self.passage_1, *self.passage_2]
                     if self.mirror_passage is True
                     else [*self.passage_1]
                 ):
                     penalty = self.passage_collision_penalty
                 else:
                     penalty = self.obstacle_collision_penalty
                 agent.obstacle_collision_rew[
-                    self.world.get_distance(agent, l) <= self.min_collision_distance
+                    self.world.get_distance(agent, landmark)
+                    <= self.min_collision_distance
                 ] += penalty
 
         # Energy reward
         agent.energy_expenditure = torch.linalg.vector_norm(
             agent.action.u, dim=-1
         ) / math.sqrt(self.world.dim_p * (agent.f_range**2))
 
@@ -312,18 +312,15 @@
             agent.state.vel,
         ]
         if self.observe_rel_pos:
             observations += rel
 
         if self.obs_noise > 0:
             for i, obs in enumerate(observations):
-                noise = torch.zeros(
-                    *obs.shape,
-                    device=self.world.device,
-                ).uniform_(
+                noise = torch.zeros(*obs.shape, device=self.world.device,).uniform_(
                     -self.obs_noise,
                     self.obs_noise,
                 )
                 observations[i] = obs + noise
         return torch.cat(
             observations,
             dim=-1,
@@ -418,17 +415,19 @@
 
     def reset_map(self, env_index):
         # Walls
         for i, landmark in enumerate(self.walls):
             landmark.set_pos(
                 torch.tensor(
                     [
-                        -self.scenario_length / 2
-                        if i == 0
-                        else self.scenario_length / 2,
+                        (
+                            -self.scenario_length / 2
+                            if i == 0
+                            else self.scenario_length / 2
+                        ),
                         0.0,
                     ],
                     dtype=torch.float32,
                     device=self.world.device,
                 ),
                 batch_index=env_index,
             )
@@ -502,17 +501,19 @@
                 )
 
             # Asymmetric hole
             for i, landmark in enumerate(self.passage_2[:-1]):
                 landmark.set_pos(
                     torch.tensor(
                         [
-                            -self.passage_length / 2
-                            if i == 0
-                            else self.passage_length / 2,
+                            (
+                                -self.passage_length / 2
+                                if i == 0
+                                else self.passage_length / 2
+                            ),
                             -self.passage_length / 2 - self.passage_width / 2,
                         ],
                         dtype=torch.float32,
                         device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
```

### Comparing `vmas-1.4.0/vmas/scenarios/joint_passage.py` & `vmas-1.4.1/vmas/scenarios/joint_passage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 import math
 from typing import Dict
 
 import torch
 from torch import Tensor
 
 from vmas import render_interactively
-from vmas.simulator.core import Agent, Box, Landmark, Sphere, World, Line
+from vmas.simulator.controllers.velocity_controller import VelocityController
+from vmas.simulator.core import Agent, Box, Landmark, Line, Sphere, World
 from vmas.simulator.joints import Joint
 from vmas.simulator.scenario import BaseScenario
-from vmas.simulator.utils import Color, Y, X
-from vmas.simulator.controllers.velocity_controller import VelocityController
+from vmas.simulator.utils import Color, X, Y
 
 
 def get_line_angle_0_90(rot: Tensor):
     angle = torch.abs(rot) % torch.pi
     other_angle = torch.pi - angle
     return torch.minimum(angle, other_angle)
 
@@ -28,15 +28,16 @@
 
 def get_line_angle_dist_0_180(angle, goal):
     angle = get_line_angle_0_180(angle)
     goal = get_line_angle_0_180(goal)
     return torch.minimum(
         (angle - goal).abs(),
         torch.minimum(
-            (angle - (goal - torch.pi)).abs(), ((angle - torch.pi) - goal).abs()
+            (angle - (goal - torch.pi)).abs(),
+            ((angle - torch.pi) - goal).abs(),
         ),
     ).squeeze(-1)
 
 
 def angle_to_vector(angle):
     return torch.cat([torch.cos(angle), torch.sin(angle)], dim=1)
 
@@ -381,15 +382,17 @@
             )
 
     def reward(self, agent: Agent):
         is_first = agent == self.world.agents[0]
 
         if is_first:
             self.rew = torch.zeros(
-                self.world.batch_dim, device=self.world.device, dtype=torch.float32
+                self.world.batch_dim,
+                device=self.world.device,
+                dtype=torch.float32,
             )
             self.pos_rew[:] = 0
             self.rot_rew[:] = 0
             self.collision_rew[:] = 0
 
             joint_passed = self.joint.landmark.state.pos[:, Y] > 0
             self.all_passed = (
@@ -455,15 +458,15 @@
                     for wall in self.walls:
                         self.collision_rew[
                             self.world.get_distance(a, wall)
                             <= self.min_collision_distance
                         ] += self.collision_reward
 
             # Joint collisions
-            for i, p in enumerate(self.passages):
+            for p in self.passages:
                 if p.collide:
                     self.collision_rew[
                         self.world.get_distance(p, self.joint.landmark)
                         <= self.min_collision_distance
                     ] += self.collision_reward
 
             # Energy reward
@@ -494,15 +497,17 @@
         return is_out_or_touching_perimeter
 
     def observation(self, agent: Agent):
         if self.observe_joint_angle:
             joint_angle = self.joint.landmark.state.rot
             angle_noise = (
                 torch.randn(
-                    *joint_angle.shape, device=self.world.device, dtype=torch.float32
+                    *joint_angle.shape,
+                    device=self.world.device,
+                    dtype=torch.float32,
                 )
                 * self.joint_angle_obs_noise
                 if self.joint_angle_obs_noise
                 else 0.0
             )
             joint_angle += angle_noise
 
@@ -517,18 +522,15 @@
             agent.state.vel,
             agent.state.pos - self.goal.state.pos,
             *passage_obs,
             angle_to_vector(self.goal.state.rot),
         ] + ([angle_to_vector(joint_angle)] if self.observe_joint_angle else [])
 
         for i, obs in enumerate(observations):
-            noise = torch.zeros(
-                *obs.shape,
-                device=self.world.device,
-            ).uniform_(
+            noise = torch.zeros(*obs.shape, device=self.world.device,).uniform_(
                 -self.obs_noise,
                 self.obs_noise,
             )
             # noise = (
             #     torch.randn(*obs.shape, device=self.world.device, dtype=torch.float32)
             #     * agent.obs_noise
             #     if agent.obs_noise
@@ -678,36 +680,41 @@
             i += 1
 
     def spawn_walls(self, env_index):
         for i, wall in enumerate(self.walls):
             wall.set_pos(
                 torch.tensor(
                     [
-                        0.0
-                        if i % 2
-                        else (
-                            self.world.x_semidim + self.agent_radius
-                            if i == 0
-                            else -self.world.x_semidim - self.agent_radius
+                        (
+                            0.0
+                            if i % 2
+                            else (
+                                self.world.x_semidim + self.agent_radius
+                                if i == 0
+                                else -self.world.x_semidim - self.agent_radius
+                            )
                         ),
-                        0.0
-                        if not i % 2
-                        else (
-                            self.world.y_semidim + self.agent_radius
-                            if i == 1
-                            else -self.world.y_semidim - self.agent_radius
+                        (
+                            0.0
+                            if not i % 2
+                            else (
+                                self.world.y_semidim + self.agent_radius
+                                if i == 1
+                                else -self.world.y_semidim - self.agent_radius
+                            )
                         ),
                     ],
                     device=self.world.device,
                 ),
                 batch_index=env_index,
             )
             wall.set_rot(
                 torch.tensor(
-                    [torch.pi / 2 if not i % 2 else 0.0], device=self.world.device
+                    [torch.pi / 2 if not i % 2 else 0.0],
+                    device=self.world.device,
                 ),
                 batch_index=env_index,
             )
 
     def extra_render(self, env_index: int = 0):
         from vmas.simulator import rendering
```

### Comparing `vmas-1.4.0/vmas/scenarios/joint_passage_size.py` & `vmas-1.4.1/vmas/scenarios/joint_passage_size.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 import math
 from typing import Dict
 
 import torch
 from torch import Tensor
 
 from vmas import render_interactively
-from vmas.simulator.core import Agent, Box, Landmark, Sphere, World, Line
+from vmas.simulator.controllers.velocity_controller import VelocityController
+from vmas.simulator.core import Agent, Box, Landmark, Line, Sphere, World
 from vmas.simulator.joints import Joint
 from vmas.simulator.scenario import BaseScenario
-from vmas.simulator.utils import Color, Y, X
-from vmas.simulator.controllers.velocity_controller import VelocityController
+from vmas.simulator.utils import Color, X, Y
 
 
 def angle_to_vector(angle):
     return torch.cat([torch.cos(angle), torch.sin(angle)], dim=1)
 
 
 def get_line_angle_0_90(rot: Tensor):
@@ -38,15 +38,16 @@
 
 def get_line_angle_dist_0_180(angle, goal):
     angle = get_line_angle_0_180(angle)
     goal = get_line_angle_0_180(goal)
     return torch.minimum(
         (angle - goal).abs(),
         torch.minimum(
-            (angle - (goal - torch.pi)).abs(), ((angle - torch.pi) - goal).abs()
+            (angle - (goal - torch.pi)).abs(),
+            ((angle - torch.pi) - goal).abs(),
         ),
     ).squeeze(-1)
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         self.fixed_passage = kwargs.get("fixed_passage", False)
@@ -203,15 +204,15 @@
 
     def set_n_passages(self, val):
         if val == 4:
             self.middle_angle_180 = True
         elif val == 3:
             self.middle_angle_180 = False
         else:
-            assert False
+            raise AssertionError()
         self.n_passages = val
         del self.world._landmarks[-self.n_boxes :]
         self.create_passage_map(self.world)
         self.reset_world_at()
 
     def reset_world_at(self, env_index: int = None):
         start_angle = torch.rand(
@@ -320,15 +321,17 @@
 
         self.spawn_passage_map(env_index)
 
         self.spawn_walls(env_index)
 
         if env_index is None:
             self.t = torch.zeros(
-                self.world.batch_dim, device=self.world.device, dtype=torch.float32
+                self.world.batch_dim,
+                device=self.world.device,
+                dtype=torch.float32,
             )
             self.passed = torch.zeros((self.world.batch_dim,), device=self.world.device)
 
             self.joint.pos_shaping_pre = (
                 torch.linalg.vector_norm(
                     self.joint.landmark.state.pos - self.pass_center, dim=1
                 )
@@ -383,15 +386,17 @@
 
     def reward(self, agent: Agent):
         is_first = agent == self.world.agents[0]
 
         if is_first:
             self.t += 1
             self.rew = torch.zeros(
-                self.world.batch_dim, device=self.world.device, dtype=torch.float32
+                self.world.batch_dim,
+                device=self.world.device,
+                dtype=torch.float32,
             )
             self.pos_rew[:] = 0
             self.rot_rew[:] = 0
             self.collision_rew[:] = 0
             self.energy_rew[:] = 0
 
             joint_passed = self.joint.landmark.state.pos[:, Y] > 0
@@ -489,15 +494,17 @@
         return is_out_or_touching_perimeter
 
     def observation(self, agent: Agent):
         if self.observe_joint_angle:
             joint_angle = self.joint.landmark.state.rot
             angle_noise = (
                 torch.randn(
-                    *joint_angle.shape, device=self.world.device, dtype=torch.float32
+                    *joint_angle.shape,
+                    device=self.world.device,
+                    dtype=torch.float32,
                 )
                 * self.joint_angle_obs_noise
                 if self.joint_angle_obs_noise
                 else 0.0
             )
             joint_angle += angle_noise
 
@@ -508,18 +515,15 @@
             agent.state.pos - self.big_passage_pos,
             agent.state.pos - self.small_passage_pos,
             angle_to_vector(self.goal.state.rot),
         ] + ([angle_to_vector(joint_angle)] if self.observe_joint_angle else [])
 
         if self.obs_noise > 0:
             for i, obs in enumerate(observations):
-                noise = torch.zeros(
-                    *obs.shape,
-                    device=self.world.device,
-                ).uniform_(
+                noise = torch.zeros(*obs.shape, device=self.world.device,).uniform_(
                     -self.obs_noise,
                     self.obs_noise,
                 )
                 observations[i] = obs + noise
         return torch.cat(
             observations,
             dim=-1,
@@ -692,36 +696,41 @@
             i += 1
 
     def spawn_walls(self, env_index):
         for i, wall in enumerate(self.walls):
             wall.set_pos(
                 torch.tensor(
                     [
-                        0.0
-                        if i % 2
-                        else (
-                            self.world.x_semidim + self.agent_radius
-                            if i == 0
-                            else -self.world.x_semidim - self.agent_radius
+                        (
+                            0.0
+                            if i % 2
+                            else (
+                                self.world.x_semidim + self.agent_radius
+                                if i == 0
+                                else -self.world.x_semidim - self.agent_radius
+                            )
                         ),
-                        0.0
-                        if not i % 2
-                        else (
-                            self.world.y_semidim + self.agent_radius
-                            if i == 1
-                            else -self.world.y_semidim - self.agent_radius
+                        (
+                            0.0
+                            if not i % 2
+                            else (
+                                self.world.y_semidim + self.agent_radius
+                                if i == 1
+                                else -self.world.y_semidim - self.agent_radius
+                            )
                         ),
                     ],
                     device=self.world.device,
                 ),
                 batch_index=env_index,
             )
             wall.set_rot(
                 torch.tensor(
-                    [torch.pi / 2 if not i % 2 else 0.0], device=self.world.device
+                    [torch.pi / 2 if not i % 2 else 0.0],
+                    device=self.world.device,
                 ),
                 batch_index=env_index,
             )
 
     def extra_render(self, env_index: int = 0):
         from vmas.simulator import rendering
```

### Comparing `vmas-1.4.0/vmas/scenarios/mpe/simple.py` & `vmas-1.4.1/vmas/scenarios/mpe/simple.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 import torch
 
 from vmas import render_interactively
-from vmas.simulator.core import Agent, World, Landmark
+from vmas.simulator.core import Agent, Landmark, World
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         # Make world
@@ -29,43 +29,48 @@
 
         return world
 
     def reset_world_at(self, env_index: int = None):
         for agent in self.world.agents:
             agent.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -1.0,
                     1.0,
                 ),
                 batch_index=env_index,
             )
         for landmark in self.world.landmarks:
             landmark.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -1.0,
                     1.0,
                 ),
                 batch_index=env_index,
             )
 
     def reward(self, agent: Agent):
         dist2 = torch.sum(
-            torch.square(agent.state.pos - self.world.landmarks[0].state.pos), dim=-1
+            torch.square(agent.state.pos - self.world.landmarks[0].state.pos),
+            dim=-1,
         )
         return -dist2
 
     def observation(self, agent: Agent):
         # get positions of all entities in this agent's reference frame
         entity_pos = []
         for entity in self.world.landmarks:
```

### Comparing `vmas-1.4.0/vmas/scenarios/mpe/simple_adversary.py` & `vmas-1.4.1/vmas/scenarios/mpe/simple_adversary.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 import torch
 
 from vmas import render_interactively
-from vmas.simulator.core import World, Agent, Landmark, Sphere
+from vmas.simulator.core import Agent, Landmark, Sphere, World
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         n_agents = kwargs.get("n_agents", 3)
@@ -56,32 +56,36 @@
             goal.color = Color.GREEN
             for agent in self.world.agents:
                 agent.goal = goal
 
         for agent in self.world.agents:
             agent.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -1.0,
                     1.0,
                 ),
                 batch_index=env_index,
             )
 
         for landmark in self.world.landmarks:
             landmark.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -1.0,
                     1.0,
                 ),
                 batch_index=env_index,
@@ -112,65 +116,75 @@
         adversary_agents = self.adversaries()
         if shaped_adv_reward:  # distance-based adversary reward
             adv_rew = torch.sum(
                 torch.stack(
                     [
                         torch.sqrt(
                             torch.sum(
-                                torch.square(a.state.pos - a.goal.state.pos), dim=-1
+                                torch.square(a.state.pos - a.goal.state.pos),
+                                dim=-1,
                             )
                         )
                         for a in adversary_agents
                     ],
                     dim=1,
                 ),
                 dim=-1,
             )
         else:  # proximity-based adversary reward (binary)
             adv_rew = torch.zeros(
-                self.world.batch_dim, device=self.world.device, dtype=torch.float32
+                self.world.batch_dim,
+                device=self.world.device,
+                dtype=torch.float32,
             )
             for a in adversary_agents:
                 is_too_close = (
                     torch.sqrt(
-                        torch.sum(torch.square(a.state.pos - a.goal.state.pos), dim=-1)
+                        torch.sum(
+                            torch.square(a.state.pos - a.goal.state.pos),
+                            dim=-1,
+                        )
                     )
                     < 2 * a.goal.size
                 )
                 adv_rew[is_too_close] -= 5
 
         # Calculate positive reward for agents
         good_agents = self.good_agents()
         if shaped_reward:  # distance-based agent reward
             pos_rew = -torch.min(
                 torch.stack(
                     [
                         torch.sqrt(
                             torch.sum(
-                                torch.square(a.state.pos - a.goal.state.pos), dim=-1
+                                torch.square(a.state.pos - a.goal.state.pos),
+                                dim=-1,
                             )
                         )
                         for a in good_agents
                     ],
                     dim=1,
                 ),
                 dim=-1,
             )[0]
 
         else:  # proximity-based agent reward (binary)
             pos_rew = torch.zeros(
-                self.world.batch_dim, device=self.world.device, dtype=torch.float32
+                self.world.batch_dim,
+                device=self.world.device,
+                dtype=torch.float32,
             )
             is_close_enough = (
                 torch.min(
                     torch.stack(
                         [
                             torch.sqrt(
                                 torch.sum(
-                                    torch.square(a.state.pos - a.goal.state.pos), dim=-1
+                                    torch.square(a.state.pos - a.goal.state.pos),
+                                    dim=-1,
                                 )
                             )
                             for a in good_agents
                         ],
                         dim=1,
                     ),
                     dim=-1,
@@ -179,15 +193,16 @@
             )
             pos_rew[is_close_enough] += 5
             pos_rew -= torch.min(
                 torch.stack(
                     [
                         torch.sqrt(
                             torch.sum(
-                                torch.square(a.state.pos - a.goal.state.pos), dim=-1
+                                torch.square(a.state.pos - a.goal.state.pos),
+                                dim=-1,
                             )
                         )
                         for a in good_agents
                     ],
                     dim=1,
                 ),
                 dim=-1,
@@ -195,25 +210,31 @@
         return pos_rew + adv_rew
 
     def adversary_reward(self, agent: Agent):
         # Rewarded based on proximity to the goal landmark
         shaped_reward = True
         if shaped_reward:  # distance-based reward
             return -torch.sqrt(
-                torch.sum(torch.square(agent.state.pos - agent.goal.state.pos), dim=-1)
+                torch.sum(
+                    torch.square(agent.state.pos - agent.goal.state.pos),
+                    dim=-1,
+                )
             )
 
         else:  # proximity-based reward (binary)
             adv_rew = torch.zeros(
-                self.world.batch_dim, device=self.world.device, dtype=torch.float32
+                self.world.batch_dim,
+                device=self.world.device,
+                dtype=torch.float32,
             )
             close_enough = (
                 torch.sqrt(
                     torch.sum(
-                        torch.square(agent.state.pos - agent.goal.state.pos), dim=-1
+                        torch.square(agent.state.pos - agent.goal.state.pos),
+                        dim=-1,
                     )
                 )
                 < 2 * agent.goal.size
             )
             adv_rew[close_enough] += 5
             return adv_rew
 
@@ -227,15 +248,19 @@
         for other in self.world.agents:
             if other is agent:
                 continue
             other_pos.append(other.state.pos - agent.state.pos)
 
         if not agent.adversary:
             return torch.cat(
-                [agent.goal.state.pos - agent.state.pos, *entity_pos, *other_pos],
+                [
+                    agent.goal.state.pos - agent.state.pos,
+                    *entity_pos,
+                    *other_pos,
+                ],
                 dim=-1,
             )
         else:
             return torch.cat([*entity_pos, *other_pos], dim=-1)
 
 
 if __name__ == "__main__":
```

### Comparing `vmas-1.4.0/vmas/scenarios/mpe/simple_crypto.py` & `vmas-1.4.1/vmas/scenarios/mpe/simple_crypto.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Scenario:
 1 speaker, 2 listeners (one of which is an adversary). Good agents rewarded for proximity to goal, and distance from
 adversary to goal. Adversary is rewarded for its distance to the goal.
 """
 
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 import torch
 
-from vmas.simulator.core import World, Agent
+from vmas.simulator.core import Agent, World
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         dim_c = kwargs.get("dim_c", 4)
@@ -33,42 +33,50 @@
         for i in range(num_agents):
             adversary = True if i < num_adversaries else False
             speaker = True if i == 2 else False
             agent = Agent(
                 name=("eve_0" if adversary else ("alice_0" if speaker else "bob_0")),
                 collide=False,
                 movable=False,
-                color=Color.RED
-                if adversary
-                else (Color.GREEN if speaker else Color.BLUE),
+                color=(
+                    Color.RED if adversary else (Color.GREEN if speaker else Color.BLUE)
+                ),
                 adversary=adversary,
                 silent=False,
             )
             agent.speaker = speaker
             world.add_agent(agent)
 
         return world
 
     def reset_world_at(self, env_index: int = None):
         key = torch.randint(
-            0, 2, (self.world.batch_dim, self.world.dim_c), device=self.world.device
+            0,
+            2,
+            (self.world.batch_dim, self.world.dim_c),
+            device=self.world.device,
         )
         secret = torch.randint(
-            0, 2, (self.world.batch_dim, self.world.dim_c), device=self.world.device
+            0,
+            2,
+            (self.world.batch_dim, self.world.dim_c),
+            device=self.world.device,
         )
 
         if env_index is None:
             for agent in self.world.agents:
                 agent.key = None if not agent.speaker else key
                 agent.secret = secret
                 agent.set_pos(
                     torch.zeros(
-                        (1, self.world.dim_p)
-                        if env_index is not None
-                        else (self.world.batch_dim, self.world.dim_p),
+                        (
+                            (1, self.world.dim_p)
+                            if env_index is not None
+                            else (self.world.batch_dim, self.world.dim_p)
+                        ),
                         device=self.world.device,
                         dtype=torch.float32,
                     ).uniform_(
                         -1.0,
                         1.0,
                     ),
                     batch_index=env_index,
```

### Comparing `vmas-1.4.0/vmas/scenarios/mpe/simple_push.py` & `vmas-1.4.1/vmas/scenarios/mpe/simple_push.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 import torch
 
 from vmas import render_interactively
-from vmas.simulator.core import World, Agent, Landmark
+from vmas.simulator.core import Agent, Landmark, World
 from vmas.simulator.scenario import BaseScenario
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         world = World(
             batch_dim=batch_dim,
@@ -41,25 +41,29 @@
         return world
 
     def reset_world_at(self, env_index: int = None):
         if env_index is None:
             # set goal landmark
             for i, landmark in enumerate(self.world.landmarks):
                 landmark.color = torch.tensor(
-                    [0.1, 0.1, 0.1], device=self.world.device, dtype=torch.float32
+                    [0.1, 0.1, 0.1],
+                    device=self.world.device,
+                    dtype=torch.float32,
                 )
                 landmark.color[i + 1] += 0.8
                 landmark.index = i
             # set goal landmark
             goal = self.world.landmarks[
                 torch.randint(0, len(self.world.landmarks), (1,)).item()
             ]
-            for i, agent in enumerate(self.world.agents):
+            for agent in self.world.agents:
                 agent.color = torch.tensor(
-                    [0.25, 0.25, 0.25], device=self.world.device, dtype=torch.float32
+                    [0.25, 0.25, 0.25],
+                    device=self.world.device,
+                    dtype=torch.float32,
                 )
                 if agent.adversary:
                     agent.color = torch.tensor(
                         [0.75, 0.25, 0.25],
                         device=self.world.device,
                         dtype=torch.float32,
                     )
@@ -67,31 +71,35 @@
                     j = goal.index
                     agent.color[j + 1] += 0.5  # Agent color is similar to its goal
                 agent.goal = goal
 
         for agent in self.world.agents:
             agent.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -1.0,
                     1.0,
                 ),
                 batch_index=env_index,
             )
         for landmark in self.world.landmarks:
             landmark.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -1.0,
                     1.0,
                 ),
                 batch_index=env_index,
@@ -113,15 +121,18 @@
 
     def adversary_reward(self, agent: Agent):
         # keep the nearest good agents away from the goal
         pos_rew = torch.min(
             torch.stack(
                 [
                     torch.sqrt(
-                        torch.sum(torch.square(a.state.pos - a.goal.state.pos), dim=-1)
+                        torch.sum(
+                            torch.square(a.state.pos - a.goal.state.pos),
+                            dim=-1,
+                        )
                     )
                     for a in self.world.agents
                     if not a.adversary
                 ],
                 dim=1,
             ),
             dim=-1,
```

### Comparing `vmas-1.4.0/vmas/scenarios/mpe/simple_reference.py` & `vmas-1.4.1/vmas/scenarios/mpe/simple_reference.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 import torch
 
-from vmas.simulator.core import World, Agent, Landmark
+from vmas.simulator.core import Agent, Landmark, World
 from vmas.simulator.scenario import BaseScenario
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         world = World(batch_dim=batch_dim, device=device, dim_c=10)
 
@@ -41,53 +41,65 @@
                 torch.randint(0, len(self.world.landmarks), (1,)).item()
             ]
             self.world.agents[1].goal_a = self.world.agents[0]
             self.world.agents[1].goal_b = self.world.landmarks[
                 torch.randint(0, len(self.world.landmarks), (1,)).item()
             ]
             # random properties for agents
-            for i, agent in enumerate(self.world.agents):
+            for agent in self.world.agents:
                 agent.color = torch.tensor(
-                    [0.25, 0.25, 0.25], device=self.world.device, dtype=torch.float32
+                    [0.25, 0.25, 0.25],
+                    device=self.world.device,
+                    dtype=torch.float32,
                 )
             # random properties for landmarks
             self.world.landmarks[0].color = torch.tensor(
-                [0.75, 0.25, 0.25], device=self.world.device, dtype=torch.float32
+                [0.75, 0.25, 0.25],
+                device=self.world.device,
+                dtype=torch.float32,
             )
             self.world.landmarks[1].color = torch.tensor(
-                [0.25, 0.75, 0.25], device=self.world.device, dtype=torch.float32
+                [0.25, 0.75, 0.25],
+                device=self.world.device,
+                dtype=torch.float32,
             )
             self.world.landmarks[2].color = torch.tensor(
-                [0.25, 0.25, 0.75], device=self.world.device, dtype=torch.float32
+                [0.25, 0.25, 0.75],
+                device=self.world.device,
+                dtype=torch.float32,
             )
             # special colors for goals
             self.world.agents[0].goal_a.color = self.world.agents[0].goal_b.color
             self.world.agents[1].goal_a.color = self.world.agents[1].goal_b.color
 
         # set random initial states
         for agent in self.world.agents:
             agent.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -1.0,
                     1.0,
                 ),
                 batch_index=env_index,
             )
         for landmark in self.world.landmarks:
             landmark.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -1.0,
                     1.0,
                 ),
                 batch_index=env_index,
@@ -102,15 +114,16 @@
                     return torch.zeros(
                         self.world.batch_dim,
                         device=self.world.device,
                         dtype=torch.float32,
                     )
                 self.rew += -torch.sqrt(
                     torch.sum(
-                        torch.square(a.goal_a.state.pos - a.goal_b.state.pos), dim=-1
+                        torch.square(a.goal_a.state.pos - a.goal_b.state.pos),
+                        dim=-1,
                     )
                 )
         return self.rew
 
     def observation(self, agent: Agent):
         # goal color
         goal_color = agent.goal_b.color
```

### Comparing `vmas-1.4.0/vmas/scenarios/mpe/simple_speaker_listener.py` & `vmas-1.4.1/vmas/scenarios/mpe/simple_speaker_listener.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 import torch
 
-from vmas.simulator.core import World, Agent, Landmark, Sphere
+from vmas.simulator.core import Agent, Landmark, Sphere, World
 from vmas.simulator.scenario import BaseScenario
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         world = World(batch_dim=batch_dim, device=device, dim_c=3)
         # set any world properties first
@@ -44,56 +44,70 @@
                 agent.goal_b = None
             # want listener to go to the goal landmark
             self.world.agents[0].goal_a = self.world.agents[1]
             self.world.agents[0].goal_b = self.world.landmarks[
                 torch.randint(0, len(self.world.landmarks), (1,)).item()
             ]
             # random properties for agents
-            for i, agent in enumerate(self.world.agents):
+            for agent in self.world.agents:
                 agent.color = torch.tensor(
-                    [0.25, 0.25, 0.25], device=self.world.device, dtype=torch.float32
+                    [0.25, 0.25, 0.25],
+                    device=self.world.device,
+                    dtype=torch.float32,
                 )
             # random properties for landmarks
             self.world.landmarks[0].color = torch.tensor(
-                [0.65, 0.15, 0.15], device=self.world.device, dtype=torch.float32
+                [0.65, 0.15, 0.15],
+                device=self.world.device,
+                dtype=torch.float32,
             )
             self.world.landmarks[1].color = torch.tensor(
-                [0.15, 0.65, 0.15], device=self.world.device, dtype=torch.float32
+                [0.15, 0.65, 0.15],
+                device=self.world.device,
+                dtype=torch.float32,
             )
             self.world.landmarks[2].color = torch.tensor(
-                [0.15, 0.15, 0.65], device=self.world.device, dtype=torch.float32
+                [0.15, 0.15, 0.65],
+                device=self.world.device,
+                dtype=torch.float32,
             )
             # special colors for goals
             self.world.agents[0].goal_a.color = self.world.agents[
                 0
             ].goal_b.color + torch.tensor(
-                [0.45, 0.45, 0.45], device=self.world.device, dtype=torch.float32
+                [0.45, 0.45, 0.45],
+                device=self.world.device,
+                dtype=torch.float32,
             )
 
         # set random initial states
         for agent in self.world.agents:
             agent.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -1.0,
                     1.0,
                 ),
                 batch_index=env_index,
             )
         for landmark in self.world.landmarks:
             landmark.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -1.0,
                     1.0,
                 ),
                 batch_index=env_index,
@@ -104,15 +118,16 @@
         is_first = agent == self.world.agents[0]
         if is_first:
             self.rew = torch.zeros(self.world.batch_dim, device=self.world.device)
             for _ in self.world.agents:
                 a = self.world.agents[0]
                 self.rew += -torch.sqrt(
                     torch.sum(
-                        torch.square(a.goal_a.state.pos - a.goal_b.state.pos), dim=-1
+                        torch.square(a.goal_a.state.pos - a.goal_b.state.pos),
+                        dim=-1,
                     )
                 )
         return self.rew
 
     def observation(self, agent):
         # goal color
         goal_color = torch.zeros(3, device=self.world.device, dtype=torch.float32)
```

### Comparing `vmas-1.4.0/vmas/scenarios/mpe/simple_spread.py` & `vmas-1.4.1/vmas/scenarios/mpe/simple_spread.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 import torch
 
 from vmas import render_interactively
 from vmas.simulator.core import Agent, Landmark, Sphere, World
@@ -40,47 +40,53 @@
 
         return world
 
     def reset_world_at(self, env_index: int = None):
         for agent in self.world.agents:
             agent.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -1.0,
                     1.0,
                 ),
                 batch_index=env_index,
             )
 
         for landmark in self.world.landmarks:
             landmark.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -1.0,
                     1.0,
                 ),
                 batch_index=env_index,
             )
 
     def reward(self, agent: Agent):
         is_first = agent == self.world.agents[0]
         if is_first:
             # Agents are rewarded based on minimum agent distance to each landmark, penalized for collisions
             self.rew = torch.zeros(
-                self.world.batch_dim, device=self.world.device, dtype=torch.float32
+                self.world.batch_dim,
+                device=self.world.device,
+                dtype=torch.float32,
             )
             for single_agent in self.world.agents:
                 for landmark in self.world.landmarks:
                     closest = torch.min(
                         torch.stack(
                             [
                                 torch.linalg.vector_norm(
```

### Comparing `vmas-1.4.0/vmas/scenarios/mpe/simple_tag.py` & `vmas-1.4.1/vmas/scenarios/mpe/simple_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 import torch
 
 from vmas import render_interactively
-from vmas.simulator.core import World, Agent, Landmark, Sphere, Line
+from vmas.simulator.core import Agent, Landmark, Line, Sphere, World
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         num_good_agents = kwargs.get("num_good_agents", 1)
@@ -63,32 +63,36 @@
 
         return world
 
     def reset_world_at(self, env_index: int = None):
         for agent in self.world.agents:
             agent.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -self.bound,
                     self.bound,
                 ),
                 batch_index=env_index,
             )
 
         for landmark in self.world.landmarks:
             landmark.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -(self.bound - 0.1),
                     self.bound - 0.1,
                 ),
                 batch_index=env_index,
@@ -236,27 +240,31 @@
                 length=2
                 * ((self.bound - self.adversary_radius) + self.adversary_radius * 2)
             ).get_geometry()
             xform = rendering.Transform()
             geom.add_attr(xform)
 
             xform.set_translation(
-                0.0
-                if i % 2
-                else (
-                    self.bound + self.adversary_radius
-                    if i == 0
-                    else -self.bound - self.adversary_radius
+                (
+                    0.0
+                    if i % 2
+                    else (
+                        self.bound + self.adversary_radius
+                        if i == 0
+                        else -self.bound - self.adversary_radius
+                    )
                 ),
-                0.0
-                if not i % 2
-                else (
-                    self.bound + self.adversary_radius
-                    if i == 1
-                    else -self.bound - self.adversary_radius
+                (
+                    0.0
+                    if not i % 2
+                    else (
+                        self.bound + self.adversary_radius
+                        if i == 1
+                        else -self.bound - self.adversary_radius
+                    )
                 ),
             )
             xform.set_rotation(torch.pi / 2 if not i % 2 else 0.0)
             color = Color.BLACK.value
             if isinstance(color, torch.Tensor) and len(color.shape) > 1:
                 color = color[env_index]
             geom.set_color(*color)
```

### Comparing `vmas-1.4.0/vmas/scenarios/mpe/simple_world_comm.py` & `vmas-1.4.1/vmas/scenarios/mpe/simple_world_comm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 import torch
 
-from vmas.simulator.core import World, Agent, Landmark, Sphere
+from vmas.simulator.core import Agent, Landmark, Sphere, World
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         world = World(
-            batch_dim=batch_dim, device=device, x_semidim=1, y_semidim=1, dim_c=4
+            batch_dim=batch_dim,
+            device=device,
+            x_semidim=1,
+            y_semidim=1,
+            dim_c=4,
         )
         num_good_agents = kwargs.get("num_good_agents", 2)
         num_adversaries = kwargs.get("num_adversaries", 4)
         num_landmarks = kwargs.get("num_landmarks", 1)
         num_food = kwargs.get("num_food", 2)
         num_forests = kwargs.get("num_forests", 2)
         num_agents = num_good_agents + num_adversaries
@@ -73,15 +77,15 @@
             world.add_landmark(landmark)
 
         return world
 
     def reset_world_at(self, env_index: int = None):
         if env_index is None:
             # random properties for agents
-            for i, agent in enumerate(self.world.agents):
+            for agent in self.world.agents:
                 agent.color = (
                     torch.tensor(
                         [0.45, 0.95, 0.45],
                         device=self.world.device,
                         dtype=torch.float32,
                     )
                     if not agent.adversary
@@ -89,56 +93,70 @@
                         [0.95, 0.45, 0.45],
                         device=self.world.device,
                         dtype=torch.float32,
                     )
                 )
                 agent.color -= (
                     torch.tensor(
-                        [0.3, 0.3, 0.3], device=self.world.device, dtype=torch.float32
+                        [0.3, 0.3, 0.3],
+                        device=self.world.device,
+                        dtype=torch.float32,
                     )
                     if agent.leader
                     else torch.tensor(
-                        [0, 0, 0], device=self.world.device, dtype=torch.float32
+                        [0, 0, 0],
+                        device=self.world.device,
+                        dtype=torch.float32,
                     )
                 )
                 # random properties for landmarks
-            for i, landmark in enumerate(self.world.landmarks):
+            for landmark in self.world.landmarks:
                 landmark.color = torch.tensor(
-                    [0.25, 0.25, 0.25], device=self.world.device, dtype=torch.float32
+                    [0.25, 0.25, 0.25],
+                    device=self.world.device,
+                    dtype=torch.float32,
                 )
-            for i, landmark in enumerate(self.world.food):
+            for landmark in self.world.food:
                 landmark.color = torch.tensor(
-                    [0.15, 0.15, 0.65], device=self.world.device, dtype=torch.float32
+                    [0.15, 0.15, 0.65],
+                    device=self.world.device,
+                    dtype=torch.float32,
                 )
-            for i, landmark in enumerate(self.world.forests):
+            for landmark in self.world.forests:
                 landmark.color = torch.tensor(
-                    [0.6, 0.9, 0.6], device=self.world.device, dtype=torch.float32
+                    [0.6, 0.9, 0.6],
+                    device=self.world.device,
+                    dtype=torch.float32,
                 )
 
         for agent in self.world.agents:
             agent.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -1.0,
                     1.0,
                 ),
                 batch_index=env_index,
             )
 
         for landmark in self.world.landmarks:
             landmark.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -0.9,
                     0.9,
                 ),
                 batch_index=env_index,
@@ -191,15 +209,16 @@
         rew -= (
             0.05
             * torch.min(
                 torch.stack(
                     [
                         torch.sqrt(
                             torch.sum(
-                                torch.square(food.state.pos - agent.state.pos), dim=-1
+                                torch.square(food.state.pos - agent.state.pos),
+                                dim=-1,
                             )
                         )
                         for food in self.world.food
                     ],
                     dim=1,
                 ),
                 dim=-1,
@@ -309,29 +328,31 @@
             -1,
             device=self.world.device,
         )
         ga = self.good_agents()
         for i, a in enumerate(ga):
             index = torch.any(
                 torch.stack(
-                    [self.is_collision(a, f) for f in self.world.forests], dim=1
+                    [self.is_collision(a, f) for f in self.world.forests],
+                    dim=1,
                 ),
                 dim=-1,
             )
             prey_forest[index][:, i] = 1
 
         # to tell leader when pred are in forest
         prey_forest = torch.full(
             (self.world.batch_dim, len(self.world.forests)),
             -1,
             device=self.world.device,
         )
         for i, f in enumerate(self.world.forests):
             index = torch.any(
-                torch.stack([self.is_collision(a, f) for a in ga], dim=1), dim=-1
+                torch.stack([self.is_collision(a, f) for a in ga], dim=1),
+                dim=-1,
             )
             prey_forest[index, i] = 1
 
         comm = self.world.agents[0].state.c
 
         if agent.adversary and not agent.leader:
             return torch.cat(
```

### Comparing `vmas-1.4.0/vmas/scenarios/multi_give_way.py` & `vmas-1.4.1/vmas/scenarios/multi_give_way.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 import typing
 from typing import List
 
 import torch
 
 from vmas import render_interactively
-from vmas.simulator.core import Agent, World, Landmark, Sphere, Line, Box
+from vmas.simulator.controllers.velocity_controller import VelocityController
+from vmas.simulator.core import Agent, Box, Landmark, Line, Sphere, World
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color, TorchUtils
-from vmas.simulator.controllers.velocity_controller import VelocityController
 
 if typing.TYPE_CHECKING:
     from vmas.simulator.rendering import Geom
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
@@ -64,17 +64,19 @@
 
         # Add agents
         for i in range(self.n_agents):
             agent = Agent(
                 name=f"agent_{i}",
                 rotatable=False,
                 linear_friction=self.linear_friction,
-                shape=Sphere(radius=self.agent_radius)
-                if not self.box_agents
-                else Box(length=self.agent_box_length, width=self.agent_box_width),
+                shape=(
+                    Sphere(radius=self.agent_radius)
+                    if not self.box_agents
+                    else Box(length=self.agent_box_length, width=self.agent_box_width)
+                ),
                 u_range=self.u_range,
                 f_range=self.f_range,
                 render_action=True,
                 color=self.colors[i],
             )
             agent.controller = VelocityController(
                 agent, world, controller_params, "standard"
@@ -149,15 +151,15 @@
                         ],
                         dtype=torch.float32,
                         device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
 
-        for i, agent in enumerate(self.world.agents):
+        for agent in self.world.agents:
             if env_index is None:
                 agent.shaping = (
                     torch.linalg.vector_norm(
                         agent.state.pos - agent.goal.state.pos, dim=1
                     )
                     * self.pos_shaping_factor
                 )
@@ -216,15 +218,16 @@
                     else -a.distance_to_goal * 0.0001
                 )
                 a.shaping = pos_shaping
 
                 self.pos_rew += a.pos_rew
 
             self.all_goal_reached = torch.all(
-                torch.stack([a.on_goal for a in self.world.agents], dim=-1), dim=-1
+                torch.stack([a.on_goal for a in self.world.agents], dim=-1),
+                dim=-1,
             )
 
             self.final_rew[self.all_goal_reached] = self.final_reward
             self.reached_goal += self.all_goal_reached
 
         agent.agent_collision_rew[:] = 0
         # agent.obstacle_collision_rew = torch.zeros(
@@ -269,18 +272,15 @@
                 agent.state.pos - agent.goal.state.pos,
                 dim=-1,
             ).unsqueeze(-1),
         ]
 
         if self.obs_noise > 0:
             for i, obs in enumerate(observations):
-                noise = torch.zeros(
-                    *obs.shape,
-                    device=self.world.device,
-                ).uniform_(
+                noise = torch.zeros(*obs.shape, device=self.world.device,).uniform_(
                     -self.obs_noise,
                     self.obs_noise,
                 )
                 observations[i] = obs + noise
         return torch.cat(
             observations,
             dim=-1,
@@ -354,17 +354,19 @@
 
     def reset_map(self, env_index):
         for i, landmark in enumerate(self.short_walls):
             if i < 2:
                 landmark.set_pos(
                     torch.tensor(
                         [
-                            -self.scenario_length / 2
-                            if i % 2 == 0
-                            else self.scenario_length / 2,
+                            (
+                                -self.scenario_length / 2
+                                if i % 2 == 0
+                                else self.scenario_length / 2
+                            ),
                             0.0,
                         ],
                         dtype=torch.float32,
                         device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
@@ -377,17 +379,19 @@
                     batch_index=env_index,
                 )
             else:
                 landmark.set_pos(
                     torch.tensor(
                         [
                             0.0,
-                            -self.scenario_length / 2
-                            if i % 2 == 0
-                            else self.scenario_length / 2,
+                            (
+                                -self.scenario_length / 2
+                                if i % 2 == 0
+                                else self.scenario_length / 2
+                            ),
                         ],
                         dtype=torch.float32,
                         device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
```

### Comparing `vmas-1.4.0/vmas/scenarios/navigation.py` & `vmas-1.4.1/vmas/scenarios/navigation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 import typing
-from typing import Dict, Callable, List
+from typing import Callable, Dict, List
 
 import torch
 from torch import Tensor
 
 from vmas import render_interactively
-from vmas.simulator.core import Agent, Landmark, World, Sphere, Entity
+from vmas.simulator.core import Agent, Entity, Landmark, Sphere, World
 from vmas.simulator.heuristic_policy import BaseHeuristicPolicy
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.sensors import Lidar
 from vmas.simulator.utils import Color, ScenarioUtils, X, Y
 
 if typing.TYPE_CHECKING:
     from vmas.simulator.rendering import Geom
@@ -84,24 +84,26 @@
             # Constraint: all agents have same action range and multiplier
             agent = Agent(
                 name=f"agent_{i}",
                 collide=self.collisions,
                 color=color,
                 shape=Sphere(radius=self.agent_radius),
                 render_action=True,
-                sensors=[
-                    Lidar(
-                        world,
-                        n_rays=12,
-                        max_range=self.lidar_range,
-                        entity_filter=entity_filter_agents,
-                    ),
-                ]
-                if self.collisions
-                else None,
+                sensors=(
+                    [
+                        Lidar(
+                            world,
+                            n_rays=12,
+                            max_range=self.lidar_range,
+                            entity_filter=entity_filter_agents,
+                        ),
+                    ]
+                    if self.collisions
+                    else None
+                ),
             )
             agent.pos_rew = torch.zeros(batch_dim, device=device)
             agent.agent_collision_rew = agent.pos_rew.clone()
             world.add_agent(agent)
 
             # Add goals
             goal = Landmark(
@@ -178,15 +180,16 @@
             self.final_rew[:] = 0
 
             for a in self.world.agents:
                 self.pos_rew += self.agent_reward(a)
                 a.agent_collision_rew[:] = 0
 
             self.all_goal_reached = torch.all(
-                torch.stack([a.on_goal for a in self.world.agents], dim=-1), dim=-1
+                torch.stack([a.on_goal for a in self.world.agents], dim=-1),
+                dim=-1,
             )
 
             self.final_rew[self.all_goal_reached] = self.final_reward
 
             for i, a in enumerate(self.world.agents):
                 for j, b in enumerate(self.world.agents):
                     if i <= j:
@@ -361,19 +364,25 @@
             lfV_param + lgV_params @ u + self.clf_epsilon * V_param + clf_slack <= 0
         ]
 
         QP_problem = cp.Problem(qp_objective, constraints)
 
         # Initialize CVXPY layers
         QP_controller = CvxpyLayer(
-            QP_problem, parameters=[V_param, lfV_param, lgV_params], variables=[u]
+            QP_problem,
+            parameters=[V_param, lfV_param, lgV_params],
+            variables=[u],
         )
 
         # Solve QP
-        CVXpylayer_parameters = [V_value.unsqueeze(1), LfV_val.unsqueeze(1), LgV_vals]
+        CVXpylayer_parameters = [
+            V_value.unsqueeze(1),
+            LfV_val.unsqueeze(1),
+            LgV_vals,
+        ]
         action = QP_controller(*CVXpylayer_parameters, solver_args={"max_iters": 500})[
             0
         ]
 
         return action
```

### Comparing `vmas-1.4.0/vmas/scenarios/passage.py` & `vmas-1.4.1/vmas/scenarios/passage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 import torch
 
 from vmas import render_interactively
-from vmas.simulator.core import Agent, Box, Landmark, Sphere, World, Line
+from vmas.simulator.core import Agent, Box, Landmark, Line, Sphere, World
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         self.n_passages = kwargs.get("n_passages", 1)
@@ -26,15 +26,17 @@
         self.passage_length = 0.103
 
         # Make world
         world = World(batch_dim, device, x_semidim=1, y_semidim=1)
         # Add agents
         for i in range(self.n_agents):
             agent = Agent(
-                name=f"agent_{i}", shape=Sphere(self.agent_radius), u_multiplier=0.7
+                name=f"agent_{i}",
+                shape=Sphere(self.agent_radius),
+                u_multiplier=0.7,
             )
             world.add_agent(agent)
             goal = Landmark(
                 name=f"goal {i}",
                 collide=False,
                 shape=Sphere(radius=self.agent_radius),
                 color=Color.LIGHT_GREEN,
@@ -115,27 +117,31 @@
                 )
             else:
                 goal.set_pos(
                     central_goal_pos
                     + torch.tensor(
                         [
                             [
-                                0.0
-                                if i % 2
-                                else (
-                                    self.agent_spacing
-                                    if i == 0
-                                    else -self.agent_spacing
+                                (
+                                    0.0
+                                    if i % 2
+                                    else (
+                                        self.agent_spacing
+                                        if i == 0
+                                        else -self.agent_spacing
+                                    )
                                 ),
-                                0.0
-                                if not i % 2
-                                else (
-                                    self.agent_spacing
-                                    if i == 1
-                                    else -self.agent_spacing
+                                (
+                                    0.0
+                                    if not i % 2
+                                    else (
+                                        self.agent_spacing
+                                        if i == 1
+                                        else -self.agent_spacing
+                                    )
                                 ),
                             ],
                         ],
                         device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
@@ -147,27 +153,31 @@
                 )
             else:
                 agent.set_pos(
                     central_agent_pos
                     + torch.tensor(
                         [
                             [
-                                0.0
-                                if i % 2
-                                else (
-                                    self.agent_spacing
-                                    if i == 0
-                                    else -self.agent_spacing
+                                (
+                                    0.0
+                                    if i % 2
+                                    else (
+                                        self.agent_spacing
+                                        if i == 0
+                                        else -self.agent_spacing
+                                    )
                                 ),
-                                0.0
-                                if not i % 2
-                                else (
-                                    self.agent_spacing
-                                    if i == 1
-                                    else -self.agent_spacing
+                                (
+                                    0.0
+                                    if not i % 2
+                                    else (
+                                        self.agent_spacing
+                                        if i == 1
+                                        else -self.agent_spacing
+                                    )
                                 ),
                             ],
                         ],
                         device=self.world.device,
                     ),
                     batch_index=env_index,
                 )
@@ -208,26 +218,30 @@
 
     def reward(self, agent: Agent):
         is_first = agent == self.world.agents[0]
 
         if self.shared_reward:
             if is_first:
                 self.rew = torch.zeros(
-                    self.world.batch_dim, device=self.world.device, dtype=torch.float32
+                    self.world.batch_dim,
+                    device=self.world.device,
+                    dtype=torch.float32,
                 )
                 for a in self.world.agents:
                     dist_to_goal = torch.linalg.vector_norm(
                         a.state.pos - a.goal.state.pos, dim=1
                     )
                     agent_shaping = dist_to_goal * self.shaping_factor
                     self.rew += a.global_shaping - agent_shaping
                     a.global_shaping = agent_shaping
         else:
             self.rew = torch.zeros(
-                self.world.batch_dim, device=self.world.device, dtype=torch.float32
+                self.world.batch_dim,
+                device=self.world.device,
+                dtype=torch.float32,
             )
             dist_to_goal = torch.linalg.vector_norm(
                 agent.state.pos - agent.goal.state.pos, dim=1
             )
             agent_shaping = dist_to_goal * self.shaping_factor
             self.rew += agent.global_shaping - agent_shaping
             agent.global_shaping = agent_shaping
@@ -278,27 +292,31 @@
         geoms = []
         for i in range(4):
             geom = Line(length=2 + self.agent_radius * 2).get_geometry()
             xform = rendering.Transform()
             geom.add_attr(xform)
 
             xform.set_translation(
-                0.0
-                if i % 2
-                else (
-                    self.world.x_semidim + self.agent_radius
-                    if i == 0
-                    else -self.world.x_semidim - self.agent_radius
+                (
+                    0.0
+                    if i % 2
+                    else (
+                        self.world.x_semidim + self.agent_radius
+                        if i == 0
+                        else -self.world.x_semidim - self.agent_radius
+                    )
                 ),
-                0.0
-                if not i % 2
-                else (
-                    self.world.x_semidim + self.agent_radius
-                    if i == 1
-                    else -self.world.x_semidim - self.agent_radius
+                (
+                    0.0
+                    if not i % 2
+                    else (
+                        self.world.x_semidim + self.agent_radius
+                        if i == 1
+                        else -self.world.x_semidim - self.agent_radius
+                    )
                 ),
             )
             xform.set_rotation(torch.pi / 2 if not i % 2 else 0.0)
             color = Color.BLACK.value
             if isinstance(color, torch.Tensor) and len(color.shape) > 1:
                 color = color[env_index]
             geom.set_color(*color)
```

### Comparing `vmas-1.4.0/vmas/scenarios/reverse_transport.py` & `vmas-1.4.1/vmas/scenarios/reverse_transport.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,19 @@
         self.package_length = kwargs.get("package_length", 0.6)
         self.package_mass = kwargs.get("package_mass", 50)
 
         self.shaping_factor = 100
 
         # Make world
         world = World(
-            batch_dim, device, contact_margin=6e-3, substeps=5, collision_force=500
+            batch_dim,
+            device,
+            contact_margin=6e-3,
+            substeps=5,
+            collision_force=500,
         )
         # Add agents
         for i in range(n_agents):
             agent = Agent(name=f"agent_{i}", shape=Sphere(0.03), u_multiplier=0.5)
             world.add_agent(agent)
         # Add landmarks
         goal = Landmark(
@@ -37,59 +41,67 @@
         )
         world.add_landmark(goal)
 
         self.package = Landmark(
             name=f"package {i}",
             collide=True,
             movable=True,
-            mass=50,
+            mass=self.package_mass,
             shape=Box(
-                length=self.package_length, width=self.package_width, hollow=True
+                length=self.package_length,
+                width=self.package_width,
+                hollow=True,
             ),
             color=Color.RED,
         )
         self.package.goal = goal
         world.add_landmark(self.package)
 
         return world
 
     def reset_world_at(self, env_index: int = None):
         package_pos = torch.zeros(
-            (1, self.world.dim_p)
-            if env_index is not None
-            else (self.world.batch_dim, self.world.dim_p),
+            (
+                (1, self.world.dim_p)
+                if env_index is not None
+                else (self.world.batch_dim, self.world.dim_p)
+            ),
             device=self.world.device,
             dtype=torch.float32,
         ).uniform_(
             -1.0,
             1.0,
         )
 
         self.package.set_pos(
             package_pos,
             batch_index=env_index,
         )
-        for i, agent in enumerate(self.world.agents):
+        for agent in self.world.agents:
             agent.set_pos(
                 torch.cat(
                     [
                         torch.zeros(
-                            (1, 1)
-                            if env_index is not None
-                            else (self.world.batch_dim, 1),
+                            (
+                                (1, 1)
+                                if env_index is not None
+                                else (self.world.batch_dim, 1)
+                            ),
                             device=self.world.device,
                             dtype=torch.float32,
                         ).uniform_(
                             -self.package_length / 2 + agent.shape.radius,
                             self.package_length / 2 - agent.shape.radius,
                         ),
                         torch.zeros(
-                            (1, 1)
-                            if env_index is not None
-                            else (self.world.batch_dim, 1),
+                            (
+                                (1, 1)
+                                if env_index is not None
+                                else (self.world.batch_dim, 1)
+                            ),
                             device=self.world.device,
                             dtype=torch.float32,
                         ).uniform_(
                             -self.package_width / 2 + agent.shape.radius,
                             self.package_width / 2 - agent.shape.radius,
                         ),
                     ],
@@ -97,17 +109,19 @@
                 )
                 + package_pos,
                 batch_index=env_index,
             )
 
         self.package.goal.set_pos(
             torch.zeros(
-                (1, self.world.dim_p)
-                if env_index is not None
-                else (self.world.batch_dim, self.world.dim_p),
+                (
+                    (1, self.world.dim_p)
+                    if env_index is not None
+                    else (self.world.batch_dim, self.world.dim_p)
+                ),
                 device=self.world.device,
                 dtype=torch.float32,
             ).uniform_(
                 -1.0,
                 1.0,
             ),
             batch_index=env_index,
@@ -117,15 +131,17 @@
             self.package.global_shaping = (
                 torch.linalg.vector_norm(
                     self.package.state.pos - self.package.goal.state.pos, dim=1
                 )
                 * self.shaping_factor
             )
             self.package.on_goal = torch.zeros(
-                self.world.batch_dim, dtype=torch.bool, device=self.world.device
+                self.world.batch_dim,
+                dtype=torch.bool,
+                device=self.world.device,
             )
         else:
             self.package.global_shaping[env_index] = (
                 torch.linalg.vector_norm(
                     self.package.state.pos[env_index]
                     - self.package.goal.state.pos[env_index]
                 )
@@ -134,28 +150,32 @@
             self.package.on_goal[env_index] = False
 
     def reward(self, agent: Agent):
         is_first = agent == self.world.agents[0]
 
         if is_first:
             self.rew = torch.zeros(
-                self.world.batch_dim, device=self.world.device, dtype=torch.float32
+                self.world.batch_dim,
+                device=self.world.device,
+                dtype=torch.float32,
             )
 
             self.package.dist_to_goal = torch.linalg.vector_norm(
                 self.package.state.pos - self.package.goal.state.pos, dim=1
             )
             self.package.on_goal = self.world.is_overlapping(
                 self.package, self.package.goal
             )
             self.package.color = torch.tensor(
                 Color.RED.value, device=self.world.device, dtype=torch.float32
             ).repeat(self.world.batch_dim, 1)
             self.package.color[self.package.on_goal] = torch.tensor(
-                Color.GREEN.value, device=self.world.device, dtype=torch.float32
+                Color.GREEN.value,
+                device=self.world.device,
+                dtype=torch.float32,
             )
 
             package_shaping = self.package.dist_to_goal * self.shaping_factor
             self.rew[~self.package.on_goal] += (
                 self.package.global_shaping[~self.package.on_goal]
                 - package_shaping[~self.package.on_goal]
             )
```

### Comparing `vmas-1.4.0/vmas/scenarios/sampling.py` & `vmas-1.4.1/vmas/scenarios/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #  Copyright (c) 2023-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
-from typing import Dict, Callable
+from typing import Callable, Dict
 
 import torch
 from torch import Tensor
 from torch.distributions import MultivariateNormal
+
 from vmas import render_interactively
-from vmas.simulator.core import World, Line, Agent, Sphere, Entity
+from vmas.simulator.core import Agent, Entity, Line, Sphere, World
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.sensors import Lidar
 from vmas.simulator.utils import Color, X, Y
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
@@ -61,26 +62,28 @@
         entity_filter_agents: Callable[[Entity], bool] = lambda e: isinstance(e, Agent)
         for i in range(self.n_agents):
             agent = Agent(
                 name=f"agent_{i}",
                 render_action=True,
                 collide=self.collisions,
                 shape=Sphere(radius=self.agent_radius),
-                sensors=[
-                    Lidar(
-                        world,
-                        angle_start=0.05,
-                        angle_end=2 * torch.pi + 0.05,
-                        n_rays=12,
-                        max_range=self.lidar_range,
-                        entity_filter=entity_filter_agents,
-                    ),
-                ]
-                if self.collisions
-                else None,
+                sensors=(
+                    [
+                        Lidar(
+                            world,
+                            angle_start=0.05,
+                            angle_end=2 * torch.pi + 0.05,
+                            n_rays=12,
+                            max_range=self.lidar_range,
+                            entity_filter=entity_filter_agents,
+                        ),
+                    ]
+                    if self.collisions
+                    else None
+                ),
             )
 
             world.add_agent(agent)
 
         self.sampled = torch.zeros(
             (batch_dim, self.n_x_cells, self.n_y_cells),
             device=device,
@@ -97,15 +100,15 @@
             ).expand(batch_dim, world.dim_p, world.dim_p)
             for cov in self.covs
         ]
 
         return world
 
     def reset_world_at(self, env_index: int = None):
-        for i, loc in enumerate(self.locs):
+        for i in range(len(self.locs)):
             x = torch.zeros(
                 (1,) if env_index is not None else (self.world.batch_dim, 1),
                 device=self.world.device,
                 dtype=torch.float32,
             ).uniform_(-self.xdim, self.xdim)
             y = torch.zeros(
                 (1,) if env_index is not None else (self.world.batch_dim, 1),
@@ -135,24 +138,28 @@
         self.nomrlize_pdf(env_index=env_index)
 
         for agent in self.world.agents:
             agent.set_pos(
                 torch.cat(
                     [
                         torch.zeros(
-                            (1, 1)
-                            if env_index is not None
-                            else (self.world.batch_dim, 1),
+                            (
+                                (1, 1)
+                                if env_index is not None
+                                else (self.world.batch_dim, 1)
+                            ),
                             device=self.world.device,
                             dtype=torch.float32,
                         ).uniform_(-self.agent_xspawn_range, self.agent_xspawn_range),
                         torch.zeros(
-                            (1, 1)
-                            if env_index is not None
-                            else (self.world.batch_dim, 1),
+                            (
+                                (1, 1)
+                                if env_index is not None
+                                else (self.world.batch_dim, 1)
+                            ),
                             device=self.world.device,
                             dtype=torch.float32,
                         ).uniform_(-self.agent_yspawn_range, self.agent_yspawn_range),
                     ],
                     dim=-1,
                 ),
                 batch_index=env_index,
@@ -175,15 +182,16 @@
         pos[:, Y].clamp_(-self.world.y_semidim, self.world.y_semidim)
 
         index = pos / self.grid_spacing
         index[:, X] += self.n_x_cells / 2
         index[:, Y] += self.n_y_cells / 2
         index = index.to(torch.long)
         v = torch.stack(
-            [gaussian.log_prob(pos).exp() for gaussian in self.gaussians], dim=-1
+            [gaussian.log_prob(pos).exp() for gaussian in self.gaussians],
+            dim=-1,
         ).sum(-1)
         if norm:
             v = v / self.max_pdf
 
         sampled = self.sampled[
             torch.arange(self.world.batch_dim), index[:, 0], index[:, 1]
         ]
@@ -217,15 +225,16 @@
         index[:, X] += self.n_x_cells / 2
         index[:, Y] += self.n_y_cells / 2
         index = index.to(torch.long)
 
         pos = pos.unsqueeze(1).expand(pos.shape[0], self.world.batch_dim, 2)
 
         v = torch.stack(
-            [gaussian.log_prob(pos).exp() for gaussian in self.gaussians], dim=-1
+            [gaussian.log_prob(pos).exp() for gaussian in self.gaussians],
+            dim=-1,
         ).sum(-1)[:, env_index]
         if norm:
             v = v / self.max_pdf[env_index]
 
         sampled = self.sampled[env_index, index[:, 0], index[:, 1]]
 
         v[sampled + out_of_bounds] = 0
@@ -263,15 +272,19 @@
             self.sampling_rew = torch.stack(
                 [a.sample for a in self.world.agents], dim=-1
             ).sum(-1)
 
         return self.sampling_rew if self.shared_rew else agent.sample
 
     def observation(self, agent: Agent) -> Tensor:
-        observations = [agent.state.pos, agent.state.vel, agent.sensors[0].measure()]
+        observations = [
+            agent.state.pos,
+            agent.state.vel,
+            agent.sensors[0].measure(),
+        ]
 
         for delta in [
             [self.grid_spacing, 0],
             [-self.grid_spacing, 0],
             [0, self.grid_spacing],
             [0, -self.grid_spacing],
             [-self.grid_spacing, -self.grid_spacing],
@@ -349,27 +362,31 @@
                 * ((self.ydim if i % 2 == 0 else self.xdim) - self.agent_radius)
                 + self.agent_radius * 2
             ).get_geometry()
             xform = rendering.Transform()
             geom.add_attr(xform)
 
             xform.set_translation(
-                0.0
-                if i % 2
-                else (
-                    self.x_semidim + self.agent_radius
-                    if i == 0
-                    else -self.x_semidim - self.agent_radius
+                (
+                    0.0
+                    if i % 2
+                    else (
+                        self.x_semidim + self.agent_radius
+                        if i == 0
+                        else -self.x_semidim - self.agent_radius
+                    )
                 ),
-                0.0
-                if not i % 2
-                else (
-                    self.y_semidim + self.agent_radius
-                    if i == 1
-                    else -self.y_semidim - self.agent_radius
+                (
+                    0.0
+                    if not i % 2
+                    else (
+                        self.y_semidim + self.agent_radius
+                        if i == 1
+                        else -self.y_semidim - self.agent_radius
+                    )
                 ),
             )
             xform.set_rotation(torch.pi / 2 if not i % 2 else 0.0)
             color = Color.BLACK.value
             if isinstance(color, torch.Tensor) and len(color.shape) > 1:
                 color = color[env_index]
             geom.set_color(*color)
```

### Comparing `vmas-1.4.0/vmas/scenarios/transport.py` & `vmas-1.4.1/vmas/scenarios/transport.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,17 @@
             y_semidim=self.world_semidim
             + 2 * self.agent_radius
             + max(self.package_length, self.package_width),
         )
         # Add agents
         for i in range(n_agents):
             agent = Agent(
-                name=f"agent_{i}", shape=Sphere(self.agent_radius), u_multiplier=0.6
+                name=f"agent_{i}",
+                shape=Sphere(self.agent_radius),
+                u_multiplier=0.6,
             )
             world.add_agent(agent)
         # Add landmarks
         goal = Landmark(
             name="goal",
             collide=False,
             shape=Sphere(radius=0.15),
@@ -50,15 +52,15 @@
         world.add_landmark(goal)
         self.packages = []
         for i in range(self.n_packages):
             package = Landmark(
                 name=f"package {i}",
                 collide=True,
                 movable=True,
-                mass=50,
+                mass=self.package_mass,
                 shape=Box(length=self.package_length, width=self.package_width),
                 color=Color.RED,
             )
             package.goal = goal
             self.packages.append(package)
             world.add_landmark(package)
 
@@ -102,15 +104,15 @@
             y_bounds=(
                 -self.world_semidim,
                 self.world_semidim,
             ),
             occupied_positions=agent_occupied_positions,
         )
 
-        for i, package in enumerate(self.packages):
+        for package in self.packages:
             package.on_goal = self.world.is_overlapping(package, package.goal)
 
             if env_index is None:
                 package.global_shaping = (
                     torch.linalg.vector_norm(
                         package.state.pos - package.goal.state.pos, dim=1
                     )
@@ -125,27 +127,33 @@
                 )
 
     def reward(self, agent: Agent):
         is_first = agent == self.world.agents[0]
 
         if is_first:
             self.rew = torch.zeros(
-                self.world.batch_dim, device=self.world.device, dtype=torch.float32
+                self.world.batch_dim,
+                device=self.world.device,
+                dtype=torch.float32,
             )
 
-            for i, package in enumerate(self.packages):
+            for package in self.packages:
                 package.dist_to_goal = torch.linalg.vector_norm(
                     package.state.pos - package.goal.state.pos, dim=1
                 )
                 package.on_goal = self.world.is_overlapping(package, package.goal)
                 package.color = torch.tensor(
-                    Color.RED.value, device=self.world.device, dtype=torch.float32
+                    Color.RED.value,
+                    device=self.world.device,
+                    dtype=torch.float32,
                 ).repeat(self.world.batch_dim, 1)
                 package.color[package.on_goal] = torch.tensor(
-                    Color.GREEN.value, device=self.world.device, dtype=torch.float32
+                    Color.GREEN.value,
+                    device=self.world.device,
+                    dtype=torch.float32,
                 )
 
                 package_shaping = package.dist_to_goal * self.shaping_factor
                 self.rew[~package.on_goal] += (
                     package.global_shaping[~package.on_goal]
                     - package_shaping[~package.on_goal]
                 )
@@ -196,15 +204,15 @@
         self.dribble_slowdown_dist = 0.0
         self.speed = 0.95
 
     def compute_action(self, observation: torch.Tensor, u_range: float) -> torch.Tensor:
         self.n_env = observation.shape[0]
         self.device = observation.device
         agent_pos = observation[:, :2]
-        agent_vel = observation[:, 2:4]
+        # agent_vel = observation[:, 2:4]
         package_pos = observation[:, 6:8] + agent_pos
         goal_pos = -observation[:, 4:6] + package_pos
         # control = self.get_action(goal_pos, curr_pos=agent_pos, curr_vel=agent_vel)
         control = self.dribble(agent_pos, package_pos, goal_pos)
         control *= self.speed * u_range
         return torch.clamp(control, -u_range, u_range)
```

### Comparing `vmas-1.4.0/vmas/scenarios/wheel.py` & `vmas-1.4.1/vmas/scenarios/wheel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 import torch
 
 from vmas import render_interactively
-from vmas.simulator.core import Agent, Landmark, World, Line, Sphere
+from vmas.simulator.core import Agent, Landmark, Line, Sphere, World
 from vmas.simulator.heuristic_policy import BaseHeuristicPolicy
 from vmas.simulator.scenario import BaseScenario
 from vmas.simulator.utils import Color, TorchUtils
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
@@ -46,17 +46,19 @@
         return world
 
     def reset_world_at(self, env_index: int = None):
         for agent in self.world.agents:
             # Random pos between -1 and 1
             agent.set_pos(
                 torch.zeros(
-                    (1, self.world.dim_p)
-                    if env_index is not None
-                    else (self.world.batch_dim, self.world.dim_p),
+                    (
+                        (1, self.world.dim_p)
+                        if env_index is not None
+                        else (self.world.batch_dim, self.world.dim_p)
+                    ),
                     device=self.world.device,
                     dtype=torch.float32,
                 ).uniform_(
                     -1.0,
                     1.0,
                 ),
                 batch_index=env_index,
```

### Comparing `vmas-1.4.0/vmas/scenarios/wind_flocking.py` & `vmas-1.4.1/vmas/scenarios/wind_flocking.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 import typing
 from typing import Dict, List
 
 import torch
 from torch import Tensor
+
 from vmas import render_interactively
-from vmas.simulator.core import Agent, World, Sphere
-from vmas.simulator.scenario import BaseScenario
-from vmas.simulator.utils import Y, Color, X
 from vmas.simulator.controllers.velocity_controller import VelocityController
+from vmas.simulator.core import Agent, Sphere, World
+from vmas.simulator.scenario import BaseScenario
+from vmas.simulator.utils import Color, X, Y
 
 if typing.TYPE_CHECKING:
     from vmas.simulator.rendering import Geom
 
 
 def angle_to_vector(angle):
     return torch.cat([torch.cos(angle), torch.sin(angle)], dim=1)
@@ -39,15 +40,16 @@
 
 def get_line_angle_dist_0_180(angle, goal):
     angle = get_line_angle_0_180(angle)
     goal = get_line_angle_0_180(goal)
     return torch.minimum(
         (angle - goal).abs(),
         torch.minimum(
-            (angle - (goal - torch.pi)).abs(), ((angle - torch.pi) - goal).abs()
+            (angle - (goal - torch.pi)).abs(),
+            ((angle - torch.pi) - goal).abs(),
         ),
     ).squeeze(-1)
 
 
 class Scenario(BaseScenario):
     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
         self.plot_grid = True
@@ -174,15 +176,17 @@
 
             if env_index is None:
                 agent.vel_shaping = (
                     torch.linalg.vector_norm(agent.state.vel - self.desired_vel, dim=-1)
                     * self.vel_shaping_factor
                 )
                 agent.energy_shaping = torch.zeros(
-                    self.world.batch_dim, device=self.world.device, dtype=torch.float32
+                    self.world.batch_dim,
+                    device=self.world.device,
+                    dtype=torch.float32,
                 )
                 agent.wind_shaping = (
                     torch.linalg.vector_norm(agent.gravity, dim=-1)
                     * self.wind_shaping_factor
                 )
 
             else:
@@ -200,23 +204,25 @@
 
         if env_index is None:
             self.t = torch.zeros(
                 self.world.batch_dim, device=self.world.device, dtype=torch.int
             )
             self.distance_shaping = (
                 torch.linalg.vector_norm(
-                    self.small_agent.state.pos - self.big_agent.state.pos, dim=-1
+                    self.small_agent.state.pos - self.big_agent.state.pos,
+                    dim=-1,
                 )
                 - self.desired_distance
             ).abs() * self.dist_shaping_factor
 
             self.pos_shaping = (
                 (
                     torch.maximum(
-                        self.big_agent.state.pos[:, Y], self.small_agent.state.pos[:, Y]
+                        self.big_agent.state.pos[:, Y],
+                        self.small_agent.state.pos[:, Y],
                     )
                     - self.desired_pos
                 ).abs()
             ) * self.pos_shaping_factor
 
             self.rot_shaping = (
                 get_line_angle_dist_0_180(self.get_agents_angle(), 0)
@@ -258,15 +264,16 @@
         if is_first:
             self.t += 1
             self.set_friction()
 
             # Dist reward
             distance_shaping = (
                 torch.linalg.vector_norm(
-                    self.small_agent.state.pos - self.big_agent.state.pos, dim=-1
+                    self.small_agent.state.pos - self.big_agent.state.pos,
+                    dim=-1,
                 )
                 - self.desired_distance
             ).abs() * self.dist_shaping_factor
             self.dist_rew = self.distance_shaping - distance_shaping
             self.distance_shaping = distance_shaping
 
             # Rot shaping
@@ -280,15 +287,16 @@
             self.rot_rew = self.rot_shaping - rot_shaping
             self.rot_shaping = rot_shaping
 
             # Pos reward
             pos_shaping = (
                 (
                     torch.maximum(
-                        self.big_agent.state.pos[:, Y], self.small_agent.state.pos[:, Y]
+                        self.big_agent.state.pos[:, Y],
+                        self.small_agent.state.pos[:, Y],
                     )
                     - self.desired_pos
                 ).abs()
             ) * self.pos_shaping_factor
             self.pos_rew = self.pos_shaping - pos_shaping
             self.pos_shaping = pos_shaping
```

### Comparing `vmas-1.4.0/vmas/simulator/controllers/velocity_controller.py` & `vmas-1.4.1/vmas/simulator/controllers/velocity_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 import math
 import warnings
-from typing import Union
+from typing import Optional
 
 import torch
-from torch import Tensor
 
 import vmas.simulator.core
 import vmas.simulator.utils
+from vmas.simulator.utils import TorchUtils
 
 
 class VelocityController:
     """
     Implements PID controller for velocity targets found in agent.action.u.
     Two forms of the PID controller are implemented: standard, and parallel. The controller takes 3 params, which
     are interpreted differently based on the form.
@@ -26,15 +26,15 @@
                         intg_ts = kP/kI and kD/kP = derv_ts
     """
 
     def __init__(
         self,
         agent: vmas.simulator.core.Agent,
         world: vmas.simulator.core.World,
-        ctrl_params=[1, 0, 0],
+        ctrl_params=(1, 0, 0),
         pid_form="standard",
     ):
         self.agent = agent
         self.world = world
         self.dt = world.dt
         # controller parameters: standard=[kP, intgTs ,dervTs], parallel=[kP, kI, kD]
         #    in parallel form, kI = kP/intgTs and kD = kP*dervTs
@@ -67,31 +67,29 @@
                 self.integrator_windup_cutoff = (
                     0.5 * fmax * self.integralTs / (self.dt * self.ctrl_gain)
                 )
             else:
                 self.integrator_windup_cutoff = None
                 warnings.warn("Force limits not specified. Integrator can wind up!")
 
-        # containers for integral & derivative control
-        self.accum_errs = torch.zeros(
-            (world.batch_dim, world.dim_p), device=world.device
-        )
-        self.prev_err = torch.zeros((world.batch_dim, world.dim_p), device=world.device)
+        self.reset()
 
-    def reset(self, index: Union[Tensor, int] = None):
+    def reset(self, index: Optional[int] = None):
         if index is None:
             self.accum_errs = torch.zeros(
-                (self.world.batch_dim, self.world.dim_p), device=self.world.device
+                (self.world.batch_dim, self.world.dim_p),
+                device=self.world.device,
             )
             self.prev_err = torch.zeros(
-                (self.world.batch_dim, self.world.dim_p), device=self.world.device
+                (self.world.batch_dim, self.world.dim_p),
+                device=self.world.device,
             )
         else:
-            self.accum_errs[index] = 0.0
-            self.prev_err[index] = 0.0
+            self.accum_errs = TorchUtils.where_from_index(index, 0.0, self.accum_errs)
+            self.prev_err = TorchUtils.where_from_index(index, 0.0, self.prev_err)
 
     def integralError(self, err):
         if not self.use_integrator:
             return 0
         # fixed-length history (not recommended):
         # if len( self.accum_errs ) > self.integrator_hist-1:
         #    self.accum_errs.pop(0);
```

### Comparing `vmas-1.4.0/vmas/simulator/core.py` & `vmas-1.4.1/vmas/simulator/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,44 +3,44 @@
 #  All rights reserved.
 
 from __future__ import annotations
 
 import math
 import typing
 from abc import ABC, abstractmethod
-from typing import Callable, List, Tuple, Union, Sequence
+from typing import Callable, List, Sequence, Tuple, Union
 
 import torch
 from torch import Tensor
 
 from vmas.simulator.dynamics.common import Dynamics
 from vmas.simulator.dynamics.holonomic import Holonomic
 from vmas.simulator.joints import Joint
 from vmas.simulator.physics import (
-    _get_closest_point_line,
-    _get_closest_point_box,
-    _get_closest_line_box,
     _get_closest_box_box,
+    _get_closest_line_box,
+    _get_closest_point_box,
+    _get_closest_point_line,
     _get_closest_points_line_line,
     _get_inner_point_box,
 )
 from vmas.simulator.sensors import Sensor
 from vmas.simulator.utils import (
-    Color,
-    X,
-    Y,
-    override,
-    LINE_MIN_DIST,
+    ANGULAR_FRICTION,
     COLLISION_FORCE,
-    JOINT_FORCE,
-    Observable,
+    Color,
     DRAG,
+    JOINT_FORCE,
+    LINE_MIN_DIST,
     LINEAR_FRICTION,
-    ANGULAR_FRICTION,
+    Observable,
+    override,
     TorchUtils,
+    X,
+    Y,
 )
 
 if typing.TYPE_CHECKING:
     from vmas.simulator.rendering import Geom
 
 
 class TorchVectorizedObject(object):
@@ -278,20 +278,30 @@
         assert (
             rot.shape[0] == self._batch_dim
         ), f"Internal state must match batch dim, got {rot.shape[0]}, expected {self._batch_dim}"
 
         self._rot = rot.to(self._device)
 
     def _reset(self, env_index: typing.Optional[int]):
-        for attr in [self.pos, self.rot, self.vel, self.ang_vel]:
+        for attr_name in ["pos", "rot", "vel", "ang_vel"]:
+            attr = self.__getattribute__(attr_name)
             if attr is not None:
                 if env_index is None:
-                    attr[:] = 0.0
+                    self.__setattr__(attr_name, torch.zeros_like(attr))
                 else:
-                    attr[env_index] = 0.0
+                    self.__setattr__(
+                        attr_name,
+                        TorchUtils.where_from_index(env_index, 0, attr),
+                    )
+
+    def zero_grad(self):
+        for attr_name in ["pos", "rot", "vel", "ang_vel"]:
+            attr = self.__getattribute__(attr_name)
+            if attr is not None:
+                self.__setattr__(attr_name, attr.detach())
 
     def _spawn(self, dim_c: int, dim_p: int):
         self.pos = torch.zeros(
             self.batch_dim, dim_p, device=self.device, dtype=torch.float32
         )
         self.vel = torch.zeros(
             self.batch_dim, dim_p, device=self.device, dtype=torch.float32
@@ -359,23 +369,35 @@
             value.shape[0] == self._batch_dim
         ), f"Internal state must match batch dim, got {value.shape[0]}, expected {self._batch_dim}"
 
         self._torque = value.to(self._device)
 
     @override(EntityState)
     def _reset(self, env_index: typing.Optional[int]):
-        for attr in [self.c, self.force, self.torque]:
+        for attr_name in ["c", "force", "torque"]:
+            attr = self.__getattribute__(attr_name)
             if attr is not None:
                 if env_index is None:
-                    attr[:] = 0.0
+                    self.__setattr__(attr_name, torch.zeros_like(attr))
                 else:
-                    attr[env_index] = 0.0
+                    self.__setattr__(
+                        attr_name,
+                        TorchUtils.where_from_index(env_index, 0, attr),
+                    )
         super()._reset(env_index)
 
     @override(EntityState)
+    def zero_grad(self):
+        for attr_name in ["c", "force", "torque"]:
+            attr = self.__getattribute__(attr_name)
+            if attr is not None:
+                self.__setattr__(attr_name, attr.detach())
+        super().zero_grad()
+
+    @override(EntityState)
     def _spawn(self, dim_c: int, dim_p: int):
         if dim_c > 0:
             self.c = torch.zeros(
                 self.batch_dim, dim_c, device=self.device, dtype=torch.float32
             )
         self.force = torch.zeros(
             self.batch_dim, dim_p, device=self.device, dtype=torch.float32
@@ -416,16 +438,16 @@
 
         self._check_action_init()
 
     def _check_action_init(self):
         for attr in (self.u_multiplier, self.u_range, self.u_noise):
             if isinstance(attr, List):
                 assert len(attr) == self.action_size, (
-                    f"Action attributes u_... must be either a float or a list of floats"
-                    f" (one per action) all with same length"
+                    "Action attributes u_... must be either a float or a list of floats"
+                    " (one per action) all with same length"
                 )
 
     @property
     def u(self):
         return self._u
 
     @u.setter
@@ -488,43 +510,56 @@
         return torch.tensor(
             value if isinstance(value, Sequence) else [value] * self.action_size,
             device=self.device,
             dtype=torch.float,
         )
 
     def _reset(self, env_index: typing.Optional[int]):
-        for attr in [self.u, self.c]:
+        for attr_name in ["u", "c"]:
+            attr = self.__getattribute__(attr_name)
             if attr is not None:
                 if env_index is None:
-                    attr[:] = 0.0
+                    self.__setattr__(attr_name, torch.zeros_like(attr))
                 else:
-                    attr[env_index] = 0.0
+                    self.__setattr__(
+                        attr_name,
+                        TorchUtils.where_from_index(env_index, 0, attr),
+                    )
+
+    def zero_grad(self):
+        for attr_name in ["u", "c"]:
+            attr = self.__getattribute__(attr_name)
+            if attr is not None:
+                self.__setattr__(attr_name, attr.detach())
 
 
 # properties and state of physical world entity
 class Entity(TorchVectorizedObject, Observable, ABC):
     def __init__(
         self,
         name: str,
         movable: bool = False,
         rotatable: bool = False,
         collide: bool = True,
         density: float = 25.0,  # Unused for now
         mass: float = 1.0,
-        shape: Shape = Sphere(),
+        shape: Shape = None,
         v_range: float = None,
         max_speed: float = None,
         color=Color.GRAY,
         is_joint: bool = False,
         drag: float = None,
         linear_friction: float = None,
         angular_friction: float = None,
         gravity: typing.Union[float, Tensor] = None,
         collision_filter: Callable[[Entity], bool] = lambda _: True,
     ):
+        if shape is None:
+            shape = Sphere()
+
         TorchVectorizedObject.__init__(self)
         Observable.__init__(self)
         # name
         self._name = name
         # entity can move / be pushed
         self._movable = movable
         # entity can rotate
@@ -686,14 +721,17 @@
 
     def _spawn(self, dim_c: int, dim_p: int):
         self.state._spawn(dim_c, dim_p)
 
     def _reset(self, env_index: int):
         self.state._reset(env_index)
 
+    def zero_grad(self):
+        self.state.zero_grad()
+
     def set_pos(self, pos: Tensor, batch_index: int):
         self._set_state_property(EntityState.pos, self.state, pos, batch_index)
 
     def set_vel(self, vel: Tensor, batch_index: int):
         self._set_state_property(EntityState.vel, self.state, vel, batch_index)
 
     def set_rot(self, rot: Tensor, batch_index: int):
@@ -746,15 +784,15 @@
 
 
 # properties of landmark entities
 class Landmark(Entity):
     def __init__(
         self,
         name: str,
-        shape: Shape = Sphere(),
+        shape: Shape = None,
         movable: bool = False,
         rotatable: bool = False,
         collide: bool = True,
         density: float = 25.0,  # Unused for now
         mass: float = 1.0,
         v_range: float = None,
         max_speed: float = None,
@@ -787,15 +825,15 @@
 
 
 # properties of agent entities
 class Agent(Entity):
     def __init__(
         self,
         name: str,
-        shape: Shape = Sphere(),
+        shape: Shape = None,
         movable: bool = True,
         rotatable: bool = True,
         collide: bool = True,
         density: float = 25.0,  # Unused for now
         mass: float = 1.0,
         f_range: float = None,
         max_f: float = None,
@@ -984,14 +1022,19 @@
 
     @override(Entity)
     def _reset(self, env_index: int):
         self.action._reset(env_index)
         self.dynamics.reset(env_index)
         super()._reset(env_index)
 
+    def zero_grad(self):
+        self.action.zero_grad()
+        self.dynamics.zero_grad()
+        super().zero_grad()
+
     @override(Entity)
     def to(self, device: torch.device):
         super().to(device)
         self.action.to(device)
         for sensor in self.sensors:
             sensor.to(device)
 
@@ -1108,14 +1151,18 @@
                 }
             )
 
     def reset(self, env_index: int):
         for e in self.entities:
             e._reset(env_index)
 
+    def zero_grad(self):
+        for e in self.entities:
+            e.zero_grad()
+
     @property
     def agents(self) -> List[Agent]:
         return self._agents
 
     @property
     def landmarks(self) -> List[Landmark]:
         return self._landmarks
@@ -1323,15 +1370,15 @@
             if isinstance(e.shape, Box):
                 d = self._cast_ray_to_box(e, pos, angles, max_range)
             elif isinstance(e.shape, Sphere):
                 d = self._cast_ray_to_sphere(e, pos, angles, max_range)
             elif isinstance(e.shape, Line):
                 d = self._cast_ray_to_line(e, pos, angles, max_range)
             else:
-                assert False, f"Shape {e.shape} currently not handled by cast_ray"
+                raise RuntimeError(f"Shape {e.shape} currently not handled by cast_ray")
             dists.append(d)
         dist, _ = torch.min(torch.stack(dists, dim=-1), dim=-1)
         return dist
 
     def get_distance_from_point(
         self, entity: Entity, test_point_pos, env_index: int = None
     ):
@@ -1349,20 +1396,23 @@
                 entity.shape.length,
                 test_point_pos,
             )
             distance = torch.linalg.vector_norm(test_point_pos - closest_point, dim=-1)
             return_value = distance - LINE_MIN_DIST
         elif isinstance(entity.shape, Line):
             closest_point = _get_closest_point_line(
-                entity.state.pos, entity.state.rot, entity.shape.length, test_point_pos
+                entity.state.pos,
+                entity.state.rot,
+                entity.shape.length,
+                test_point_pos,
             )
             distance = torch.linalg.vector_norm(test_point_pos - closest_point, dim=-1)
             return_value = distance - LINE_MIN_DIST
         else:
-            assert False, "Distance not computable for given entity"
+            raise RuntimeError("Distance not computable for given entity")
         if env_index is not None:
             return_value = return_value[env_index]
         return return_value
 
     def get_distance(self, entity_a: Entity, entity_b: Entity, env_index: int = None):
         a_shape = entity_a.shape
         b_shape = entity_b.shape
@@ -1441,15 +1491,15 @@
                 entity_b.state.rot,
                 entity_b.shape.width,
                 entity_b.shape.length,
             )
             dist = torch.linalg.vector_norm(point_a - point_b, dim=-1)
             return_value = dist - LINE_MIN_DIST
         else:
-            assert False, "Distance not computable for given entities"
+            raise RuntimeError("Distance not computable for given entities")
         return return_value
 
     def is_overlapping(self, entity_a: Entity, entity_b: Entity, env_index: int = None):
         a_shape = entity_a.shape
         b_shape = entity_b.shape
         self._check_batch_index(env_index)
 
@@ -1503,15 +1553,15 @@
                 box.state.pos - closest_point, dim=-1
             )
             dist_min = sphere.shape.radius + LINE_MIN_DIST
             return_value = (distance_sphere_box < distance_closest_point_box) + (
                 distance_sphere_closest_point < dist_min
             )
         else:
-            assert False, "Overlap not computable for give entities"
+            raise RuntimeError("Overlap not computable for give entities")
         if env_index is not None:
             return_value = return_value[env_index]
         return return_value
 
     # update state of the world
     def step(self):
         self.entity_index_map = {e: i for i, e in enumerate(self.entities)}
@@ -1532,30 +1582,30 @@
                     1,
                     device=self.device,
                     dtype=torch.float32,
                 )
                 for e in self.entities
             }
 
-            for i, entity in enumerate(self.entities):
+            for entity in self.entities:
                 if isinstance(entity, Agent):
                     # apply agent force controls
                     self._apply_action_force(entity)
                     # apply agent torque controls
                     self._apply_action_torque(entity)
                 # apply friction
                 self._apply_friction_force(entity)
                 # apply gravity
                 self._apply_gravity(entity)
 
                 # self._apply_environment_force(entity, i)
 
             self._apply_vectorized_enviornment_force()
 
-            for i, entity in enumerate(self.entities):
+            for entity in self.entities:
                 # integrate physical state
                 self._integrate_state(entity, substep)
 
         # update non-differentiable comm state
         if self._dim_c > 0:
             for agent in self._agents:
                 self._update_comm_state(agent)
@@ -1713,15 +1763,15 @@
                     )
                     b_l.append((box, line))
                 elif isinstance(entity_a.shape, Box) and isinstance(
                     entity_b.shape, Box
                 ):
                     b_b.append((entity_a, entity_b))
                 else:
-                    assert False
+                    raise AssertionError()
         # Joints
         self._vectorized_joint_constraints(joints)
 
         # Sphere and sphere
         self._sphere_sphere_vectorized_collision(s_s)
         # Line and sphere
         self._sphere_line_vectorized_collision(l_s)
@@ -1773,15 +1823,15 @@
             )
             rotate_prior = torch.stack(
                 rotate,
                 dim=-1,
             )
             rotate = rotate_prior.unsqueeze(0).expand(self.batch_dim, -1).unsqueeze(-1)
 
-            force_a_attractive, force_b_attractive = self._get_constraint_forces(
+            (force_a_attractive, force_b_attractive,) = self._get_constraint_forces(
                 pos_joint_a,
                 pos_joint_b,
                 dist_min=dist,
                 attractive=True,
                 force_multiplier=self._joint_force,
             )
             force_a_repulsive, force_b_repulsive = self._get_constraint_forces(
@@ -1864,20 +1914,20 @@
     def _sphere_line_vectorized_collision(self, l_s):
         if len(l_s):
             pos_l = []
             pos_s = []
             rot_l = []
             radius_s = []
             length_l = []
-            for l, s in l_s:
-                pos_l.append(l.state.pos)
-                pos_s.append(s.state.pos)
-                rot_l.append(l.state.rot)
-                radius_s.append(torch.tensor(s.shape.radius, device=self.device))
-                length_l.append(torch.tensor(l.shape.length, device=self.device))
+            for line, sphere in l_s:
+                pos_l.append(line.state.pos)
+                pos_s.append(sphere.state.pos)
+                rot_l.append(line.state.rot)
+                radius_s.append(torch.tensor(sphere.shape.radius, device=self.device))
+                length_l.append(torch.tensor(line.shape.length, device=self.device))
             pos_l = torch.stack(pos_l, dim=-2)
             pos_s = torch.stack(pos_s, dim=-2)
             rot_l = torch.stack(rot_l, dim=-2)
             radius_s = (
                 torch.stack(
                     radius_s,
                     dim=-1,
@@ -2380,20 +2430,24 @@
             if entity.v_range is not None:
                 entity.state.vel = entity.state.vel.clamp(
                     -entity.v_range, entity.v_range
                 )
             new_pos = entity.state.pos + entity.state.vel * self._sub_dt
             entity.state.pos = torch.stack(
                 [
-                    new_pos[..., X].clamp(-self._x_semidim, self._x_semidim)
-                    if self._x_semidim is not None
-                    else new_pos[..., X],
-                    new_pos[..., Y].clamp(-self._y_semidim, self._y_semidim)
-                    if self._y_semidim is not None
-                    else new_pos[..., Y],
+                    (
+                        new_pos[..., X].clamp(-self._x_semidim, self._x_semidim)
+                        if self._x_semidim is not None
+                        else new_pos[..., X]
+                    ),
+                    (
+                        new_pos[..., Y].clamp(-self._y_semidim, self._y_semidim)
+                        if self._y_semidim is not None
+                        else new_pos[..., Y]
+                    ),
                 ],
                 dim=-1,
             )
 
         if entity.rotatable:
             # Compute rotation
             if substep == 0:
```

### Comparing `vmas-1.4.0/vmas/simulator/dynamics/common.py` & `vmas-1.4.1/vmas/simulator/dynamics/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,33 +11,40 @@
 class Dynamics(ABC):
     def __init__(
         self,
     ):
         self._agent = None
 
     def reset(self, index: Union[Tensor, int] = None):
-        pass
+        return
+
+    def zero_grad(self):
+        return
 
     @property
     def agent(self):
         if self._agent is None:
             raise ValueError(
                 "You need to add the dynamics to an agent during construction before accessing its properties"
             )
         return self._agent
 
     @agent.setter
     def agent(self, value):
         if self._agent is not None:
             raise ValueError("Agent in dynamics has already been set")
-        if value.action_size < self.needed_action_size:
+        self._agent = value
+
+    def check_and_process_action(self):
+        action = self.agent.action.u
+        if action.shape[1] < self.needed_action_size:
             raise ValueError(
-                f"Agent action size {value.action_size} is less than the required dynamics action size {self.needed_action_size}"
+                f"Agent action size {action.shape[1]} is less than the required dynamics action size {self.needed_action_size}"
             )
-        self._agent = value
+        self.process_action()
 
     @property
     @abc.abstractmethod
     def needed_action_size(self) -> int:
         raise NotImplementedError
 
     @abc.abstractmethod
```

### Comparing `vmas-1.4.0/vmas/simulator/dynamics/diff_drive.py` & `vmas-1.4.1/vmas/simulator/dynamics/diff_drive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
-import math
+
 
 import torch
+
 import vmas.simulator.core
 import vmas.simulator.utils
 from vmas.simulator.dynamics.common import Dynamics
 
 
 class DiffDrive(Dynamics):
     def __init__(
```

### Comparing `vmas-1.4.0/vmas/simulator/dynamics/kinematic_bicycle.py` & `vmas-1.4.1/vmas/simulator/dynamics/kinematic_bicycle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #  Copyright (c) 2023-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
-from typing import Union
 
 import torch
+
 import vmas.simulator.core
 import vmas.simulator.utils
 from vmas.simulator.dynamics.common import Dynamics
 
 
 class KinematicBicycle(Dynamics):
     # For the implementation of the kinematic bicycle model, see the equation (2) of the paper Polack, Philip, et al. "The kinematic bicycle model: A consistent model for planning feasible trajectories for autonomous vehicles?." 2017 IEEE intelligent vehicles symposium (IV). IEEE, 2017.
```

### Comparing `vmas-1.4.0/vmas/simulator/environment/__init__.py` & `vmas-1.4.1/vmas/simulator/environment/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2022.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 from enum import Enum
 
 from vmas.simulator.environment.environment import Environment
```

### Comparing `vmas-1.4.0/vmas/simulator/environment/environment.py` & `vmas-1.4.1/vmas/simulator/environment/environment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 import random
 from ctypes import byref
-from typing import List, Tuple, Callable, Optional, Union, Dict
+from typing import Callable, Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import torch
 from gym import spaces
 from torch import Tensor
+
+import vmas.simulator.utils
 from vmas.simulator.core import Agent, TorchVectorizedObject
 from vmas.simulator.scenario import BaseScenario
-import vmas.simulator.utils
 from vmas.simulator.utils import (
-    VIEWER_MIN_ZOOM,
     AGENT_OBS_TYPE,
-    X,
-    Y,
     ALPHABET,
     DEVICE_TYPING,
     override,
     TorchUtils,
+    X,
+    Y,
 )
 
 
 # environment for all agents in the multiagent world
 # currently code assumes that no agents will be created/destroyed at runtime!
 class Environment(TorchVectorizedObject):
     metadata = {
@@ -144,30 +144,32 @@
         if get_observations:
             obs = {} if dict_agent_names else []
         if get_rewards:
             rewards = {} if dict_agent_names else []
         if get_infos:
             infos = {} if dict_agent_names else []
 
-        for agent in self.agents:
-            if get_rewards:
+        if get_rewards:
+            for agent in self.agents:
                 reward = self.scenario.reward(agent).clone()
                 if dict_agent_names:
                     rewards.update({agent.name: reward})
                 else:
                     rewards.append(reward)
-            if get_observations:
+        if get_observations:
+            for agent in self.agents:
                 observation = TorchUtils.recursive_clone(
                     self.scenario.observation(agent)
                 )
                 if dict_agent_names:
                     obs.update({agent.name: observation})
                 else:
                     obs.append(observation)
-            if get_infos:
+        if get_infos:
+            for agent in self.agents:
                 info = TorchUtils.recursive_clone(self.scenario.info(agent))
                 if dict_agent_names:
                     infos.update({agent.name: info})
                 else:
                     infos.append(info)
 
         if get_dones:
@@ -192,14 +194,29 @@
         Returns:
             obs: List on len 'self.n_agents' of which each element is a torch.Tensor
                  of shape '(self.num_envs, obs_size_of_agent)'
             rewards: List on len 'self.n_agents' of which each element is a torch.Tensor of shape '(self.num_envs)'
             dones: Tensor of len 'self.num_envs' of which each element is a bool
             infos : List on len 'self.n_agents' of which each element is a dictionary for which each key is a metric
                     and the value is a tensor of shape '(self.num_envs, metric_size_per_agent)'
+
+        Examples:
+            >>> import vmas
+            >>> env = vmas.make_env(
+            ...     scenario="waterfall",  # can be scenario name or BaseScenario class
+            ...     num_envs=32,
+            ...     device="cpu",  # Or "cuda" for GPU
+            ...     continuous_actions=True,
+            ...     max_steps=None,  # Defines the horizon. None is infinite horizon.
+            ...     seed=None,  # Seed of the environment
+            ...     n_agents=3,  # Additional arguments you want to pass to the scenario
+            ... )
+            >>> obs = env.reset()
+            >>> for _ in range(10):
+            ...     obs, rews, dones, info = env.step(env.get_random_actions())
         """
         if isinstance(actions, Dict):
             actions_dict = actions
             actions = []
             for agent in self.agents:
                 try:
                     actions.append(actions_dict[agent.name])
@@ -237,33 +254,20 @@
             self.scenario.env_process_action(agent)
 
         # advance world state
         self.world.step()
 
         self.steps += 1
         obs, rewards, dones, infos = self.get_from_scenario(
-            get_observations=True, get_infos=True, get_rewards=True, get_dones=True
+            get_observations=True,
+            get_infos=True,
+            get_rewards=True,
+            get_dones=True,
         )
 
-        # print("\nStep results in unwrapped environment")
-        # print(
-        #     f"Actions len (n_agents): {len(actions)}, "
-        #     f"actions[0] shape (num_envs, agent 0 action shape): {actions[0].shape}, "
-        #     f"actions[0][0] (action agent 0 env 0): {actions[0][0]}"
-        # )
-        # print(
-        #     f"Obs len (n_agents): {len(obs)}, "
-        #     f"obs[0] shape (num_envs, agent 0 obs shape): {obs[0].shape}, obs[0][0] (obs agent 0 env 0): {obs[0][0]}"
-        # )
-        # print(
-        #     f"Rewards len (n_agents): {len(rewards)}, rewards[0] shape (num_envs, 1): {rewards[0].shape}, "
-        #     f"rewards[0][0] (agent 0 env 0): {rewards[0][0]}"
-        # )
-        # print(f"Dones len (n_envs): {len(dones)}, dones[0] (done env 0): {dones[0]}")
-        # print(f"Info len (n_agents): {len(infos)}, info[0] (infos agent 0): {infos[0]}")
         return obs, rewards, dones, infos
 
     def done(self):
         dones = self.scenario.done().clone()
         if self.max_steps is not None:
             dones += self.steps >= self.max_steps
         return dones
@@ -345,44 +349,117 @@
             )
 
     def get_agent_observation_space(self, agent: Agent, obs: AGENT_OBS_TYPE):
         if isinstance(obs, Tensor):
             return spaces.Box(
                 low=-np.float32("inf"),
                 high=np.float32("inf"),
-                shape=(len(obs[0]),),
+                shape=obs.shape[1:],
                 dtype=np.float32,
             )
         elif isinstance(obs, Dict):
             return spaces.Dict(
                 {
                     key: self.get_agent_observation_space(agent, value)
                     for key, value in obs.items()
                 }
             )
         else:
             raise NotImplementedError(
                 f"Invalid type of observation {obs} for agent {agent.name}"
             )
 
+    def get_random_action(self, agent: Agent) -> torch.Tensor:
+        """Returns a random action for the given agent.
+
+        Args:
+            agent (Agent): The agent to get the action for
+
+        Returns:
+            torch.tensor: the random actions tensor with shape ``(agent.batch_dim, agent.action_size)``
+
+        """
+        if self.continuous_actions:
+            actions = []
+            for action_index in range(agent.action_size):
+                actions.append(
+                    torch.zeros(
+                        agent.batch_dim,
+                        device=agent.device,
+                        dtype=torch.float32,
+                    ).uniform_(
+                        -agent.action.u_range_tensor[action_index],
+                        agent.action.u_range_tensor[action_index],
+                    )
+                )
+            if self.world.dim_c != 0 and not agent.silent:
+                # If the agent needs to communicate
+                for _ in range(self.world.dim_c):
+                    actions.append(
+                        torch.zeros(
+                            agent.batch_dim,
+                            device=agent.device,
+                            dtype=torch.float32,
+                        ).uniform_(
+                            0,
+                            1,
+                        )
+                    )
+            action = torch.stack(actions, dim=-1)
+        else:
+            action = torch.randint(
+                low=0,
+                high=self.get_agent_action_space(agent).n,
+                size=(agent.batch_dim,),
+                device=agent.device,
+            )
+        return action
+
+    def get_random_actions(self) -> Sequence[torch.Tensor]:
+        """Returns random actions for all agents that you can feed to :class:`step`
+
+        Returns:
+            Sequence[torch.tensor]: the random actions for the agents
+
+        Examples:
+            >>> import vmas
+            >>> env = vmas.make_env(
+            ...     scenario="waterfall",  # can be scenario name or BaseScenario class
+            ...     num_envs=32,
+            ...     device="cpu",  # Or "cuda" for GPU
+            ...     continuous_actions=True,
+            ...     max_steps=None,  # Defines the horizon. None is infinite horizon.
+            ...     seed=None,  # Seed of the environment
+            ...     n_agents=3,  # Additional arguments you want to pass to the scenario
+            ... )
+            >>> obs = env.reset()
+            >>> for _ in range(10):
+            ...     obs, rews, dones, info = env.step(env.get_random_actions())
+
+        """
+        return [self.get_random_action(agent) for agent in self.agents]
+
     def _check_discrete_action(self, action: Tensor, low: int, high: int, type: str):
         assert torch.all(
             (action >= torch.tensor(low, device=self.device))
             * (action < torch.tensor(high, device=self.device))
         ), f"Discrete {type} actions are out of bounds, allowed int range [{low},{high})"
 
     # set env action for a particular agent
     def _set_action(self, action, agent):
         action = action.clone()
         if not self.grad_enabled:
             action = action.detach()
         action = action.to(self.device)
         assert not action.isnan().any()
         agent.action.u = torch.zeros(
-            self.batch_dim, agent.action_size, device=self.device, dtype=torch.float32
+            self.batch_dim,
+            agent.action_size,
+            device=self.device,
+            dtype=torch.float32,
         )
 
         assert action.shape[1] == self.get_agent_action_size(agent), (
             f"Agent {agent.name} has wrong action size, got {action.shape[1]}, "
             f"expected {self.get_agent_action_size(agent)}"
         )
         if self.clamp_action and self.continuous_actions:
@@ -452,15 +529,17 @@
                 action_index += 1
 
         agent.action.u *= agent.action.u_multiplier_tensor
 
         if agent.action.u_noise > 0:
             noise = (
                 torch.randn(
-                    *agent.action.u.shape, device=self.device, dtype=torch.float32
+                    *agent.action.u.shape,
+                    device=self.device,
+                    dtype=torch.float32,
                 )
                 * agent.u_noise
             )
             agent.action.u += noise
         if self.world.dim_c > 0 and not agent.silent:
             if not self.continuous_actions:
                 comm_action = action[:, action_index:]
@@ -481,15 +560,17 @@
                 assert not torch.any(comm_action > 1) and not torch.any(
                     comm_action < 0
                 ), "Comm actions are out of range [0,1]"
                 agent.action.c = comm_action
             if agent.c_noise > 0:
                 noise = (
                     torch.randn(
-                        *agent.action.c.shape, device=self.device, dtype=torch.float32
+                        *agent.action.c.shape,
+                        device=self.device,
+                        dtype=torch.float32,
                     )
                     * agent.c_noise
                 )
                 agent.action.c += noise
 
     def render(
         self,
@@ -568,61 +649,68 @@
                 )
 
             try:
                 # Try to use EGL
                 pyglet.lib.load_library("EGL")
 
                 # Only if we have GPUs
-                from pyglet.libs.egl import egl
-                from pyglet.libs.egl import eglext
+                from pyglet.libs.egl import egl, eglext
 
                 num_devices = egl.EGLint()
                 eglext.eglQueryDevicesEXT(0, None, byref(num_devices))
                 assert num_devices.value > 0
 
             except (ImportError, AssertionError):
                 self.headless = False
             pyglet.options["headless"] = self.headless
 
             self._init_rendering()
 
-        zoom = max(VIEWER_MIN_ZOOM, self.scenario.viewer_zoom)
+        if self.scenario.viewer_zoom <= 0:
+            raise ValueError("Scenario viewer zoom must be > 0")
+        zoom = self.scenario.viewer_zoom
 
         if aspect_ratio < 1:
             cam_range = torch.tensor([zoom, zoom / aspect_ratio], device=self.device)
         else:
             cam_range = torch.tensor([zoom * aspect_ratio, zoom], device=self.device)
 
         if shared_viewer:
             # zoom out to fit everyone
             all_poses = torch.stack(
-                [agent.state.pos[env_index] for agent in self.world.agents], dim=0
+                [agent.state.pos[env_index] for agent in self.world.agents],
+                dim=0,
             )
             max_agent_radius = max(
                 [agent.shape.circumscribed_radius() for agent in self.world.agents]
             )
             viewer_size_fit = (
                 torch.stack(
                     [
-                        torch.max(torch.abs(all_poses[:, X])),
-                        torch.max(torch.abs(all_poses[:, Y])),
+                        torch.max(
+                            torch.abs(all_poses[:, X] - self.scenario.render_origin[X])
+                        ),
+                        torch.max(
+                            torch.abs(all_poses[:, Y] - self.scenario.render_origin[Y])
+                        ),
                     ]
                 )
                 + 2 * max_agent_radius
             )
 
             viewer_size = torch.maximum(
-                viewer_size_fit / cam_range, torch.tensor(zoom, device=self.device)
+                viewer_size_fit / cam_range,
+                torch.tensor(zoom, device=self.device),
             )
             cam_range *= torch.max(viewer_size)
             self.viewer.set_bounds(
-                -cam_range[X],
-                cam_range[X],
-                -cam_range[Y],
-                cam_range[Y],
+                -cam_range[X] + self.scenario.render_origin[X],
+                cam_range[X] + self.scenario.render_origin[X],
+                -cam_range[Y] + self.scenario.render_origin[Y],
+                cam_range[Y] + self.scenario.render_origin[Y],
             )
         else:
             # update bounds to center around agent
             pos = self.agents[agent_index_focus].state.pos[env_index]
             self.viewer.set_bounds(
                 pos[X] - cam_range[X],
                 pos[X] + cam_range[X],
```

### Comparing `vmas-1.4.0/vmas/simulator/environment/gym.py` & `vmas-1.4.1/vmas/simulator/environment/gym.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 from typing import List, Optional
 
 import gym
 import numpy as np
 import torch
 
 from vmas.simulator.environment.environment import Environment
-from vmas.simulator.utils import (
-    extract_nested_with_index,
-)
+from vmas.simulator.utils import extract_nested_with_index
 
 
 class GymWrapper(gym.Env):
     metadata = Environment.metadata
 
     def __init__(
         self,
```

### Comparing `vmas-1.4.0/vmas/simulator/environment/rllib.py` & `vmas-1.4.1/vmas/simulator/environment/rllib.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,21 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
-from typing import List, Optional, Tuple, Dict
+from typing import Dict, List, Optional, Tuple
 
 import numpy as np
 import torch
 from numpy import ndarray
 from ray import rllib
 from ray.rllib.utils.typing import EnvActionType, EnvInfoDict, EnvObsType
 from torch import Tensor
+
 from vmas.simulator.environment.environment import Environment
-from vmas.simulator.utils import (
-    OBS_TYPE,
-    REWARD_TYPE,
-    INFO_TYPE,
-    TorchUtils,
-)
+from vmas.simulator.utils import INFO_TYPE, OBS_TYPE, REWARD_TYPE, TorchUtils
 
 
 class VectorEnvWrapper(rllib.VectorEnv):
     """
     Vector environment wrapper for rllib
     """
 
@@ -52,30 +48,14 @@
     ) -> Tuple[List[EnvObsType], List[float], List[bool], List[EnvInfoDict]]:
         # saved_actions = actions
         actions = self._action_list_to_tensor(actions)
         obs, rews, dones, infos = TorchUtils.to_numpy(self._env.step(actions))
 
         obs, infos, rews = self._read_data(obs, infos, rews)
 
-        # print("\nStep results in wrapped environment")
-        # print(
-        #     f"Actions len (num_envs): {len(saved_actions)}, len actions[0] (n_agents): {len(saved_actions[0])},"
-        #     f" actions[0][0] (action agent 0 env 0): {saved_actions[0][0]}"
-        # )
-        # print(
-        #     f"Obs len (num_envs): {len(obs_list)}, len obs[0] (n_agents): {len(obs_list[0])},"
-        #     f" obs[0][0] (obs agent 0 env 0): {obs_list[0][0]}"
-        # )
-        # print(
-        #     f"Total rews len (num_envs): {len(total_rews)}, total_rews[0] (total rew env 0): {total_rews[0]}"
-        # )
-        # print(f"Dones len (num_envs): {len(dones)}, dones[0] (done env 0): {dones[0]}")
-        # print(
-        #     f"Total infos len (num_envs): {len(total_infos)}, total_infos[0] (infos env 0): {total_infos[0]}"
-        # )
         return obs, rews, dones, infos
 
     def seed(self, seed=None):
         return self._env.seed(seed)
 
     def try_render_at(
         self,
@@ -144,15 +124,15 @@
                         ] == self._env.get_agent_action_size(self._env.agents[i]), (
                             f"Action of agent {i} in env {j} hase wrong shape: "
                             f"expected {self._env.get_agent_action_size(self._env.agents[i])}, got {act.shape[0]}"
                         )
                     actions[i][j] = act
             return actions
         else:
-            assert False, "Input action is not in correct format"
+            raise TypeError("Input action is not in correct format")
 
     def _read_data(
         self,
         obs: Optional[OBS_TYPE],
         info: Optional[INFO_TYPE] = None,
         reward: Optional[REWARD_TYPE] = None,
         env_index: Optional[int] = None,
```

### Comparing `vmas-1.4.0/vmas/simulator/heuristic_policy.py` & `vmas-1.4.1/vmas/simulator/heuristic_policy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2022.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 from abc import ABC, abstractmethod
 
 import torch
```

### Comparing `vmas-1.4.0/vmas/simulator/joints.py` & `vmas-1.4.1/vmas/simulator/joints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Tuple, List
+from typing import List, Tuple, TYPE_CHECKING
 
 import torch
+
 import vmas.simulator.core
 import vmas.simulator.utils
 
 if TYPE_CHECKING:
     from vmas.simulator.rendering import Geom
 
 UNCOLLIDABLE_JOINT_RENDERING_WIDTH = 1
@@ -64,17 +65,19 @@
 
             self.landmark = vmas.simulator.core.Landmark(
                 name=f"joint {entity_a.name} {entity_b.name}",
                 collide=collidable,
                 movable=True,
                 rotatable=rotate_a and rotate_b,
                 mass=mass,
-                shape=vmas.simulator.core.Box(length=dist, width=width)
-                if width != 0
-                else vmas.simulator.core.Line(length=dist),
+                shape=(
+                    vmas.simulator.core.Box(length=dist, width=width)
+                    if width != 0
+                    else vmas.simulator.core.Line(length=dist)
+                ),
                 color=vmas.simulator.utils.Color.BLACK,
                 is_joint=True,
             )
             self.joint_constraints += [
                 JointConstraint(
                     self.landmark,
                     entity_a,
@@ -143,15 +146,15 @@
     def _delta_anchor_tensor(self, entity):
         if entity not in self._delta_anchor_tensor_map:
             if entity == self.entity_a:
                 anchor = self.anchor_a
             elif entity == self.entity_b:
                 anchor = self.anchor_b
             else:
-                assert False
+                raise AssertionError()
 
             delta_anchor_tensor = (
                 torch.tensor(
                     entity.shape.get_delta_from_anchor(anchor),
                     device=entity.state.pos.device,
                 )
                 .unsqueeze(0)
```

### Comparing `vmas-1.4.0/vmas/simulator/physics.py` & `vmas-1.4.1/vmas/simulator/physics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #  Copyright (c) 2023-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 from __future__ import annotations
 
 import torch
+
 from vmas.simulator.utils import TorchUtils
 
 
 def _get_inner_point_box(outside_point, surface_point, box_pos):
     v = surface_point - outside_point
     u = box_pos - surface_point
     v_norm = torch.linalg.vector_norm(v, dim=-1).unsqueeze(-1)
@@ -107,15 +108,18 @@
     closest_point_2 = torch.full(
         box_pos.shape,
         float("inf"),
         device=box_pos.device,
         dtype=torch.float32,
     )
     distance = torch.full(
-        box_pos.shape[:-1], float("inf"), device=box_pos.device, dtype=torch.float32
+        box_pos.shape[:-1],
+        float("inf"),
+        device=box_pos.device,
+        dtype=torch.float32,
     )
     for p1, p2 in zip(p1s, p2s):
         d = torch.linalg.vector_norm(p1 - p2, dim=-1)
         is_closest = d < distance
         is_closest_exp = is_closest.unsqueeze(-1).expand(p1.shape)
         closest_point_1 = torch.where(is_closest_exp, p1, closest_point_1)
         closest_point_2 = torch.where(is_closest_exp, p2, closest_point_2)
@@ -190,15 +194,18 @@
     closest_point_2 = torch.full(
         line_pos.shape,
         float("inf"),
         device=line_pos.device,
         dtype=torch.float32,
     )
     min_distance = torch.full(
-        line_pos.shape[:-1], float("inf"), device=line_pos.device, dtype=torch.float32
+        line_pos.shape[:-1],
+        float("inf"),
+        device=line_pos.device,
+        dtype=torch.float32,
     )
     for p1, p2 in point_pairs:
         d = torch.linalg.vector_norm(p1 - p2, dim=-1)
         is_closest = d < min_distance
         is_closest_exp = is_closest.unsqueeze(-1).expand(p1.shape)
         closest_point_1 = torch.where(is_closest_exp, p1, closest_point_1)
         closest_point_2 = torch.where(is_closest_exp, p2, closest_point_2)
@@ -227,15 +234,18 @@
     t = cross_q_minus_p_s / cross_r_s
     t_in_range = (0 <= t) * (t <= 1)
     u_in_range = (0 <= u) * (u <= 1)
 
     cross_r_s_is_zero = cross_r_s == 0
 
     distance = torch.full(
-        point_a1.shape[:-1], float("inf"), device=point_a1.device, dtype=torch.float32
+        point_a1.shape[:-1],
+        float("inf"),
+        device=point_a1.device,
+        dtype=torch.float32,
     )
     point = torch.full(
         point_a1.shape,
         float("inf"),
         device=point_a1.device,
         dtype=torch.float32,
     )
@@ -265,15 +275,18 @@
     closest_point = torch.full(
         box_pos.shape,
         float("inf"),
         device=box_pos.device,
         dtype=torch.float32,
     )
     distance = torch.full(
-        box_pos.shape[:-1], float("inf"), device=box_pos.device, dtype=torch.float32
+        box_pos.shape[:-1],
+        float("inf"),
+        device=box_pos.device,
+        dtype=torch.float32,
     )
     for p in closest_points:
         d = torch.linalg.vector_norm(test_point_pos - p, dim=-1)
         is_closest = d < distance
         is_closest_exp = is_closest.unsqueeze(-1).expand(p.shape)
         closest_point = torch.where(is_closest_exp, p, closest_point)
         distance = torch.where(is_closest, d, distance)
@@ -300,15 +313,19 @@
     rots = []
     lengths = []
     for i, p in enumerate([p1, p2, p3, p4]):
         ps.append(p)
         rots.append(box_rot + torch.pi / 2 if i <= 1 else box_rot)
         lengths.append(box_width if i <= 1 else box_length)
 
-    return torch.stack(ps, dim=0), torch.stack(rots, dim=0), torch.stack(lengths, dim=0)
+    return (
+        torch.stack(ps, dim=0),
+        torch.stack(rots, dim=0),
+        torch.stack(lengths, dim=0),
+    )
 
 
 def _get_closest_line_box(
     box_pos, box_rot, box_width, box_length, line_pos, line_rot, line_length
 ):
     if not isinstance(box_width, torch.Tensor):
         box_width = torch.tensor(
@@ -336,15 +353,18 @@
     closest_point_2 = torch.full(
         box_pos.shape,
         float("inf"),
         device=box_pos.device,
         dtype=torch.float32,
     )
     distance = torch.full(
-        box_pos.shape[:-1], float("inf"), device=box_pos.device, dtype=torch.float32
+        box_pos.shape[:-1],
+        float("inf"),
+        device=box_pos.device,
+        dtype=torch.float32,
     )
     ps_box, ps_line = _get_closest_points_line_line(
         lines_pos,
         lines_rot,
         lines_length,
         line_pos.unsqueeze(0).expand(lines_pos.shape),
         line_rot.unsqueeze(0).expand(lines_rot.shape),
```

### Comparing `vmas-1.4.0/vmas/simulator/rendering.py` & `vmas-1.4.1/vmas/simulator/rendering.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
 2D rendering framework
 """
-#  Copyright (c) 2022-2023.
+
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 from __future__ import division
 
 import math
 import os
 import sys
 from itertools import chain
-from typing import Callable, Tuple, Optional, Union
+from typing import Callable, Optional, Tuple, Union
 
 import numpy as np
 import pyglet
 import six
 import torch
-from vmas.simulator.utils import x_to_rgb_colormap, TorchUtils
+
+from vmas.simulator.utils import TorchUtils, x_to_rgb_colormap
 
 try:
     from pyglet.gl import (
         GL_BLEND,
         GL_LINE_LOOP,
         GL_LINE_SMOOTH,
         GL_LINE_SMOOTH_HINT,
@@ -122,15 +124,16 @@
 
     def set_bounds(self, left, right, bottom, top):
         assert right > left and top > bottom
         self.bounds = torch.tensor([left, right, bottom, top], device=left.device)
         scalex = self.width / (right - left)
         scaley = self.height / (top - bottom)
         self.transform = Transform(
-            translation=(-left * scalex, -bottom * scaley), scale=(scalex, scaley)
+            translation=(-left * scalex, -bottom * scaley),
+            scale=(scalex, scaley),
         )
 
     def add_geom(self, geom):
         self.geoms.append(geom)
 
     def add_onetime(self, geom):
         self.onetime_geoms.append(geom)
@@ -445,15 +448,17 @@
             glVertex2f(self.length / 2, point)
             glEnd()
 
 
 def render_function_util(
     f: Callable,
     plot_range: Union[
-        float, Tuple[float, float], Tuple[Tuple[float, float], Tuple[float, float]]
+        float,
+        Tuple[float, float],
+        Tuple[Tuple[float, float], Tuple[float, float]],
     ],
     precision: float = 0.01,
     cmap_range: Optional[Tuple[float, float]] = None,
     cmap_alpha: float = 1.0,
     cmap_name: str = "viridis",
 ):
     if isinstance(plot_range, int) or isinstance(plot_range, float):
```

### Comparing `vmas-1.4.0/vmas/simulator/scenario.py` & `vmas-1.4.1/vmas/simulator/scenario.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,116 @@
 #  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 import typing
 from abc import ABC, abstractmethod
-from typing import List
+from typing import List, Optional
 
 import torch
 from torch import Tensor
 
-from vmas.simulator.core import World, Agent
+from vmas.simulator.core import Agent, World
 from vmas.simulator.utils import (
-    INITIAL_VIEWER_SIZE,
-    VIEWER_MIN_ZOOM,
+    AGENT_INFO_TYPE,
     AGENT_OBS_TYPE,
     AGENT_REWARD_TYPE,
-    AGENT_INFO_TYPE,
+    INITIAL_VIEWER_SIZE,
+    VIEWER_DEFAULT_ZOOM,
 )
 
 if typing.TYPE_CHECKING:
     from vmas.simulator.rendering import Geom
 
 
 class BaseScenario(ABC):
+    """Base class for scenarios.
+
+    This is the class that scenarios inherit from.
+
+    The methods that are **compulsory to instantiate** are:
+
+    - :class:`make_world`
+    - :class:`reset_world_at`
+    - :class:`observation`
+    - :class:`reward`
+
+    The methods that are **optional to instantiate** are:
+
+    - :class:`info`
+    - :class:`extra_render`
+    - :class:`process_action`
+
+    """
+
     def __init__(self):
-        """Do not override"""
+        """Do not override."""
         self._world = None
-        # This is the viewer size and can be set in the `make_world' function
         self.viewer_size = INITIAL_VIEWER_SIZE
-        # This is the zoom level of the rendering
-        self.viewer_zoom = VIEWER_MIN_ZOOM
-        # Whether to plot a grid in the scenario background
+        """The size of the rendering viewer window. This can be changed in the :class:`~make_world` function. """
+        self.viewer_zoom = VIEWER_DEFAULT_ZOOM
+        """The zoom of the rendering camera (a lower value means more zoom). This can be changed in the :class:`~make_world` function. """
+        self.render_origin = (0.0, 0.0)
+        """The origin of the rendering camera when ``agent_index_to_focus`` is None in the ``render()`` arguments. This can be changed in the :class:`~make_world` function. """
         self.plot_grid = False
-        # The distance between lines in the background grid
+        """Whether to plot a grid in the scenario rendering background. This can be changed in the :class:`~make_world` function. """
         self.grid_spacing = 0.1
+        """If :class:`~plot_grid`, the distance between lines in the background grid. This can be changed in the :class:`~make_world` function. """
 
     @property
     def world(self):
-        """Do not override"""
+        """The :class:`~vmas.simulator.core.World` associated toi this scenario."""
         assert (
             self._world is not None
         ), "You first need to set `self._world` in the `make_world` method"
         return self._world
 
     def to(self, device: torch.device):
-        """Do not override"""
+        """Casts the scenario to a different device.
+
+        Args:
+            device (Union[str, int, torch.device]): the device to cast to
+        """
         for attr, value in self.__dict__.items():
             if isinstance(value, Tensor):
                 self.__dict__[attr] = value.to(device)
         self.world.to(device)
 
     def env_make_world(self, batch_dim: int, device: torch.device, **kwargs) -> World:
-        """Do not override"""
+        # Do not override
         self._world = self.make_world(batch_dim, device, **kwargs)
         return self._world
 
     def env_reset_world_at(self, env_index: typing.Optional[int]):
-        """Do not override"""
+        # Do not override
         self.world.reset(env_index)
         self.reset_world_at(env_index)
 
     def env_process_action(self, agent: Agent):
-        """Do not override"""
+        # Do not override
         if agent.action_script is not None:
             agent.action_callback(self.world)
         # Customizable action processor
         self.process_action(agent)
-        agent.dynamics.process_action()
+        agent.dynamics.check_and_process_action()
 
     @abstractmethod
     def make_world(self, batch_dim: int, device: torch.device, **kwargs) -> World:
         """
-        This function needs to be implemented when creating a scenario
-        In this function the user should instantiate the world and insert agents and landmarks in it
+        This function needs to be implemented when creating a scenario.
+        In this function the user should instantiate the world and insert agents and landmarks in it.
 
         Args:
-        :param batch_dim: the number of environments to step parallely
-        :param device: the torch device to use
-        :param kwargs: named arguments passed during environment creation
-        :return world: returns the instantiated world which is automatically set in 'self.world'
+            batch_dim (int): the number of vecotrized environments.
+            device (Union[str, int, torch.device], optional): the device of the environmemnt.
+            kwargs (dict, optional): named arguments passed from environment creation
+
+        Returns:
+            :class:`~vmas.simulator.core.World` : the :class:`~vmas.simulator.core.World`
+            instance which is automatically set in :class:`~world`.
+
         Examples:
             >>> from vmas.simulator.core import Agent, World, Landmark, Sphere, Box
             >>> from vmas.simulator.scenario import BaseScenario
             >>> from vmas.simulator.utils import Color
             >>> class Scenario(BaseScenario):
             >>>     def make_world(self, batch_dim: int, device: torch.device, **kwargs):
             ...         # Pass any kwargs you desire when creating the environment
@@ -112,33 +141,45 @@
             ...             )
             ...             world.add_landmark(landmark)
             ...         return world
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def reset_world_at(self, env_index: int = None):
-        """
-        Resets the world at the specified env_index.
-        When a None index is passed, the world should make a vectorized (batched) reset.
-        The 'entity.set_x()' methodes already have this logic integrated and will perform
-        batched operations when index is None
+    def reset_world_at(self, env_index: Optional[int] = None):
+        """Resets the world at the specified env_index.
+
+        When a ``None`` index is passed, the world should make a vectorized (batched) reset.
+        The ``entity.set_x()`` methods already have this logic integrated and will perform
+        batched operations when index is ``None``.
+
+        When this function is called, all entities have already had their state reset to zeros according to the ``env_index``.
+        In this function you shoud change the values of the reset states according to your task.
+        For example, some functions you might want to use are:
+
+        - ``entity.set_pos()``,
+        - ``entity.set_vel()``,
+        - ``entity.set_rot()``,
+        - ``entity.set_ang_vel()``.
+
+        Implementors can access the world at :class:`world`.
 
-        Implementors can access the world at 'self.world'
+        To increase performance, torch tensors should be created with the device already set, like:
+        ``torch.tensor(..., device=self.world.device)``
+
+        Args:
+            env_index (int, otpional): index of the environment to reset. If ``None`` a vectorized reset should be performed.
 
-        To increase performance, torch tensors created with the device set, like:
-        torch.tensor(..., device=self.world.device)
+        Spawning at fixed positions
 
-        :param env_index: index of the environment to reset. If None a vectorized reset should be performed
         Examples:
-            >>> from vmas.simulator.core import Agent, World, Landmark, Sphere, Box
             >>> from vmas.simulator.scenario import BaseScenario
-            >>> from vmas.simulator.utils import Color
+            >>> import torch
             >>> class Scenario(BaseScenario):
-            >>>     def reset_world_at(self, env_index: int = None)
+            >>>     def reset_world_at(self, env_index)
             ...        for i, agent in enumerate(self.world.agents):
             ...            agent.set_pos(
             ...                torch.tensor(
             ...                     [-0.2 + 0.1 * i, 1.0],
             ...                     dtype=torch.float32,
             ...                     device=self.world.device,
             ...                ),
@@ -157,120 +198,206 @@
             ...                torch.tensor(
             ...                     [torch.pi / 4 if i % 2 else -torch.pi / 4],
             ...                     dtype=torch.float32,
             ...                     device=self.world.device,
             ...                ),
             ...                 batch_index=env_index,
             ...            )
+
+        Spawning at random positions
+
+        Examples:
+            >>> from vmas.simulator.scenario import BaseScenario
+            >>> from vmas.simulator.utils import ScenarioUtils
+            >>> class Scenario(BaseScenario):
+            >>>     def reset_world_at(self, env_index)
+            >>>         ScenarioUtils.spawn_entities_randomly(
+            ...             self.world.agents + self.world.landmarks,
+            ...             self.world,
+            ...             env_index,
+            ...             min_dist_between_entities=0.02,
+            ...             x_bounds=(-1.0,1.0),
+            ...             y_bounds=(-1.0,1.0),
+            ...         )
+
         """
         raise NotImplementedError()
 
     @abstractmethod
     def observation(self, agent: Agent) -> AGENT_OBS_TYPE:
-        """
-        This function computes the observations for 'agent' in a vectorized way
-        The returned tensor should contain the observations for 'agent' in all envs and should have
-        shape (n_envs, n_agent_obs)
+        """This function computes the observations for ``agent`` in a vectorized way.
+
+        The returned tensor should contain the observations for ``agent`` in all envs and should have
+        shape ``(self.world.batch_dim, n_agent_obs)``, or be a dict with leaves following that shape.
 
-        Implementors can access the world at 'self.world'
+        Implementors can access the world at :class:`world`.
 
-        To increase performance, tensors created should have the device set, like:
-        torch.tensor(..., device=self.world.device)
+        To increase performance, torch tensors should be created with the device already set, like:
+        ``torch.tensor(..., device=self.world.device)``
+
+        Args:
+            agent (Agent): the agent to compute the observations for
+
+        Returns:
+             Union[torch.Tensor, Dict[str, torch.Tensor]]: the observation
+
+        Examples:
+            >>> from vmas.simulator.scenario import BaseScenario
+            >>> import torch
+            >>> class Scenario(BaseScenario):
+            >>>     def observation(self, agent):
+            ...         # get positions of all landmarks in this agent's reference frame
+            ...         landmark_rel_poses = []
+            ...         for landmark in self.world.landmarks:
+            ...             landmark_rel_poses.append(landmark.state.pos - agent.state.pos)
+            ...         return torch.cat([agent.state.pos, agent.state.vel, *landmark_rel_poses], dim=-1)
+
+        You can also return observations in a dictionary
 
-        :param agent: Agent batch to compute observation of
-        :return observation: Tensor of shape (n_envs, n_agent_obs)
         Examples:
-            >>> from vmas.simulator.core import Agent, World, Landmark, Sphere, Box
             >>> from vmas.simulator.scenario import BaseScenario
             >>> from vmas.simulator.utils import Color
-            >>> def observation(self, agent: Agent):
-            ...      # get positions of all entities in this agent's reference frame
-            ...      entity_pos = []
-            ...      for entity in self.world.landmarks:
-            ...          entity_pos.append(entity.state.pos - agent.state.pos)
-            ...      return torch.cat([agent.state.vel, *entity_pos], dim=-1)
+            >>> class Scenario(BaseScenario):
+            >>>     def observation(self, agent):
+            ...         return {"pos": agent.state.pos, "vel": agent.state.vel}
+
         """
 
         raise NotImplementedError()
 
     @abstractmethod
     def reward(self, agent: Agent) -> AGENT_REWARD_TYPE:
-        """
-        This function computes the reward for 'agent' in a vectorized way
-        The returned tensor should contain the reward for 'agent' in all envs and should have
-        shape (n_envs)
+        """This function computes the reward for ``agent`` in a vectorized way.
+
+        The returned tensor should contain the reward for ``agent`` in all envs and should have
+        shape ``(self.world.batch_dim)`` and dtype ``torch.float``.
+
+        Implementors can access the world at :class:`world`.
+
+        To increase performance, torch tensors should be created with the device already set, like:
+        ``torch.tensor(..., device=self.world.device)``
 
-        Implementors can access the world at 'self.world'
+        Args:
+            agent (Agent): the agent to compute the reward for
 
-        To increase performance, tensors created should have the device set, like:
-        torch.tensor(..., device=self.world.device)
+        Returns:
+             torch.Tensor: reward tensor of shape ``(self.world.batch_dim)``
 
-        :param agent: Agent batch to compute reward of
-        :return observation: Tensor of shape (n_envs)
         Examples:
-            >>> from vmas.simulator.core import Agent, World, Landmark, Sphere, Box
             >>> from vmas.simulator.scenario import BaseScenario
-            >>> from vmas.simulator.utils import Color
-            >>> def observation(self, agent: Agent):
-            ...      # reward every agent proportionally to distance from first landmark
-            ...      dist2 = torch.sum(
-            ...          torch.square(agent.state.pos - self.world.landmarks[0].state.pos), dim=-1
-            ...      )
-            ...      return -dist2
+            >>> import torch
+            >>> class Scenario(BaseScenario):
+            >>>     def reward(self, agent):
+            ...         # reward every agent proportionally to distance from first landmark
+            ...         rew = -torch.linalg.vector_norm(agent.state.pos - self.world.landmarks[0].state.pos, dim=-1)
+            ...         return rew
         """
         raise NotImplementedError()
 
     def done(self):
-        """
-        This function computes the done flag for each env in a vectorized way
-        The returned tensor should contain the 'done' for all envs and should have
-        shape (n_envs)
+        """This function computes the done flag for each env in a vectorized way.
 
-        Implementors can access the world at 'self.world'
+        The returned tensor should contain the ``done`` for all envs and should have
+        shape ``(n_envs)`` and dtype ``torch.bool``.
 
-        To increase performance, tensors created should have the device set, like:
-        torch.tensor(..., device=self.world.device)
+        Implementors can access the world at :class:`world`.
 
-        :return dones: Bool tensor of shape (n_envs)
+        To increase performance, torch tensors should be created with the device already set, like:
+        ``torch.tensor(..., device=self.world.device)``
+
+        By default, this function returns all ``False`` s.
+
+        The scenario can still be done if ``max_steps`` has been set at envirtonment construction.
+
+        Returns:
+            torch.Tensor: done tensor of shape ``(self.world.batch_dim)``
+
+        Examples:
+            >>> from vmas.simulator.scenario import BaseScenario
+            >>> import torch
+            >>> class Scenario(BaseScenario):
+            >>>     def done(self):
+            ...         # retrun done when all agents have battery level lower than a threshold
+            ...         return torch.stack([a.battery_level < threshold for a in self.world.agents], dim=-1).all(-1)
         """
         return torch.tensor([False], device=self.world.device).expand(
             self.world.batch_dim
         )
 
     def info(self, agent: Agent) -> AGENT_INFO_TYPE:
-        """
-        This function computes the info dict for 'agent' in a vectorized way
+        """This function computes the info dict for ``agent`` in a vectorized way.
+
         The returned dict should have a key for each info of interest and the corresponding value should
-        be a tensor of shape (n_envs, info_size)
+        be a tensor of shape ``(n_envs, info_size)``
+
+        By default this function returns an empty dictionary.
 
-        Implementors can access the world at 'self.world'
+        Implementors can access the world at :class:`world`.
 
-        To increase performance, tensors created should have the device set, like:
-        torch.tensor(..., device=self.world.device)
+        To increase performance, torch tensors should be created with the device already set, like:
+        ``torch.tensor(..., device=self.world.device)``
 
-        :param agent: Agent batch to compute info of
-        :return: info: A dict with a key for each info of interest, and a tensor value  of shape (n_envs, info_size)
+        Args:
+            agent (Agent): the agent to compute the info for
+
+        Returns:
+             Union[torch.Tensor, Dict[str, torch.Tensor]]: the info
         """
         return {}
 
     def extra_render(self, env_index: int = 0) -> "List[Geom]":
         """
         This function facilitates additional user/scenario-level rendering for a specific environment index.
+
         The returned list is a list of geometries. It is the user's responsibility to set attributes such as color,
         position and rotation.
 
-        :param env_index: index of the environment to render.
-        :return: A list of geometries to render for the current time step.
+        Args:
+            env_index (int, optional): index of the environment to render. Defaults to ``0``.
+
+        Returns: A list of geometries to render for the current time step.
+
+        Examples:
+            >>> from vmas.simulator.utils import Color
+            >>> from vmas.simulator.scenario import BaseScenario
+            >>> class Scenario(BaseScenario):
+            >>>     def extra_render(self, env_index):
+            >>>         from vmas.simulator import rendering
+            >>>         color = Color.BLACK.value
+            >>>         line = rendering.Line(
+            ...            (self.world.agents[0].state.pos[env_index]),
+            ...            (self.world.agents[1].state.pos[env_index]),
+            ...            width=1,
+            ...         )
+            >>>         xform = rendering.Transform()
+            >>>         line.add_attr(xform)
+            >>>         line.set_color(*color)
+            >>>         return [line]
         """
         return []
 
     def process_action(self, agent: Agent):
-        """
-        This function can be overridden to process the agent actions before the simulation step.
-        It has access to the world through the `self.world` attribute
+        """This function can be overridden to process the agent actions before the simulation step.
+
+        It has access to the world through the :class:`world` attribute
 
         It can also be used for any other type of computation that has to happen after
-         the input actions have been set but before the simulation step
+        the input actions have been set but before the simulation step.
+
+        For example here you can manage additional actions before passing them to the dynamics.
+
+        Args:
+            agent (Agent): the agent process the action of
+
+        Examples:
+            >>> from vmas.simulator.scenario import BaseScenario
+            >>> from vmas.simulator.utils import TorchUtils
+            >>> class Scenario(BaseScenario):
+            >>>     def process_action(self, agent):
+            >>>         # Clamp square to circle
+            >>>         agent.action.u = TorchUtils.clamp_with_norm(agent.action.u, agent.u_range)
+            >>>         # Can use a PID controller
+            >>>         agent.controller.process_force()
+            >>>         return
 
-        :param agent: the agent whose actions have to be processed.
         """
-        pass
+        return
```

### Comparing `vmas-1.4.0/vmas/simulator/secrcode.ttf` & `vmas-1.4.1/vmas/simulator/secrcode.ttf`

 * *Files identical despite different names*

### Comparing `vmas-1.4.0/vmas/simulator/sensors.py` & `vmas-1.4.1/vmas/simulator/sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-#  Copyright (c) 2022-2023.
+#  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 
 from __future__ import annotations
 
 import typing
 from abc import ABC, abstractmethod
-from typing import List, Union, Callable
+from typing import Callable, List, Union
 
 import torch
 
 import vmas.simulator.core
 import vmas.simulator.utils
 
 if typing.TYPE_CHECKING:
```

### Comparing `vmas-1.4.0/vmas/simulator/utils.py` & `vmas-1.4.1/vmas/simulator/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #  Copyright (c) 2022-2024.
 #  ProrokLab (https://www.proroklab.org/)
 #  All rights reserved.
 import importlib
 import os
 from abc import ABC, abstractmethod
 from enum import Enum
-from typing import List, Tuple, Union, Dict, Sequence
+from typing import Dict, List, Sequence, Tuple, Union
 
 import numpy as np
 import torch
 from torch import Tensor
 
 _has_matplotlib = importlib.util.find_spec("matplotlib") is not None
 
 if _has_matplotlib:
     from matplotlib import cm
 
 X = 0
 Y = 1
 Z = 2
 ALPHABET = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
-VIEWER_MIN_ZOOM = 1.2
+VIEWER_DEFAULT_ZOOM = 1.2
 INITIAL_VIEWER_SIZE = (700, 700)
 LINE_MIN_DIST = 4 / 6e2
 COLLISION_FORCE = 100
 JOINT_FORCE = 130
 
 DRAG = 0.25
 LINEAR_FRICTION = 0.0
@@ -70,15 +70,15 @@
         os.environ["PYGLET_HEADLESS_DEVICE"] = (
             available_devices.split(",")[0]
             if len(available_devices) > 1
             else available_devices
         )
 
 
-class Observable(ABC):
+class Observable:
     def __init__(self):
         self._observers = []
 
     def subscribe(self, observer):
         self._observers.append(observer)
 
     def notify_observers(self, *args, **kwargs):
@@ -214,14 +214,20 @@
         elif isinstance(value, Dict):
             for val in value.values():
                 TorchUtils.recursive_require_grad_(val)
         else:
             for val in value:
                 TorchUtils.recursive_require_grad_(val)
 
+    @staticmethod
+    def where_from_index(env_index, new_value, old_value):
+        mask = torch.zeros_like(old_value, dtype=torch.bool, device=old_value.device)
+        mask[env_index] = True
+        return torch.where(mask, new_value, old_value)
+
 
 class ScenarioUtils:
     @staticmethod
     def spawn_entities_randomly(
         entities,
         world,
         env_index: int,
```

### Comparing `vmas-1.4.0/vmas.egg-info/SOURCES.txt` & `vmas-1.4.1/vmas.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+tests/test_vmas.py
 vmas/__init__.py
 vmas/interactive_rendering.py
 vmas/make_env.py
 vmas.egg-info/PKG-INFO
 vmas.egg-info/SOURCES.txt
 vmas.egg-info/dependency_links.txt
 vmas.egg-info/requires.txt
@@ -36,14 +37,15 @@
 vmas/scenarios/transport.py
 vmas/scenarios/wheel.py
 vmas/scenarios/wind_flocking.py
 vmas/scenarios/debug/__init__.py
 vmas/scenarios/debug/asym_joint.py
 vmas/scenarios/debug/circle_trajectory.py
 vmas/scenarios/debug/diff_drive.py
+vmas/scenarios/debug/drone.py
 vmas/scenarios/debug/goal.py
 vmas/scenarios/debug/het_mass.py
 vmas/scenarios/debug/kinematic_bicycle.py
 vmas/scenarios/debug/line_trajectory.py
 vmas/scenarios/debug/pollock.py
 vmas/scenarios/debug/vel_control.py
 vmas/scenarios/debug/waterfall.py
@@ -68,14 +70,15 @@
 vmas/simulator/sensors.py
 vmas/simulator/utils.py
 vmas/simulator/controllers/__init__.py
 vmas/simulator/controllers/velocity_controller.py
 vmas/simulator/dynamics/__init__.py
 vmas/simulator/dynamics/common.py
 vmas/simulator/dynamics/diff_drive.py
+vmas/simulator/dynamics/drone.py
 vmas/simulator/dynamics/holonomic.py
 vmas/simulator/dynamics/holonomic_with_rot.py
 vmas/simulator/dynamics/kinematic_bicycle.py
 vmas/simulator/environment/__init__.py
 vmas/simulator/environment/environment.py
 vmas/simulator/environment/gym.py
 vmas/simulator/environment/rllib.py
```

