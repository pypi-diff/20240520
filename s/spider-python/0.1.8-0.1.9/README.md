# Comparing `tmp/spider-python-0.1.8.tar.gz` & `tmp/spider-python-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spider-python-0.1.8.tar", last modified: Mon Dec 18 08:54:07 2023, max compression
+gzip compressed data, was "spider-python-0.1.9.tar", last modified: Wed Dec 20 11:03:53 2023, max compression
```

## Comparing `spider-python-0.1.8.tar` & `spider-python-0.1.9.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.446800 spider-python-0.1.8/
--rw-rw-rw-   0        0        0     1096 2023-11-30 09:35:45.000000 spider-python-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     1015 2023-12-18 08:54:07.446800 spider-python-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      542 2023-12-11 08:47:39.000000 spider-python-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-12-18 08:54:07.446800 spider-python-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1090 2023-12-18 08:53:58.000000 spider-python-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.389354 spider-python-0.1.8/spider/
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.390472 spider-python-0.1.8/spider/RL/
--rw-rw-rw-   0        0        0        0 2023-09-11 10:57:17.000000 spider-python-0.1.8/spider/RL/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.393765 spider-python-0.1.8/spider/RL/agents/
--rw-rw-rw-   0        0        0    18282 2023-11-07 11:54:04.000000 spider-python-0.1.8/spider/RL/agents/Base_Agent.py
--rw-rw-rw-   0        0        0     5238 2023-09-08 11:16:20.000000 spider-python-0.1.8/spider/RL/agents/DQNAgent.py
--rw-rw-rw-   0        0        0     5055 2023-03-09 02:28:00.000000 spider-python-0.1.8/spider/RL/agents/HER_Base.py
--rw-rw-rw-   0        0        0     7134 2023-09-11 09:46:06.000000 spider-python-0.1.8/spider/RL/agents/MBRLAgent.py
--rw-rw-rw-   0        0        0    15144 2023-12-10 02:13:07.000000 spider-python-0.1.8/spider/RL/agents/Trainer.py
--rw-rw-rw-   0        0        0       98 2023-09-08 09:10:17.000000 spider-python-0.1.8/spider/RL/agents/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.393765 spider-python-0.1.8/spider/RL/dataset/
--rw-rw-rw-   0        0        0     1789 2023-09-06 03:11:41.000000 spider-python-0.1.8/spider/RL/dataset/ExperienceBuffer.py
--rw-rw-rw-   0        0        0       54 2023-08-10 08:26:43.000000 spider-python-0.1.8/spider/RL/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.397767 spider-python-0.1.8/spider/RL/reward/
--rw-rw-rw-   0        0        0      391 2023-12-14 08:18:12.000000 spider-python-0.1.8/spider/RL/reward/BasicReward.py
--rw-rw-rw-   0        0        0     5398 2023-12-14 08:27:48.000000 spider-python-0.1.8/spider/RL/reward/FstateControlReward.py
--rw-rw-rw-   0        0        0     5254 2023-12-14 08:27:48.000000 spider-python-0.1.8/spider/RL/reward/FstateTrajectoryReward.py
--rw-rw-rw-   0        0        0     1732 2023-12-14 08:17:23.000000 spider-python-0.1.8/spider/RL/reward/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.397767 spider-python-0.1.8/spider/RL/state/
--rw-rw-rw-   0        0        0      413 2023-08-10 07:32:59.000000 spider-python-0.1.8/spider/RL/state/ElementState.py
--rw-rw-rw-   0        0        0       75 2023-07-06 19:05:13.000000 spider-python-0.1.8/spider/RL/state/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.399712 spider-python-0.1.8/spider/RL/transition/
--rw-rw-rw-   0        0        0     4128 2023-09-10 13:48:40.000000 spider-python-0.1.8/spider/RL/transition/DeterministicTransition.py
--rw-rw-rw-   0        0        0     3207 2023-07-06 19:12:46.000000 spider-python-0.1.8/spider/RL/transition/GaussianTransition.py
--rw-rw-rw-   0        0        0      128 2023-09-08 07:10:19.000000 spider-python-0.1.8/spider/RL/transition/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.405785 spider-python-0.1.8/spider/RL/utilities/
--rw-rw-rw-   0        0        0     2792 2023-03-09 02:28:01.000000 spider-python-0.1.8/spider/RL/utilities/Deepmind_RMS_Prop.py
--rw-rw-rw-   0        0        0     5048 2023-03-09 02:28:01.000000 spider-python-0.1.8/spider/RL/utilities/Memory_Shaper.py
--rw-rw-rw-   0        0        0      718 2023-03-09 02:28:01.000000 spider-python-0.1.8/spider/RL/utilities/OU_Noise.py
--rw-rw-rw-   0        0        0     4005 2023-03-09 02:28:01.000000 spider-python-0.1.8/spider/RL/utilities/Parallel_Experience_Generator.py
--rw-rw-rw-   0        0        0     2529 2023-03-09 02:28:01.000000 spider-python-0.1.8/spider/RL/utilities/Tensorboard.py
--rw-rw-rw-   0        0        0     6080 2023-03-09 02:28:01.000000 spider-python-0.1.8/spider/RL/utilities/Utility_Functions.py
--rw-rw-rw-   0        0        0        0 2023-11-30 09:22:26.000000 spider-python-0.1.8/spider/RL/utilities/__init__.py
--rw-rw-rw-   0        0        0     8732 2023-11-07 11:54:04.000000 spider-python-0.1.8/spider/RL/utilities/kinematic_model.py
--rw-rw-rw-   0        0        0     5709 2023-07-06 11:48:15.000000 spider-python-0.1.8/spider/RL/utilities/predmlp.py
--rw-rw-rw-   0        0        0      248 2023-12-01 04:19:34.000000 spider-python-0.1.8/spider/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.405785 spider-python-0.1.8/spider/constraints/
--rw-rw-rw-   0        0        0     3766 2023-09-12 07:54:02.000000 spider-python-0.1.8/spider/constraints/ConstraintCollection.py
--rw-rw-rw-   0        0        0      533 2023-09-12 03:43:26.000000 spider-python-0.1.8/spider/constraints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.409870 spider-python-0.1.8/spider/constraints/constraint_checker/
--rw-rw-rw-   0        0        0      209 2023-09-11 10:16:15.000000 spider-python-0.1.8/spider/constraints/constraint_checker/BaseConstraintChecker.py
--rw-rw-rw-   0        0        0     1339 2023-09-12 04:29:10.000000 spider-python-0.1.8/spider/constraints/constraint_checker/CartConstraintChecker.py
--rw-rw-rw-   0        0        0      365 2023-09-11 10:31:46.000000 spider-python-0.1.8/spider/constraints/constraint_checker/ControlConstraintChecker.py
--rw-rw-rw-   0        0        0        0 2023-09-11 10:15:01.000000 spider-python-0.1.8/spider/constraints/constraint_checker/FrenetConstraintChecker.py
--rw-rw-rw-   0        0        0      194 2023-09-12 04:10:01.000000 spider-python-0.1.8/spider/constraints/constraint_checker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.411101 spider-python-0.1.8/spider/constraints/constraint_formulator/
--rw-rw-rw-   0        0        0        0 2023-09-11 10:01:49.000000 spider-python-0.1.8/spider/constraints/constraint_formulator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.411101 spider-python-0.1.8/spider/data/
--rw-rw-rw-   0        0        0        0 2023-12-10 13:21:45.000000 spider-python-0.1.8/spider/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.415716 spider-python-0.1.8/spider/elements/
--rw-rw-rw-   0        0        0     5336 2023-08-09 10:26:22.000000 spider-python-0.1.8/spider/elements/Box.py
--rw-rw-rw-   0        0        0      418 2023-11-13 08:15:02.000000 spider-python-0.1.8/spider/elements/__init__.py
--rw-rw-rw-   0        0        0    38167 2023-12-18 04:42:04.000000 spider-python-0.1.8/spider/elements/curves.py
--rw-rw-rw-   0        0        0      183 2023-02-22 16:59:46.000000 spider-python-0.1.8/spider/elements/graph.py
--rw-rw-rw-   0        0        0    14968 2023-12-02 16:11:02.000000 spider-python-0.1.8/spider/elements/grid.py
--rw-rw-rw-   0        0        0     3970 2023-12-14 07:28:36.000000 spider-python-0.1.8/spider/elements/map.py
--rw-rw-rw-   0        0        0      615 2023-03-10 14:40:55.000000 spider-python-0.1.8/spider/elements/obstacles.py
--rw-rw-rw-   0        0        0     5431 2023-12-10 01:44:31.000000 spider-python-0.1.8/spider/elements/trajectory.py
--rw-rw-rw-   0        0        0     2104 2023-09-06 03:56:56.000000 spider-python-0.1.8/spider/elements/vector.py
--rw-rw-rw-   0        0        0     3109 2023-11-07 10:59:22.000000 spider-python-0.1.8/spider/elements/vehicle.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.418223 spider-python-0.1.8/spider/evaluator/
--rw-rw-rw-   0        0        0     1869 2023-09-17 10:38:24.000000 spider-python-0.1.8/spider/evaluator/CostEvaluator.py
--rw-rw-rw-   0        0        0       66 2023-07-06 18:00:47.000000 spider-python-0.1.8/spider/evaluator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.418223 spider-python-0.1.8/spider/interface/
--rw-rw-rw-   0        0        0        0 2023-10-12 07:55:41.000000 spider-python-0.1.8/spider/interface/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.418223 spider-python-0.1.8/spider/interface/carla/
--rw-rw-rw-   0        0        0        0 2023-10-12 07:56:01.000000 spider-python-0.1.8/spider/interface/carla/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.421245 spider-python-0.1.8/spider/interface/highway_env/
--rw-rw-rw-   0        0        0       33 2023-11-07 09:39:00.000000 spider-python-0.1.8/spider/interface/highway_env/HighwayEnvBenchmark.py
--rw-rw-rw-   0        0        0    10382 2023-12-14 08:09:05.000000 spider-python-0.1.8/spider/interface/highway_env/HighwayEnvInterface.py
--rw-rw-rw-   0        0        0        0 2023-10-12 07:55:55.000000 spider-python-0.1.8/spider/interface/highway_env/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.422251 spider-python-0.1.8/spider/interface/nuplan/
--rw-rw-rw-   0        0        0        0 2023-10-12 07:56:11.000000 spider-python-0.1.8/spider/interface/nuplan/__init__.py
--rw-rw-rw-   0        0        0      544 2023-02-22 15:10:10.000000 spider-python-0.1.8/spider/main.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.422251 spider-python-0.1.8/spider/motion_planning/
--rw-rw-rw-   0        0        0        0 2023-12-01 04:16:28.000000 spider-python-0.1.8/spider/motion_planning/__init__.py
--rw-rw-rw-   0        0        0     9948 2023-12-10 02:13:07.000000 spider-python-0.1.8/spider/motion_planning/optimize.py
--rw-rw-rw-   0        0        0     1970 2023-11-07 11:54:04.000000 spider-python-0.1.8/spider/param.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.423496 spider-python-0.1.8/spider/path_planning/
--rw-rw-rw-   0        0        0        0 2023-12-01 04:16:19.000000 spider-python-0.1.8/spider/path_planning/__init__.py
--rw-rw-rw-   0        0        0      548 2023-03-10 15:22:15.000000 spider-python-0.1.8/spider/path_planning/hybridAstar.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.426433 spider-python-0.1.8/spider/planner_zoo/
--rw-rw-rw-   0        0        0      122 2023-07-02 09:51:30.000000 spider-python-0.1.8/spider/planner_zoo/BasicPlanner.py
--rw-rw-rw-   0        0        0    19206 2023-12-09 13:59:42.000000 spider-python-0.1.8/spider/planner_zoo/BezierPlanner.py
--rw-rw-rw-   0        0        0    19216 2023-12-07 11:12:25.000000 spider-python-0.1.8/spider/planner_zoo/LatticePlanner.py
--rw-rw-rw-   0        0        0    17756 2023-12-07 11:12:25.000000 spider-python-0.1.8/spider/planner_zoo/MBRLPlanner.py
--rw-rw-rw-   0        0        0    28419 2023-12-14 07:51:12.000000 spider-python-0.1.8/spider/planner_zoo/MFRLPlanner.py
--rw-rw-rw-   0        0        0        0 2023-07-01 17:02:06.000000 spider-python-0.1.8/spider/planner_zoo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.428584 spider-python-0.1.8/spider/sampler/
--rw-rw-rw-   0        0        0      197 2023-07-01 18:04:01.000000 spider-python-0.1.8/spider/sampler/BasicSampler.py
--rw-rw-rw-   0        0        0     4731 2023-12-10 02:13:07.000000 spider-python-0.1.8/spider/sampler/Combiner.py
--rw-rw-rw-   0        0        0     1637 2023-12-14 08:37:19.000000 spider-python-0.1.8/spider/sampler/PolynomialSampler.py
--rw-rw-rw-   0        0        0        0 2023-07-01 17:40:10.000000 spider-python-0.1.8/spider/sampler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.430662 spider-python-0.1.8/spider/utils/
--rw-rw-rw-   0        0        0      847 2023-03-07 20:19:43.000000 spider-python-0.1.8/spider/utils/Visualize.py
--rw-rw-rw-   0        0        0        0 2023-07-04 12:07:55.000000 spider-python-0.1.8/spider/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.435070 spider-python-0.1.8/spider/utils/collision/
--rw-rw-rw-   0        0        0      765 2023-02-23 15:38:15.000000 spider-python-0.1.8/spider/utils/collision/AABB.py
--rw-rw-rw-   0        0        0     2876 2023-10-16 03:51:55.000000 spider-python-0.1.8/spider/utils/collision/CollisionChecker.py
--rw-rw-rw-   0        0        0     4031 2023-12-10 02:13:08.000000 spider-python-0.1.8/spider/utils/collision/CollisionConstraints.py
--rw-rw-rw-   0        0        0      953 2023-03-10 14:51:14.000000 spider-python-0.1.8/spider/utils/collision/Disks.py
--rw-rw-rw-   0        0        0     1663 2023-07-04 11:57:07.000000 spider-python-0.1.8/spider/utils/collision/SAT.py
--rw-rw-rw-   0        0        0      132 2023-10-13 13:33:03.000000 spider-python-0.1.8/spider/utils/collision/__init__.py
--rw-rw-rw-   0        0        0     3432 2023-07-04 13:06:54.000000 spider-python-0.1.8/spider/utils/geometry.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.435070 spider-python-0.1.8/spider/utils/predict/
--rw-rw-rw-   0        0        0       56 2023-12-02 14:27:18.000000 spider-python-0.1.8/spider/utils/predict/__init__.py
--rw-rw-rw-   0        0        0      327 2023-02-23 08:29:00.000000 spider-python-0.1.8/spider/utils/predict/linear.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.438576 spider-python-0.1.8/spider/utils/transform/
--rw-rw-rw-   0        0        0        0 2023-07-04 11:42:25.000000 spider-python-0.1.8/spider/utils/transform/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-22 17:27:41.000000 spider-python-0.1.8/spider/utils/transform/box.py
--rw-rw-rw-   0        0        0    15532 2023-12-18 03:43:58.000000 spider-python-0.1.8/spider/utils/transform/frenet.py
--rw-rw-rw-   0        0        0        0 2023-02-22 16:51:22.000000 spider-python-0.1.8/spider/utils/transform/gps.py
--rw-rw-rw-   0        0        0    12587 2023-12-02 16:08:57.000000 spider-python-0.1.8/spider/utils/transform/grid.py
--rw-rw-rw-   0        0        0        0 2023-02-22 16:51:06.000000 spider-python-0.1.8/spider/utils/transform/polar.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.440274 spider-python-0.1.8/spider/vehicle_model/
--rw-rw-rw-   0        0        0       50 2023-09-06 09:07:59.000000 spider-python-0.1.8/spider/vehicle_model/__init__.py
--rw-rw-rw-   0        0        0     2806 2023-12-10 02:13:07.000000 spider-python-0.1.8/spider/vehicle_model/bicycle.py
-drwxrwxrwx   0        0        0        0 2023-12-18 08:54:07.446800 spider-python-0.1.8/spider_python.egg-info/
--rw-rw-rw-   0        0        0     1015 2023-12-18 08:54:07.000000 spider-python-0.1.8/spider_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3267 2023-12-18 08:54:07.000000 spider-python-0.1.8/spider_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-18 08:54:07.000000 spider-python-0.1.8/spider_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-12-18 08:54:07.000000 spider-python-0.1.8/spider_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.689581 spider-python-0.1.9/
+-rw-rw-rw-   0        0        0     1096 2023-11-30 09:35:45.000000 spider-python-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1015 2023-12-20 11:03:53.689581 spider-python-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2023-12-11 08:47:39.000000 spider-python-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-12-20 11:03:53.689581 spider-python-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1090 2023-12-20 11:03:36.000000 spider-python-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.041909 spider-python-0.1.9/spider/
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.044153 spider-python-0.1.9/spider/RL/
+-rw-rw-rw-   0        0        0        0 2023-09-11 10:57:17.000000 spider-python-0.1.9/spider/RL/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.127249 spider-python-0.1.9/spider/RL/agents/
+-rw-rw-rw-   0        0        0    18282 2023-11-07 11:54:04.000000 spider-python-0.1.9/spider/RL/agents/Base_Agent.py
+-rw-rw-rw-   0        0        0     5238 2023-09-08 11:16:20.000000 spider-python-0.1.9/spider/RL/agents/DQNAgent.py
+-rw-rw-rw-   0        0        0     5055 2023-03-09 02:28:00.000000 spider-python-0.1.9/spider/RL/agents/HER_Base.py
+-rw-rw-rw-   0        0        0     7134 2023-09-11 09:46:06.000000 spider-python-0.1.9/spider/RL/agents/MBRLAgent.py
+-rw-rw-rw-   0        0        0    15144 2023-12-10 02:13:07.000000 spider-python-0.1.9/spider/RL/agents/Trainer.py
+-rw-rw-rw-   0        0        0       98 2023-09-08 09:10:17.000000 spider-python-0.1.9/spider/RL/agents/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.144064 spider-python-0.1.9/spider/RL/dataset/
+-rw-rw-rw-   0        0        0     1789 2023-09-06 03:11:41.000000 spider-python-0.1.9/spider/RL/dataset/ExperienceBuffer.py
+-rw-rw-rw-   0        0        0       54 2023-08-10 08:26:43.000000 spider-python-0.1.9/spider/RL/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.170712 spider-python-0.1.9/spider/RL/reward/
+-rw-rw-rw-   0        0        0      391 2023-12-14 08:18:12.000000 spider-python-0.1.9/spider/RL/reward/BasicReward.py
+-rw-rw-rw-   0        0        0     5398 2023-12-14 08:27:48.000000 spider-python-0.1.9/spider/RL/reward/FstateControlReward.py
+-rw-rw-rw-   0        0        0     5254 2023-12-14 08:27:48.000000 spider-python-0.1.9/spider/RL/reward/FstateTrajectoryReward.py
+-rw-rw-rw-   0        0        0     1732 2023-12-14 08:17:23.000000 spider-python-0.1.9/spider/RL/reward/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.187771 spider-python-0.1.9/spider/RL/state/
+-rw-rw-rw-   0        0        0      413 2023-08-10 07:32:59.000000 spider-python-0.1.9/spider/RL/state/ElementState.py
+-rw-rw-rw-   0        0        0       75 2023-07-06 19:05:13.000000 spider-python-0.1.9/spider/RL/state/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.225238 spider-python-0.1.9/spider/RL/transition/
+-rw-rw-rw-   0        0        0     4128 2023-09-10 13:48:40.000000 spider-python-0.1.9/spider/RL/transition/DeterministicTransition.py
+-rw-rw-rw-   0        0        0     3207 2023-07-06 19:12:46.000000 spider-python-0.1.9/spider/RL/transition/GaussianTransition.py
+-rw-rw-rw-   0        0        0      128 2023-09-08 07:10:19.000000 spider-python-0.1.9/spider/RL/transition/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.306393 spider-python-0.1.9/spider/RL/utilities/
+-rw-rw-rw-   0        0        0     2792 2023-03-09 02:28:01.000000 spider-python-0.1.9/spider/RL/utilities/Deepmind_RMS_Prop.py
+-rw-rw-rw-   0        0        0     5048 2023-03-09 02:28:01.000000 spider-python-0.1.9/spider/RL/utilities/Memory_Shaper.py
+-rw-rw-rw-   0        0        0      718 2023-03-09 02:28:01.000000 spider-python-0.1.9/spider/RL/utilities/OU_Noise.py
+-rw-rw-rw-   0        0        0     4005 2023-03-09 02:28:01.000000 spider-python-0.1.9/spider/RL/utilities/Parallel_Experience_Generator.py
+-rw-rw-rw-   0        0        0     2529 2023-03-09 02:28:01.000000 spider-python-0.1.9/spider/RL/utilities/Tensorboard.py
+-rw-rw-rw-   0        0        0     6080 2023-03-09 02:28:01.000000 spider-python-0.1.9/spider/RL/utilities/Utility_Functions.py
+-rw-rw-rw-   0        0        0        0 2023-11-30 09:22:26.000000 spider-python-0.1.9/spider/RL/utilities/__init__.py
+-rw-rw-rw-   0        0        0     8732 2023-11-07 11:54:04.000000 spider-python-0.1.9/spider/RL/utilities/kinematic_model.py
+-rw-rw-rw-   0        0        0     5709 2023-07-06 11:48:15.000000 spider-python-0.1.9/spider/RL/utilities/predmlp.py
+-rw-rw-rw-   0        0        0      248 2023-12-01 04:19:34.000000 spider-python-0.1.9/spider/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.327875 spider-python-0.1.9/spider/constraints/
+-rw-rw-rw-   0        0        0     3766 2023-09-12 07:54:02.000000 spider-python-0.1.9/spider/constraints/ConstraintCollection.py
+-rw-rw-rw-   0        0        0      533 2023-09-12 03:43:26.000000 spider-python-0.1.9/spider/constraints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.355608 spider-python-0.1.9/spider/constraints/constraint_checker/
+-rw-rw-rw-   0        0        0      209 2023-09-11 10:16:15.000000 spider-python-0.1.9/spider/constraints/constraint_checker/BaseConstraintChecker.py
+-rw-rw-rw-   0        0        0     1339 2023-09-12 04:29:10.000000 spider-python-0.1.9/spider/constraints/constraint_checker/CartConstraintChecker.py
+-rw-rw-rw-   0        0        0      365 2023-09-11 10:31:46.000000 spider-python-0.1.9/spider/constraints/constraint_checker/ControlConstraintChecker.py
+-rw-rw-rw-   0        0        0        0 2023-09-11 10:15:01.000000 spider-python-0.1.9/spider/constraints/constraint_checker/FrenetConstraintChecker.py
+-rw-rw-rw-   0        0        0      194 2023-09-12 04:10:01.000000 spider-python-0.1.9/spider/constraints/constraint_checker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.356494 spider-python-0.1.9/spider/constraints/constraint_formulator/
+-rw-rw-rw-   0        0        0        0 2023-09-11 10:01:49.000000 spider-python-0.1.9/spider/constraints/constraint_formulator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.356494 spider-python-0.1.9/spider/data/
+-rw-rw-rw-   0        0        0        0 2023-12-10 13:21:45.000000 spider-python-0.1.9/spider/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.446798 spider-python-0.1.9/spider/elements/
+-rw-rw-rw-   0        0        0     5336 2023-08-09 10:26:22.000000 spider-python-0.1.9/spider/elements/Box.py
+-rw-rw-rw-   0        0        0      418 2023-11-13 08:15:02.000000 spider-python-0.1.9/spider/elements/__init__.py
+-rw-rw-rw-   0        0        0    38144 2023-12-20 03:48:55.000000 spider-python-0.1.9/spider/elements/curves.py
+-rw-rw-rw-   0        0        0      183 2023-02-22 16:59:46.000000 spider-python-0.1.9/spider/elements/graph.py
+-rw-rw-rw-   0        0        0    14968 2023-12-02 16:11:02.000000 spider-python-0.1.9/spider/elements/grid.py
+-rw-rw-rw-   0        0        0     3970 2023-12-14 07:28:36.000000 spider-python-0.1.9/spider/elements/map.py
+-rw-rw-rw-   0        0        0      615 2023-03-10 14:40:55.000000 spider-python-0.1.9/spider/elements/obstacles.py
+-rw-rw-rw-   0        0        0     5431 2023-12-10 01:44:31.000000 spider-python-0.1.9/spider/elements/trajectory.py
+-rw-rw-rw-   0        0        0     2104 2023-09-06 03:56:56.000000 spider-python-0.1.9/spider/elements/vector.py
+-rw-rw-rw-   0        0        0     3109 2023-11-07 10:59:22.000000 spider-python-0.1.9/spider/elements/vehicle.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.457803 spider-python-0.1.9/spider/evaluator/
+-rw-rw-rw-   0        0        0     1869 2023-09-17 10:38:24.000000 spider-python-0.1.9/spider/evaluator/CostEvaluator.py
+-rw-rw-rw-   0        0        0       66 2023-07-06 18:00:47.000000 spider-python-0.1.9/spider/evaluator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.458786 spider-python-0.1.9/spider/interface/
+-rw-rw-rw-   0        0        0        0 2023-10-12 07:55:41.000000 spider-python-0.1.9/spider/interface/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.458786 spider-python-0.1.9/spider/interface/carla/
+-rw-rw-rw-   0        0        0        0 2023-10-12 07:56:01.000000 spider-python-0.1.9/spider/interface/carla/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.478975 spider-python-0.1.9/spider/interface/highway_env/
+-rw-rw-rw-   0        0        0       33 2023-11-07 09:39:00.000000 spider-python-0.1.9/spider/interface/highway_env/HighwayEnvBenchmark.py
+-rw-rw-rw-   0        0        0    10382 2023-12-14 08:09:05.000000 spider-python-0.1.9/spider/interface/highway_env/HighwayEnvInterface.py
+-rw-rw-rw-   0        0        0        0 2023-10-12 07:55:55.000000 spider-python-0.1.9/spider/interface/highway_env/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.478975 spider-python-0.1.9/spider/interface/nuplan/
+-rw-rw-rw-   0        0        0        0 2023-10-12 07:56:11.000000 spider-python-0.1.9/spider/interface/nuplan/__init__.py
+-rw-rw-rw-   0        0        0      544 2023-02-22 15:10:10.000000 spider-python-0.1.9/spider/main.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.486998 spider-python-0.1.9/spider/motion_planning/
+-rw-rw-rw-   0        0        0        0 2023-12-01 04:16:28.000000 spider-python-0.1.9/spider/motion_planning/__init__.py
+-rw-rw-rw-   0        0        0     9948 2023-12-10 02:13:07.000000 spider-python-0.1.9/spider/motion_planning/optimize.py
+-rw-rw-rw-   0        0        0     1970 2023-11-07 11:54:04.000000 spider-python-0.1.9/spider/param.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.499131 spider-python-0.1.9/spider/path_planning/
+-rw-rw-rw-   0        0        0        0 2023-12-01 04:16:19.000000 spider-python-0.1.9/spider/path_planning/__init__.py
+-rw-rw-rw-   0        0        0      548 2023-03-10 15:22:15.000000 spider-python-0.1.9/spider/path_planning/hybridAstar.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.520264 spider-python-0.1.9/spider/planner_zoo/
+-rw-rw-rw-   0        0        0      122 2023-07-02 09:51:30.000000 spider-python-0.1.9/spider/planner_zoo/BasicPlanner.py
+-rw-rw-rw-   0        0        0    19206 2023-12-09 13:59:42.000000 spider-python-0.1.9/spider/planner_zoo/BezierPlanner.py
+-rw-rw-rw-   0        0        0    19552 2023-12-20 04:06:00.000000 spider-python-0.1.9/spider/planner_zoo/LatticePlanner.py
+-rw-rw-rw-   0        0        0    17958 2023-12-20 04:06:00.000000 spider-python-0.1.9/spider/planner_zoo/MBRLPlanner.py
+-rw-rw-rw-   0        0        0    28619 2023-12-20 04:06:19.000000 spider-python-0.1.9/spider/planner_zoo/MFRLPlanner.py
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:02:06.000000 spider-python-0.1.9/spider/planner_zoo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.542539 spider-python-0.1.9/spider/sampler/
+-rw-rw-rw-   0        0        0      197 2023-07-01 18:04:01.000000 spider-python-0.1.9/spider/sampler/BasicSampler.py
+-rw-rw-rw-   0        0        0     4731 2023-12-10 02:13:07.000000 spider-python-0.1.9/spider/sampler/Combiner.py
+-rw-rw-rw-   0        0        0     1637 2023-12-14 08:37:19.000000 spider-python-0.1.9/spider/sampler/PolynomialSampler.py
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:40:10.000000 spider-python-0.1.9/spider/sampler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.554764 spider-python-0.1.9/spider/utils/
+-rw-rw-rw-   0        0        0      847 2023-03-07 20:19:43.000000 spider-python-0.1.9/spider/utils/Visualize.py
+-rw-rw-rw-   0        0        0        0 2023-07-04 12:07:55.000000 spider-python-0.1.9/spider/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.604932 spider-python-0.1.9/spider/utils/collision/
+-rw-rw-rw-   0        0        0      765 2023-02-23 15:38:15.000000 spider-python-0.1.9/spider/utils/collision/AABB.py
+-rw-rw-rw-   0        0        0     2876 2023-10-16 03:51:55.000000 spider-python-0.1.9/spider/utils/collision/CollisionChecker.py
+-rw-rw-rw-   0        0        0     4031 2023-12-10 02:13:08.000000 spider-python-0.1.9/spider/utils/collision/CollisionConstraints.py
+-rw-rw-rw-   0        0        0      953 2023-03-10 14:51:14.000000 spider-python-0.1.9/spider/utils/collision/Disks.py
+-rw-rw-rw-   0        0        0     1663 2023-07-04 11:57:07.000000 spider-python-0.1.9/spider/utils/collision/SAT.py
+-rw-rw-rw-   0        0        0      132 2023-10-13 13:33:03.000000 spider-python-0.1.9/spider/utils/collision/__init__.py
+-rw-rw-rw-   0        0        0     4332 2023-12-20 10:53:35.000000 spider-python-0.1.9/spider/utils/geometry.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.627690 spider-python-0.1.9/spider/utils/predict/
+-rw-rw-rw-   0        0        0       56 2023-12-02 14:27:18.000000 spider-python-0.1.9/spider/utils/predict/__init__.py
+-rw-rw-rw-   0        0        0      327 2023-02-23 08:29:00.000000 spider-python-0.1.9/spider/utils/predict/linear.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.652497 spider-python-0.1.9/spider/utils/transform/
+-rw-rw-rw-   0        0        0        0 2023-07-04 11:42:25.000000 spider-python-0.1.9/spider/utils/transform/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-22 17:27:41.000000 spider-python-0.1.9/spider/utils/transform/box.py
+-rw-rw-rw-   0        0        0    15796 2023-12-20 10:53:35.000000 spider-python-0.1.9/spider/utils/transform/frenet.py
+-rw-rw-rw-   0        0        0        0 2023-02-22 16:51:22.000000 spider-python-0.1.9/spider/utils/transform/gps.py
+-rw-rw-rw-   0        0        0    12587 2023-12-02 16:08:57.000000 spider-python-0.1.9/spider/utils/transform/grid.py
+-rw-rw-rw-   0        0        0        0 2023-02-22 16:51:06.000000 spider-python-0.1.9/spider/utils/transform/polar.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.662505 spider-python-0.1.9/spider/vehicle_model/
+-rw-rw-rw-   0        0        0       50 2023-09-06 09:07:59.000000 spider-python-0.1.9/spider/vehicle_model/__init__.py
+-rw-rw-rw-   0        0        0     2806 2023-12-10 02:13:07.000000 spider-python-0.1.9/spider/vehicle_model/bicycle.py
+drwxrwxrwx   0        0        0        0 2023-12-20 11:03:53.688252 spider-python-0.1.9/spider_python.egg-info/
+-rw-rw-rw-   0        0        0     1015 2023-12-20 11:03:52.000000 spider-python-0.1.9/spider_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3267 2023-12-20 11:03:52.000000 spider-python-0.1.9/spider_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-20 11:03:52.000000 spider-python-0.1.9/spider_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-12-20 11:03:52.000000 spider-python-0.1.9/spider_python.egg-info/top_level.txt
```

### Comparing `spider-python-0.1.8/LICENSE` & `spider-python-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/PKG-INFO` & `spider-python-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-python
-Version: 0.1.8
+Version: 0.1.9
 Summary: SPIDER -- Self-driving Planning and Intelligent Decision-making Engine with Reinforcement learning
 Home-page: https://github.com/ZelinQian/SPIDER
 Author: Zelin Qian
 Author-email: qzl22@mails.tsinghua.edu.cn
 License: MIT
 Description: SPIDER -- Self-driving Planning and Intelligent Decision-making Engine with Reinforcement learning
