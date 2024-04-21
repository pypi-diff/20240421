# Comparing `tmp/pybts-1.8.0.tar.gz` & `tmp/pybts-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybts-1.8.0.tar", max compression
+gzip compressed data, was "pybts-1.8.2.tar", max compression
```

## Comparing `pybts-1.8.0.tar` & `pybts-1.8.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0   157658 2024-04-21 09:33:56.611530 pybts-1.8.0/README.assets/DEMO_Sequence  10-10 _ 100.png
--rw-r--r--   0        0        0   189323 2024-04-21 09:33:56.611530 pybts-1.8.0/README.assets/image-20240329031220580.png
--rw-r--r--   0        0        0   208202 2024-04-21 09:33:56.611530 pybts-1.8.0/README.assets/image-20240329031233459.png
--rw-r--r--   0        0        0   255608 2024-04-21 09:33:56.611530 pybts-1.8.0/README.assets/image-20240401211552611.png
--rw-r--r--   0        0        0   202283 2024-04-21 09:33:56.615531 pybts-1.8.0/README.assets/image-20240401211609525.png
--rw-r--r--   0        0        0     5960 2024-04-21 09:33:56.615531 pybts-1.8.0/README.md
--rw-r--r--   0        0        0      385 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/__init__.py
--rw-r--r--   0        0        0       52 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/board/__init__.py
--rw-r--r--   0        0        0     2740 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/board/board.py
--rw-r--r--   0        0        0    11048 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/board/server.py
--rw-r--r--   0        0        0     8225 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/builder.py
--rw-r--r--   0        0        0      608 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/__init__.py
--rw-r--r--   0        0        0    10363 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/composite.py
--rw-r--r--   0        0        0     3360 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/condition_branch.py
--rw-r--r--   0        0        0     5460 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/parallel.py
--rw-r--r--   0        0        0      945 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/ppa.py
--rw-r--r--   0        0        0     3221 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/selector.py
--rw-r--r--   0        0        0     3354 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/sequence.py
--rw-r--r--   0        0        0     1716 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/switcher.py
--rw-r--r--   0        0        0      182 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/composites/template.py
--rw-r--r--   0        0        0     4998 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/constants.py
--rw-r--r--   0        0        0     5981 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/converter.py
--rw-r--r--   0        0        0      121 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/decorators/__init__.py
--rw-r--r--   0        0        0    23244 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/decorators/nodes.py
--rw-r--r--   0        0        0     3269 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/display.py
--rw-r--r--   0        0        0     1521 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/main.py
--rw-r--r--   0        0        0    18037 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/nodes.py
--rw-r--r--   0        0        0      107 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/__init__.py
--rw-r--r--   0        0        0     8803 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/base_class.py
--rw-r--r--   0        0        0      268 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/builder.py
--rw-r--r--   0        0        0     1742 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/common.py
--rw-r--r--   0        0        0     2703 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/logger.py
--rw-r--r--   0        0        0    15148 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/nodes.py
--rw-r--r--   0        0        0     5784 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/off_policy.py
--rw-r--r--   0        0        0     8587 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/on_policy.py
--rw-r--r--   0        0        0     1218 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/rl/tree.py
--rw-r--r--   0        0        0    16958 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/templates/favicon.ico
--rw-r--r--   0        0        0      433 2024-04-21 09:33:56.619531 pybts-1.8.0/pybts/templates/index.html
--rw-r--r--   0        0        0  1967920 2024-04-21 09:33:56.631531 pybts-1.8.0/pybts/templates/static/index-BlldS3Jx.js
--rw-r--r--   0        0        0   320362 2024-04-21 09:33:56.631531 pybts-1.8.0/pybts/templates/static/index-DN1S--qx.css
--rw-r--r--   0        0        0     5267 2024-04-21 09:33:56.631531 pybts-1.8.0/pybts/templates/static/info-lb9hZOuB.png
--rw-r--r--   0        0        0     2140 2024-04-21 09:33:56.631531 pybts-1.8.0/pybts/tree.py
--rw-r--r--   0        0        0    10211 2024-04-21 09:33:56.631531 pybts-1.8.0/pybts/utility.py
--rw-r--r--   0        0        0      844 2024-04-21 09:33:56.631531 pybts-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 pybts-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0   157658 2024-04-21 18:57:49.399516 pybts-1.8.2/README.assets/DEMO_Sequence  10-10 _ 100.png
+-rw-r--r--   0        0        0   189323 2024-04-21 18:57:49.399516 pybts-1.8.2/README.assets/image-20240329031220580.png
+-rw-r--r--   0        0        0   208202 2024-04-21 18:57:49.399516 pybts-1.8.2/README.assets/image-20240329031233459.png
+-rw-r--r--   0        0        0   255608 2024-04-21 18:57:49.403516 pybts-1.8.2/README.assets/image-20240401211552611.png
+-rw-r--r--   0        0        0   202283 2024-04-21 18:57:49.403516 pybts-1.8.2/README.assets/image-20240401211609525.png
+-rw-r--r--   0        0        0     5960 2024-04-21 18:57:49.403516 pybts-1.8.2/README.md
+-rw-r--r--   0        0        0      385 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/board/__init__.py
+-rw-r--r--   0        0        0     2740 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/board/board.py
+-rw-r--r--   0        0        0    11048 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/board/server.py
+-rw-r--r--   0        0        0     8225 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/builder.py
+-rw-r--r--   0        0        0      608 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/composites/__init__.py
+-rw-r--r--   0        0        0    10432 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/composites/composite.py
+-rw-r--r--   0        0        0     3360 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/composites/condition_branch.py
+-rw-r--r--   0        0        0     5459 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/composites/parallel.py
+-rw-r--r--   0        0        0      945 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/composites/ppa.py
+-rw-r--r--   0        0        0     2855 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/composites/selector.py
+-rw-r--r--   0        0        0     3009 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/composites/sequence.py
+-rw-r--r--   0        0        0     1677 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/composites/switcher.py
+-rw-r--r--   0        0        0      182 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/composites/template.py
+-rw-r--r--   0        0        0     4998 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/constants.py
+-rw-r--r--   0        0        0     5910 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/converter.py
+-rw-r--r--   0        0        0      121 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/decorators/__init__.py
+-rw-r--r--   0        0        0    23244 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/decorators/nodes.py
+-rw-r--r--   0        0        0     3269 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/display.py
+-rw-r--r--   0        0        0     1521 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/main.py
+-rw-r--r--   0        0        0    18586 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/nodes.py
+-rw-r--r--   0        0        0      107 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/rl/__init__.py
+-rw-r--r--   0        0        0     8803 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/rl/base_class.py
+-rw-r--r--   0        0        0      268 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/rl/builder.py
+-rw-r--r--   0        0        0     1742 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/rl/common.py
+-rw-r--r--   0        0        0     2703 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/rl/logger.py
+-rw-r--r--   0        0        0    15148 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/rl/nodes.py
+-rw-r--r--   0        0        0     5784 2024-04-21 18:57:49.407516 pybts-1.8.2/pybts/rl/off_policy.py
+-rw-r--r--   0        0        0     8587 2024-04-21 18:57:49.411516 pybts-1.8.2/pybts/rl/on_policy.py
+-rw-r--r--   0        0        0     1218 2024-04-21 18:57:49.411516 pybts-1.8.2/pybts/rl/tree.py
+-rw-r--r--   0        0        0    16958 2024-04-21 18:57:49.411516 pybts-1.8.2/pybts/templates/favicon.ico
+-rw-r--r--   0        0        0      433 2024-04-21 18:57:49.411516 pybts-1.8.2/pybts/templates/index.html
+-rw-r--r--   0        0        0  1967920 2024-04-21 18:57:49.419516 pybts-1.8.2/pybts/templates/static/index-BlldS3Jx.js
+-rw-r--r--   0        0        0   320362 2024-04-21 18:57:49.419516 pybts-1.8.2/pybts/templates/static/index-DN1S--qx.css
+-rw-r--r--   0        0        0     5267 2024-04-21 18:57:49.423516 pybts-1.8.2/pybts/templates/static/info-lb9hZOuB.png
+-rw-r--r--   0        0        0     2140 2024-04-21 18:57:49.423516 pybts-1.8.2/pybts/tree.py
+-rw-r--r--   0        0        0    10211 2024-04-21 18:57:49.423516 pybts-1.8.2/pybts/utility.py
+-rw-r--r--   0        0        0      844 2024-04-21 18:57:49.423516 pybts-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 pybts-1.8.2/PKG-INFO
```

### Comparing `pybts-1.8.0/README.assets/DEMO_Sequence  10-10 _ 100.png` & `pybts-1.8.2/README.assets/DEMO_Sequence  10-10 _ 100.png`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/README.assets/image-20240329031220580.png` & `pybts-1.8.2/README.assets/image-20240329031220580.png`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/README.assets/image-20240329031233459.png` & `pybts-1.8.2/README.assets/image-20240329031233459.png`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/README.assets/image-20240401211552611.png` & `pybts-1.8.2/README.assets/image-20240401211552611.png`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/README.assets/image-20240401211609525.png` & `pybts-1.8.2/README.assets/image-20240401211609525.png`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/README.md` & `pybts-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/board/board.py` & `pybts-1.8.2/pybts/board/board.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/board/server.py` & `pybts-1.8.2/pybts/board/server.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/builder.py` & `pybts-1.8.2/pybts/builder.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/composites/__init__.py` & `pybts-1.8.2/pybts/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/composites/composite.py` & `pybts-1.8.2/pybts/composites/composite.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,23 +228,25 @@
         self.logger.debug("%s.tick()" % (self.__class__.__name__))
 
         if self.status in tick_again_status:
             # 重新执行上次执行的子节点
             assert self.current_child is not None
             index = self.children.index(self.current_child)
         else:
+            # Restart
             self.current_child = None  # 从头执行
             if callable(start_index):
                 start_index = start_index(self)
             index = start_index
 
         for child in itertools.islice(self.children, index, None):
             self.current_child = child
             yield from child.tick()
             if child.status not in continue_status:
+                # 不在Next里，停止执行
                 break
 
         if self.current_child is not None:
             new_status = self.current_child.status
 
             index = self.children.index(self.current_child)
```

