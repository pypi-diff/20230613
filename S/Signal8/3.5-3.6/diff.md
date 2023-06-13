# Comparing `tmp/Signal8-3.5.tar.gz` & `tmp/Signal8-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-3.5.tar", last modified: Fri Jun  9 17:03:05 2023, max compression
+gzip compressed data, was "Signal8-3.6.tar", last modified: Tue Jun 13 18:29:09 2023, max compression
```

## Comparing `Signal8-3.5.tar` & `Signal8-3.6.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 17:03:05.162217 Signal8-3.5/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-3.5/LICENSE
--rw-rw-rw-   0        0        0     5556 2023-06-09 17:03:05.160218 Signal8-3.5/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2023-06-06 03:52:31.000000 Signal8-3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 17:03:05.091228 Signal8-3.5/Signal8/
--rw-rw-rw-   0        0        0    11063 2023-06-09 17:02:14.000000 Signal8-3.5/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-05 17:11:26.000000 Signal8-3.5/Signal8/__init__.py
--rw-rw-rw-   0        0        0      268 2023-06-09 16:49:06.000000 Signal8-3.5/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 17:03:05.155218 Signal8-3.5/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-3.5/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     6036 2023-06-09 16:47:11.000000 Signal8-3.5/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2826 2023-06-09 16:43:50.000000 Signal8-3.5/Signal8/utils/npc.py
--rw-rw-rw-   0        0        0     5039 2023-06-05 17:20:08.000000 Signal8-3.5/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-3.5/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12317 2023-06-06 22:01:04.000000 Signal8-3.5/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-3.5/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-09 17:03:05.135219 Signal8-3.5/Signal8.egg-info/
--rw-rw-rw-   0        0        0     5556 2023-06-09 17:03:04.000000 Signal8-3.5/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-06-09 17:03:04.000000 Signal8-3.5/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 17:03:04.000000 Signal8-3.5/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 17:03:04.000000 Signal8-3.5/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 17:03:05.162217 Signal8-3.5/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-06-09 17:02:41.000000 Signal8-3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:29:09.632022 Signal8-3.6/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-3.6/LICENSE
+-rw-rw-rw-   0        0        0     5356 2023-06-13 18:29:09.627024 Signal8-3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4858 2023-06-12 22:34:01.000000 Signal8-3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 18:29:09.542024 Signal8-3.6/Signal8/
+-rw-rw-rw-   0        0        0    11138 2023-06-13 18:22:14.000000 Signal8-3.6/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-12 18:52:22.000000 Signal8-3.6/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      214 2023-06-13 18:14:07.000000 Signal8-3.6/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:29:09.620032 Signal8-3.6/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-3.6/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5469 2023-06-13 18:21:58.000000 Signal8-3.6/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     1116 2023-06-12 21:36:47.000000 Signal8-3.6/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-3.6/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12597 2023-06-13 18:21:42.000000 Signal8-3.6/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-3.6/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:29:09.588023 Signal8-3.6/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     5356 2023-06-13 18:29:09.000000 Signal8-3.6/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-06-13 18:29:09.000000 Signal8-3.6/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 18:29:09.000000 Signal8-3.6/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-13 18:29:09.000000 Signal8-3.6/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 18:29:09.632022 Signal8-3.6/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-13 18:28:09.000000 Signal8-3.6/setup.py
```

### Comparing `Signal8-3.5/LICENSE` & `Signal8-3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-3.5/PKG-INFO` & `Signal8-3.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 3.5
+Version: 3.6
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
@@ -36,33 +36,33 @@
 ```
 
 ## Usage
 
 ```
 import Signal8
 
-env = Signal8.env(problem_type='disaster_response')
-env.reset(options={"instance_num": 0}))
+env = Signal8.env()
+env.reset(options={'problem_instance': 'corners'}))
 observation, _, terminations, truncations, _ = env.last()
 env.step(action)
 env.close()
 ```
 
 ## List of Problem Instances
 
-|   Problem Type   | Instance Name |                 Visualization                 |
-| :---------------: | :------------: | :--------------------------------------------: |
-| Disaster Response | ``instance 0`` | ![1686023513741](image/README/1686023513741.png) |
-| Disaster Response | ``instance 1`` | ![1686023519237](image/README/1686023519237.png) |
-| Disaster Response | ``instance 2`` | ![1686023523656](image/README/1686023523656.png) |
-| Disaster Response | ``instance 3`` | ![1686023529431](image/README/1686023529431.png) |
-| Precision Farming | ``instance 0`` | ![1686023534970](image/README/1686023534970.png) |
-| Precision Farming | ``instance 1`` | ![1686023540501](image/README/1686023540501.png) |
-| Precision Farming | ``instance 2`` | ![1686023545379](image/README/1686023545379.png) |
-| Precision Farming | ``instance 3`` | ![1686023549246](image/README/1686023549246.png) |
+| Problem Instance |                 Visualization                 |
+| :--------------: | :--------------------------------------------: |
+|  ``corners``Â   | ![1686604788813](image/README/1686604788813.png) |
+|   ``quarters``   | ![1686604799335](image/README/1686604799335.png) |
+|    ``cross``    | ![1686604808540](image/README/1686604808540.png) |
+|   ``cluster``   | ![1686604839072](image/README/1686604839072.png) |
+|     ``left``     | ![1686604845732](image/README/1686604845732.png) |
+|    ``right``    | ![1686604851758](image/README/1686604851758.png) |
+|      ``up``      | ![1686604859851](image/README/1686604859851.png) |
+|     ``down``     | ![1686604868138](image/README/1686604868138.png) |
 
 Each of the colored regions represents an area where the respective entity can be instantiated. Blue regions are starting regions, yellow regions represent goal regions and in the case of precision farming, if a goal region is not generated in the yellow region then changes to a static obstacle region but this is not the case for disaster response, instead the region where the goal was not instantiated does not impact the episode at all, the light red regions represent static obstacles, and dark red regions represent dynamic obstacles.
 
 In the case of disaster response, the dynamic obstacle does not move, instead it incrementally increases the obstacle radius to simulate a fire. In the precision farming case, the dynamic obstacle represents the behavior of a hockey rink ice cleaner moving in zig zags.
 
 ## Paper Citation
```

