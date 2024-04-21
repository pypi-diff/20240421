# Comparing `tmp/py_wanderer-1.0.3.tar.gz` & `tmp/py_wanderer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_wanderer-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_wanderer-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_wanderer-1.0.3.tar` & `py_wanderer-1.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1102 2024-04-18 01:43:22.051405 py_wanderer-1.0.3/LICENSE
--rw-r--r--   0        0        0      563 2024-04-19 13:35:24.710119 py_wanderer-1.0.3/py_wanderer/__init__.py
--rw-r--r--   0        0        0    10691 2024-04-19 13:22:41.475609 py_wanderer-1.0.3/py_wanderer/algorithms.py
--rw-r--r--   0        0        0     2360 2024-04-17 23:41:47.137929 py_wanderer-1.0.3/py_wanderer/heuristics.py
--rw-r--r--   0        0        0     3030 2024-04-18 01:53:51.748090 py_wanderer-1.0.3/py_wanderer/maze.py
--rw-r--r--   0        0        0      527 2024-04-18 01:58:25.863533 py_wanderer-1.0.3/py_wanderer/plotter.py
--rw-r--r--   0        0        0      421 2024-04-18 18:32:04.901324 py_wanderer-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 py_wanderer-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-18 01:43:22.051405 py_wanderer-1.0.4/LICENSE
+-rw-r--r--   0        0        0      563 2024-04-21 15:52:41.035632 py_wanderer-1.0.4/py_wanderer/__init__.py
+-rw-r--r--   0        0        0    10691 2024-04-19 13:22:41.475609 py_wanderer-1.0.4/py_wanderer/algorithms.py
+-rw-r--r--   0        0        0     2360 2024-04-17 23:41:47.137929 py_wanderer-1.0.4/py_wanderer/heuristics.py
+-rw-r--r--   0        0        0     3257 2024-04-21 15:51:54.034337 py_wanderer-1.0.4/py_wanderer/maze.py
+-rw-r--r--   0        0        0     1194 2024-04-21 15:50:33.927889 py_wanderer-1.0.4/py_wanderer/plotter.py
+-rw-r--r--   0        0        0      421 2024-04-18 18:32:04.901324 py_wanderer-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 py_wanderer-1.0.4/PKG-INFO
```

### Comparing `py_wanderer-1.0.3/LICENSE` & `py_wanderer-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_wanderer-1.0.3/py_wanderer/__init__.py` & `py_wanderer-1.0.4/py_wanderer/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Maze builder and pathfinding algorithms."""
 
 from .algorithms import ALGORITHMS, PathfindingAlgorithm, Heuristic
 from .heuristics import HEURISTICS
 from .maze import Maze
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 ALGORITHMS = ALGORITHMS
 HEURISTICS = HEURISTICS
 
 
 def __getattr__(name):
     if name in globals():
```

### Comparing `py_wanderer-1.0.3/py_wanderer/algorithms.py` & `py_wanderer-1.0.4/py_wanderer/algorithms.py`

 * *Files identical despite different names*

### Comparing `py_wanderer-1.0.3/py_wanderer/heuristics.py` & `py_wanderer-1.0.4/py_wanderer/heuristics.py`

 * *Files identical despite different names*

### Comparing `py_wanderer-1.0.3/py_wanderer/maze.py` & `py_wanderer-1.0.4/py_wanderer/maze.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import random
 
+
 class Maze:
-    def __init__(self, width, height, start=None, end = None, num_rooms = 3, room_size_range = (3, 5)):
+    def __init__(self, width, height, start=None, end=None, num_rooms=3, room_size_range=(3, 5)):
         if width % 2 == 0 or height % 2 == 0:
             raise ValueError("Maze dimensions must be odd to ensure proper wall and path placement.")
         self.width = width
         self.height = height
         self.start = start if start else (1, 1)
         self.end = end if end else (height - 2, width - 2)
         self.num_rooms = num_rooms
@@ -54,31 +55,34 @@
         for x in range(self.width):
             self.maze[0][x] = 1
             self.maze[self.height - 1][x] = 1
         for y in range(self.height):
             self.maze[y][0] = 1
             self.maze[y][self.width - 1] = 1
 
-    def solve(self, pathfinder, heuristic):
+    def solve(self, pathfinder, heuristic) -> list[tuple[int, int]]:
         if not self.maze:
             self.generate()
         return pathfinder(self.maze, self.start, self.end, heuristic).run()
-    
+
+    def solve_many(self, pairs) -> list[tuple[str, list[tuple[int, int]]]]:
+        return [(f"{algorithm.__name__}: {heuristic.__name__}", self.solve(algorithm, heuristic))
+                for algorithm, heuristic in pairs]
+
     @property
     def maze(self):
         if not (self.__dict__.get("_maze")):
             self.generate()
         return self._maze
-    
+
     @maze.setter
     def maze(self, value):
         self.__dict__["_maze"] = value
 
+
 if __name__ == "__main__":
     from algorithms import AStar
     from heuristics import manhattan
+
     maze = Maze(21, 21, (1, 1))
     print(maze.maze)
     print(maze.solve(AStar, manhattan))
-
-            
-
```