### Comparing `pybts-1.8.0/pybts/composites/condition_branch.py` & `pybts-1.8.2/pybts/composites/condition_branch.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/composites/parallel.py` & `pybts-1.8.2/pybts/composites/parallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 
     def to_data(self):
         return {
             **super().to_data(),
             'success_threshold': self.success_threshold
         }
 
-
 # class ReactiveParallel(Parallel):
 #     """
 #     反应式并行节点
 #     忽略RUNNING节点的并行节点
 #     """
 #
 #     def tick(self) -> typing.Iterator[py_trees.behaviour.Behaviour]:
```

### Comparing `pybts-1.8.0/pybts/composites/ppa.py` & `pybts-1.8.2/pybts/composites/ppa.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/composites/selector.py` & `pybts-1.8.2/pybts/composites/selector.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,33 +15,29 @@
     返回最后一个执行节点的状态，如果没有孩子，则返回FAILURE
     """
 
     def gen_index(self):
         # 想要过滤掉前面的节点的话，可以继承Selector然后重写这个函数
         return 0
 
-    def tick(self) -> typing.Iterator[behaviour.Behaviour]:
+    def tick_again_status(self: Composite):
+        """计算需要TickAgain的状态"""
         if self.reactive:
-            return self.seq_sel_tick(
-                    tick_again_status=[],
-                    continue_status=[Status.FAILURE, Status.INVALID],
-                    no_child_status=Status.FAILURE,
-                    start_index=lambda _: self.gen_index())
+            return []
         elif self.memory:
-            return self.seq_sel_tick(
-                    tick_again_status=[Status.SUCCESS, Status.RUNNING],
-                    continue_status=[Status.FAILURE, Status.INVALID],
-                    no_child_status=Status.FAILURE,
-                    start_index=lambda _: self.gen_index())
+            return [Status.RUNNING, Status.SUCCESS]
         else:
-            return self.seq_sel_tick(
-                    tick_again_status=[Status.RUNNING],
-                    continue_status=[Status.FAILURE, Status.INVALID],
-                    no_child_status=Status.FAILURE,
-                    start_index=lambda _: self.gen_index())
+            return [Status.RUNNING]
+
+    def tick(self) -> typing.Iterator[behaviour.Behaviour]:
+        return self.seq_sel_tick(
+                tick_again_status=self.tick_again_status(),
+                continue_status=[Status.FAILURE, Status.INVALID],
+                no_child_status=Status.FAILURE,
+                start_index=lambda _: self.gen_index())
 
 
 class SelectorWithMemory(Selector):
     """
     记忆选择节点
     - 当前执行节点返回 FAILURE/INVALID，继续执行后续节点
     - 当前执行节点返回 SUCCESS/RUNNING，停止执行后续节点，下次执行还是从这个节点开始