### Comparing `Signal8-3.5/README.md` & `Signal8-3.6/Signal8.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,30 @@
+Metadata-Version: 2.1
+Name: Signal8
+Version: 3.6
+Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
+Home-page: https://github.com/ethanmclark1/signal8
+Author: Ethan Clark
+Author-email: eclark715@gmail.com.com
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # A Fork of Multi-Agent Particle Environment
 
 Signal8 is an enhanced version of the Simple environment, originally developed by the [Farama Foundation](https://farama.org/) as part of their [Multi-Agent Particle Environment (MPE)](https://pettingzoo.farama.org/environments/mpe/).
 
 # Signal8
 
 Signal8 is an open-source research project devoted to facilitating the evolution of communication strategies in multi-agent systems. The project, drawing inspiration from real-world scenarios such as disaster response and precision farming, features a dynamic environment that elevates the principles of the Lewis signaling game. This unique setting serves as a testing ground for the advancement of robot-to-robot communication protocols.
 
 Each problem set within Signal8 encompasses four distinct instances, with each one posing different constraints on the positioning of entities such as starting points, goals, and both static and dynamic obstacles. This dynamic feature fosters examination of communication strategies in diverse settings, enhancing the environment's realism and adaptability.
 
-A notable characteristic of Signal8 is its incorporation of asymmetric information, whereby two types of agents – an 'eye in the sky' agent with global information and ground agents with only local information – operate simultaneously. This asymmetry replicates real-world situations, presenting challenges for the development of efficient communication strategies. It also provides intriguing prospects for the generation of context-dependent language and high-level directives.
+A notable characteristic of Signal8 is its incorporation of asymmetric information, whereby two types of agents â€“ an 'eye in the sky' agent with global information and ground agents with only local information â€“ operate simultaneously. This asymmetry replicates real-world situations, presenting challenges for the development of efficient communication strategies. It also provides intriguing prospects for the generation of context-dependent language and high-level directives.
 
 In Signal8, both static and dynamic obstacles are present, creating further complexities for agents navigating through the environment. Static obstacles provide persistent barriers, while dynamic obstacles introduce predictable elements that can move or change over time. This complexity enriches the environment, making it an even more challenging and realistic platform for testing multi-agent communication strategies.
 
 For more information on utilizing the environment API, please refer to the [PettingZoo API documentation](https://pettingzoo.farama.org/content/basic_usage/).
 
 ## Installation
 
@@ -24,33 +36,33 @@
 ```
 
 ## Usage
 
 ```
 import Signal8
 
-env = Signal8.env(problem_type='disaster_response')
-env.reset(options={"instance_num": 0}))
+env = Signal8.env()
+env.reset(options={'problem_instance': 'corners'}))
 observation, _, terminations, truncations, _ = env.last()
 env.step(action)
 env.close()
 ```
 
 ## List of Problem Instances
 
-|   Problem Type   | Instance Name |                 Visualization                 |
-| :---------------: | :------------: | :--------------------------------------------: |
-| Disaster Response | ``instance 0`` | ![1686023513741](image/README/1686023513741.png) |
-| Disaster Response | ``instance 1`` | ![1686023519237](image/README/1686023519237.png) |
-| Disaster Response | ``instance 2`` | ![1686023523656](image/README/1686023523656.png) |
-| Disaster Response | ``instance 3`` | ![1686023529431](image/README/1686023529431.png) |
-| Precision Farming | ``instance 0`` | ![1686023534970](image/README/1686023534970.png) |
-| Precision Farming | ``instance 1`` | ![1686023540501](image/README/1686023540501.png) |
-| Precision Farming | ``instance 2`` | ![1686023545379](image/README/1686023545379.png) |
-| Precision Farming | ``instance 3`` | ![1686023549246](image/README/1686023549246.png) |
+| Problem Instance |                 Visualization                 |
+| :--------------: | :--------------------------------------------: |
+|  ``corners``Â   | ![1686604788813](image/README/1686604788813.png) |
+|   ``quarters``   | ![1686604799335](image/README/1686604799335.png) |
+|    ``cross``    | ![1686604808540](image/README/1686604808540.png) |
+|   ``cluster``   | ![1686604839072](image/README/1686604839072.png) |
+|     ``left``     | ![1686604845732](image/README/1686604845732.png) |
+|    ``right``    | ![1686604851758](image/README/1686604851758.png) |
+|      ``up``      | ![1686604859851](image/README/1686604859851.png) |
+|     ``down``     | ![1686604868138](image/README/1686604868138.png) |
 
 Each of the colored regions represents an area where the respective entity can be instantiated. Blue regions are starting regions, yellow regions represent goal regions and in the case of precision farming, if a goal region is not generated in the yellow region then changes to a static obstacle region but this is not the case for disaster response, instead the region where the goal was not instantiated does not impact the episode at all, the light red regions represent static obstacles, and dark red regions represent dynamic obstacles.
 
 In the case of disaster response, the dynamic obstacle does not move, instead it incrementally increases the obstacle radius to simulate a fire. In the precision farming case, the dynamic obstacle represents the behavior of a hockey rink ice cleaner moving in zig zags.
 
 ## Paper Citation
```

### Comparing `Signal8-3.5/Signal8/Signal8.py` & `Signal8-3.6/Signal8/Signal8.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,249 +1,245 @@
-import time
 import copy
-import random
-import logging
-import threading
 import numpy as np
+import matplotlib.path as mpath
 
-from .utils.npc import NPC
+from functools import partial
 from .utils.scenario import BaseScenario
 from .utils.simple_env import SimpleEnv, make_env
 from .utils.core import Agent, Goal, Obstacle, World
-from .utils.problems import get_problem_instance
+from .utils.problems import get_problem_list, get_problem_instance
 
 from gymnasium.utils import EzPickle
 
 
 class raw_env(SimpleEnv, EzPickle):