```

### Comparing `spider-python-0.1.8/README.md` & `spider-python-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/setup.py` & `spider-python-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="spider-python",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_packages(),
     install_requires=[
         # 在这里列出你的库所需的其他Python包
     ],
 
     author="Zelin Qian",
     author_email="qzl22@mails.tsinghua.edu.cn",
```

### Comparing `spider-python-0.1.8/spider/RL/agents/Base_Agent.py` & `spider-python-0.1.9/spider/RL/agents/Base_Agent.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/agents/DQNAgent.py` & `spider-python-0.1.9/spider/RL/agents/DQNAgent.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/agents/HER_Base.py` & `spider-python-0.1.9/spider/RL/agents/HER_Base.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/agents/MBRLAgent.py` & `spider-python-0.1.9/spider/RL/agents/MBRLAgent.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/agents/Trainer.py` & `spider-python-0.1.9/spider/RL/agents/Trainer.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/dataset/ExperienceBuffer.py` & `spider-python-0.1.9/spider/RL/dataset/ExperienceBuffer.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/reward/FstateControlReward.py` & `spider-python-0.1.9/spider/RL/reward/FstateControlReward.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/reward/FstateTrajectoryReward.py` & `spider-python-0.1.9/spider/RL/reward/FstateTrajectoryReward.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/reward/__init__.py` & `spider-python-0.1.9/spider/RL/reward/__init__.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/transition/DeterministicTransition.py` & `spider-python-0.1.9/spider/RL/transition/DeterministicTransition.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/transition/GaussianTransition.py` & `spider-python-0.1.9/spider/RL/transition/GaussianTransition.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/utilities/Deepmind_RMS_Prop.py` & `spider-python-0.1.9/spider/RL/utilities/Deepmind_RMS_Prop.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/utilities/Memory_Shaper.py` & `spider-python-0.1.9/spider/RL/utilities/Memory_Shaper.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/utilities/OU_Noise.py` & `spider-python-0.1.9/spider/RL/utilities/OU_Noise.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/utilities/Parallel_Experience_Generator.py` & `spider-python-0.1.9/spider/RL/utilities/Parallel_Experience_Generator.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/utilities/Tensorboard.py` & `spider-python-0.1.9/spider/RL/utilities/Tensorboard.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/utilities/Utility_Functions.py` & `spider-python-0.1.9/spider/RL/utilities/Utility_Functions.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/utilities/kinematic_model.py` & `spider-python-0.1.9/spider/RL/utilities/kinematic_model.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/RL/utilities/predmlp.py` & `spider-python-0.1.9/spider/RL/utilities/predmlp.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/constraints/ConstraintCollection.py` & `spider-python-0.1.9/spider/constraints/ConstraintCollection.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/constraints/__init__.py` & `spider-python-0.1.9/spider/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/constraints/constraint_checker/CartConstraintChecker.py` & `spider-python-0.1.9/spider/constraints/constraint_checker/CartConstraintChecker.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/elements/Box.py` & `spider-python-0.1.9/spider/elements/Box.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/elements/curves.py` & `spider-python-0.1.9/spider/elements/curves.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 import math
 import numpy as np
 import bisect
 from abc import abstractmethod
 from typing import Union
 