```

### Comparing `pybts-1.8.0/pybts/composites/sequence.py` & `pybts-1.8.2/pybts/composites/sequence.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,33 +13,29 @@
     - 当前执行节点返回 FAILURE/INVALID，停止执行后续节点，下次执行从第一个节点开始
     返回最后一个执行节点的状态，如果没有孩子，则返回SUCCESS
     """
 
     def gen_index(self):
         return 0
 
-    def tick(self: Composite) -> typing.Iterator[behaviour.Behaviour]:
+    def tick_again_status(self: Composite):
+        """计算需要TickAgain的状态"""
         if self.reactive:
-            return self.seq_sel_tick(
-                    tick_again_status=[],
-                    continue_status=[Status.SUCCESS],
-                    no_child_status=Status.SUCCESS,
-                    start_index=lambda _: self.gen_index())
+            return []
         elif self.memory:
-            return self.seq_sel_tick(
-                    tick_again_status=[Status.RUNNING, Status.FAILURE],
-                    continue_status=[Status.SUCCESS],
-                    no_child_status=Status.SUCCESS,
-                    start_index=lambda _: self.gen_index())
+            return [Status.RUNNING, Status.FAILURE]
         else:
-            return self.seq_sel_tick(
-                    tick_again_status=[Status.RUNNING],
-                    continue_status=[Status.SUCCESS],
-                    no_child_status=Status.SUCCESS,
-                    start_index=lambda _: self.gen_index())
+            return [Status.RUNNING]
+
+    def tick(self) -> typing.Iterator[behaviour.Behaviour]:
+        return self.seq_sel_tick(
+                tick_again_status=self.tick_again_status(),
+                continue_status=[Status.SUCCESS],
+                no_child_status=Status.SUCCESS,
+                start_index=lambda _: self.gen_index())
 
 
 class SequenceWithMemory(Sequence):
     """
     记忆顺序节点
     依次顺序执行子节点
     - 当前执行节点返回 SUCCESS，继续执行后续节点
