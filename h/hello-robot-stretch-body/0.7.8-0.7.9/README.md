# Comparing `tmp/hello_robot_stretch_body-0.7.8.tar.gz` & `tmp/hello_robot_stretch_body-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_robot_stretch_body-0.7.8.tar", last modified: Thu Feb 15 02:18:01 2024, max compression
+gzip compressed data, was "hello_robot_stretch_body-0.7.9.tar", last modified: Fri Feb 16 19:34:44 2024, max compression
```

## Comparing `hello_robot_stretch_body-0.7.8.tar` & `hello_robot_stretch_body-0.7.9.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-02-15 02:18:01.196343 hello_robot_stretch_body-0.7.8/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      918 2024-02-14 01:41:40.000000 hello_robot_stretch_body-0.7.8/LICENSE.md
--rw-r--r--   0 hello-robot  (1000) hello-robot  (1000)     4176 2024-02-15 02:18:01.196343 hello_robot_stretch_body-0.7.8/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2262 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/README.md
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      255 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/deploy.sh
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-02-15 02:18:01.196343 hello_robot_stretch_body-0.7.8/hello_robot_stretch_body.egg-info/
--rw-r--r--   0 hello-robot  (1000) hello-robot  (1000)     4176 2024-02-15 02:18:01.000000 hello_robot_stretch_body-0.7.8/hello_robot_stretch_body.egg-info/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2183 2024-02-15 02:18:01.000000 hello_robot_stretch_body-0.7.8/hello_robot_stretch_body.egg-info/SOURCES.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2024-02-15 02:18:01.000000 hello_robot_stretch_body-0.7.8/hello_robot_stretch_body.egg-info/dependency_links.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      671 2024-02-15 02:18:01.000000 hello_robot_stretch_body-0.7.8/hello_robot_stretch_body.egg-info/requires.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       18 2024-02-15 02:18:01.000000 hello_robot_stretch_body-0.7.8/hello_robot_stretch_body.egg-info/top_level.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2024-02-15 02:18:01.196343 hello_robot_stretch_body-0.7.8/setup.cfg
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2238 2024-02-14 01:41:40.000000 hello_robot_stretch_body-0.7.8/setup.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-02-15 02:18:01.192343 hello_robot_stretch_body-0.7.8/stretch_body/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       34 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/stretch_body/__init__.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      970 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/stretch_body/arm.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    35481 2024-02-14 01:41:40.000000 hello_robot_stretch_body-0.7.8/stretch_body/base.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3304 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/stretch_body/cobbs_framing.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6086 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/stretch_body/device.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    43947 2024-02-14 01:41:40.000000 hello_robot_stretch_body-0.7.8/stretch_body/dynamixel_XL430.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    12266 2024-02-14 01:41:40.000000 hello_robot_stretch_body-0.7.8/stretch_body/dynamixel_X_chain.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    55686 2024-02-15 02:16:26.000000 hello_robot_stretch_body-0.7.8/stretch_body/dynamixel_hello_XL430.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4319 2024-02-14 20:13:53.000000 hello_robot_stretch_body-0.7.8/stretch_body/end_of_arm.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5376 2024-02-14 01:41:40.000000 hello_robot_stretch_body-0.7.8/stretch_body/end_of_arm_tools.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    13538 2024-01-25 23:19:08.000000 hello_robot_stretch_body-0.7.8/stretch_body/gamepad_controller.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    21655 2024-01-25 23:19:08.000000 hello_robot_stretch_body-0.7.8/stretch_body/gamepad_joints.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    20912 2024-02-14 01:15:58.000000 hello_robot_stretch_body-0.7.8/stretch_body/gamepad_teleop.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3321 2024-02-14 01:41:40.000000 hello_robot_stretch_body-0.7.8/stretch_body/gripper_conversion.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3055 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/stretch_body/head.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    24871 2024-01-26 02:54:53.000000 hello_robot_stretch_body-0.7.8/stretch_body/hello_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1019 2023-12-20 15:46:51.000000 hello_robot_stretch_body-0.7.8/stretch_body/lift.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    41124 2024-01-25 23:19:08.000000 hello_robot_stretch_body-0.7.8/stretch_body/pimu.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    36339 2024-02-14 01:41:40.000000 hello_robot_stretch_body-0.7.8/stretch_body/prismatic_joint.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    26912 2024-02-14 01:41:40.000000 hello_robot_stretch_body-0.7.8/stretch_body/robot.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    18836 2024-02-14 01:41:40.000000 hello_robot_stretch_body-0.7.8/stretch_body/robot_collision.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6859 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/stretch_body/robot_monitor.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     9740 2024-02-14 01:41:40.000000 hello_robot_stretch_body-0.7.8/stretch_body/robot_params.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    33115 2024-02-14 01:41:40.000000 hello_robot_stretch_body-0.7.8/stretch_body/robot_params_RE1V0.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    27190 2024-02-14 01:41:40.000000 hello_robot_stretch_body-0.7.8/stretch_body/robot_params_RE2V0.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    30877 2024-02-14 01:41:40.000000 hello_robot_stretch_body-0.7.8/stretch_body/robot_params_SE3.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4504 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/stretch_body/robot_trace.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    12072 2024-02-02 03:26:44.000000 hello_robot_stretch_body-0.7.8/stretch_body/scope.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    65668 2024-01-25 23:19:08.000000 hello_robot_stretch_body-0.7.8/stretch_body/stepper.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4885 2024-02-14 01:41:40.000000 hello_robot_stretch_body-0.7.8/stretch_body/stretch_gripper.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    29097 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/stretch_body/trajectories.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    45535 2023-12-20 15:46:51.000000 hello_robot_stretch_body-0.7.8/stretch_body/transport.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      206 2024-02-15 02:17:32.000000 hello_robot_stretch_body-0.7.8/stretch_body/version.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    20436 2024-01-26 18:29:16.000000 hello_robot_stretch_body-0.7.8/stretch_body/wacc.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2549 2024-02-14 23:43:21.000000 hello_robot_stretch_body-0.7.8/stretch_body/wrist_pitch.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2236 2024-02-15 02:16:26.000000 hello_robot_stretch_body-0.7.8/stretch_body/wrist_roll.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2020 2024-01-25 23:19:08.000000 hello_robot_stretch_body-0.7.8/stretch_body/wrist_yaw.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-02-15 02:18:01.196343 hello_robot_stretch_body-0.7.8/test/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       82 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/README.md
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/__init__.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-02-15 02:18:01.196343 hello_robot_stretch_body-0.7.8/test/rates/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5866 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/rates/test_arm_command_at_max_rate.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1748 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/rates/test_comm_loads.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1727 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/rates/test_pimu_sync_100hz.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4497 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/rates/test_robot_command_at_max_rate.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1112 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/rates/test_robot_dxl_rates.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3835 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/rates/test_robot_nondxl_rates.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1668 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/rates/test_single_nondxl_rates.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5087 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/rates/test_thread_locks.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5384 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_arm.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6813 2023-12-20 15:46:51.000000 hello_robot_stretch_body-0.7.8/test/test_base.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     9977 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_collisions.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3198 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_device.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1111 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_dxl_comms.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5424 2023-12-20 15:46:51.000000 hello_robot_stretch_body-0.7.8/test/test_dxl_sine_vel.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3747 2023-12-20 15:46:51.000000 hello_robot_stretch_body-0.7.8/test/test_dxl_vel.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     7882 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_dynamixel_XL430.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    14520 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_dynamixel_hello_XL430.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1435 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_end_of_arm.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1914 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_end_of_arm_tools.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3833 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_head.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    23286 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_hello_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4761 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_lift.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2069 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_pimu.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     8989 2023-12-20 15:46:51.000000 hello_robot_stretch_body-0.7.8/test/test_robot.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2391 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_robot_params.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    26117 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_steppers.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1657 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_stretch_gripper.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6263 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_sync.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4381 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_timing_stats.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    29747 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_trajectories.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3918 2023-12-16 09:17:01.000000 hello_robot_stretch_body-0.7.8/test/test_wrist_yaw.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-02-16 19:34:44.263486 hello_robot_stretch_body-0.7.9/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      918 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/LICENSE.md
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2774 2024-02-16 19:34:44.263486 hello_robot_stretch_body-0.7.9/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2262 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/README.md
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      255 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/deploy.sh
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-02-16 19:34:44.259486 hello_robot_stretch_body-0.7.9/hello_robot_stretch_body.egg-info/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2774 2024-02-16 19:34:44.000000 hello_robot_stretch_body-0.7.9/hello_robot_stretch_body.egg-info/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2183 2024-02-16 19:34:44.000000 hello_robot_stretch_body-0.7.9/hello_robot_stretch_body.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2024-02-16 19:34:44.000000 hello_robot_stretch_body-0.7.9/hello_robot_stretch_body.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      671 2024-02-16 19:34:44.000000 hello_robot_stretch_body-0.7.9/hello_robot_stretch_body.egg-info/requires.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       18 2024-02-16 19:34:44.000000 hello_robot_stretch_body-0.7.9/hello_robot_stretch_body.egg-info/top_level.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2024-02-16 19:34:44.263486 hello_robot_stretch_body-0.7.9/setup.cfg
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2238 2024-02-12 21:49:18.000000 hello_robot_stretch_body-0.7.9/setup.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-02-16 19:34:44.263486 hello_robot_stretch_body-0.7.9/stretch_body/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       34 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/__init__.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      970 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/arm.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    35481 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/base.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3304 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/cobbs_framing.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6086 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/device.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    43947 2024-02-16 19:32:56.000000 hello_robot_stretch_body-0.7.9/stretch_body/dynamixel_XL430.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    12266 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/dynamixel_X_chain.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    55686 2024-02-16 19:32:56.000000 hello_robot_stretch_body-0.7.9/stretch_body/dynamixel_hello_XL430.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4319 2024-02-16 19:32:56.000000 hello_robot_stretch_body-0.7.9/stretch_body/end_of_arm.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5376 2024-02-16 19:32:56.000000 hello_robot_stretch_body-0.7.9/stretch_body/end_of_arm_tools.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    13538 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/gamepad_controller.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    21663 2024-02-16 19:34:09.000000 hello_robot_stretch_body-0.7.9/stretch_body/gamepad_joints.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    20912 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/gamepad_teleop.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3321 2024-02-12 21:49:18.000000 hello_robot_stretch_body-0.7.9/stretch_body/gripper_conversion.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3055 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/head.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    24871 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/hello_utils.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1019 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/lift.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    41124 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/pimu.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    36339 2024-02-13 17:07:35.000000 hello_robot_stretch_body-0.7.9/stretch_body/prismatic_joint.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    26912 2024-02-16 19:32:56.000000 hello_robot_stretch_body-0.7.9/stretch_body/robot.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    18836 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/robot_collision.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6859 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/robot_monitor.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     9740 2024-02-12 21:49:18.000000 hello_robot_stretch_body-0.7.9/stretch_body/robot_params.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    33115 2024-02-16 19:32:56.000000 hello_robot_stretch_body-0.7.9/stretch_body/robot_params_RE1V0.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    27190 2024-02-16 19:32:56.000000 hello_robot_stretch_body-0.7.9/stretch_body/robot_params_RE2V0.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    30877 2024-02-16 19:32:56.000000 hello_robot_stretch_body-0.7.9/stretch_body/robot_params_SE3.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4504 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/robot_trace.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    12072 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/scope.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    65668 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/stepper.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4885 2024-02-12 21:49:18.000000 hello_robot_stretch_body-0.7.9/stretch_body/stretch_gripper.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    29097 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/trajectories.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    45535 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/transport.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      206 2024-02-16 19:33:28.000000 hello_robot_stretch_body-0.7.9/stretch_body/version.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    20436 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/wacc.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2549 2024-02-16 19:32:56.000000 hello_robot_stretch_body-0.7.9/stretch_body/wrist_pitch.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2236 2024-02-16 19:32:56.000000 hello_robot_stretch_body-0.7.9/stretch_body/wrist_roll.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2020 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/stretch_body/wrist_yaw.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-02-16 19:34:44.263486 hello_robot_stretch_body-0.7.9/test/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       82 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/README.md
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/__init__.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-02-16 19:34:44.263486 hello_robot_stretch_body-0.7.9/test/rates/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5866 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/rates/test_arm_command_at_max_rate.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1748 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/rates/test_comm_loads.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1727 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/rates/test_pimu_sync_100hz.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4497 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/rates/test_robot_command_at_max_rate.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1112 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/rates/test_robot_dxl_rates.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3835 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/rates/test_robot_nondxl_rates.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1668 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/rates/test_single_nondxl_rates.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5087 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/rates/test_thread_locks.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5384 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_arm.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6813 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_base.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     9977 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_collisions.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3198 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_device.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1111 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_dxl_comms.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5424 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_dxl_sine_vel.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3747 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_dxl_vel.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     7882 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_dynamixel_XL430.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    14520 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_dynamixel_hello_XL430.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1435 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_end_of_arm.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1914 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_end_of_arm_tools.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3833 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_head.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    23286 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_hello_utils.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4761 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_lift.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2069 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_pimu.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     8989 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_robot.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2391 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_robot_params.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    26117 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_steppers.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1657 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_stretch_gripper.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6263 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_sync.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4381 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_timing_stats.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    29747 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_trajectories.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3918 2024-02-07 18:04:04.000000 hello_robot_stretch_body-0.7.9/test/test_wrist_yaw.py
```

### Comparing `hello_robot_stretch_body-0.7.8/LICENSE.md` & `hello_robot_stretch_body-0.7.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/README.md` & `hello_robot_stretch_body-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/hello_robot_stretch_body.egg-info/SOURCES.txt` & `hello_robot_stretch_body-0.7.9/hello_robot_stretch_body.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/setup.py` & `hello_robot_stretch_body-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/arm.py` & `hello_robot_stretch_body-0.7.9/stretch_body/arm.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/base.py` & `hello_robot_stretch_body-0.7.9/stretch_body/base.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/cobbs_framing.py` & `hello_robot_stretch_body-0.7.9/stretch_body/cobbs_framing.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/device.py` & `hello_robot_stretch_body-0.7.9/stretch_body/device.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/dynamixel_XL430.py` & `hello_robot_stretch_body-0.7.9/stretch_body/dynamixel_XL430.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/dynamixel_X_chain.py` & `hello_robot_stretch_body-0.7.9/stretch_body/dynamixel_X_chain.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/dynamixel_hello_XL430.py` & `hello_robot_stretch_body-0.7.9/stretch_body/dynamixel_hello_XL430.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/end_of_arm.py` & `hello_robot_stretch_body-0.7.9/stretch_body/end_of_arm.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/end_of_arm_tools.py` & `hello_robot_stretch_body-0.7.9/stretch_body/end_of_arm_tools.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/gamepad_controller.py` & `hello_robot_stretch_body-0.7.9/stretch_body/gamepad_controller.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/gamepad_joints.py` & `hello_robot_stretch_body-0.7.9/stretch_body/gamepad_joints.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,17 +197,17 @@
 class CommandLift:
     def __init__(self):
         """Lift motion command class.
         """
         self.params = RobotParams().get_params()[1]['lift']
         self.dead_zone = 0.0001
         self._prev_set_vel_ts = None