+from scipy.special import binom
 import scipy
 import cv2
 
 
 
 
 ################## 基础的一维曲线类(抽象类) 现在已经弃用！#####################
@@ -923,15 +924,15 @@
         return dddx, dddy
 
 
 ################# 贝塞尔曲线 #####################
 class BezierCurve(ParametricCurve):
     # 预先计算二项式系数
     # 类变量的定义语句在类被定义时就会执行，并且只执行一次, 多次初始化多个类的实例时，类变量的定义语句不会被重新执行
-    _binom_coeff_dict = {n: scipy.special.binom(n, np.arange(n+1)) for n in range(1, 9)} # 预先算至多8个控制点的情况
+    _binom_coeff_dict = {n: binom(n, np.arange(n+1)) for n in range(1, 9)} # 预先算至多8个控制点的情况
     # 字典中,n:[B_n_0, B_n_1,...B_n_n]储存了n下的所有的二项式系数
 
     def __init__(self, control_points, pre_calculation=True):
         super(BezierCurve, self).__init__()
         assert len(control_points) >= 2
         self.n = len(control_points) - 1 # 贝塞尔曲线的阶数
         self.control_points = np.array(control_points)
@@ -940,15 +941,15 @@
         # self._binom_coeff_dict = {}
 
         self._derivative_bezier_curve = None
         self._arclength = None
 
         # if pre_calculation:
         #     # 提前计算二项式系数
