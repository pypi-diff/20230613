# Comparing `tmp/chess_ant-0.0.7.tar.gz` & `tmp/chess_ant-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_ant-0.0.7.tar", last modified: Thu Feb 23 10:17:34 2023, max compression
+gzip compressed data, was "chess_ant-0.0.8.tar", last modified: Tue Jun 13 11:28:03 2023, max compression
```

## Comparing `chess_ant-0.0.7.tar` & `chess_ant-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 10:17:34.606644 chess_ant-0.0.7/
--rw-rw-r--   0 root         (0) root         (0)    35149 2022-07-04 07:52:40.000000 chess_ant-0.0.7/LICENSE.txt
--rw-rw-r--   0 root         (0) root         (0)       61 2022-01-12 10:01:21.000000 chess_ant-0.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1955 2023-02-23 10:17:34.602644 chess_ant-0.0.7/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      847 2022-06-26 10:37:55.000000 chess_ant-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 10:17:34.582644 chess_ant-0.0.7/chess_ant/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-01-11 12:27:27.000000 chess_ant-0.0.7/chess_ant/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12958 2023-02-08 10:00:21.000000 chess_ant-0.0.7/chess_ant/chess_ant.py
--rw-r--r--   0 root         (0) root         (0)     2116 2022-08-22 12:06:02.000000 chess_ant-0.0.7/chess_ant/chess_mcts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 10:17:34.602644 chess_ant-0.0.7/chess_ant.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1955 2023-02-23 10:17:33.000000 chess_ant-0.0.7/chess_ant.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      360 2023-02-23 10:17:34.000000 chess_ant-0.0.7/chess_ant.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 10:17:33.000000 chess_ant-0.0.7/chess_ant.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      115 2023-02-23 10:17:33.000000 chess_ant-0.0.7/chess_ant.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 10:17:33.000000 chess_ant-0.0.7/chess_ant.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       93 2023-02-23 10:17:33.000000 chess_ant-0.0.7/chess_ant.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-02-23 10:17:33.000000 chess_ant-0.0.7/chess_ant.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       28 2022-08-11 11:55:44.000000 chess_ant-0.0.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-23 10:17:34.606644 chess_ant-0.0.7/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1941 2023-02-15 09:58:47.000000 chess_ant-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:28:02.992789 chess_ant-0.0.8/
+-rw-rw-r--   0 root         (0) root         (0)    35149 2022-07-04 07:52:40.000000 chess_ant-0.0.8/LICENSE.txt
+-rw-rw-r--   0 root         (0) root         (0)       61 2022-01-12 10:01:21.000000 chess_ant-0.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-06-13 11:28:02.992789 chess_ant-0.0.8/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      847 2022-06-26 10:37:55.000000 chess_ant-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:28:02.976789 chess_ant-0.0.8/chess_ant/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-01-11 12:27:27.000000 chess_ant-0.0.8/chess_ant/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    13067 2023-06-13 09:59:43.000000 chess_ant-0.0.8/chess_ant/chess_ant.py
+-rw-rw-r--   0 root         (0) root         (0)     2116 2023-05-14 14:21:00.000000 chess_ant-0.0.8/chess_ant/chess_mcts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:28:02.988789 chess_ant-0.0.8/chess_ant.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-06-13 11:28:02.000000 chess_ant-0.0.8/chess_ant.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      360 2023-06-13 11:28:02.000000 chess_ant-0.0.8/chess_ant.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 11:28:02.000000 chess_ant-0.0.8/chess_ant.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      115 2023-06-13 11:28:02.000000 chess_ant-0.0.8/chess_ant.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 11:28:02.000000 chess_ant-0.0.8/chess_ant.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       93 2023-06-13 11:28:02.000000 chess_ant-0.0.8/chess_ant.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-13 11:28:02.000000 chess_ant-0.0.8/chess_ant.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       28 2022-08-11 11:55:44.000000 chess_ant-0.0.8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 11:28:02.992789 chess_ant-0.0.8/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1941 2023-06-12 13:07:51.000000 chess_ant-0.0.8/setup.py
```

### Comparing `chess_ant-0.0.7/LICENSE.txt` & `chess_ant-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chess_ant-0.0.7/PKG-INFO` & `chess_ant-0.0.8/chess_ant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: chess_ant
-Version: 0.0.7
+Name: chess-ant
+Version: 0.0.8
 Summary: Simulator to solve chess problems with MCTS Solver and Genetic Programming.
 Home-page: https://github.com/akuroiwa/chess-ant
 Author: Akihiro Kuroiwa
 Author-email: akuroiwa@env-reform.com
 License: GNU/GPLv3+
 Keywords: evolutionary algorithms,genetic programming,gp,chess,fen,pgn
 Platform: any
