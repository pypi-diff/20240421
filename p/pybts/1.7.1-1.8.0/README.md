# Comparing `tmp/pybts-1.7.1.tar.gz` & `tmp/pybts-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybts-1.7.1.tar", max compression
+gzip compressed data, was "pybts-1.8.0.tar", max compression
```

## Comparing `pybts-1.7.1.tar` & `pybts-1.8.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0   157658 2024-04-15 10:19:50.544755 pybts-1.7.1/README.assets/DEMO_Sequence  10-10 _ 100.png
--rw-r--r--   0        0        0   189323 2024-04-15 10:19:50.544755 pybts-1.7.1/README.assets/image-20240329031220580.png
--rw-r--r--   0        0        0   208202 2024-04-15 10:19:50.544755 pybts-1.7.1/README.assets/image-20240329031233459.png
--rw-r--r--   0        0        0   255608 2024-04-15 10:19:50.544755 pybts-1.7.1/README.assets/image-20240401211552611.png
--rw-r--r--   0        0        0   202283 2024-04-15 10:19:50.548755 pybts-1.7.1/README.assets/image-20240401211609525.png
--rw-r--r--   0        0        0     5960 2024-04-15 10:19:50.548755 pybts-1.7.1/README.md
--rw-r--r--   0        0        0      385 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/__init__.py
--rw-r--r--   0        0        0       52 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/board/__init__.py
--rw-r--r--   0        0        0     2258 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/board/board.py
--rw-r--r--   0        0        0    11048 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/board/server.py
--rw-r--r--   0        0        0     8197 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/builder.py
--rw-r--r--   0        0        0      596 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/__init__.py
--rw-r--r--   0        0        0     9344 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/composite.py
--rw-r--r--   0        0        0     2175 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/condition_branch.py
--rw-r--r--   0        0        0     5460 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/parallel.py
--rw-r--r--   0        0        0      945 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/ppa.py
--rw-r--r--   0        0        0     2235 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/selector.py
--rw-r--r--   0        0        0     2460 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/sequence.py
--rw-r--r--   0        0        0     1510 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/switcher.py
--rw-r--r--   0        0        0      182 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/template.py
--rw-r--r--   0        0        0     3243 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/constants.py
--rw-r--r--   0        0        0     4943 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/converter.py
--rw-r--r--   0        0        0      121 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/decorators/__init__.py
--rw-r--r--   0        0        0    22898 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/decorators/nodes.py
--rw-r--r--   0        0        0     1073 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/display.py
--rw-r--r--   0        0        0     1521 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/main.py
--rw-r--r--   0        0        0    17662 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/nodes.py
--rw-r--r--   0        0        0       63 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/rl/__init__.py
--rw-r--r--   0        0        0     8803 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/rl/base_class.py
--rw-r--r--   0        0        0      268 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/rl/builder.py
--rw-r--r--   0        0        0      460 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/rl/common.py
--rw-r--r--   0        0        0    15167 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/rl/nodes.py
--rw-r--r--   0        0        0     5687 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/rl/off_policy.py
--rw-r--r--   0        0        0     8587 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/rl/on_policy.py
--rw-r--r--   0        0        0     1218 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/rl/tree.py
--rw-r--r--   0        0        0    16958 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/templates/favicon.ico
--rw-r--r--   0        0        0      433 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/templates/index.html
--rw-r--r--   0        0        0  1967920 2024-04-15 10:19:50.560755 pybts-1.7.1/pybts/templates/static/index-BlldS3Jx.js
--rw-r--r--   0        0        0   320362 2024-04-15 10:19:50.564755 pybts-1.7.1/pybts/templates/static/index-DN1S--qx.css
--rw-r--r--   0        0        0     5267 2024-04-15 10:19:50.564755 pybts-1.7.1/pybts/templates/static/info-lb9hZOuB.png
--rw-r--r--   0        0        0     2140 2024-04-15 10:19:50.564755 pybts-1.7.1/pybts/tree.py
--rw-r--r--   0        0        0    10045 2024-04-15 10:19:50.564755 pybts-1.7.1/pybts/utility.py
--rw-r--r--   0        0        0      844 2024-04-15 10:19:50.564755 pybts-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 pybts-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0   157658 2024-04-21 09:33:56.611530 pybts-1.8.0/README.assets/DEMO_Sequence  10-10 _ 100.png
+-rw-r--r--   0        0        0   189323 2024-04-21 09:33:56.611530 pybts-1.8.0/README.assets/image-20240329031220580.png
+-rw-r--r--   0        0        0   208202 2024-04-21 09:33:56.611530 pybts-1.8.0/README.assets/image-20240329031233459.png
+-rw-r--r--   0        0        0   255608 2024-04-21 09:33:56.611530 pybts-1.8.0/README.assets/image-20240401211552611.png
+-rw-r--r--   0        0        0   202283 2024-04-21 09:33:56.615531 pybts-1.8.0/README.assets/image-20240401211609525.png
+-rw-r--r--   0        0        0     5960 2024-04-21 09:33:56.615531 pybts-1.8.0/README.md
+-rw-r--r--   0        0        0      385 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/board/__init__.py
+-rw-r--r--   0        0        0     2740 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/board/board.py
+-rw-r--r--   0        0        0    11048 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/board/server.py
+-rw-r--r--   0        0        0     8225 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/builder.py
+-rw-r--r--   0        0        0      608 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/__init__.py
+-rw-r--r--   0        0        0    10363 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/composite.py
+-rw-r--r--   0        0        0     3360 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/condition_branch.py
+-rw-r--r--   0        0        0     5460 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/parallel.py
+-rw-r--r--   0        0        0      945 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/ppa.py
+-rw-r--r--   0        0        0     3221 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/selector.py
+-rw-r--r--   0        0        0     3354 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/sequence.py
+-rw-r--r--   0        0        0     1716 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/switcher.py
+-rw-r--r--   0        0        0      182 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/template.py
+-rw-r--r--   0        0        0     4998 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/constants.py
+-rw-r--r--   0        0        0     5981 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/converter.py
+-rw-r--r--   0        0        0      121 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/decorators/__init__.py
+-rw-r--r--   0        0        0    23244 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/decorators/nodes.py
+-rw-r--r--   0        0        0     3269 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/display.py
+-rw-r--r--   0        0        0     1521 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/main.py
+-rw-r--r--   0        0        0    18037 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/nodes.py
+-rw-r--r--   0        0        0      107 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/__init__.py
+-rw-r--r--   0        0        0     8803 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/base_class.py
+-rw-r--r--   0        0        0      268 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/builder.py
+-rw-r--r--   0        0        0     1742 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/common.py
+-rw-r--r--   0        0        0     2703 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/logger.py
+-rw-r--r--   0        0        0    15148 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/nodes.py
+-rw-r--r--   0        0        0     5784 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/off_policy.py
+-rw-r--r--   0        0        0     8587 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/on_policy.py
+-rw-r--r--   0        0        0     1218 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/tree.py
+-rw-r--r--   0        0        0    16958 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/templates/favicon.ico
+-rw-r--r--   0        0        0      433 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/templates/index.html
+-rw-r--r--   0        0        0  1967920 2024-04-21 09:33:56.631531 pybts-1.8.0/pybts/templates/static/index-BlldS3Jx.js
+-rw-r--r--   0        0        0   320362 2024-04-21 09:33:56.631531 pybts-1.8.0/pybts/templates/static/index-DN1S--qx.css
+-rw-r--r--   0        0        0     5267 2024-04-21 09:33:56.631531 pybts-1.8.0/pybts/templates/static/info-lb9hZOuB.png
+-rw-r--r--   0        0        0     2140 2024-04-21 09:33:56.631531 pybts-1.8.0/pybts/tree.py
+-rw-r--r--   0        0        0    10211 2024-04-21 09:33:56.631531 pybts-1.8.0/pybts/utility.py
+-rw-r--r--   0        0        0      844 2024-04-21 09:33:56.631531 pybts-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 pybts-1.8.0/PKG-INFO
```

### Comparing `pybts-1.7.1/README.assets/DEMO_Sequence  10-10 _ 100.png` & `pybts-1.8.0/README.assets/DEMO_Sequence  10-10 _ 100.png`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/README.assets/image-20240329031220580.png` & `pybts-1.8.0/README.assets/image-20240329031220580.png`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/README.assets/image-20240329031233459.png` & `pybts-1.8.0/README.assets/image-20240329031233459.png`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/README.assets/image-20240401211552611.png` & `pybts-1.8.0/README.assets/image-20240401211552611.png`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/README.assets/image-20240401211609525.png` & `pybts-1.8.0/README.assets/image-20240401211609525.png`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/README.md` & `pybts-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/pybts/board/board.py` & `pybts-1.8.0/pybts/board/board.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,36 @@
 import os
 import time
 import typing
 
 from pybts import utility
 from pybts.tree import Tree
 
+
 class Board:
     def __init__(self, tree: Tree, log_dir: str = '.'):
+        """
+        :param tree: Board监听的树
+        :param log_dir: Board的日志存储目录
+
+        """
         self.tree = tree
         self.project = tree.name
         self.log_dir = os.path.join(log_dir, self.project)
         self.history_dir = os.path.join(self.log_dir, 'pybts-history')
         self.current_path = os.path.join(self.log_dir, 'pybts.json')
         os.makedirs(self.history_dir, exist_ok=True)
         self.track_id = 0
 
-    def track(self, info: dict = None):
+    def track(self, info: dict = None, render: bool = False, render_format: str = 'png'):
         """
         track当前运行信息
         :param info: 额外信息
+        :param render: 是否画出来图
+        :param render_format: 画图的格式
         :return:
         """
         self.track_id += 1
         json_data = {
             'id'   : self.track_id,
             'step' : self.tree.count,
             'round': self.tree.round,
@@ -40,14 +48,18 @@
                     'tree': tree_data
                 }, f, ensure_ascii=False)
             except Exception as e:
                 print(e)
                 raise e
         with open(self.current_path, 'w') as f:
             utility.json_dump(json_data, f, ensure_ascii=False)
+        if render:
+            from pybts.display import render_node
+            render_path = os.path.join(self.history_dir, f'{self.track_id}.{render_format}')
+            render_node(node=self.tree.root, filepath=render_path)
 
     def clear(self):
         self.track_id = 0
         utility.clear_project(self.log_dir, self.tree.name)
 
     def iterate(self) -> typing.Iterator[dict]:
         # 遍历所有的历史数据
@@ -58,8 +70,7 @@
         if os.path.exists(self.history_dir):
             for filename in os.listdir(self.history_dir):
                 if filename.endswith('.json'):
                     filepath = os.path.join(self.history_dir, filename)
                     with open(filepath, 'r', encoding='utf') as f:
                         json_data = utility.json_loads(f.read())
                         yield json_data
-
```