-        #     values = scipy.special.binom(self.n, np.arange(self.n+1))
+        #     values = binom(self.n, np.arange(self.n+1))
         #     for i, val in enumerate(values):
         #         self._binom_coeff_dict[(self.n, i)] = val
         #     # 提前计算
 
     @property
     def derivative_bezier_curve(self):
         if self._derivative_bezier_curve is None:
@@ -982,15 +983,15 @@
 
 
     def _binom(self, n, i):
         assert i >= 0 and i <= n
         if n in self._binom_coeff_dict:
             return self._binom_coeff_dict[n][i]
         else:
-            self._binom_coeff_dict[n] = scipy.special.binom(n, np.arange(n+1))
+            self._binom_coeff_dict[n] = binom(n, np.arange(n+1))
             return self._binom_coeff_dict[n][i]
 
 
     def calc_point_t(self, t):
         '''
         输入贝塞尔曲线的参数t，输出对应的x,y
         若t是一个数，输出(1,2)的点
@@ -1084,15 +1085,15 @@
 
     from time import time
     t1 = time()
     for _ in range(10000):
         a = c.arclength
     t2 = time()
     for _ in range(10000):
-        # a = {n: scipy.special.binom(n, np.arange(n + 1)) for n in range(1, 9)}
+        # a = {n: binom(n, np.arange(n + 1)) for n in range(1, 9)}
         b = c.arclength2
     t3 = time()
 
     print(t2-t1)
     print(t3-t2)
     print(a)
     print(b)
```

### Comparing `spider-python-0.1.8/spider/elements/grid.py` & `spider-python-0.1.9/spider/elements/grid.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/elements/map.py` & `spider-python-0.1.9/spider/elements/map.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/elements/obstacles.py` & `spider-python-0.1.9/spider/elements/obstacles.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/elements/trajectory.py` & `spider-python-0.1.9/spider/elements/trajectory.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/elements/vector.py` & `spider-python-0.1.9/spider/elements/vector.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/elements/vehicle.py` & `spider-python-0.1.9/spider/elements/vehicle.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/evaluator/CostEvaluator.py` & `spider-python-0.1.9/spider/evaluator/CostEvaluator.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/interface/highway_env/HighwayEnvInterface.py` & `spider-python-0.1.9/spider/interface/highway_env/HighwayEnvInterface.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/main.py` & `spider-python-0.1.9/spider/main.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/motion_planning/optimize.py` & `spider-python-0.1.9/spider/motion_planning/optimize.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/param.py` & `spider-python-0.1.9/spider/param.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/path_planning/hybridAstar.py` & `spider-python-0.1.9/spider/path_planning/hybridAstar.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/planner_zoo/BezierPlanner.py` & `spider-python-0.1.9/spider/planner_zoo/BezierPlanner.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/planner_zoo/LatticePlanner.py` & `spider-python-0.1.9/spider/planner_zoo/LatticePlanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,17 @@
         self.trajectory_evaluator = FrenetCostEvaluator()
 
         # self.collision_checker = BoxCollisionChecker(self.config["ego_veh_length"], self.config["ego_veh_width"])
         self.constraint_checker = CartConstriantChecker(
             self.config, BoxCollisionChecker(self.config["ego_veh_length"], self.config["ego_veh_width"])
         )
 
+        self._candidate_trajectories = None
+        self._candidate_trajectories_cost = None
+
 
     @classmethod
     def default_config(cls) -> dict:
         """
         :return: a configuration dict
         """
         return {
@@ -86,14 +89,18 @@
         # self.max_curvature = self.config["max_curvature"]
         # self.end_s_candidates = self.config["end_s_candidates"]
         # self.end_d_candidates = self.config["end_d_candidates"]
         # self.end_v_candidates = self.config["end_v_candidates"]
         # self.end_T_candidates = self.config["end_T_candidates"]
 
 
+    def get_candidate_traj_with_cost(self):
+        return self._candidate_trajectories, self._candidate_trajectories_cost
+
+
     def constraint_check(self, sorted_candidate_trajectories:List[FrenetTrajectory], sorted_cost, obstacles:TrackingBoxList):
         for traj, cost in zip(sorted_candidate_trajectories, sorted_cost):
             if self.constraint_checker.check(traj, obstacles):
                 return traj, cost
 
             # if np.any(np.array(traj.v) > self.config["max_speed"]): continue
             # if np.any(np.array(traj.v) < self.config["min_speed"]): continue
@@ -161,14 +168,17 @@
 
         # 轨迹坐标转换，把每个轨迹点转到笛卡尔坐标
         candidate_trajectories = [self.coordinate_transformer.frenet2cart4traj(t, order=2) for t in candidate_trajectories]
 
         # 评估+筛选
         sorted_candidates, sorted_cost = self.trajectory_evaluator.evaluate_candidates(candidate_trajectories)
         optimal_trajectory, min_cost = self.constraint_check(sorted_candidates, sorted_cost, predicted_obstacles)
+
+        self._candidate_trajectories, self._candidate_trajectories_cost = sorted_candidates, sorted_cost
+
         if not (optimal_trajectory is None):
             print("Optimal trajectory found! s_dot_end=%.2f,l_end=%.2f" %
                   (optimal_trajectory.s_dot[-1], optimal_trajectory.l[-1]))
         else:
             print("WARNING: NO feasible trajectory!")
 
         t2 = time.time()
```

### Comparing `spider-python-0.1.8/spider/planner_zoo/MBRLPlanner.py` & `spider-python-0.1.9/spider/planner_zoo/MBRLPlanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,16 @@
         self.next_state = None
         self.action = None
         self.reward_function = FstateControlReward(self.config)
         self.agent = MBRLAgent(self.config["state_veh_num"], self.config["state_feat_num"], action_dim,
                                self.config["dt"], reward_function=self.reward_function, device=self.device)
         self.closed_loop = self.config["closed_loop"]
 
+        self._candidate_trajectories = None
+
     @classmethod
     def default_config(cls) -> dict:
         """
         :return: a configuration dict
         """
         return {
             "steps": 20,
@@ -116,14 +118,17 @@
             "end_v_candidates": tuple(i * 60 / 3.6 / 2 + 1 for i in range(3)),  # 改这一项的时候，要连着限速一起改了
             "end_T_candidates": (3, 5)  # s_dot, T采样生成纵向轨迹
         }
 
     def configure(self, config: dict):
         self.__init__(config)
 
+    def get_candidate_trajectories(self):
+        return self._candidate_trajectories
+
     def set_reward_function(self):
         pass
 
     def set_local_map(self, local_map: RoutedLocalMap):
         self.local_map = local_map
 
     def build_frenet_lane(self, target_lane_idx):
@@ -227,14 +232,16 @@
         action_idx, self.action = self.agent.act(self.state.to(self.device), action_sequences, egreedy=egreedy, epsilon=1.0)  # policy
 
         ################################### decode action into trajectory #################################
 
         # 轨迹坐标转换，把每个轨迹点转到笛卡尔坐标
         optimal_trajectory = self.decode_action(action_idx, candidate_trajectories)  # 动作解码器
 
+        self._candidate_trajectories = candidate_trajectories
+
         t2 = time.time()
         if not train:
             print("Planning Succeed! Time: %.2f seconds, FPS: %.2f" % (t2-t1, 1/(t2-t1)))
             print("action:", self.action)
         return optimal_trajectory
```

### Comparing `spider-python-0.1.8/spider/planner_zoo/MFRLPlanner.py` & `spider-python-0.1.9/spider/planner_zoo/MFRLPlanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,16 @@
         self.state = None#ElementFrenetState()
         self.next_state = None
         self.action = None
         self.agent = DQNAgent(state_dim, action_dim, gamma=self.config["discount_factor"], device=self.device)
         self.reward_function = FstateTrajectoryReward(self.config)
         self.closed_loop = self.config["closed_loop"]
 
+        self._candidate_trajectories = None
+
 
     @classmethod
     def default_config(cls) -> dict:
         """
         :return: a configuration dict
         """
         return {
@@ -122,14 +124,16 @@
 
     def configure(self, config: dict):
         self.__init__(config)
 
     def set_reward_function(self, reward_model):
         self.reward_function = reward_model
 
+    def get_candidate_trajectories(self):
+        return self._candidate_trajectories
 
     def set_local_map(self, local_map:RoutedLocalMap):
         self.local_map = local_map
 
     def build_frenet_lane(self, target_lane_idx):
         if target_lane_idx < 0 or target_lane_idx >= len(self.local_map.lanes):
             raise ValueError("Invalid target lane index")
@@ -232,14 +236,16 @@
         self.reward_function.set_trajectory_candidates(candidate_trajectories)
 
         # 轨迹坐标转换，把每个轨迹点转到笛卡尔坐标
         # todo:qzl: 其实candidates_trajectories不用算出来的，会耗损计算资源，能不能储存Generator形式的？调用的时候再进行计算
         candidate_trajectories = [self.coordinate_transformer.frenet2cart4traj(t, order=2) for t in candidate_trajectories]
         optimal_trajectory = self.decode_action(self.action,candidate_trajectories)  # 动作解码器
 
+        self._candidate_trajectories = candidate_trajectories
+
         return optimal_trajectory
 
 
 
 
 if __name__ == '__main__':
     from spider.elements.map import Lane
```

### Comparing `spider-python-0.1.8/spider/sampler/Combiner.py` & `spider-python-0.1.9/spider/sampler/Combiner.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/sampler/PolynomialSampler.py` & `spider-python-0.1.9/spider/sampler/PolynomialSampler.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/utils/Visualize.py` & `spider-python-0.1.9/spider/utils/Visualize.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/utils/collision/AABB.py` & `spider-python-0.1.9/spider/utils/collision/AABB.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/utils/collision/CollisionChecker.py` & `spider-python-0.1.9/spider/utils/collision/CollisionChecker.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/utils/collision/CollisionConstraints.py` & `spider-python-0.1.9/spider/utils/collision/CollisionConstraints.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/utils/collision/Disks.py` & `spider-python-0.1.9/spider/utils/collision/Disks.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/utils/collision/SAT.py` & `spider-python-0.1.9/spider/utils/collision/SAT.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/utils/transform/frenet.py` & `spider-python-0.1.9/spider/utils/transform/frenet.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,27 +64,31 @@
 
     def __cart2frenet_order0(self, x, y):
         nearest_idx, min_dist = find_nearest_point(np.array([x, y]), self.refer_line_arr)
 
         # 计算两个线段之间的距离并选择最短的作为l
         if 0 < nearest_idx < len(self.refer_line_arr) - 1:
             proj1, dist1 = point_to_segment_distance(np.array([x, y]), self.refer_line_arr[nearest_idx - 1],
-                                                     self.refer_line_arr[nearest_idx])
+                                                     self.refer_line_arr[nearest_idx],allow_extension=False)
             proj2, dist2 = point_to_segment_distance(np.array([x, y]), self.refer_line_arr[nearest_idx],
-                                                     self.refer_line_arr[nearest_idx + 1])
+                                                     self.refer_line_arr[nearest_idx + 1],allow_extension=False)
+
+            # 选择距离更短的投影点及距离
             if abs(dist1) < abs(dist2):
-                s_end, l = proj1, dist1
+                s_end, l = proj1, dist1 # s_end指的是最后一段segment上面s的距离
                 segment_start_idx = nearest_idx - 1
             else:
                 s_end, l = proj2, dist2
                 segment_start_idx = nearest_idx
+        # 处理最近点在参考线起始点的情况
         elif nearest_idx == 0:
             s_end, l = point_to_segment_distance(np.array([x, y]), self.refer_line_arr[nearest_idx],
                                                  self.refer_line_arr[nearest_idx + 1])
             segment_start_idx = nearest_idx
+        # 处理最近点在参考线末尾的情况
         else:
             s_end, l = point_to_segment_distance(np.array([x, y]), self.refer_line_arr[nearest_idx - 1],
                                                  self.refer_line_arr[nearest_idx])
             segment_start_idx = nearest_idx - 1
 
         # 计算纵向位置s和横向导数l_prime
         s = np.sum(
```

### Comparing `spider-python-0.1.8/spider/utils/transform/grid.py` & `spider-python-0.1.9/spider/utils/transform/grid.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider/vehicle_model/bicycle.py` & `spider-python-0.1.9/spider/vehicle_model/bicycle.py`

 * *Files identical despite different names*

### Comparing `spider-python-0.1.8/spider_python.egg-info/PKG-INFO` & `spider-python-0.1.9/spider_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-python
-Version: 0.1.8
+Version: 0.1.9
 Summary: SPIDER -- Self-driving Planning and Intelligent Decision-making Engine with Reinforcement learning
 Home-page: https://github.com/ZelinQian/SPIDER
 Author: Zelin Qian
 Author-email: qzl22@mails.tsinghua.edu.cn
 License: MIT
 Description: SPIDER -- Self-driving Planning and Intelligent Decision-making Engine with Reinforcement learning
```

### Comparing `spider-python-0.1.8/spider_python.egg-info/SOURCES.txt` & `spider-python-0.1.9/spider_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