-    def __init__(self, problem_type, num_agents=1, render_mode=None):
-        
-        if problem_type not in {'disaster_response', 'precision_farming'}:
-            raise ValueError("Signal8 only supports 'disaster_response' and 'precision_farming' problem types.")
+    def __init__(
+        self, 
+        num_agents=1, 
+        num_large_obstacles=4, 
+        num_small_obstacles=10, 
+        render_mode=None
+        ):
         
         if num_agents > 2:
             raise ValueError("Signal8 currently can only support up to 2 agents.")
         
+        if num_large_obstacles > 4:
+            raise ValueError("Signal8 can only support up to 4 obstacles.")
+        
         scenario = Scenario()
-        world = scenario.make_world(problem_type, num_agents)
+        world = scenario.make_world(num_agents, num_large_obstacles, num_small_obstacles)
         
         super().__init__(
             scenario=scenario, 
             world=world, 
             render_mode=render_mode,
             max_cycles=500, 
         )
         
 env = make_env(raw_env)
 
 class Scenario(BaseScenario):
-    def make_world(self, problem_type, num_agents):
+    def make_world(self, num_agents, num_large_obstacles, num_small_obstacles):
         world = World()
-        self._add_logger()
-        world.problem_type = problem_type
-        
-        self.npc = []
-        self.scripted_obstacle_threads = []
-        self.scripted_obstacle_running = False
+        world.problem_list = get_problem_list()
 
-        world.agents = [Agent() for _ in range(num_agents)]
-        for i, agent in enumerate(world.agents):
+        for i in range(num_agents):
+            agent = Agent()
             agent.name = f"agent_{i}"
             agent.collide = True
-
+            agent.color = np.array([1, 0.95, 0.8])
+            world.agents.append(agent)
+        
         # Agents has two goals (i.e., actual goal and start position)
-        # This is to ensure agent returns safely to start position
-        world.goals = [Goal() for _ in range(len(world.agents*2))]
-        for i, goal in enumerate(world.goals):
+        # This is to ensure agent returns safely to start position after reaching goal
+        for i in range(num_agents*2):
+            goal = Goal()
             goal.name = f"goal_{i}"
             goal.collide = False
+            # goal_a is the actual goal
+            if i < num_agents:
+                goal.color = np.array([0.835, 0.90, 0.831])
+            # goal_b is the start position to return to after reaching goal
+            else:
+                goal.color = np.array([0.85, 0.90, 0.99])
+            world.goals.append(goal)
         
-        # Minimum number of obstacles in a problem instance 
-        world.obstacles = [Obstacle() for _ in range(4)]
-        for i, obstacle in enumerate(world.obstacles):
+        # Large obstacles can only be observed by aerial agent
+        for i in range(num_large_obstacles):
+            obstacle = Obstacle(size=0.1)
             obstacle.name = f"obs_{i}"
-                
+            obstacle.color = np.array([0.97, 0.801, 0.8])
+            world.large_obstacles.append(obstacle)
+        
+        # Small obstacles can only be observed by ground agent(s)
+        for i in range(num_small_obstacles):
+            obstacle = Obstacle(size=0.01)
+            obstacle.name = f"obs_{i}"
+            obstacle.color = np.array([0.97, 0.801, 0.8])
+            world.small_obstacles.append(obstacle)    
+        
+        world.buffer_dist = world.agents[0].size + world.large_obstacles[0].size
         return world
     
-    # Get constraints on entities given the problem instance name
-    def _set_problem_instance(self, world, np_random, instance_num):
-        instance_name, instance = get_problem_instance(world.problem_type, instance_num, np_random)
+    # Get constraints on entities given problem instance name
+    def _set_problem_instance(self, world, instance_name):
+        instance_constr = get_problem_instance(instance_name)
         world.problem_instance = instance_name
-        world.start_constr = instance['start']
-        world.goal_constr = instance['goal']
-        world.static_obstacle_constr = instance['static_obs']
-        world.dynamic_obstacle_constr = instance['dynamic_obs']
-    
-    """
-    Returns goal constraints that haven't been selected to be used as an obstacle
-    for the precision farming case (i.e., crop that wasn't selected as goal becomes an obstacle)
-    """
-    def _reset_agents_and_goals(self, world, np_random):
-        temp_goal_constr = copy.copy(world.goal_constr)
-        for i, agent in enumerate(world.agents):
-            agent.color = np.array([1, 0.95, 0.8])
-            agent.state.p_vel = np.zeros(world.dim_p)
-            agent_constr = random.choice(world.start_constr)
-            agent.state.p_pos = np_random.uniform(*zip(*agent_constr))
+        world.instance_constr = instance_constr
+    
+    # Generate valid points according to some condition
+    def _generate_position(self, np_random, condition):
+        while True:
+            point = np_random.uniform(-1, +1, 2)
+            if condition(point):
+                break
+        return point
+    
+    # Check if point is outside of rectangular obstacle regions
+    def _safe_position(self, point, epsilon, x_constraints, y_constraints):
+        return all(not (low - epsilon <= point[0] <= high + epsilon) for low, high in x_constraints) \
+            and all(not (low - epsilon <= point[1] <= high + epsilon) for low, high in y_constraints)
+
+    # Check if point is outside of triangular obstacle regions
+    def _outside_triangle(self, point, paths, epsilon):
+        enlarged_paths = []
+        for path in paths:
+            centroid = np.mean(path.vertices[:-1], axis=0)
+            enlarged_vertices = path.vertices + epsilon * (path.vertices - centroid)
+            enlarged_paths.append(mpath.Path(enlarged_vertices))
+        return not any(path.contains_points(point[None, :]) for path in enlarged_paths)
+    
+    # Reset agents and goals to their initial positions
+    def _reset_agents_and_goals(self, world, np_random, paths):
+        epsilon = world.buffer_dist
+        
+        if paths is None:
+            x_constraints = [constr[0] for constr in world.instance_constr]
+            y_constraints = [constr[1] for constr in world.instance_constr]
 
+        for i, agent in enumerate(world.agents):
             agent.goal_a = world.goals[i]