### Comparing `pybts-1.7.1/pybts/board/server.py` & `pybts-1.8.0/pybts/board/server.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/pybts/builder.py` & `pybts-1.8.0/pybts/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
                 SequenceWithMemory,
                 ReactiveSequence,
                 Parallel,
                 ReactiveSelector,
                 Selector,
                 ReactiveSelector,
                 SelectorWithMemory,
+                CondBranch,
                 ConditionBranch,
                 Template,
                 PreCondition,
                 PostCondition,
                 Switcher,
                 ReactiveSwitcher,
         )
```

### Comparing `pybts-1.7.1/pybts/composites/__init__.py` & `pybts-1.8.0/pybts/composites/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .composite import Composite
 from .parallel import Parallel
 from .selector import Selector, SelectorWithMemory, ReactiveSelector
 from .sequence import Sequence, SequenceWithMemory, ReactiveSequence
-from .condition_branch import ConditionBranch
+from .condition_branch import CondBranch, ConditionBranch
 from .template import Template
 from .ppa import PreCondition, PostCondition
 from .switcher import Switcher, ReactiveSwitcher
 # TODO: RUNNING节点的打断操作应该怎么在行为树上体现出来
 # 通过ReactiveSelector/ReactiveSequence来起到打断后续节点的效果
 # ReactiveSequence: 前面的节点条件如果满足，则会一直
```

### Comparing `pybts-1.7.1/pybts/composites/composite.py` & `pybts-1.8.0/pybts/composites/composite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import py_trees
 from pybts.nodes import Node
 from abc import ABC
 import typing
 from py_trees.common import Status
 from py_trees import behaviour
 import itertools