-        self.max_linear_vel = self.params['motion']['max']['vel_m']
+        self.max_linear_vel = self.params['motion']['default']['vel_m']
         self.precision_mode = False
-        self.acc = self.params['motion']['max']['accel_m']
+        self.acc = self.params['motion']['default']['accel_m']
         
         # Precision mode params
         self.start_pos = None
         self.target_position = self.start_pos
         self.precision_kp = 0.5 # Very Precise: 0.5
         self.precision_max_vel = 0.04 # m/s Very Precise: 0.02 m/s
         self.stopped_for_precision = False
```

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/gamepad_teleop.py` & `hello_robot_stretch_body-0.7.9/stretch_body/gamepad_teleop.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/gripper_conversion.py` & `hello_robot_stretch_body-0.7.9/stretch_body/gripper_conversion.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/head.py` & `hello_robot_stretch_body-0.7.9/stretch_body/head.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/hello_utils.py` & `hello_robot_stretch_body-0.7.9/stretch_body/hello_utils.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/lift.py` & `hello_robot_stretch_body-0.7.9/stretch_body/lift.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/pimu.py` & `hello_robot_stretch_body-0.7.9/stretch_body/pimu.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/prismatic_joint.py` & `hello_robot_stretch_body-0.7.9/stretch_body/prismatic_joint.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/robot.py` & `hello_robot_stretch_body-0.7.9/stretch_body/robot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/robot_collision.py` & `hello_robot_stretch_body-0.7.9/stretch_body/robot_collision.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/robot_monitor.py` & `hello_robot_stretch_body-0.7.9/stretch_body/robot_monitor.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/robot_params.py` & `hello_robot_stretch_body-0.7.9/stretch_body/robot_params.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/robot_params_RE1V0.py` & `hello_robot_stretch_body-0.7.9/stretch_body/robot_params_RE1V0.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/robot_params_RE2V0.py` & `hello_robot_stretch_body-0.7.9/stretch_body/robot_params_RE2V0.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/robot_params_SE3.py` & `hello_robot_stretch_body-0.7.9/stretch_body/robot_params_SE3.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/robot_trace.py` & `hello_robot_stretch_body-0.7.9/stretch_body/robot_trace.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/scope.py` & `hello_robot_stretch_body-0.7.9/stretch_body/scope.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/stepper.py` & `hello_robot_stretch_body-0.7.9/stretch_body/stepper.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/stretch_gripper.py` & `hello_robot_stretch_body-0.7.9/stretch_body/stretch_gripper.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/trajectories.py` & `hello_robot_stretch_body-0.7.9/stretch_body/trajectories.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/transport.py` & `hello_robot_stretch_body-0.7.9/stretch_body/transport.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/wacc.py` & `hello_robot_stretch_body-0.7.9/stretch_body/wacc.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/wrist_pitch.py` & `hello_robot_stretch_body-0.7.9/stretch_body/wrist_pitch.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/wrist_roll.py` & `hello_robot_stretch_body-0.7.9/stretch_body/wrist_roll.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/stretch_body/wrist_yaw.py` & `hello_robot_stretch_body-0.7.9/stretch_body/wrist_yaw.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/rates/test_arm_command_at_max_rate.py` & `hello_robot_stretch_body-0.7.9/test/rates/test_arm_command_at_max_rate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/rates/test_comm_loads.py` & `hello_robot_stretch_body-0.7.9/test/rates/test_comm_loads.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/rates/test_pimu_sync_100hz.py` & `hello_robot_stretch_body-0.7.9/test/rates/test_pimu_sync_100hz.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/rates/test_robot_command_at_max_rate.py` & `hello_robot_stretch_body-0.7.9/test/rates/test_robot_command_at_max_rate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/rates/test_robot_dxl_rates.py` & `hello_robot_stretch_body-0.7.9/test/rates/test_robot_dxl_rates.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/rates/test_robot_nondxl_rates.py` & `hello_robot_stretch_body-0.7.9/test/rates/test_robot_nondxl_rates.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/rates/test_single_nondxl_rates.py` & `hello_robot_stretch_body-0.7.9/test/rates/test_single_nondxl_rates.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/rates/test_thread_locks.py` & `hello_robot_stretch_body-0.7.9/test/rates/test_thread_locks.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_arm.py` & `hello_robot_stretch_body-0.7.9/test/test_arm.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_base.py` & `hello_robot_stretch_body-0.7.9/test/test_base.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_collisions.py` & `hello_robot_stretch_body-0.7.9/test/test_collisions.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_device.py` & `hello_robot_stretch_body-0.7.9/test/test_device.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_dxl_comms.py` & `hello_robot_stretch_body-0.7.9/test/test_dxl_comms.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_dxl_sine_vel.py` & `hello_robot_stretch_body-0.7.9/test/test_dxl_sine_vel.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_dxl_vel.py` & `hello_robot_stretch_body-0.7.9/test/test_dxl_vel.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_dynamixel_XL430.py` & `hello_robot_stretch_body-0.7.9/test/test_dynamixel_XL430.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_dynamixel_hello_XL430.py` & `hello_robot_stretch_body-0.7.9/test/test_dynamixel_hello_XL430.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_end_of_arm.py` & `hello_robot_stretch_body-0.7.9/test/test_end_of_arm.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_end_of_arm_tools.py` & `hello_robot_stretch_body-0.7.9/test/test_end_of_arm_tools.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_head.py` & `hello_robot_stretch_body-0.7.9/test/test_head.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_hello_utils.py` & `hello_robot_stretch_body-0.7.9/test/test_hello_utils.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_lift.py` & `hello_robot_stretch_body-0.7.9/test/test_lift.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_pimu.py` & `hello_robot_stretch_body-0.7.9/test/test_pimu.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_robot.py` & `hello_robot_stretch_body-0.7.9/test/test_robot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_robot_params.py` & `hello_robot_stretch_body-0.7.9/test/test_robot_params.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_steppers.py` & `hello_robot_stretch_body-0.7.9/test/test_steppers.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_stretch_gripper.py` & `hello_robot_stretch_body-0.7.9/test/test_stretch_gripper.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_sync.py` & `hello_robot_stretch_body-0.7.9/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_timing_stats.py` & `hello_robot_stretch_body-0.7.9/test/test_timing_stats.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_trajectories.py` & `hello_robot_stretch_body-0.7.9/test/test_trajectories.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.7.8/test/test_wrist_yaw.py` & `hello_robot_stretch_body-0.7.9/test/test_wrist_yaw.py`

 * *Files identical despite different names*