```

### Comparing `pybts-1.8.0/pybts/composites/switcher.py` & `pybts-1.8.2/pybts/composites/switcher.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,33 +16,36 @@
     返回当前执行节点的状态
 
     index:
     - 具体的数字
     - jinja2模版: 从context中获取
     - random: 随机数
     """
-
+    
     def __init__(self, index: typing.Union[int, str] = 'random', **kwargs):
         super().__init__(**kwargs)
         self.index = index
 
     def gen_index(self) -> int:
         if self.index == 'random':
             return random.randint(0, len(self.children) - 1)
         else:
             return self.converter.int(self.index)
 
-    def tick(self) -> typing.Iterator[Behaviour]:
+    def tick_again_status(self: Composite):
+        """计算需要重新执行的状态"""
         if self.reactive:
-            return self.switch_tick(index=lambda _: self.gen_index(), tick_again_status=[])
+            return []
         elif self.memory:
-            return self.switch_tick(index=lambda _: self.gen_index(),
-                                    tick_again_status=[Status.RUNNING, Status.FAILURE])
+            return [Status.RUNNING, Status.FAILURE]
         else:
-            return self.switch_tick(index=lambda _: self.gen_index(), tick_again_status=[Status.RUNNING])
+            return [Status.RUNNING]
+
+    def tick(self) -> typing.Iterator[Behaviour]:
+        return self.switch_tick(index=lambda _: self.gen_index(), tick_again_status=self.tick_again_status())
 
 
 class ReactiveSwitcher(Switcher):
     """
     相应式选择其中一个子节点执行，每次都会重新选择index
     返回当前执行节点的状态
     """
```

### Comparing `pybts-1.8.0/pybts/constants.py` & `pybts-1.8.2/pybts/constants.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/converter.py` & `pybts-1.8.2/pybts/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,18 +95,16 @@
             return [value]
         elif isinstance(value, list):
             return [self.float(value=item) for item in value]
         elif isinstance(value, str):
             value_list = value.split(sep)
             return [self.float(value=item) for item in value_list if item != '']
 
-    def str_list(self, value: Union[str, list[str], float], sep: str = ',') -> list[str]:
-        if isinstance(value, str):
-            return [value]
-        elif isinstance(value, list):
+    def str_list(self, value: Union[str, list[str]], sep: str = ',') -> list[str]:
+        if isinstance(value, list):
             return [self.render(value=item) for item in value]
         elif isinstance(value, str):
             value_list = value.split(sep)
             return [self.render(value=item) for item in value_list if item != '']
 
     def str(self, value: str):
         return self.render(value)
```

### Comparing `pybts-1.8.0/pybts/decorators/nodes.py` & `pybts-1.8.2/pybts/decorators/nodes.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/display.py` & `pybts-1.8.2/pybts/display.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/main.py` & `pybts-1.8.2/pybts/main.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/nodes.py` & `pybts-1.8.2/pybts/nodes.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,29 +37,43 @@
         self.attrs: typing.Dict[str, typing.AnyStr] = kwargs or { }  # 在builder和xml中传递的参数，会在__init__之后提供一个更完整的
         self.context: typing.Optional[dict] = None  # 共享的字典，在tree.setup的时候提供，所以不要在__init__的时候修改或使用它，而是在setup的时候使用
         super().__init__(name=name or self.__class__.__name__)
         self._updater_iter = None
         self.debug_info = {
             'tick_count'      : 0,
             'update_count'    : 0,
-            'reset_count'     : 0,
             'terminate_count' : 0,
-            'initialise_count': 0
+            'initialise_count': 0,
+            'success_count'   : 0,
+            'failure_count'   : 0,
+            'invalid_count'   : 0,
+            'running_count'   : 0
         }
+        self.reset_count = 0
         if children is not None:
             self.children = children
             for child in children:
                 child.parent = self
 
     def setup(self, **kwargs: typing.Any) -> None:
         super().setup(**kwargs)
         self.name = self.converter.render(self.name)
 
     def reset(self):
-        self.debug_info['reset_count'] += 1
+        self.reset_count += 1
+        self.debug_info = {
+            'tick_count'      : 0,
+            'update_count'    : 0,
+            'terminate_count' : 0,
+            'initialise_count': 0,
+            'success_count'   : 0,
+            'failure_count'   : 0,
+            'invalid_count'   : 0,
+            'running_count'   : 0
+        }
         self._updater_iter = None
         if self.status != Status.INVALID:
             self.stop(Status.INVALID)
 
     @property
     def label(self):
         if 'label' in self.attrs:
@@ -70,16 +84,17 @@
     def converter(self):
         from pybts.converter import Converter
         return Converter(self)
 
     def to_data(self):
         # 在board上查看的信息
         return {
-            'debug_info': self.debug_info,
-            'attrs'     : self.attrs,
+            'debug_info' : self.debug_info,
+            'attrs'      : self.attrs,
+            'reset_count': self.reset_count
         }
 
     def update(self) -> Status:
         self.logger.debug("%s.update()" % (self.__class__.__name__))
         self.debug_info['update_count'] += 1
         if self._updater_iter is None:
             self._updater_iter = self.updater()
@@ -138,14 +153,15 @@
                     self.__class__.__name__,
                     "%s->%s" % (self.status, new_status)
                 )
         )
         self.terminate(new_status)
         self.status = new_status
         self.iterator = self.tick()
+        self.debug_info[new_status.value.lower() + '_count'] += 1
         if new_status == Status.INVALID:
             self._updater_iter = None  # 停止updater
 
     def terminate(self, new_status: common.Status) -> None:
         super().terminate(new_status)
         self.logger.debug(
                 "%s.terminate(%s)"
```

### Comparing `pybts-1.8.0/pybts/rl/base_class.py` & `pybts-1.8.2/pybts/rl/base_class.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/rl/common.py` & `pybts-1.8.2/pybts/rl/common.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/rl/logger.py` & `pybts-1.8.2/pybts/rl/logger.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/rl/nodes.py` & `pybts-1.8.2/pybts/rl/nodes.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/rl/off_policy.py` & `pybts-1.8.2/pybts/rl/off_policy.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/rl/on_policy.py` & `pybts-1.8.2/pybts/rl/on_policy.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/rl/tree.py` & `pybts-1.8.2/pybts/rl/tree.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/templates/favicon.ico` & `pybts-1.8.2/pybts/templates/favicon.ico`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/templates/static/index-BlldS3Jx.js` & `pybts-1.8.2/pybts/templates/static/index-BlldS3Jx.js`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/templates/static/index-DN1S--qx.css` & `pybts-1.8.2/pybts/templates/static/index-DN1S--qx.css`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/templates/static/info-lb9hZOuB.png` & `pybts-1.8.2/pybts/templates/static/info-lb9hZOuB.png`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/tree.py` & `pybts-1.8.2/pybts/tree.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pybts/utility.py` & `pybts-1.8.2/pybts/utility.py`

 * *Files identical despite different names*

### Comparing `pybts-1.8.0/pyproject.toml` & `pybts-1.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybts"
-version = "1.8.0"
+version = "1.8.2"
 description = ""
 authors = ["王童 <785271992@qq.com>"]
 readme = "README.md"
 homepage = "https://github.com/wangtong2015/pybts"
 repository = "https://github.com/wangtong2015/pybts"
 keywords = ["BehaviorTree", "AI"]
 include = ["README.md", "pybts/templates/static/*", 'pybts/templates/*', 'README.assets']
```

### Comparing `pybts-1.8.0/PKG-INFO` & `pybts-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybts
-Version: 1.8.0
+Version: 1.8.2
 Summary: 
 Home-page: https://github.com/wangtong2015/pybts
 Keywords: BehaviorTree,AI
 Author: 王童
 Author-email: 785271992@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