@@ -211,31 +212,33 @@
         Returns:
             uuid.UUID: unique id of the child
         """
         self.children.insert(index, child)
         child.parent = self
         return child.id
 
-    def SEQ_SEL_tick(
+    def seq_sel_tick(
             self,
             tick_again_status: list[Status],
             continue_status: list[Status],
             no_child_status: Status,
-            start_index: int = 0
+            start_index: int | typing.Callable[['Composite'], int] = 0
     ):
         """Sequence/Selector的tick逻辑"""
         self.debug_info['tick_count'] += 1
         self.logger.debug("%s.tick()" % (self.__class__.__name__))
 
         if self.status in tick_again_status:
             # 重新执行上次执行的子节点
             assert self.current_child is not None
             index = self.children.index(self.current_child)
         else:
             self.current_child = None  # 从头执行
+            if callable(start_index):
+                start_index = start_index(self)
             index = start_index
 
         for child in itertools.islice(self.children, index, None):
             self.current_child = child
             yield from child.tick()
             if child.status not in continue_status:
                 break
@@ -248,30 +251,59 @@
             # 剩余的子节点全部停止
             for child in itertools.islice(self.children, index + 1, None):
                 # 清除子节点的状态（停止正在执行的子节点）
                 child.stop(Status.INVALID)
         else:
             new_status = no_child_status
 
-        # TODO: 这里要不要加这个是存疑的（组合节点invalid stop会停止所有子节点，所以某个子节点返回invalid是否要将所有的其他节点都停止？）
-        # if new_status != Status.RUNNING:
-        #     self.stop(new_status)
+        # # TODO: 这里要不要加这个是存疑的（组合节点invalid stop会停止所有子节点，所以某个子节点返回invalid是否要将所有的其他节点都停止？）
+        if new_status != Status.RUNNING:
+            self.stop(new_status)
 
         self.status = new_status
         yield self
 
-    def switch_tick(self, index: int, tick_again_status: list[Status]) -> typing.Iterator[py_trees.behaviour.Behaviour]:
+    def switch_tick(self, index: int | typing.Callable[['Composite'], int], tick_again_status: list[Status]) -> \
+            typing.Iterator[py_trees.behaviour.Behaviour]:
         if self.status in tick_again_status:
             # 重新执行上次执行的子节点
             assert self.current_child is not None
         else:
+            if callable(index):
+                index = index(self)
             self.current_child = self.children[index]  # 执行对应的index
 
         yield from self.current_child.tick()
         for child in self.children:
             if child != self.current_child:
                 # 清除子节点的状态（停止正在执行的子节点）
                 child.stop(Status.INVALID)
 
         self.status = self.current_child.status
         yield self
 
+    def gen_index(self):
+        """每个组合节点都有对于这个函数的不同定义"""
+        return 0
+
+    @property
+    def reactive(self) -> bool:
+        return self.converter.bool(self.attrs.get('reactive', False))
+
+    @property
+    def memory(self) -> bool:
+        return self.converter.bool(self.attrs.get('memory', False))
+
+    @property
+    def current_index(self):
+        if self.current_child is None:
+            return None
+        else:
+            return self.children.index(self.current_child)
+
+    def to_data(self):
+        return {
+            **super().to_data(),
+            'reactive'     : self.reactive,
+            'memory'       : self.memory,
+            'current_index': self.current_index
+        }
```

### Comparing `pybts-1.7.1/pybts/composites/condition_branch.py` & `pybts-1.8.0/pybts/composites/condition_branch.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from py_trees.behaviour import Behaviour
 import typing
 from py_trees.common import Status
 from pybts.composites.composite import Composite
 
 
-class ConditionBranch(Composite):
+class CondBranch(Composite):
     """
     条件分支节点
     只能有2或3个子节点
 
     也可以起到打断RUNNING节点的效果（由前面的条件节点来判断是否要进行打断）
 
     2个子节点，当前面的节点执行成功时，执行第二个节点
@@ -32,38 +32,78 @@
     <Parallel>
     """
 
     def setup(self, **kwargs: typing.Any) -> None:
         super().setup(**kwargs)
         assert len(self.children) in [2, 3], 'ConditionBranch must have 2 or 3 children'
 
-    def tick(self) -> typing.Iterator[Behaviour]:
+    def cond_tick(self: Composite, tick_again_status: list[Status]):
+        if self.status in tick_again_status and self.current_index != 0:
+            assert self.current_child is not None
+            # 重新执行上次执行的动作节点
+            yield from self.current_child.tick()
+            new_status = self.current_child.status
+            if new_status != Status.RUNNING:
+                self.stop(new_status)
+            self.status = new_status
+            yield self
+            return
+
         condition = self.children[0]
         self.current_child = condition
-
         yield from condition.tick()
 
-        exec_child = None  # 准备执行的节点
+        if condition.status == Status.RUNNING:
+            self.status = Status.RUNNING
+            yield self
+            return
 
         if condition.status == Status.SUCCESS:
             # 执行第1个节点
-            exec_child = self.children[1]
+            self.current_child = self.children[1]
         elif condition.status == Status.FAILURE:
             # 执行第2个节点（如果第二个节点存在的话）
             if len(self.children) == 3:
-                exec_child = self.children[2]
-
-        if condition.status != Status.RUNNING:
-            # 如果条件的状态是RUNNING，则不停止其他节点
-            for child in self.children[1:]:
-                # 停止其他节点
-                if child != exec_child:
-                    child.stop(Status.INVALID)
+                self.current_child = self.children[2]
+            else:
+                self.current_child = None
+
+        for child in self.children[1:]:
+            # 停止其他节点
+            if child != self.current_child:
+                child.stop(Status.INVALID)
 
         # 执行选择的子节点
-        if exec_child is not None:
-            self.current_child = exec_child
-            yield from exec_child.tick()
-
-        new_status = self.current_child.status
+        if self.current_child is not None:
+            yield from self.current_child.tick()
+            new_status = self.current_child.status
+        else:
+            new_status = condition.status
+        if new_status != Status.RUNNING:
+            self.stop(new_status)
         self.status = new_status
         yield self
+
+    def tick(self) -> typing.Iterator[Behaviour]:
+        if self.reactive:
+            return self.cond_tick(tick_again_status=[])
+        elif self.memory:
+            return self.cond_tick(tick_again_status=[Status.RUNNING, Status.FAILURE])
+        else:
+            return self.cond_tick(tick_again_status=[Status.RUNNING])
+
+
+class ConditionBranch(CondBranch):
+    """条件分支节点的别名"""
+    pass
+
+
+class ReactiveCondBranch(CondBranch):
+
+    def reactive(self) -> bool:
+        return True
+
+
+class CondBranchWithMemory(CondBranch):
+
+    def memory(self) -> bool:
+        return True
```

### Comparing `pybts-1.7.1/pybts/composites/parallel.py` & `pybts-1.8.0/pybts/composites/parallel.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/pybts/composites/ppa.py` & `pybts-1.8.0/pybts/composites/ppa.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/pybts/composites/selector.py` & `pybts-1.8.0/pybts/composites/sequence.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,84 @@
-import py_trees
 import typing
 from py_trees.common import Status
 from py_trees import behaviour
 from pybts.composites.composite import Composite
 
 
-class Selector(Composite):
+class Sequence(Composite):
     """
-    组合节点：选择节点
+    组合节点：顺序节点 ->
     依次顺序执行子节点
-    - 当前执行节点返回 FAILURE/INVALID，继续执行后续节点
+    - 当前执行节点返回 SUCCESS，继续执行后续节点
     - 当前执行节点返回 RUNNING，停止执行后续节点，下次执行还是从这个节点开始