```

### Comparing `chess_ant-0.0.7/README.md` & `chess_ant-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `chess_ant-0.0.7/chess_ant/chess_ant.py` & `chess_ant-0.0.8/chess_ant/chess_ant.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 import os
 
 import argparse
 import pandas as pd
 from collections import deque
 # import sys
 # from concurrent.futures.process import ProcessPoolExecutor
+from multiprocessing import Lock
 
 
 # def progn(*args):
 #     with ProcessPoolExecutor(max_workers=os.cpu_count()) as executor:
 #         for arg in args:
 #             executor.submit(arg)
 
@@ -71,14 +72,15 @@
         self.previous_length = float("inf")
         self.previous_is_check = False
         self.numVisits = 0
         self.improvement = 0
         self.shortcut = 0
         self.result = 0
         self.pruning = 0
+        self.lock = Lock()
 
     def _reset(self):
         self.previous_eaten = 0
         self.eaten = 0
         self.previous_length = float("inf")
         self.previous_is_check = False
         self.numVisits = 0
@@ -108,15 +110,15 @@
         # except ImportError or ModuleNotFoundError:
         # except:
             from chess_classification import ChessClassification
         self.mcts_instance.model = ChessClassification(output_dir)
 
     def selectNode_1(self):
         node = self.mcts_instance.selectNode_num(self.root, 1 / math.sqrt(1))
-        self._executeRound(node, 3)
+        self._executeRound(node, 1)
 
     def selectNode(self):
         node = self.mcts_instance.selectNode(self.root)
         self._executeRound(node, 2)
 
     def selectNode_3(self):
         node = self.mcts_instance.selectNode_num(self.root, 1 / math.sqrt(3))
@@ -247,16 +249,17 @@
 
 # Structure initializers
 toolbox.register("individual", tools.initIterate, creator.Individual, toolbox.expr_init)
 toolbox.register("population", tools.initRepeat, list, toolbox.individual)
 
 def evalArtificialAnt(individual):
     # Transform the tree expression to functionnal Python code
-    routine = gp.compile(individual, pset)
-    ant.run(routine)
+    with ant.lock:
+        routine = gp.compile(individual, pset)
+        ant.run(routine)
     return ant.eaten,
 
 toolbox.register("evaluate", evalArtificialAnt)
 toolbox.register("select", tools.selTournament, tournsize=7)
 toolbox.register("mate", gp.cxOnePoint)
 toolbox.register("expr_mut", gp.genFull, min_=0, max_=2)
 toolbox.register("mutate", gp.mutUniform, expr=toolbox.expr_mut, pset=pset)
@@ -280,15 +283,15 @@
     move = ant.get_prediction
     print('\nBest choice:\n', move)
 
     best_ind = tools.selBest(pop, 1)[0]
     print("\nBest individual is %s, %s" % (best_ind, best_ind.fitness.values))
 
     # return pop, hof, stats
-    return pop, hof, stats, move
+    return pop, hof, stats, move, move.uci()
 
 def run(fen=None, population=500, generation=15, dl=False, output_dir='outputs/'):
     if not fen:
         board = chess.Board()
     else:
         board = chess.Board(fen)
     n = 0
@@ -297,15 +300,15 @@
     while n < 100:
         if n%2 == 0:
             move = input("Enter move: ")
             move = chess.Move.from_uci(str(move))
             board.push(move)
         else:
             print("Computers Turn:")
-            pop, hof, stats, move = main(board.fen(), population, generation, dl, output_dir)
+            pop, hof, stats, move, uci = main(board.fen(), population, generation, dl, output_dir)
             board.push(move)
         print("\n")
         print(board)
         n += 1
 
 def selfPlay(fen=None, population=500, generation=15, dl=False, path="train-pgn", loop=1, create_pgn=False, output_dir='outputs/'):
     if create_pgn:
@@ -320,15 +323,15 @@
             game.headers["Event"]
             game.setup(board)
             node = game
         print("\n")
         print(board)
         print("\n")
         while not board.is_game_over():
-            pop, hof, stats, move = main(board.fen(), population, generation, dl, output_dir)
+            pop, hof, stats, move, uci = main(board.fen(), population, generation, dl, output_dir)
             board.push(move)
             print("\n")
             print(board)
             print("\n")
             if create_pgn:
                 node = node.add_variation(move)
         if create_pgn:
```

### Comparing `chess_ant-0.0.7/chess_ant/chess_mcts.py` & `chess_ant-0.0.8/chess_ant/chess_mcts.py`

 * *Files identical despite different names*

### Comparing `chess_ant-0.0.7/chess_ant.egg-info/PKG-INFO` & `chess_ant-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: chess-ant
-Version: 0.0.7
+Name: chess_ant
+Version: 0.0.8
 Summary: Simulator to solve chess problems with MCTS Solver and Genetic Programming.
 Home-page: https://github.com/akuroiwa/chess-ant
 Author: Akihiro Kuroiwa
 Author-email: akuroiwa@env-reform.com
 License: GNU/GPLv3+
 Keywords: evolutionary algorithms,genetic programming,gp,chess,fen,pgn
 Platform: any
```

### Comparing `chess_ant-0.0.7/setup.py` & `chess_ant-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import glob
 from setuptools import setup, find_packages
 
 setup(
     name='chess_ant',
-    version='0.0.7',
+    version='0.0.8',
     url='https://github.com/akuroiwa/chess-ant',
     # # PyPI url
     # download_url='',
     license='GNU/GPLv3+',
     author='Akihiro Kuroiwa',
     author_email='akuroiwa@env-reform.com',
     description='Simulator to solve chess problems with MCTS Solver and Genetic Programming.',
```