-            agent.goal_a.color = np.array([0.835, 0.90, 0.831])
-            agent.goal_a.state.p_vel = np.zeros(world.dim_p)
-            goal_constr = random.choice(temp_goal_constr)
-            agent.goal_a.state.p_pos = np_random.uniform(*zip(*goal_constr))
-            temp_goal_constr.remove(goal_constr)
-            
             agent.goal_b = world.goals[len(world.goals) - 1 - i]
-            agent.goal_b.color = np.array([0.85, 0.90, 0.99])
+
+            agent.state.p_vel = np.zeros(world.dim_p)
+            agent.goal_a.state.p_vel = np.zeros(world.dim_p)
             agent.goal_b.state.p_vel = np.zeros(world.dim_p)
-            agent.goal_b.state.p_pos = copy.copy(agent.state.p_pos)
 
-        return temp_goal_constr
-    
-    # Reset position of dynamic obstacles
-    def _reset_dynamic_obstacle(self, world, obstacle, np_random, temp_dynamic_obs_constr):
-        obstacle.size = 0.025
-        obstacle.movable = True
-        obstacle.lock = threading.Lock()
-        obstacle.color = np.array([0.26, 0.32, 0.36])
-        obstacle.state.p_vel = np.zeros(world.dim_p)
-        dynamic_obs_constr = random.choice(temp_dynamic_obs_constr)
-        obstacle.state.p_pos = np_random.uniform(*zip(*dynamic_obs_constr))
-        temp_dynamic_obs_constr.remove(dynamic_obs_constr)
-
-    # Reset position of static obstacles, taking leftover entities from goal constraints
-    def _reset_static_obstacle(self, world, obstacle, np_random, temp_static_obs_constr):
-        obstacle.color = np.array([0.97, 0.801, 0.8])
-        obstacle.state.p_vel = np.zeros(world.dim_p)
-        static_obs_constr = random.choice(temp_static_obs_constr)
-        obstacle.state.p_pos = np_random.uniform(*zip(*static_obs_constr))  
-        temp_static_obs_constr.remove(static_obs_constr)
-    
-    # Add or remove obstacles to match the number of obstacles in problem instance
-    def _match_obstacles_to_instance(self, world, num_static):
-        num_total_obstacles = num_static + len(world.dynamic_obstacle_constr)
-        if len(world.obstacles) > num_total_obstacles:
-            world.obstacles = world.obstacles[:num_total_obstacles]
-        elif len(world.obstacles) < num_total_obstacles:
-            additional_obstacles = [Obstacle() for _ in range(len(world.obstacles), num_total_obstacles)]
-            [setattr(obstacle, 'name', f"obs_{i+len(world.obstacles)}") for i, obstacle in enumerate(additional_obstacles)]
-            world.obstacles.extend(additional_obstacles)
-    
-    # Reset position of obstacles
-    def _reset_obstacles(self, world, np_random, leftover_entities):
-        temp_static_obs_constr = copy.copy(world.static_obstacle_constr)
-        if world.problem_type.startswith('precision_farming'):
-            temp_static_obs_constr += leftover_entities
-        temp_dynamic_obs_constr = copy.copy(world.dynamic_obstacle_constr)
-        
-        num_dynamic_obs = len(temp_dynamic_obs_constr)        
-        self._match_obstacles_to_instance(world, len(temp_static_obs_constr))
-
-        for i, obstacle in enumerate(world.obstacles):
-            if i < num_dynamic_obs:
-                self._reset_dynamic_obstacle(world, obstacle, np_random, temp_dynamic_obs_constr)
-                self.npc += [NPC(obstacle.state.p_pos)]
+            if world.problem_instance == 'corners':
+                condition = partial(
+                    self._outside_triangle, 
+                    paths=paths, 
+                    epsilon=epsilon
+                    )
             else:
-                self._reset_static_obstacle(world, obstacle, np_random, temp_static_obs_constr)
+                condition = partial(
+                    self._safe_position, 
+                    epsilon=epsilon, 
+                    x_constraints=x_constraints, 
+                    y_constraints=y_constraints
+                    )
+
+            agent.state.p_pos = self._generate_position(np_random, condition)
+            agent.goal_a.state.p_pos = self._generate_position(np_random, condition)
+            agent.goal_b.state.p_pos = copy.copy(agent.state.p_pos)
     
-    # Start a thread for each dynamic obstacle
-    def _start_scripted_obstacles(self, world):
-        self.scripted_obstacle_running = True
-        for obstacle in world.obstacles:
-            if obstacle.movable:
-                t = threading.Thread(target=self.run_scripted_obstacle, args=(world, obstacle))
-                t.start()
-                self.scripted_obstacle_threads.append(t)   
+    # Reset all large obstacles to a position that does not intersect with the agents
+    def _reset_large_obstacles(self, world, np_random, paths):
+        def inside_triangle_condition(point):
+            return any(path.contains_points(point[None, :]) for path in paths)
                 