-    - 当前执行节点返回 SUCCESS，停止执行后续节点，下次执行从第一个节点开始
-    返回最后一个执行节点的状态，如果没有孩子，则返回FAILURE
+    - 当前执行节点返回 FAILURE/INVALID，停止执行后续节点，下次执行从第一个节点开始
+    返回最后一个执行节点的状态，如果没有孩子，则返回SUCCESS
     """
 
-    def tick(self) -> typing.Iterator[behaviour.Behaviour]:
-        return self.SEQ_SEL_tick(
-                tick_again_status=[Status.RUNNING],
-                continue_status=[Status.FAILURE, Status.INVALID],
-                no_child_status=Status.FAILURE,
-                start_index=0)
+    def gen_index(self):
+        return 0
 
+    def tick(self: Composite) -> typing.Iterator[behaviour.Behaviour]:
+        if self.reactive:
+            return self.seq_sel_tick(
+                    tick_again_status=[],
+                    continue_status=[Status.SUCCESS],
+                    no_child_status=Status.SUCCESS,
+                    start_index=lambda _: self.gen_index())
+        elif self.memory:
+            return self.seq_sel_tick(
+                    tick_again_status=[Status.RUNNING, Status.FAILURE],
+                    continue_status=[Status.SUCCESS],
+                    no_child_status=Status.SUCCESS,
+                    start_index=lambda _: self.gen_index())
+        else:
+            return self.seq_sel_tick(
+                    tick_again_status=[Status.RUNNING],
+                    continue_status=[Status.SUCCESS],
+                    no_child_status=Status.SUCCESS,
+                    start_index=lambda _: self.gen_index())
 
-class SelectorWithMemory(Selector):
+
+class SequenceWithMemory(Sequence):
     """
-    记忆选择节点
-    - 当前执行节点返回 FAILURE/INVALID，继续执行后续节点
-    - 当前执行节点返回 SUCCESS/RUNNING，停止执行后续节点，下次执行还是从这个节点开始
-    返回最后一个执行节点的状态，如果没有孩子，则返回FAILURE
+    记忆顺序节点
+    依次顺序执行子节点
+    - 当前执行节点返回 SUCCESS，继续执行后续节点
+    - 当前执行节点返回 FAILURE/RUNNING，停止执行后续节点，下次执行还是从这个节点开始
+    - 当前执行节点返回 INVALID，停止执行后续节点，下次执行从第一个节点开始
+    返回最后一个执行节点的状态，如果没有孩子，则返回SUCCESS
     """
 
-    def tick(self) -> typing.Iterator[behaviour.Behaviour]:
-        return self.SEQ_SEL_tick(
-                tick_again_status=[Status.SUCCESS, Status.RUNNING],
-                continue_status=[Status.FAILURE, Status.INVALID],
-                no_child_status=Status.FAILURE,
-                start_index=0)
+    @property
+    def memory(self) -> bool:
+        return True
+
+    def tick(self: Composite) -> typing.Iterator[behaviour.Behaviour]:
+        return self.seq_sel_tick(
+                tick_again_status=[Status.RUNNING, Status.FAILURE],
+                continue_status=[Status.SUCCESS],
+                no_child_status=Status.SUCCESS,
+                start_index=lambda _: self.gen_index())
 
 
-class ReactiveSelector(Selector):
+class ReactiveSequence(Sequence):
     """
-    反应式选择节点
+    反应式顺序节点
     依次顺序执行子节点
