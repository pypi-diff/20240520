# Comparing `tmp/hello_robot_stretch_body_tools-0.7.8.tar.gz` & `tmp/hello-robot-stretch-body-tools-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_robot_stretch_body_tools-0.7.8.tar", last modified: Tue May  7 04:08:58 2024, max compression
+gzip compressed data, was "hello-robot-stretch-body-tools-0.7.9.tar", last modified: Mon May 20 17:16:21 2024, max compression
```

## Comparing `hello_robot_stretch_body_tools-0.7.8.tar` & `hello-robot-stretch-body-tools-0.7.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 hello-user  (1001) hello-user  (1001)        0 2024-05-07 04:08:58.344573 hello_robot_stretch_body_tools-0.7.8/
--rw-rw-r--   0 hello-user  (1001) hello-user  (1001)      923 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/LICENSE.md
--rw-rw-r--   0 hello-user  (1001) hello-user  (1001)     2885 2024-05-07 04:08:58.344573 hello_robot_stretch_body_tools-0.7.8/PKG-INFO
--rw-rw-r--   0 hello-user  (1001) hello-user  (1001)     2405 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/README.md
-drwxrwxr-x   0 hello-user  (1001) hello-user  (1001)        0 2024-05-07 04:08:58.344573 hello_robot_stretch_body_tools-0.7.8/bin/
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     2339 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_about.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      790 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_about_text.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      366 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_arm_home.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     3240 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_arm_jog.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      484 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_audio_test.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     6251 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_base_jog.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     8350 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_camera_streams_check.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)    15767 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_configure_tool.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      406 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_dex_wrist_float.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     3324 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_dex_wrist_jog.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      309 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_free_robot_process.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      318 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_gamepad_teleop.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      439 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_gripper_home.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     2672 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_gripper_jog.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     4384 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_hardware_echo.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     3998 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_head_jog.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      385 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_lift_home.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     3245 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_lift_jog.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     2105 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_params.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     1965 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_pimu_jog.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     8759 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_pimu_scope.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)    17359 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_realsense_visualizer.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)    11374 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_respeaker_test.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     1049 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_battery_check.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     5570 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_collision_visualizer.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      766 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_dynamixel_reboot.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     5296 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_home.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     4461 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_keyboard_teleop.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      597 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_monitor.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      448 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_stow.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      197 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_system_check.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     8829 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_urdf_visualizer.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     2333 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_rp_lidar_jog.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)    25882 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_system_check.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)    17476 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_trajectory_jog.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     1874 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_version.sh
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     1336 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_wacc_jog.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     2882 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_wacc_scope.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     2447 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_wrist_pitch_jog.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     2450 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_wrist_roll_jog.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      404 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_wrist_yaw_home.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     2446 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_wrist_yaw_jog.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)    25967 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_xbox_controller_teleop.py
--rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      267 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/deploy.sh
-drwxrwxr-x   0 hello-user  (1001) hello-user  (1001)        0 2024-05-07 04:08:58.344573 hello_robot_stretch_body_tools-0.7.8/hello_robot_stretch_body_tools.egg-info/
--rw-rw-r--   0 hello-user  (1001) hello-user  (1001)     2885 2024-05-07 04:08:58.000000 hello_robot_stretch_body_tools-0.7.8/hello_robot_stretch_body_tools.egg-info/PKG-INFO
--rw-rw-r--   0 hello-user  (1001) hello-user  (1001)     2937 2024-05-07 04:08:58.000000 hello_robot_stretch_body_tools-0.7.8/hello_robot_stretch_body_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 hello-user  (1001) hello-user  (1001)        1 2024-05-07 04:08:58.000000 hello_robot_stretch_body_tools-0.7.8/hello_robot_stretch_body_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 hello-user  (1001) hello-user  (1001)      366 2024-05-07 04:08:58.000000 hello_robot_stretch_body_tools-0.7.8/hello_robot_stretch_body_tools.egg-info/requires.txt
--rw-rw-r--   0 hello-user  (1001) hello-user  (1001)        5 2024-05-07 04:08:58.000000 hello_robot_stretch_body_tools-0.7.8/hello_robot_stretch_body_tools.egg-info/top_level.txt
--rw-rw-r--   0 hello-user  (1001) hello-user  (1001)       38 2024-05-07 04:08:58.344573 hello_robot_stretch_body_tools-0.7.8/setup.cfg
--rw-rw-r--   0 hello-user  (1001) hello-user  (1001)     1533 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/setup.py
-drwxrwxr-x   0 hello-user  (1001) hello-user  (1001)        0 2024-05-07 04:08:58.344573 hello_robot_stretch_body_tools-0.7.8/test/
--rw-rw-r--   0 hello-user  (1001) hello-user  (1001)       34 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/test/__init__.py
--rw-rw-r--   0 hello-user  (1001) hello-user  (1001)     2173 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/test/test_tools_launch.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-05-20 17:16:21.761938 hello-robot-stretch-body-tools-0.7.9/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      923 2024-02-14 01:41:40.000000 hello-robot-stretch-body-tools-0.7.9/LICENSE.md
+-rw-r--r--   0 hello-robot  (1000) hello-robot  (1000)     3676 2024-05-20 17:16:21.761938 hello-robot-stretch-body-tools-0.7.9/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2405 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/README.md
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-05-20 17:16:21.757938 hello-robot-stretch-body-tools-0.7.9/bin/
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2339 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_about.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      790 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_about_text.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      366 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_arm_home.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3240 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_arm_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      484 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_audio_test.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6251 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_base_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     8350 2024-03-05 22:36:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_camera_streams_check.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    15990 2024-05-20 17:05:52.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_configure_tool.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      406 2024-01-25 23:19:08.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_dex_wrist_float.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3324 2024-02-14 01:41:40.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_dex_wrist_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      309 2024-05-20 17:05:47.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_free_robot_process.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      318 2024-02-14 01:15:58.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_gamepad_teleop.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      439 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_gripper_home.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2672 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_gripper_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4384 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_hardware_echo.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3998 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_head_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      385 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_lift_home.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3245 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_lift_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2105 2024-02-14 01:41:40.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_params.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1965 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_pimu_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     8759 2023-12-20 15:46:51.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_pimu_scope.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    17359 2024-05-09 18:15:46.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_realsense_visualizer.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    11374 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_respeaker_test.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1049 2024-05-20 17:05:47.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_robot_battery_check.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5570 2024-02-27 22:48:09.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_robot_collision_visualizer.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      766 2023-12-20 15:46:51.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_robot_dynamixel_reboot.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5296 2024-05-20 17:05:47.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_robot_home.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4461 2024-05-20 17:05:47.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_robot_keyboard_teleop.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      597 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_robot_monitor.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      448 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_robot_stow.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      197 2024-02-27 22:48:09.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_robot_system_check.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     8829 2023-12-20 15:46:51.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_robot_urdf_visualizer.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2333 2024-05-09 18:15:46.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_rp_lidar_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    25882 2024-05-20 17:05:47.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_system_check.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    17476 2024-02-13 19:45:20.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_trajectory_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1874 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_version.sh
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1336 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_wacc_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2882 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_wacc_scope.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2447 2024-01-25 23:19:08.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_wrist_pitch_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2450 2024-01-25 23:19:08.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_wrist_roll_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      404 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_wrist_yaw_home.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2446 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_wrist_yaw_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    25967 2023-12-20 15:46:51.000000 hello-robot-stretch-body-tools-0.7.9/bin/stretch_xbox_controller_teleop.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      267 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/deploy.sh
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-05-20 17:16:21.761938 hello-robot-stretch-body-tools-0.7.9/hello_robot_stretch_body_tools.egg-info/
+-rw-r--r--   0 hello-robot  (1000) hello-robot  (1000)     3676 2024-05-20 17:16:21.000000 hello-robot-stretch-body-tools-0.7.9/hello_robot_stretch_body_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2937 2024-05-20 17:16:21.000000 hello-robot-stretch-body-tools-0.7.9/hello_robot_stretch_body_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2024-05-20 17:16:21.000000 hello-robot-stretch-body-tools-0.7.9/hello_robot_stretch_body_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      366 2024-05-20 17:16:21.000000 hello-robot-stretch-body-tools-0.7.9/hello_robot_stretch_body_tools.egg-info/requires.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        5 2024-05-20 17:16:21.000000 hello-robot-stretch-body-tools-0.7.9/hello_robot_stretch_body_tools.egg-info/top_level.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2024-05-20 17:16:21.761938 hello-robot-stretch-body-tools-0.7.9/setup.cfg
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1533 2024-05-20 17:06:16.000000 hello-robot-stretch-body-tools-0.7.9/setup.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-05-20 17:16:21.761938 hello-robot-stretch-body-tools-0.7.9/test/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       34 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/test/__init__.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2173 2023-12-16 09:17:01.000000 hello-robot-stretch-body-tools-0.7.9/test/test_tools_launch.py
```

### Comparing `hello_robot_stretch_body_tools-0.7.8/LICENSE.md` & `hello-robot-stretch-body-tools-0.7.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/PKG-INFO` & `hello-robot-stretch-body-tools-0.7.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: hello_robot_stretch_body_tools
-Version: 0.7.8
-Summary: Stretch Body Tools
-Home-page: https://github.com/hello-robot/stretch_body
-Author: Hello Robot Inc
-Author-email: support@hello-robot.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: Apache Software License
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 Stretch Body Command Line Tools
 ===============================
 
 This package provides Python tools that work with the Hello Robot Stretch Body package. These tools perform common tasks when working with Stretch (e.g. homing and stowing), and serve as tutorial code for working on various parts of the robot. This package comes pre-installed on Stretch robots. A tutorial for using this package can be found [on the docs](https://docs.hello-robot.com/0.2/stretch-tutorials/stretch_body/tutorial_command_line_tools/).
 
 Installing
 ----------
@@ -64,9 +49,7 @@
 
 Now, make desired edits to the [stretch_robot_home.py](./bin/stretch_robot_home.py) file. Executing the script on the command-line will now run your modified version.
 
 Deploying
 ---------
 
 Increment the version number and run the `deploy.sh` script. Verify the new release is reflected [on PyPI](https://pypi.org/project/hello-robot-stretch-body-tools/).
-
-
```

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_about.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_about.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_about_text.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_about_text.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_arm_jog.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_arm_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_base_jog.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_base_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_camera_streams_check.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_camera_streams_check.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_configure_tool.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_configure_tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,22 +81,22 @@
     cli_device.logger.info(f'Your software is currently configured for the {Fore.CYAN + stretch_tool + Style.RESET_ALL} tool')
 
     # check if current tool is supported
     if stretch_tool not in supported_tools:
         cli_device.logger.info(f"But {Fore.CYAN + stretch_tool + Style.RESET_ALL} isn't a supported tool for your robot")
         cli_device.logger.debug(f"The supported tools for your robot are: {Fore.YELLOW + str(supported_tools) + Style.RESET_ALL}")
         return True
-
     # check if the existing hardware, num dxls, matches the current tool
     tool_numdxls_d405_map = {
         'tool_none': (1, False),
         'tool_stretch_gripper': (2, False),
         'tool_stretch_dex_wrist': (4, False),
         'eoa_wrist_dw3_tool_nil': (3, True),
         'eoa_wrist_dw3_tool_sg3': (4, True),
+        'eoa_wrist_dw3_tool_tablet_12in': (3, True),
     }
     expected_num_wrist_dxls, expected_d405_present = tool_numdxls_d405_map.get(stretch_tool, (-1, False))
     if num_wrist_dxls != expected_num_wrist_dxls:
         cli_device.logger.info(f"But the wrist chain has the wrong number of motors")
         cli_device.logger.debug(f"Num Dxls: {num_wrist_dxls}, Expected Num Dxls: {expected_num_wrist_dxls}")
         return True
 
@@ -116,25 +116,25 @@
     matches = supported_tools
     cli_device.logger.debug(f"Starting with the supported tools for your model: {Fore.YELLOW + str(matches) + Style.RESET_ALL}")
 
     # filter by num dxls
     numdxls_tool_map = {
         1: ['tool_none'],
         2: ['tool_stretch_gripper'],
-        3: ['eoa_wrist_dw3_tool_nil'],
+        3: ['eoa_wrist_dw3_tool_nil', 'eoa_wrist_dw3_tool_tablet_12in'],
         4: ['tool_stretch_dex_wrist', 'eoa_wrist_dw3_tool_sg3']
     }
     numdxls_match = numdxls_tool_map.get(num_wrist_dxls, [])
     cli_device.logger.debug(f"These tools match based on {num_wrist_dxls} number of wrist dxls: {Fore.YELLOW + str(numdxls_match) + Style.RESET_ALL}")
     matches = list(set(matches) & set(numdxls_match))
     cli_device.logger.debug(f"Filtering based on this brings the matches to: {Fore.YELLOW + str(matches) + Style.RESET_ALL}")
 
     # filter by d405 present
     d405_tool_map = {
-        False: ['tool_none', 'tool_stretch_gripper', 'tool_stretch_dex_wrist', 'eoa_wrist_dw3_tool_nil'],
+        False: ['tool_none', 'tool_stretch_gripper', 'tool_stretch_dex_wrist', 'eoa_wrist_dw3_tool_nil', 'eoa_wrist_dw3_tool_tablet_12in'],
         True: ['eoa_wrist_dw3_tool_sg3'],
     }
     d405_match = d405_tool_map.get(d405_present, [])
     cli_device.logger.debug(f"These tools match based on present={d405_present} gripper camera: {Fore.YELLOW + str(d405_match) + Style.RESET_ALL}")
     matches = list(set(matches) & set(d405_match))
     cli_device.logger.debug(f"Filtering based on this brings the matches to: {Fore.YELLOW + str(matches) + Style.RESET_ALL}")
 
@@ -214,14 +214,15 @@
     # update the robot parameters for the next tool
     if stretch_model == 'RE1V0': # Stretch RE1
         tool_feedforward_map = {
             'tool_none': 0.4,
             'tool_stretch_gripper': 0.4,
             'tool_stretch_dex_wrist': 0.75,
             'eoa_wrist_dw3_tool_nil': 0.75,
+            'eoa_wrist_dw3_tool_tablet_12in': 0.75,
             'eoa_wrist_dw3_tool_sg3': 0.75,
         }
         feedforward_value = tool_feedforward_map.get(target_tool_name, 0.8)
         cli_device.logger.debug(f'For model={stretch_model} and tool={target_tool_name}, choosing i_feedforward={feedforward_value}')
 
         tool_yaml = {
             'robot': {'tool': target_tool_name},
@@ -230,14 +231,15 @@
         }
     else: # Stretch 2 and Stretch 3
         tool_feedforward_map = {
             'tool_none': 1.2,
             'tool_stretch_gripper': 1.2,
             'tool_stretch_dex_wrist': 1.8,
             'eoa_wrist_dw3_tool_nil': 1.8,
+            'eoa_wrist_dw3_tool_tablet_12in': 1.8,
             'eoa_wrist_dw3_tool_sg3': 1.8,
         }
         feedforward_value = tool_feedforward_map.get(target_tool_name, 1.9)
         cli_device.logger.debug(f'For model={stretch_model} and tool={target_tool_name}, choosing i_feedforward={feedforward_value}')
 
         tool_yaml = {
             'robot': {'tool': target_tool_name},
```

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_dex_wrist_jog.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_dex_wrist_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_gripper_jog.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_gripper_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_hardware_echo.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_hardware_echo.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_head_jog.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_head_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_lift_jog.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_lift_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_params.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_params.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_pimu_jog.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_pimu_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_pimu_scope.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_pimu_scope.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_realsense_visualizer.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_realsense_visualizer.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_respeaker_test.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_respeaker_test.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_battery_check.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_robot_battery_check.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_collision_visualizer.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_robot_collision_visualizer.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_dynamixel_reboot.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_robot_dynamixel_reboot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_home.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_robot_home.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_keyboard_teleop.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_robot_keyboard_teleop.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_monitor.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_robot_monitor.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_urdf_visualizer.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_robot_urdf_visualizer.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_rp_lidar_jog.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_rp_lidar_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_system_check.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_system_check.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_trajectory_jog.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_trajectory_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_version.sh` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_version.sh`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_wacc_jog.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_wacc_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_wacc_scope.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_wacc_scope.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_wrist_pitch_jog.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_wrist_pitch_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_wrist_roll_jog.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_wrist_roll_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_wrist_yaw_jog.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_wrist_yaw_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/bin/stretch_xbox_controller_teleop.py` & `hello-robot-stretch-body-tools-0.7.9/bin/stretch_xbox_controller_teleop.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/hello_robot_stretch_body_tools.egg-info/SOURCES.txt` & `hello-robot-stretch-body-tools-0.7.9/hello_robot_stretch_body_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.8/setup.py` & `hello-robot-stretch-body-tools-0.7.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     long_description = fh.read()
 
 script_path='./bin'
 ex_scripts = glob.glob(script_path+'/*.py') + glob.glob(script_path+'/*.sh')
 stretch_scripts=[f for f in ex_scripts if isfile(f)]
 
 setuptools.setup(
-    name="hello_robot_stretch_body_tools",
-    version="0.7.8",
+    name="hello-robot-stretch-body-tools",
+    version="0.7.9",
     author="Hello Robot Inc",
     author_email="support@hello-robot.com",
     description="Stretch Body Tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hello-robot/stretch_body",
     scripts = stretch_scripts,
```

### Comparing `hello_robot_stretch_body_tools-0.7.8/test/test_tools_launch.py` & `hello-robot-stretch-body-tools-0.7.9/test/test_tools_launch.py`

 * *Files identical despite different names*