-    def reset_world(self, world, np_random, instance_name=None):
-        self.npc.clear()
-        self.stop_scripted_obstacles()
-        self._set_problem_instance(world, np_random, instance_name)
-        leftover_entities = self._reset_agents_and_goals(world, np_random)
-        self._reset_obstacles(world, np_random, leftover_entities)
-        self._start_scripted_obstacles(world)
+        occupied_triangles = set()
+        for i, large_obstacle in enumerate(world.large_obstacles):            
+            large_obstacle.state.p_vel = np.zeros(world.dim_p)
+            idx = i % len(world.instance_constr)
+            
+            # Each corner may only have one large_obstacle in it
+            if world.problem_instance == 'corners':
+                while True:
+                    pos = self._generate_position(np_random, inside_triangle_condition)
+                    triangle_idx = next((i for i, path in enumerate(paths) if path.contains_points(pos[None, :])), None)
+                    if triangle_idx not in occupied_triangles:
+                        large_obstacle.state.p_pos = pos
+                        occupied_triangles.add(triangle_idx)
+                        break
+            else:                
+                large_obstacle.state.p_pos = np_random.uniform(*zip(*world.instance_constr[idx]))
+    
+    # Reset all small obstacles to a position that does not intersect with the agents or the large obstacles
+    def _reset_small_obstacles(self, world, np_random, paths):
+        epsilon = world.small_obstacles[0].size + world.large_obstacles[0].size
+        
+        x_constraints = [constr[0] for constr in world.instance_constr]
+        y_constraints = [constr[1] for constr in world.instance_constr]
+        agent_positions = [agent.state.p_pos for agent in world.agents]
+        goal_positions = [goal.state.p_pos for goal in world.goals]
+        large_obstacle_positions = [obstacle.state.p_pos for obstacle in world.large_obstacles]
+        
+        def safe_position(point):
+            if world.problem_instance == 'corners':
+                within_obstacle_constraints = any(path.contains_points(point[None, :]) for path in paths)
+            else:
+                within_obstacle_constraints = any(low - epsilon <= point[0] <= high + epsilon for low, high in x_constraints) \
+                    or any(low - epsilon <= point[1] <= high + epsilon for low, high in y_constraints)
+
+            within_other_positions = any(np.linalg.norm(point - pos) <= epsilon for pos in agent_positions + goal_positions + large_obstacle_positions)
+
+            return not (within_obstacle_constraints or within_other_positions)
+        
+        for small_obstacle in world.small_obstacles:
+            small_obstacle.state.p_vel = np.zeros(world.dim_p)
+            small_obstacle.state.p_pos = self._generate_position(np_random, safe_position)
+
+    def reset_world(self, world, np_random, problem_instance):
+        self._set_problem_instance(world, problem_instance)
+        
+        paths = [mpath.Path(np.array(triangle)) for triangle in world.instance_constr] \
+            if world.problem_instance == 'corners' else None
+            
+        self._reset_agents_and_goals(world, np_random, paths)
+        self._reset_large_obstacles(world, np_random, paths)
+        self._reset_small_obstacles(world, np_random, paths)
     
     # Reward given by agents to agents for reaching their respective goals
     def reward(self, agent, world):
         return 0
     
+    # Ground agents can only observe the positions of other agents, goals, and small obstacles
     def observation(self, agent, world):
         agent_pos = agent.state.p_pos
         agent_vel = agent.state.p_vel
         
-        num_obstacles = len(world.obstacles)
+        num_agents = len(world.agents)
+        num_small_obstacles = len(world.small_obstacles)
         max_observable_dist = agent.max_observable_dist
         
-        observed_obstacles = [np.full_like(agent_pos, max_observable_dist) for _ in range(num_obstacles)]
+        observed_agents = [np.full_like(agent_pos, max_observable_dist) for _ in range(num_agents - 1)]
         observed_goal = np.full_like(agent_pos, max_observable_dist)
+        observed_obstacles = [np.full_like(agent_pos, max_observable_dist) for _ in range(num_small_obstacles)]
         
-        for i, obstacle in enumerate(world.obstacles):
-            if obstacle.movable:
-                with obstacle.lock:
-                    obs_pos = obstacle.state.p_pos
+        idx = 0
+        for other_agent in world.agents:
+            if agent.name == other_agent.name:
+                continue
             else:
-                obs_pos = obstacle.state.p_pos
+                other_agent_pos = other_agent.state.p_pos
+                relative_pos = other_agent_pos - agent_pos
+                dist = np.linalg.norm(relative_pos)
+                if dist <= max_observable_dist:
+                    observed_agents[idx] = relative_pos
+                idx += 1
+        
+        for i, small_obstacle in enumerate(world.small_obstacles):
+            obs_pos = small_obstacle.state.p_pos
             relative_pos = obs_pos - agent_pos
             dist = np.linalg.norm(relative_pos)
             if dist <= max_observable_dist:
                 observed_obstacles[i] = relative_pos
                 
         goal_pos = agent.goal_b.state.p_pos if agent.reached_goal else agent.goal_a.state.p_pos
         relative_goal_pos = goal_pos - agent_pos
         goal_dist = np.linalg.norm(relative_goal_pos)
         if goal_dist <= max_observable_dist:
             observed_goal = relative_goal_pos
         
-        return np.concatenate((agent_pos, agent_vel, np.concatenate(observed_obstacles, axis=0), observed_goal))
-            
-    # Run a thread for each scripted obstacle
-    def run_scripted_obstacle(self, world, obstacle):
-        while self.scripted_obstacle_running:
-            # self.logger.debug(f'{obstacle.name} size: {obstacle.size:}, position: {obstacle.state.p_pos}')
-            action, size = self._action_callback(obstacle, world)
-            obstacle.update(action, size)
-            time.sleep(0.5)
-        
-    # disaster response: increase obstacle size to resemble increasing size of fire
-    # precision farming: move obstacle in a zig-zag pattern to resemble a tractor
-    def _action_callback(self, obstacle, world):
-        size = None
-        action = None
-        instance = world.problem_instance
-        if world.problem_type == 'disaster_response':
-            if instance == 'instance_0':
-                size = 0.005
-            elif instance == 'instance_1':
-                size = 0.0075
-            elif instance == 'instance_2':
-                size = 0.01
-            elif instance == 'instance_3':
-                size = 0.0125
-        else:
-            action = np.zeros(world.dim_p)
-            obstacle_num = int(obstacle.name.split('_')[-1])
-            instance_num = int(instance.split('_')[-1])
-            action = self.npc[obstacle_num].get_scripted_action(obstacle, instance_num)
-            sensitivity = 2.0
-            action *= sensitivity
-
-        return action, size
-
-    # Stop all threads for scripted obstacles
-    def stop_scripted_obstacles(self):
-        self.scripted_obstacle_running = False
-        for t in self.scripted_obstacle_threads:
-            t.join()
-        self.scripted_obstacle_threads.clear()
-        
-    # Create a logger to log information from threads
-    def _add_logger(self):
-        self.logger = logging.getLogger('Dynamic Obstacles')
-        self.logger.setLevel(logging.DEBUG)
-
-        ch = logging.StreamHandler()
-        ch.setLevel(logging.DEBUG)
-
-        formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
-        ch.setFormatter(formatter)
-
-        self.logger.addHandler(ch)
+        return np.concatenate((agent_pos, agent_vel, np.concatenate(observed_obstacles, axis=0), observed_goal))
```

### Comparing `Signal8-3.5/Signal8/utils/core.py` & `Signal8-3.6/Signal8/utils/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class Entity:  # properties and state of physical world entity
     def __init__(self):
         # name
         self.name = ""
         # properties:
-        self.size = 0.1
+        self.size = 0.050
         # entity can move / be pushed
         self.movable = False
         # entity collides with others
         self.collide = True
         # color
         self.color = None
         # state
@@ -38,81 +38,67 @@
 
 class Goal(Entity): # properties of goal entities
     def __init__(self):
         super().__init__()
 
 
 class Obstacle(Entity):  # properties of obstacles entities
-    def __init__(self):
+    def __init__(self, size):
         super().__init__()
         # entity can be moved / pushed
         self.movable = False
-        # script behavior to execute
-        self.action_callback = None
-        self.lock = None
-    
-    # updates the state of the obstacle
-    def update(self, action=None, size=None, dt=0.1, damping=0.25):
-        with self.lock:
-            if action is not None:
-                self.state.p_vel = self.state.p_vel * (1 - damping)
-                self.state.p_vel += (action / self.mass) * dt
-                self.state.p_pos += self.state.p_vel * dt
-            elif size is not None:
-                self.size += size
-            else:
-                raise ValueError("Either action or size must be specified")
+        # entity size
+        self.size = size
         
 
 class Agent(Entity):  # properties of agent entities
     def __init__(self):
         super().__init__()
         # agents are movable by default
         self.movable = True
         # reached goal state
         self.goal_a = None
         self.reached_goal = False
         # reached start state after reaching goal
         self.goal_b = None
-        self.returned_to_safety = False
         # state
         self.state = AgentState()
         # action
         self.action = None
-        # how far the agent can see
+        # how far the agent can sense around itself
         self.max_observable_dist = 0.30
 
 class World:  # multi-agent world
     def __init__(self):
         # list of agents and entities (can change at execution-time!)
         self.agents = []
         self.goals = []
-        self.obstacles = []
+        self.small_obstacles = []
+        self.large_obstacles = []
         # position dimensionality
         self.dim_p = 2
         # color dimensionality
         self.dim_color = 3
         # simulation timestep
         self.dt = 0.1
         # physical damping
         self.damping = 0.25
         # contact response parameters
         self.contact_force = 1e2
         self.contact_margin = 1e-3
-        self.problem_type = None
+        # minimum distance required between entities (used for resetting positions)
+        self.buffer_dist = 0
+        # problem instance
         self.problem_instance = None
-        self.start_constr = None
-        self.goal_constr = None
-        self.static_obstacle_constr = None
-        self.dynamic_obstacle_constr = None
+        self.instance_constr = None
         
     # return all entities in the world
     @property
     def entities(self):
-        return self.agents + self.goals + self.obstacles
+        return self.agents + self.goals + self.large_obstacles
 
     # update state of the world
     def step(self):
         # gather forces applied to entities
         p_force = [None] * len(self.entities)
         # apply agent physical controls
         p_force = self.apply_action_force(p_force)
```

### Comparing `Signal8-3.5/Signal8/utils/simple_env.py` & `Signal8-3.6/Signal8/utils/simple_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,42 +40,52 @@
         self.width = 700
         self.height = 700
         self.screen = pygame.Surface([self.width, self.height])
         self.max_size = 1
         self.game_font = pygame.freetype.Font(None, 20)
 
         self.renderOn = False
-        self._reset_called = False
         self.seed()
+        self._reset_called = False
 
         self.max_cycles = max_cycles
         self.scenario = scenario
         self.world = world
         self.local_ratio = local_ratio
 
+        self.scenario.reset_world(self.world, self.np_random, 'corners')
         self.agents = [agent.name for agent in self.world.agents]
         self.possible_agents = self.agents[:]
         self._index_map = {agent.name: idx for idx, agent in enumerate(self.world.agents)}
 
         self._agent_selector = agent_selector(self.agents)
 
         # set spaces
         self.action_spaces = dict()
         self.observation_spaces = dict()
-        obs_dim = 14 if world.problem_type == 'disaster_response' else 24
+        
         for agent in self.world.agents:
             space_dim = self.world.dim_p * 2 + 1
             self.action_spaces[agent.name] = spaces.Discrete(space_dim)
+            obs_dim = len(self.scenario.observation(agent, self.world))
             self.observation_spaces[agent.name] = spaces.Box(
                 low=-np.float32(1),
                 high=+np.float32(1),
                 shape=(obs_dim,),
                 dtype=np.float32,
             )
-            
+        
+        # state space is used by aerial agent, encodes agents and large obstacles
+        state_dim = len(world.agents) * 2 + len(world.large_obstacles) * 2
+        self.state_space = spaces.Box(
+            low=-np.float32(1),
+            high=+np.float32(1),
+            shape=(state_dim,),
+            dtype=np.float32,
+        )
         self.steps = 0
         self.current_actions = [None] * self.num_agents
 
     def observation_space(self, agent):
         return self.observation_spaces[agent]
 
     def action_space(self, agent):
@@ -86,61 +96,63 @@
 
     def observe(self, agent):
         return self.scenario.observation(
             self.world.agents[self._index_map[agent]], self.world
         ).astype(np.float32)
         
     def state(self):
-        states = tuple(
-            self.scenario.observation(
-                self.world.agents[self._index_map[agent]], self.world
-            ).astype(np.float32)
-            for agent in self.possible_agents
-        )
-        return np.concatenate(states, axis=None)
+        if self.steps > 0:
+            raise Exception('The state of the system can only be retrieved at the start of an episode before any steps have been taken.')
+        
+        state = np.zeros(self.state_space.shape)
+        
+        for i, agent in enumerate(self.world.agents):
+            state[2*i : 2*i+2] = agent.state.p_pos
+
+        # Calculate the starting index for the obstacles in the state array
+        start_idx = 2 * len(self.world.agents)
+        for i, obstacle in enumerate(self.world.large_obstacles):
+            state[start_idx + 2*i : start_idx + 2*i+2] = obstacle.state.p_pos
+             
+        return np.concatenate(state, axis=None)
 
     def reset(self, seed=None, return_info=False, options=None):        
         if seed is not None:
             self.seed(seed=seed)
             