-    - 当前执行节点返回 FAILURE/INVALID，继续执行后续节点
-    - 当前执行节点返回 SUCCESS/RUNNING，停止执行后续节点，下次执行从第一个节点开始
-    返回最后一个执行节点的状态，如果没有孩子，则返回FAILURE
+    - 当前执行节点返回 SUCCESS，继续执行后续节点
+    - 当前执行节点返回 FAILURE/RUNNING/INVALID，停止执行后续节点，下次执行从第一个节点开始
+    返回最后一个执行节点的状态，如果没有孩子，则返回SUCCESS
+
+    可以起到打断后续RUNNING节点的效果
+    - 如果前面的节点返回SUCCESS，则后续的RUNNING节点会继续运行，否则就会打断掉
     """
 
-    def tick(self) -> typing.Iterator[behaviour.Behaviour]:
-        return self.SEQ_SEL_tick(
+    @property
+    def reactive(self) -> bool:
+        return True
+
+    def tick(self: Composite) -> typing.Iterator[behaviour.Behaviour]:
+        return self.seq_sel_tick(
                 tick_again_status=[],
-                continue_status=[Status.FAILURE, Status.INVALID],
-                no_child_status=Status.FAILURE,
-                start_index=0)
+                continue_status=[Status.SUCCESS],
+                no_child_status=Status.SUCCESS,
+                start_index=lambda _: self.gen_index())
```

### Comparing `pybts-1.7.1/pybts/constants.py` & `pybts-1.8.0/pybts/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 
 def _echarts_color(color: str) -> str:
     r, g, b = _hex_color(color)
     return f'rgb({r},{g},{b})'
 
 
+def _pydot_color(color: str) -> str:
+    return f'#{color}'
+
+
 # Map of color names to RGB values
 ECHARTS_COLORS = {
     # "red"   : _echarts_color('d81e06'),
     "red"       : _echarts_color('F95D7B'),
     # "blue"  : _echarts_color('1296db'), # 0AD2F3
     'blue'      : _echarts_color('0AD2F3'),
     # "green" : _echarts_color('1afa29'),
@@ -30,40 +34,88 @@
     # "grey"  : _echarts_color('8a8a8a'),
     'grey'      : _echarts_color('888888'),
     'light_grey': _echarts_color('bbbbbb'),
     'black'     : _echarts_color('555555'),
     'white'     : _echarts_color('ffffff')
 }
 
+PYDOT_COLORS = {
+    # "red"   : _echarts_color('d81e06'),
+    "red"       : _pydot_color('F95D7B'),
+    # "blue"  : _echarts_color('1296db'), # 0AD2F3
+    'blue'      : _pydot_color('0AD2F3'),
+    # "green" : _echarts_color('1afa29'),
+    'green'     : _pydot_color('3BBD73'),
+    "pink"      : _pydot_color('d4237a'),
+    'purple'    : _pydot_color('AB69E9'),
+    # "yellow": _echarts_color('f4ea2a'),
+    'yellow'    : _pydot_color('FED969'),
+    # "grey"  : _echarts_color('8a8a8a'),
+    'grey'      : _pydot_color('888888'),
+    'light_grey': _pydot_color('bbbbbb'),
+    'black'     : _pydot_color('555555'),
+    'white'     : _pydot_color('ffffff')
+}
+
 STATUS_TO_ECHARTS_SYMBOL_COLORS = {
     Status.SUCCESS.name: ECHARTS_COLORS['blue'],
     Status.FAILURE.name: ECHARTS_COLORS['red'],
     Status.RUNNING.name: ECHARTS_COLORS['yellow'],
     Status.INVALID.name: ECHARTS_COLORS['grey'],
 }
 
+STATUS_TO_PYDOT_SYMBOL_COLORS = {
+    Status.SUCCESS.name: PYDOT_COLORS['blue'],
+    Status.FAILURE.name: PYDOT_COLORS['red'],
+    Status.RUNNING.name: PYDOT_COLORS['yellow'],
+    Status.INVALID.name: PYDOT_COLORS['grey'],
+}
+
 STATUS_TO_ECHARTS_LINE_STYLE_COLOR = {
     Status.SUCCESS.name: ECHARTS_COLORS['light_grey'],
     Status.FAILURE.name: ECHARTS_COLORS['light_grey'],
     Status.RUNNING.name: ECHARTS_COLORS['light_grey'],
     Status.INVALID.name: ECHARTS_COLORS['light_grey'],
 }
 
+STATUS_TO_PYDOT_LINE_STYLE_COLOR = {
+    Status.SUCCESS.name: PYDOT_COLORS['light_grey'],
+    Status.FAILURE.name: PYDOT_COLORS['light_grey'],
+    Status.RUNNING.name: PYDOT_COLORS['light_grey'],
+    Status.INVALID.name: PYDOT_COLORS['light_grey'],
+}
+
 
 class ECHARTS_SYMBOLS:
     CIRCLE = 'circle'
     RECT = 'rect'
     ROUNDRECT = 'roundRect'
     TRIANGLE = 'triangle'
     DIAMOND = 'diamond'
     PIN = 'pin'
     ARROW = 'arrow'
     NONE = 'none'
 
 
+class PYDOTS_SHAPES:
+    """
+  https://www.graphviz.org/doc/info/shapes.html
+  """
+    CIRCLE = 'circle'
+    BOX = 'box'
+    ELLIPSE = 'ellipse'
+    DIAMOND = 'diamond'
+    TRIANGLE = 'triangle'
+    PLAINTEXT = 'plaintext'
+    EGG = 'egg'
+    PLAIN = 'plain'
+    PARALLELOGRAM = 'parallelogram'
+    OCTAGON = 'octagon'
+
+
 class BT_NODE_TYPE:
     # 行为树节点的类型
     COMPOSITE = 'composite'
     DECORATOR = 'decorator'
     ACTION = 'action'
     CONDITION = 'condition'
 
@@ -71,14 +123,21 @@
 BT_NODE_TYPE_TO_ECHARTS_SYMBOLS = {
     BT_NODE_TYPE.COMPOSITE: ECHARTS_SYMBOLS.ROUNDRECT,
     BT_NODE_TYPE.DECORATOR: ECHARTS_SYMBOLS.CIRCLE,
     BT_NODE_TYPE.ACTION   : ECHARTS_SYMBOLS.RECT,
     BT_NODE_TYPE.CONDITION: ECHARTS_SYMBOLS.DIAMOND
 }
 
+BT_NODE_TYPE_TO_PYDOT_SHAPE = {
+    BT_NODE_TYPE.COMPOSITE: PYDOTS_SHAPES.PARALLELOGRAM,
+    BT_NODE_TYPE.DECORATOR: PYDOTS_SHAPES.ELLIPSE,
+    BT_NODE_TYPE.ACTION   : PYDOTS_SHAPES.BOX,
+    BT_NODE_TYPE.CONDITION: PYDOTS_SHAPES.BOX
+}
+
 BT_NODE_TYPE_TO_ECHARTS_SYMBOL_SIZE = {
     BT_NODE_TYPE.COMPOSITE: 24,
     BT_NODE_TYPE.DECORATOR: 15,
     BT_NODE_TYPE.ACTION   : 24,
     BT_NODE_TYPE.CONDITION: 24
 }
```

### Comparing `pybts-1.7.1/pybts/converter.py` & `pybts-1.8.0/pybts/converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import typing
 import jinja2
 import json
 from py_trees.common import Status
 from typing import Union
+import math
+import random
 
 _STATUS_MAP = {
     'SUCCESS': Status.SUCCESS,
     'FAILURE': Status.FAILURE,
     'RUNNING': Status.RUNNING,
     'INVALID': Status.INVALID
 }
@@ -37,79 +39,91 @@
 
     def bool(self, value: typing.Any):
         if isinstance(value, str):
             if value.lower() == 'true':
                 return True
             elif value.lower() == 'false':
                 return False
-            return bool(eval(self.render(value)))
+            return bool(self.eval(self.render(value)))
         return bool(value)
 
     def float(self, value: typing.Any):
         if isinstance(value, str):
-            return eval(self.render(value))
+            return float(self.eval(self.render(value)))
         else:
             return float(value)
 
     def int(self, value: typing.Any):
         if isinstance(value, str):
-            return int(eval(self.render(value)))
+            return int(self.eval(self.render(value)))
         else:
             return int(value)
 
-    def eval(self, value: str, context: dict = None):
-        ctx = { }
-        if self.node.context is not None:
-            ctx.update(self.node.context)
-        if self.node.attrs is not None:
-            ctx.update(self.node.attrs)
-        if context is not None:
-            ctx.update(context)
-        for key in ctx:
-            if callable(ctx[key]):
-                ctx[key] = ctx[key]()
-        return eval(value, ctx)
+    def eval(self, value: str):
+        return eval(value, self.node.context,
+                    { 'math': math, 'random': random, 'name': self.node.name })
 
     @classmethod
     def status(cls, value: Union[str, Status]) -> Status:
         if isinstance(value, Status):
             return value
         value = value.upper()
         if value not in _STATUS_MAP:
             raise Exception(f'{value} is not a valid status')
         return _STATUS_MAP[value]
 
     @classmethod
-    def status_list(cls, value: Union[str, Status, list[Status]]) -> list[Status]:
+    def status_list(cls, value: Union[str, Status, list[Status]], sep: str = ',') -> list[Status]:
         if isinstance(value, Status):
             return [value]
         elif isinstance(value, list):
             return [cls.status(value=item) for item in value]
         elif isinstance(value, str):
-            value_list = value.split(',')
+            value_list = value.split(sep)
             return [cls.status(value=item) for item in value_list if item != '']
 
-    def render(self, value: str, context: dict = None) -> str:
+    def int_list(self, value: Union[str, list[int], int], sep: str = ',') -> list[int]:
+        if isinstance(value, int):
+            return [value]
+        elif isinstance(value, list):
+            return [self.int(value=item) for item in value]
+        elif isinstance(value, str):
+            value_list = value.split(sep)
+            return [self.int(value=item) for item in value_list if item != '']
+
+    def float_list(self, value: Union[str, list[float], float], sep: str = ',') -> list[float]:
+        if isinstance(value, float):
+            return [value]
+        elif isinstance(value, list):
+            return [self.float(value=item) for item in value]
+        elif isinstance(value, str):
+            value_list = value.split(sep)
+            return [self.float(value=item) for item in value_list if item != '']
+
+    def str_list(self, value: Union[str, list[str], float], sep: str = ',') -> list[str]:
+        if isinstance(value, str):
+            return [value]
+        elif isinstance(value, list):
+            return [self.render(value=item) for item in value]
+        elif isinstance(value, str):
+            value_list = value.split(sep)
+            return [self.render(value=item) for item in value_list if item != '']
+
+    def str(self, value: str):
+        return self.render(value)
+
+    def render(self, value: str) -> str:
         if '{{' not in value or '}}' not in value:
             return value
 
-        ctx = { }
-        # if self.node.attrs is not None:
-        #     ctx.update(self.node.attrs)
-        if self.node.context is not None:
-            ctx.update(self.node.context)
-        if context is not None:
-            ctx.update(context)
-        for key in ctx:
-            if callable(ctx[key]):
-                ctx[key] = ctx[key]()
-
         for i in range(3):
             # 最多嵌套3层
-            rendered_value = jinja2.Template(value).render(ctx)
+            rendered_value = jinja2.Template(value).render(
+                    self.node.context, math=math, random=random,
+                    name=self.node.name)
             if '{{' not in rendered_value or '}}' not in rendered_value:
                 return rendered_value
             if rendered_value == value:
                 return rendered_value
             value = rendered_value
         return value
 
@@ -123,19 +137,25 @@
         else:
             try:
                 import numpy
                 if isinstance(value, numpy.ndarray):
                     return value.tolist()
             except ImportError:
                 pass
+            try:
+                import torch
+                if isinstance(value, torch.Tensor):
+                    return value.cpu().tolist()
+            except ImportError:
+                pass
             raise Exception(f'array error {value}')
 
     def dict(self, value: typing.Any) -> typing.Dict[str, typing.Any]:
         if isinstance(value, str):
-            return eval(self.render(value))
+            return self.eval(self.render(value))
         elif isinstance(value, dict):
             return value
         else:
             raise Exception(f'dict error {value}')
 
     def json_loads(self, value: typing.Any):
         if isinstance(value, str):
```

### Comparing `pybts-1.7.1/pybts/decorators/nodes.py` & `pybts-1.8.0/pybts/decorators/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,22 @@
 
     * With policy :data:`~py_trees.common.OneShotPolicy.ON_SUCCESSFUL_COMPLETION`, the oneshot will activate
       only when the underlying child returns :data:`~py_trees.Status.SUCCESS` (i.e. it permits retries).
     * With policy :data:`~py_trees.common.OneShotPolicy.ON_COMPLETION`, the oneshot will activate when the child
       returns :data:`~py_trees.Status.SUCCESS` || :data:`~py_trees.Status.FAILURE`.
 
     .. seealso:: :meth:`py_trees.idioms.oneshot`
+
+    <OneShot>
+        <Sequence>
+            <IsDoorOpen/>
+            <Reward />
+        </Sequence>
+    </OneShot>
+
     """
 
     def __init__(
             self, policy: str | list[Status] = 'SUCCESS', **kwargs
     ):
         """
         Init with the decorated child.
@@ -229,20 +237,18 @@
         Tick the child or bounce back with the original status if already completed.
 
         Yields:
             a reference to itself or a behaviour in it's child subtree
         """
         if self.final_status:
             # ignore the child
-            for node in Node.tick(self):
-                yield node
+            yield from Node.tick(self)
         else:
             # tick the child
-            for node in Decorator.tick(self):
-                yield node
+            yield from Decorator.tick(self)
 
     def terminate(self, new_status: Status) -> None:
         """
         Prevent further entry if finishing with :data:`~py_trees.Status.SUCCESS`.
 
         This uses a flag to register that the behaviour has gone through to completion.
         In future ticks, it will block entry to the child and just return the original
@@ -556,14 +562,17 @@
         return self.decorated.status
 
 
 class Throttle(Decorator):
     """
     节流: 在一定时间间隔内只执行一次
     每隔一段时间才会触发一次子节点，其他时间直接返回之前的状态
+    <Throttle duration="10" time="step">
+        <Reward domain="punish" reward="-0.001"/>
+    </Throttle>
     """
 
     def __init__(self, duration: float | str = 5.0, time: str | float = 'time', **kwargs):
         """
         Init with the decorated child and a timeout duration.
 
         Args:
@@ -602,14 +611,23 @@
     """
     子节点的状态变化后才会认为是成功
 
     如果指定了from_status和to_status，则只有子节点的状态由from_status转变到to_status，才会认为是触发了状态变化
     from_status和to_status均可以由多个状态组成，用逗号分隔
 
     immediate: 一开始是否会触发一次IsChanged
+
+
+    <IsStatusChanged from_status="FAILURE" to_status="SUCCESS">
+        <Sequence>
+            <IsDoorOpen/>
+            <Reward />
+        </Sequence>
+    </IsStatusChanged>
+
     """
 
     def __init__(self, from_status: str | Status = '', to_status: str | Status = '', immediate: bool | str = False,
                  **kwargs):
         super().__init__(**kwargs)
 
         self.from_status: list[Status] = self.converter.status_list(from_status)
```

### Comparing `pybts-1.7.1/pybts/main.py` & `pybts-1.8.0/pybts/main.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/pybts/nodes.py` & `pybts-1.8.0/pybts/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 
 class Node(py_trees.behaviour.Behaviour, ABC):
     """
     Base class for all nodes in the behavior tree
 
     被唤起的生命周期：
+    - setup 只会执行一次
+
     如果被tick到了
 
     状态为RUNNING
 
     - initialise
     - update
 
@@ -28,50 +30,56 @@
     - stop
 
     下一次tick的时候状态一开始是RUNNING，则直接调用
     update
     """
 
     def __init__(self, name: str = '', children: typing.List[py_trees.behaviour.Behaviour] = None, **kwargs):
+        self.attrs: typing.Dict[str, typing.AnyStr] = kwargs or { }  # 在builder和xml中传递的参数，会在__init__之后提供一个更完整的
+        self.context: typing.Optional[dict] = None  # 共享的字典，在tree.setup的时候提供，所以不要在__init__的时候修改或使用它，而是在setup的时候使用
         super().__init__(name=name or self.__class__.__name__)
         self._updater_iter = None
         self.debug_info = {
             'tick_count'      : 0,
             'update_count'    : 0,
             'reset_count'     : 0,
             'terminate_count' : 0,
             'initialise_count': 0
         }
-        self.attrs: typing.Dict[str, typing.AnyStr] = kwargs  # 在builder和xml中传递的参数，会在__init__之后提供一个更完整的
-        self.context: typing.Optional[dict] = None  # 共享的字典，在tree.setup的时候提供
         if children is not None:
             self.children = children
             for child in children:
                 child.parent = self
 
     def setup(self, **kwargs: typing.Any) -> None:
         super().setup(**kwargs)
         self.name = self.converter.render(self.name)
-    
+
     def reset(self):
         self.debug_info['reset_count'] += 1
         self._updater_iter = None
         if self.status != Status.INVALID:
             self.stop(Status.INVALID)
 
     @property
+    def label(self):
+        if 'label' in self.attrs:
+            return self.converter.render(self.attrs['label'])
+        return self.name
+
+    @property
     def converter(self):
         from pybts.converter import Converter
         return Converter(self)
 
     def to_data(self):
         # 在board上查看的信息
         return {
             'debug_info': self.debug_info,
-            'attrs'     : self.attrs
+            'attrs'     : self.attrs,
         }
 
     def update(self) -> Status:
         self.logger.debug("%s.update()" % (self.__class__.__name__))
         self.debug_info['update_count'] += 1
         if self._updater_iter is None:
             self._updater_iter = self.updater()