-        if 'instance_num' not in options:
-            raise ValueError("Must provide an instance_num to reset the environment with.")
+        if 'problem_instance' not in options:
+            raise ValueError("Must provide a problem_instance to reset the environment with.")
         
-        instance_num = options['instance_num']
-        if not 0 <= instance_num <= 3:
-            raise ValueError("instance_num must be between 0 and 3.")
+        problem_instance = options['problem_instance']
+        if problem_instance not in self.world.problem_list:
+            raise ValueError("problem_instance must be in the problem_list.")
         
-        self.scenario.reset_world(self.world, self.np_random, instance_num)
+        self.scenario.reset_world(self.world, self.np_random, problem_instance)
 
         self.agents = self.possible_agents[:]
-        # PettingZoo Gymansium requires rewards to be set
-        # even if they are not used
+        # PettingZoo Gymansium requires rewards to be set even if not used
         self.rewards = {name: 0.0 for name in self.agents}
         self._cumulative_rewards = {name: 0.0 for name in self.agents}
         self.terminations = {name: False for name in self.agents}
         self.truncations = {name: False for name in self.agents}
         self.infos = {name: {} for name in self.agents}
         
         self._reset_called = True
         self.agent_selection = self._agent_selector.reset()
         self.steps = 0
 
         self.current_actions = [None] * len(self.world.agents)
-        
+    
     def get_start_state(self):
         if not self._reset_called:
             raise Exception("Cannot get start state without calling reset() first")
         
         agent_pos = np.array([agent.state.p_pos for agent in self.world.agents])
         goal_pos = np.array([(agent.goal_a.state.p_pos, agent.goal_b.state.p_pos) for agent in self.world.agents])
-        try:
-            [obs.lock.acquire() for obs in self.world.obstacles if obs.lock is not None]
-            obs_pos = np.array([obs.state.p_pos for obs in self.world.obstacles])
-        finally:
-            [obs.lock.release() for obs in self.world.obstacles if obs.lock is not None]
+        obs_pos = np.array([obs.state.p_pos for obs in self.world.large_obstacles])
         
         entities = {'agents': agent_pos, 'goals': goal_pos, 'obstacles': obs_pos}
         return entities
         
     def _execute_world_step(self):
         # set action for each agent
         for i, agent in enumerate(self.world.agents):
@@ -188,52 +200,44 @@
             sensitivity = 2.0
             agent.action *= sensitivity
             action = action[1:]
         # make sure we used all elements of action
         assert len(action) == 0
     
     # Check if episode is terminated or truncated
-    def _episode_status(self):        
-        dynamic_obs = [obs for obs in self.world.obstacles if obs.movable]
-        static_obs = [obs for obs in self.world.obstacles if not obs.movable]
-
+    def _episode_status(self):    
         goal_dist_threshold = self.world.agents[0].size + self.world.agents[0].goal_a.size
-        static_obs_threshold = self.world.agents[0].size + static_obs[0].size
+        small_obs_threshold = self.world.agents[0].size + self.world.small_obstacles[0].size
+        large_obs_threshold = self.world.agents[0].size + self.world.large_obstacles[0].size
+        
+        small_obstacles = [obs for obs in self.world.small_obstacles]
+        large_obstacles = [obs for obs in self.world.large_obstacles]    
 
         goal_a_dist = [np.linalg.norm(agent.state.p_pos - agent.goal_a.state.p_pos) for agent in self.world.agents]
         goal_b_dist = [np.linalg.norm(agent.state.p_pos - agent.goal_b.state.p_pos) for agent in self.world.agents]
-        static_obs_dist = [min(np.linalg.norm(agent.state.p_pos - obs.state.p_pos) for obs in static_obs)
-                           for agent in self.world.agents]
+        small_obs_dist = [min(np.linalg.norm(agent.state.p_pos - obs.state.p_pos) for obs in small_obstacles)
+                          for agent in self.world.agents]
+        large_obs_dist = [min(np.linalg.norm(agent.state.p_pos - obs.state.p_pos) for obs in large_obstacles)
+                          for agent in self.world.agents]
 
-        crossed_threshold_static = [dist <= static_obs_threshold for dist in static_obs_dist]
-
-        [obs.lock.acquire() for obs in dynamic_obs]
-
-        try:
-            dynamic_obs_dist = [min(np.linalg.norm(agent.state.p_pos - obs.state.p_pos) for obs in dynamic_obs)
-                                for agent in self.world.agents] 
-            dynamic_obs_threshold = [agent.size + obs.size for agent, obs in zip(self.world.agents, dynamic_obs)]   
-
-            crossed_threshold_dynamic = [dist <= threshold for dist, threshold in zip(dynamic_obs_dist, dynamic_obs_threshold)]
+        crossed_threshold_small = [dist <= small_obs_threshold for dist in small_obs_dist]
+        crossed_threshold_large = [dist <= large_obs_threshold for dist in large_obs_dist]
+        
+        truncations = [(crossed_small or crossed_large) for crossed_small, crossed_large in zip(crossed_threshold_small, crossed_threshold_large)]
+        truncations = [True] * self.num_agents if self.steps >= self.max_cycles else truncations
 
-            truncations = [crossed_stat or crossed_dyn for crossed_stat, crossed_dyn in zip(crossed_threshold_static, crossed_threshold_dynamic)]
-            truncations = [True] * self.num_agents if self.steps >= self.max_cycles else truncations
+        terminations = [False] * self.num_agents
+        for i, dist in enumerate(goal_a_dist):
+            if dist <= goal_dist_threshold:
+                self.world.agents[i].reached_goal = True
 
-            terminations = [False] * self.num_agents
-            for i, dist in enumerate(goal_a_dist):
+        for i, dist in enumerate(goal_b_dist):
+            if self.world.agents[i].reached_goal:
                 if dist <= goal_dist_threshold:
-                    self.world.agents[i].reached_goal = True
-
-            for i, dist in enumerate(goal_b_dist):
-                if self.world.agents[i].reached_goal:
-                    if dist <= goal_dist_threshold:
-                        self.agents[i].reached_safety = True
-                        terminations[i] = True
-        finally:
-            [obs.lock.release() for obs in dynamic_obs]
+                    terminations[i] = True
 
         return {'terminations': terminations, 'truncations': truncations}
 
 
     def step(self, action):
         if (
             self.terminations[self.agent_selection]
@@ -313,9 +317,8 @@
                 0 < x < self.width and 0 < y < self.height
             ), f"Coordinates {(x, y)} are out of bounds."
 
     def close(self):
         if self.renderOn:
             pygame.event.pump()
             pygame.display.quit()
-            self.renderOn = False
-        self.unwrapped.scenario.stop_scripted_obstacles()
+            self.renderOn = False
```

### Comparing `Signal8-3.5/Signal8/utils/test_dynamic_obs.py` & `Signal8-3.6/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.5/Signal8.egg-info/PKG-INFO` & `Signal8-3.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,18 @@
-Metadata-Version: 2.1
-Name: Signal8
-Version: 3.5
-Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
-Home-page: https://github.com/ethanmclark1/signal8
-Author: Ethan Clark
-Author-email: eclark715@gmail.com.com
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # A Fork of Multi-Agent Particle Environment
 
 Signal8 is an enhanced version of the Simple environment, originally developed by the [Farama Foundation](https://farama.org/) as part of their [Multi-Agent Particle Environment (MPE)](https://pettingzoo.farama.org/environments/mpe/).
 
 # Signal8
 
 Signal8 is an open-source research project devoted to facilitating the evolution of communication strategies in multi-agent systems. The project, drawing inspiration from real-world scenarios such as disaster response and precision farming, features a dynamic environment that elevates the principles of the Lewis signaling game. This unique setting serves as a testing ground for the advancement of robot-to-robot communication protocols.
 
 Each problem set within Signal8 encompasses four distinct instances, with each one posing different constraints on the positioning of entities such as starting points, goals, and both static and dynamic obstacles. This dynamic feature fosters examination of communication strategies in diverse settings, enhancing the environment's realism and adaptability.
 
-A notable characteristic of Signal8 is its incorporation of asymmetric information, whereby two types of agents â€“ an 'eye in the sky' agent with global information and ground agents with only local information â€“ operate simultaneously. This asymmetry replicates real-world situations, presenting challenges for the development of efficient communication strategies. It also provides intriguing prospects for the generation of context-dependent language and high-level directives.
+A notable characteristic of Signal8 is its incorporation of asymmetric information, whereby two types of agents – an 'eye in the sky' agent with global information and ground agents with only local information – operate simultaneously. This asymmetry replicates real-world situations, presenting challenges for the development of efficient communication strategies. It also provides intriguing prospects for the generation of context-dependent language and high-level directives.
 
 In Signal8, both static and dynamic obstacles are present, creating further complexities for agents navigating through the environment. Static obstacles provide persistent barriers, while dynamic obstacles introduce predictable elements that can move or change over time. This complexity enriches the environment, making it an even more challenging and realistic platform for testing multi-agent communication strategies.
 
 For more information on utilizing the environment API, please refer to the [PettingZoo API documentation](https://pettingzoo.farama.org/content/basic_usage/).
 
 ## Installation
 
@@ -36,33 +24,33 @@
 ```
 
 ## Usage
 
 ```
 import Signal8
 
-env = Signal8.env(problem_type='disaster_response')
-env.reset(options={"instance_num": 0}))
+env = Signal8.env()
+env.reset(options={'problem_instance': 'corners'}))
 observation, _, terminations, truncations, _ = env.last()
 env.step(action)
 env.close()
 ```
 
 ## List of Problem Instances
 
-|   Problem Type   | Instance Name |                 Visualization                 |
-| :---------------: | :------------: | :--------------------------------------------: |
-| Disaster Response | ``instance 0`` | ![1686023513741](image/README/1686023513741.png) |
-| Disaster Response | ``instance 1`` | ![1686023519237](image/README/1686023519237.png) |
-| Disaster Response | ``instance 2`` | ![1686023523656](image/README/1686023523656.png) |
-| Disaster Response | ``instance 3`` | ![1686023529431](image/README/1686023529431.png) |
-| Precision Farming | ``instance 0`` | ![1686023534970](image/README/1686023534970.png) |
-| Precision Farming | ``instance 1`` | ![1686023540501](image/README/1686023540501.png) |
-| Precision Farming | ``instance 2`` | ![1686023545379](image/README/1686023545379.png) |
-| Precision Farming | ``instance 3`` | ![1686023549246](image/README/1686023549246.png) |
+| Problem Instance |                 Visualization                 |
+| :--------------: | :--------------------------------------------: |
+|  ``corners``   | ![1686604788813](image/README/1686604788813.png) |
+|   ``quarters``   | ![1686604799335](image/README/1686604799335.png) |
+|    ``cross``    | ![1686604808540](image/README/1686604808540.png) |
+|   ``cluster``   | ![1686604839072](image/README/1686604839072.png) |
+|     ``left``     | ![1686604845732](image/README/1686604845732.png) |
+|    ``right``    | ![1686604851758](image/README/1686604851758.png) |
+|      ``up``      | ![1686604859851](image/README/1686604859851.png) |
+|     ``down``     | ![1686604868138](image/README/1686604868138.png) |
 
 Each of the colored regions represents an area where the respective entity can be instantiated. Blue regions are starting regions, yellow regions represent goal regions and in the case of precision farming, if a goal region is not generated in the yellow region then changes to a static obstacle region but this is not the case for disaster response, instead the region where the goal was not instantiated does not impact the episode at all, the light red regions represent static obstacles, and dark red regions represent dynamic obstacles.
 
 In the case of disaster response, the dynamic obstacle does not move, instead it incrementally increases the obstacle radius to simulate a fire. In the precision farming case, the dynamic obstacle represents the behavior of a hockey rink ice cleaner moving in zig zags.
 
 ## Paper Citation
```

### Comparing `Signal8-3.5/setup.py` & `Signal8-3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="3.5",
+    version="3.6",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