@@ -271,16 +279,21 @@
 
     参数：
     value: 监听的值
     immediate: 是否一开始就认为发生了变化
     rule: 判断规则，默认的规则是 curr_value != last_value，可以自定义新的规则，例如 abs(curr_value - last_value) >= 10，需要确保rule返回的值是bool类型
         - rule里面也可以使用模版语法，比如 abs(curr_value - last_value) >= {{min_value}}，模版语法里的min_value需要提前在context里定义好，不然会报错
     用法示例：
-    <IsChanged value="{{agent.x}}" immediate="true">
+
     <IsChanged value="{{agent.y}}" immediate="false" rule="abs(curr_value - last_value) >= 10">
+
+    <Sequence>
+        <IsChanged value="{{agent.hit_enemy_count}}" immediate="false">
+        <Reward reward="1" domain="attack"/>
+    </Sequence>
     """
 
     def __init__(self, value: typing.Any, immediate: bool | str = False, rule: str = '', **kwargs):
         super().__init__(**kwargs)
         self.value = value  # 监听的值
         self.immediate = immediate
         self.last_value = None  # 上一次的值
```

### Comparing `pybts-1.7.1/pybts/rl/base_class.py` & `pybts-1.8.0/pybts/rl/base_class.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/pybts/rl/nodes.py` & `pybts-1.8.0/pybts/rl/nodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pybts.rl.on_policy import *
 from stable_baselines3.common.base_class import BaseAlgorithm
 from stable_baselines3.common.policies import ActorCriticPolicy
 from abc import ABC, abstractmethod
 from typing import Union, Type
 import gymnasium as gym
 from pybts.rl.common import DummyEnv
+from stable_baselines3.common.logger import Logger
 
 
 class Reward(Node):
     """
     奖励节点，返回的状态一直是SUCCESS
     当走到这个节点时，会将给定的奖励累计
 
@@ -144,28 +145,23 @@
 
     def reset(self):
         self.rl_accum_reward = 0
 
     def to_data(self):
         return {
             'rl_iteration'   : self.rl_iteration,
-            'rl_policy'      : str(self.rl_policy()),
             'rl_info'        : self.rl_info,
             'rl_reward'      : self.rl_reward,
             'rl_obs'         : self.rl_obs,
             'rl_accum_reward': self.rl_accum_reward,
             'rl_action'      : self.rl_action,
             'rl_reward_scope': self.rl_reward_scope(),
         }
 
     @abstractmethod
-    def rl_env(self) -> gym.Env:
-        raise NotImplemented
-
-    @abstractmethod
     def rl_action_space(self) -> gym.spaces.Space:
         raise NotImplemented
 
     @abstractmethod
     def rl_observation_space(self) -> gym.spaces.Space:
         raise NotImplemented
 
@@ -189,33 +185,27 @@
 
     @abstractmethod
     def rl_gen_reward(self) -> float:
         reward_scope = self.rl_reward_scope()
         if reward_scope != '':
             assert isinstance(self, Node), 'RLOnPolicyNode 必须得继承Node节点'
             assert self.context is not None, 'context必须得设置好'
-            assert 'reward' in self.context, 'context必须得含有rl_reward键'
+            assert 'reward' in self.context, 'context必须得含有rl_reward键，请使用pybts.rl.RLTree'
             scopes = reward_scope.split(',')
             curr_reward = 0
             for scope in scopes:
                 curr_reward += self.context['reward'].get(scope, 0)
             return curr_reward - self.rl_accum_reward
         raise NotImplemented
 
     @abstractmethod
     def rl_gen_done(self) -> bool:
         # 返回当前环境是否结束
         raise NotImplemented
 
-    def rl_device(self) -> str:
-        return 'cpu'
-
-    def rl_policy(self) -> Union[str, typing.Type[ActorCriticPolicy]]:
-        return 'MlpPolicy'
-
     def rl_take_action(
             self,
             train: bool,
             log_interval: int = 1,
             deterministic: bool = False,
     ):
         if isinstance(self.rl_model, OnPolicyAlgorithm):
@@ -351,73 +341,79 @@
         self.rl_action = action
         self.rl_done = done
         return action
 
     def rl_setup_model(
             self,
             model_class: Union[Type[BaseAlgorithm]],
-            train: bool,
             path: str,
-            tensorboard_log: str = '',
+            policy: Union[str, typing.Type[ActorCriticPolicy]],
+            train: bool = True,
+            logger: Logger | None = None,
+            tensorboard_log: str | None = None,
+            tb_log_name: str | None = None,
             verbose: int = 1,
-            tb_log_name: str = '',
+            device: str = 'auto',
             **kwargs
     ):
         env = DummyEnv(
-                env=self.rl_env(),
+                obs=self.rl_gen_obs(),
+                info=self.rl_gen_info(),
                 action_space=self.rl_action_space(),
                 observation_space=self.rl_observation_space())
         model: typing.Optional[BaseAlgorithm] = None
 
         if train:
             model = model_class(
-                    policy=self.rl_policy(),
+                    policy=policy,
                     env=env,
                     verbose=verbose,
+                    device=device,
                     tensorboard_log=tensorboard_log,
-                    device=self.rl_device(),
                     **kwargs
             )
 
             if path != '':
                 try:
                     model.set_parameters(
                             load_path_or_dict=path,
-                            device=self.rl_device()
+                            device=device
                     )
                 except Exception as e:
                     pass
         else:
             assert path != '', f'No model path provided: {path}'
             model = model_class.load(
                     path=path,
                     env=env,
-                    tensorboard_log=tensorboard_log,
                     verbose=verbose,
                     force_reset=False,
-                    device=self.rl_device(),
+                    device=device,
                     **kwargs
             )
+        if logger is not None:
+            model.set_logger(logger=logger)
 
         if train:
             if isinstance(model, OffPolicyAlgorithm):
                 bt_off_policy_setup_learn(
                         model,
                         tb_log_name=tb_log_name,
                 )
             elif isinstance(model, OnPolicyAlgorithm):
                 bt_on_policy_setup_learn(
                         model,
-                        tb_log_name=tb_log_name,
-                        obs=self.rl_gen_obs()
+                        obs=self.rl_gen_obs(),
+                        tb_log_name=tb_log_name
                 )
             else:
                 raise Exception('Unrecognized model type')
 
         self.rl_model = model
+
         return model
 
 
 if __name__ == '__main__':
     node = ConditionReward(scope='a,b,c', success='{{1}}/10', children=[Success()])
     node.setup()
     print(node.success)
```

### Comparing `pybts-1.7.1/pybts/rl/off_policy.py` & `pybts-1.8.0/pybts/rl/off_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from stable_baselines3.common.off_policy_algorithm import OffPolicyAlgorithm
+
 from stable_baselines3.common.utils import (
     configure_logger, TrainFreq
 )
 import typing
 from collections import deque
 import time
 import warnings
@@ -19,15 +20,14 @@
 def bt_off_policy_setup_learn(
         self: OffPolicyAlgorithm,
         tb_log_name: str = 'run',
         reset_num_timesteps: bool = True,
         total_timesteps: int = 10000,
 ):
     replay_buffer = self.replay_buffer
-
     truncate_last_traj = (
             self.optimize_memory_usage
             and reset_num_timesteps
             and replay_buffer is not None
             and (replay_buffer.full or replay_buffer.pos > 0)
     )
     if truncate_last_traj:
@@ -92,14 +92,15 @@
     env_num_envs = 1
     assert train_freq.frequency > 0, "Should at least collect one step or episode."
 
     if self.use_sde:
         self.actor.reset_noise(env_num_envs)
 
     continue_training = True
+
     while should_collect_more_steps(train_freq, num_collected_steps, num_collected_episodes):
         if self.use_sde and self.sde_sample_freq > 0 and num_collected_steps % self.sde_sample_freq == 0:
             # Sample a new noise matrix
             self.actor.reset_noise(env_num_envs)
 
         # Select action randomly or according to policy
         actions, buffer_actions = self._sample_action(learning_starts, action_noise, env_num_envs)
@@ -138,8 +139,10 @@
                 if action_noise is not None:
                     action_noise.reset()
 
                 # Log training infos
                 if log_interval is not None and self._episode_num % log_interval == 0:
                     self._dump_logs()
 
-    yield RolloutReturn(num_collected_steps * env_num_envs, num_collected_episodes, continue_training)
+    rollout_return = RolloutReturn(num_collected_steps * env_num_envs, num_collected_episodes, continue_training)
+    print('bt_off_policy_collect_rollouts', rollout_return)
+    yield rollout_return
```

### Comparing `pybts-1.7.1/pybts/rl/on_policy.py` & `pybts-1.8.0/pybts/rl/on_policy.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/pybts/rl/tree.py` & `pybts-1.8.0/pybts/rl/tree.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/pybts/templates/favicon.ico` & `pybts-1.8.0/pybts/templates/favicon.ico`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/pybts/templates/static/index-BlldS3Jx.js` & `pybts-1.8.0/pybts/templates/static/index-BlldS3Jx.js`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/pybts/templates/static/index-DN1S--qx.css` & `pybts-1.8.0/pybts/templates/static/index-DN1S--qx.css`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/pybts/templates/static/info-lb9hZOuB.png` & `pybts-1.8.0/pybts/templates/static/info-lb9hZOuB.png`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/pybts/tree.py` & `pybts-1.8.0/pybts/tree.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.1/pybts/utility.py` & `pybts-1.8.0/pybts/utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import py_trees.blackboard
 
-from pybts.nodes import *
 from pybts.constants import *
 import yaml
 from queue import Queue
 import xml.etree.ElementTree as ET
 from xml.dom import minidom
 import os
 import json
@@ -26,28 +25,32 @@
     for item in temp_list:
         q.put_nowait(item)
 
     return temp_list
 
 
 def bt_to_node_type(node: py_trees.behaviour.Behaviour) -> str:
-    if isinstance(node, py_trees.composites.Composite):
+    from pybts.nodes import Condition
+    from pybts.composites import Composite
+    from pybts.decorators import Decorator
+    if isinstance(node, py_trees.composites.Composite) or isinstance(node, Composite):
         return BT_NODE_TYPE.COMPOSITE
-    elif isinstance(node, py_trees.decorators.Decorator):
+    elif isinstance(node, py_trees.decorators.Decorator) or isinstance(node, Decorator):
         return BT_NODE_TYPE.DECORATOR
     elif isinstance(node, Condition):
         return BT_NODE_TYPE.CONDITION
     else:
         return BT_NODE_TYPE.ACTION
 
 
 def bt_to_json(node: py_trees.behaviour.Behaviour,
                ignore_children: bool = False,
                ignore_attrs: list = None,
                ignore_to_data: bool = False) -> dict:
+    from pybts.nodes import Node
     try:
         info = {
             'tag'     : node.__class__.__name__,
             'children': [],
             'data'    : {
                 BT_PRESET_DATA_KEY.ID               : node.id.hex,
                 BT_PRESET_DATA_KEY.STATUS           : node.status.name,
@@ -207,38 +210,41 @@
             return list(obj)  # Convert tuple to list
         elif isinstance(obj, uuid.UUID):
             return obj.hex  # Convert UUID to string
         elif isinstance(obj, set):
             return list(set)
         elif isinstance(obj, Status):
             return obj.value
-        elif callable(obj):
-            return obj()
-        else:
-            try:
-                import numpy as np
-                if isinstance(obj, np.integer):
-                    return int(obj)
-                elif isinstance(obj, np.floating):
-                    return float(obj)
-                elif isinstance(obj, np.ndarray):
-                    return obj.tolist()
-                elif isinstance(obj, np.bool_):
-                    return bool(obj)
-                elif isinstance(obj, np.str_):
-                    return str(obj)
-                elif isinstance(obj, enum.Enum):
-                    return obj.value
-                elif isinstance(obj, tuple):
-                    return list(obj)  # Convert tuple to list
-                elif isinstance(obj, np.unicode_):
-                    return str(obj)
-            except:
-                pass
-            return str(obj)
+
+        # if callable(obj):
+        #     try:
+        #         return obj()
+        #     except:
+        #         pass
+        try:
+            import numpy as np
+            if isinstance(obj, np.integer):
+                return int(obj)
+            elif isinstance(obj, np.floating):
+                return float(obj)
+            elif isinstance(obj, np.ndarray):
+                return obj.tolist()
+            elif isinstance(obj, np.bool_):
+                return bool(obj)
+            elif isinstance(obj, np.str_):
+                return str(obj)
+            elif isinstance(obj, enum.Enum):
+                return obj.value
+            elif isinstance(obj, tuple):
+                return list(obj)  # Convert tuple to list
+            elif isinstance(obj, np.unicode_):
+                return str(obj)
+        except:
+            pass
+        return str(obj)
 
 
 def json_dumps(json_data, indent=4, sort_keys=False, ensure_ascii=True, **kwargs):
     return json.dumps(json_data, cls=PYBTJsonEncoder, indent=indent, sort_keys=sort_keys, ensure_ascii=ensure_ascii,
                       **kwargs)
```

### Comparing `pybts-1.7.1/pyproject.toml` & `pybts-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybts"
-version = "1.7.1"
+version = "1.8.0"
 description = ""
 authors = ["王童 <785271992@qq.com>"]
 readme = "README.md"
 homepage = "https://github.com/wangtong2015/pybts"
 repository = "https://github.com/wangtong2015/pybts"
 keywords = ["BehaviorTree", "AI"]
 include = ["README.md", "pybts/templates/static/*", 'pybts/templates/*', 'README.assets']
```

### Comparing `pybts-1.7.1/PKG-INFO` & `pybts-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybts
-Version: 1.7.1
+Version: 1.8.0
 Summary: 
 Home-page: https://github.com/wangtong2015/pybts
 Keywords: BehaviorTree,AI
 Author: 王童
 Author-email: 785271992@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

