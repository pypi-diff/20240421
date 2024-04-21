# Comparing `tmp/networke-3.0.tar.gz` & `tmp/networke-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networke-3.0.tar", last modified: Tue Apr 16 16:21:37 2024, max compression
+gzip compressed data, was "networke-4.0.tar", last modified: Sun Apr 21 16:05:19 2024, max compression
```

## Comparing `networke-3.0.tar` & `networke-4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 16:21:37.090091 networke-3.0/
--rw-rw-rw-   0        0        0        0 2024-04-09 15:52:45.000000 networke-3.0/LICENSE.txt
--rw-rw-rw-   0        0        0       80 2024-04-16 16:21:37.086096 networke-3.0/PKG-INFO
--rw-rw-rw-   0        0        0        3 2024-04-09 15:52:26.000000 networke-3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 16:21:37.033124 networke-3.0/network/
--rw-rw-rw-   0        0        0       28 2024-04-09 15:55:03.000000 networke-3.0/network/__init__.py
--rw-rw-rw-   0        0        0     1720 2024-04-11 15:30:17.000000 networke-3.0/network/bst.py
--rw-rw-rw-   0        0        0      197 2024-04-11 13:17:01.000000 networke-3.0/network/comp_sum.py
--rw-rw-rw-   0        0        0     6873 2024-03-10 04:18:36.000000 networke-3.0/network/doublelinky.py
--rw-rw-rw-   0        0        0      248 2024-04-11 13:23:15.000000 networke-3.0/network/hanoi.py
--rw-rw-rw-   0        0        0     3028 2024-04-11 16:21:42.000000 networke-3.0/network/krus.py
--rw-rw-rw-   0        0        0     4619 2024-02-23 14:09:39.000000 networke-3.0/network/linked_list.py
--rw-rw-rw-   0        0        0       82 2024-04-09 15:54:50.000000 networke-3.0/network/main.py
--rw-rw-rw-   0        0        0      971 2024-04-11 13:41:30.000000 networke-3.0/network/merge_sort.py
--rw-rw-rw-   0        0        0     5710 2024-04-11 16:32:14.000000 networke-3.0/network/poley.py
--rw-rw-rw-   0        0        0      236 2024-04-11 13:19:31.000000 networke-3.0/network/pow.py
--rw-rw-rw-   0        0        0      232 2024-04-09 09:55:10.000000 networke-3.0/network/progarm_factorial.py
--rw-rw-rw-   0        0        0      254 2024-04-07 07:46:58.000000 networke-3.0/network/program_5_fibonacci.py
--rw-rw-rw-   0        0        0     2919 2024-04-09 10:58:58.000000 networke-3.0/network/program_array.py
--rw-rw-rw-   0        0        0      222 2024-04-09 09:42:53.000000 networke-3.0/network/program_asc_Desc.py
--rw-rw-rw-   0        0        0     2173 2024-04-09 12:33:55.000000 networke-3.0/network/program_dfs.py
--rw-rw-rw-   0        0        0     3463 2024-04-09 13:52:44.000000 networke-3.0/network/program_heap.py
--rw-rw-rw-   0        0        0     2205 2024-04-09 13:23:53.000000 networke-3.0/network/program_prims.py
--rw-rw-rw-   0        0        0     1056 2024-04-09 11:30:12.000000 networke-3.0/network/program_quicksort.py
--rw-rw-rw-   0        0        0     2320 2024-04-16 16:04:47.000000 networke-3.0/network/program_stack_expr.py
--rw-rw-rw-   0        0        0     2805 2024-04-11 14:23:00.000000 networke-3.0/network/qu.py
--rw-rw-rw-   0        0        0      418 2024-04-11 13:29:15.000000 networke-3.0/network/seat.py
--rw-rw-rw-   0        0        0     1516 2024-04-11 13:55:51.000000 networke-3.0/network/stackey.py
-drwxrwxrwx   0        0        0        0 2024-04-16 16:21:37.080131 networke-3.0/networke.egg-info/
--rw-rw-rw-   0        0        0       80 2024-04-16 16:21:36.000000 networke-3.0/networke.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      655 2024-04-16 16:21:36.000000 networke-3.0/networke.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 16:21:36.000000 networke-3.0/networke.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-16 16:21:36.000000 networke-3.0/networke.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 16:21:37.091089 networke-3.0/setup.cfg
--rw-rw-rw-   0        0        0      197 2024-04-16 16:00:55.000000 networke-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 16:05:19.248837 networke-4.0/
+-rw-rw-rw-   0        0        0       13 2024-04-21 16:02:30.000000 networke-4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       80 2024-04-21 16:05:19.244845 networke-4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-04-21 16:02:18.000000 networke-4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 16:05:19.069955 networke-4.0/network/
+-rw-rw-rw-   0        0        0      224 2024-04-21 15:37:20.000000 networke-4.0/network/Ascending,descendign.py
+-rw-rw-rw-   0        0        0       28 2024-04-09 15:55:03.000000 networke-4.0/network/__init__.py
+-rw-rw-rw-   0        0        0     2320 2024-04-16 16:04:47.000000 networke-4.0/network/arith_stack_expr.py
+-rw-rw-rw-   0        0        0     2928 2024-04-21 15:58:47.000000 networke-4.0/network/array.py
+-rw-rw-rw-   0        0        0     1729 2024-04-21 15:47:20.000000 networke-4.0/network/bst.py
+-rw-rw-rw-   0        0        0     6873 2024-03-10 04:18:36.000000 networke-4.0/network/doublelinky.py
+-rw-rw-rw-   0        0        0      190 2024-04-21 15:53:20.000000 networke-4.0/network/factorial.py
+-rw-rw-rw-   0        0        0      255 2024-04-21 15:36:45.000000 networke-4.0/network/fibonacci_Series.py
+-rw-rw-rw-   0        0        0      248 2024-04-11 13:23:15.000000 networke-4.0/network/hanoi.py
+-rw-rw-rw-   0        0        0     3028 2024-04-11 16:21:42.000000 networke-4.0/network/krus.py
+-rw-rw-rw-   0        0        0     4619 2024-02-23 14:09:39.000000 networke-4.0/network/linked_list.py
+-rw-rw-rw-   0        0        0       82 2024-04-09 15:54:50.000000 networke-4.0/network/main.py
+-rw-rw-rw-   0        0        0      971 2024-04-11 13:41:30.000000 networke-4.0/network/merge_sort.py
+-rw-rw-rw-   0        0        0     5710 2024-04-11 16:32:14.000000 networke-4.0/network/poley.py
+-rw-rw-rw-   0        0        0      236 2024-04-11 13:19:31.000000 networke-4.0/network/power.py
+-rw-rw-rw-   0        0        0     2317 2024-04-21 15:44:10.000000 networke-4.0/network/program_dfs.py
+-rw-rw-rw-   0        0        0     3463 2024-04-09 13:52:44.000000 networke-4.0/network/program_heap.py
+-rw-rw-rw-   0        0        0     2205 2024-04-09 13:23:53.000000 networke-4.0/network/program_prims.py
+-rw-rw-rw-   0        0        0     1056 2024-04-09 11:30:12.000000 networke-4.0/network/program_quicksort.py
+-rw-rw-rw-   0        0        0     2805 2024-04-11 14:23:00.000000 networke-4.0/network/qu.py
+-rw-rw-rw-   0        0        0      418 2024-04-11 13:29:15.000000 networke-4.0/network/seat.py
+-rw-rw-rw-   0        0        0     1516 2024-04-11 13:55:51.000000 networke-4.0/network/stackey.py
+-rw-rw-rw-   0        0        0      197 2024-04-11 13:17:01.000000 networke-4.0/network/sum of n.py
+drwxrwxrwx   0        0        0        0 2024-04-21 16:05:19.239313 networke-4.0/networke.egg-info/
+-rw-rw-rw-   0        0        0       80 2024-04-21 16:05:15.000000 networke-4.0/networke.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      640 2024-04-21 16:05:16.000000 networke-4.0/networke.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 16:05:15.000000 networke-4.0/networke.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-21 16:05:15.000000 networke-4.0/networke.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 16:05:19.249838 networke-4.0/setup.cfg
+-rw-rw-rw-   0        0        0      197 2024-04-21 16:02:10.000000 networke-4.0/setup.py
```

### Comparing `networke-3.0/network/bst.py` & `networke-4.0/network/bst.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,33 +31,36 @@
         return 0
     left = height(node.left)
     right = height(node.right)
     return 1 + max(left,right)
 def inorder(node):
     if node is not None:
         inorder(node.left)
-        print(node.value,end="")
+        print(node.value,end=" ")
         inorder(node.right)
 def preorder(node):
     if node is not None:
         
-        print(node.value,end="")
+        print(node.value,end=" ")
         preorder(node.left)
         preorder(node.right)
 def postorder(node):
     if node is not None:
         postorder(node.left)
         postorder(node.right)
-        print(node.value,end="")
+        print(node.value,end=" ")
 
 print("Binary Tree Creation")
 bst = create()
 print(bst)
 size = size(bst)
 print("Size of the Tree:",size)
 height = height(bst) - 1
 print("Height of the Tree:",height)
-print("Inorder Traversal:", inorder(bst))
-print("Preorder Traversal:", preorder(bst))
-print("Postorder Traversal:", postorder(bst))
+print("\nInorder Traversal:")
+inorder(bst)
+print("\nPreorder Traversal:")
+preorder(bst)
+print("\nPostorder Traversal:")
+postorder(bst)
```

### Comparing `networke-3.0/network/doublelinky.py` & `networke-4.0/network/doublelinky.py`

 * *Files identical despite different names*

### Comparing `networke-3.0/network/krus.py` & `networke-4.0/network/krus.py`

 * *Files identical despite different names*

### Comparing `networke-3.0/network/linked_list.py` & `networke-4.0/network/linked_list.py`

 * *Files identical despite different names*

### Comparing `networke-3.0/network/merge_sort.py` & `networke-4.0/network/merge_sort.py`

 * *Files identical despite different names*

### Comparing `networke-3.0/network/poley.py` & `networke-4.0/network/poley.py`

 * *Files identical despite different names*

### Comparing `networke-3.0/network/program_array.py` & `networke-4.0/network/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         return new_arr
 def traverse(arr):
     for i in range(len(arr)):
         print(arr[i],end= "")
 
 
 def main():
-    n = int(input("Enter the array limit:"))
+    n = int(input("Enter the Initial Array Length:"))
     array = input_array(n)
     print(array)
     while True:
         print("\n1. Insert an element")
         print("2. Delete an element")
         print("3. Search an element")
         print("4. Update an element")
```

### Comparing `networke-3.0/network/program_dfs.py` & `networke-4.0/network/program_dfs.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,64 +6,67 @@
 class Tree:
     def __init__(self):
         self.root = None
 
     def insert(self,value):
         if not self.root:
             self.root = Node(value)
-            print(f"Root node inserted {value}")
+            print(f"\nRoot node inserted {value}")
             return
         queue = [self.root]
         while queue:
             current  = queue.pop(0)
             if not current.left:
                 current.left = Node(value)
-                print(f"Node {value} inserted as Child node of {current.value} (left)")
+                print(f"\nNode {value} inserted as Child node of {current.value} (left)")
                 break
             elif not current.right:
                 current.right = Node(value)
-                print(f"Node {value} inserted as Child node of {current.value} (right)")
+                print(f"\nNode {value} inserted as Child node of {current.value} (right)")
                 break
             else:
                 queue.append(current.left)
                 queue.append(current.right)
     def inorder(self,node):
         if node:
             self.inorder(node.left)
-            print(node.value,end = "")
+            print(node.value,end = " ")
             self.inorder(node.right)
     def preorder(self,node):
         if node:
-            print(node.value,end = "")
+            print(node.value,end = " ")
             self.preorder(node.left)
             self.preorder(node.right)
     def postorder(self,node):
         if node:
             self.postorder(node.left)
             self.postorder(node.right)
-            print(node.value,end = "")
+            print(node.value,end = " ")
 def main():
     tree = Tree()
     print("DFS TRAVERSAL")
     print("\n1. Insert elements")
     print("2. Inorder Traversal")
     print("3. Preorder Traversal")
     print("4. PostOrder Traversal")
     print("5. Exit")
     while True:
-        choice = int(input("Enter your choice:"))
+        choice = int(input("\nEnter your choice:"))
         if choice == 1:
-            value = input("Enter the value to insert")
+            value = input("Enter the value to insert:")
             tree.insert(value)
         elif choice == 2:
+            print("\nInorder Traversal:")
             tree.inorder(tree.root)
 
         elif choice == 3:
+            print("\nPreorder Traversal:")
             tree.preorder(tree.root)
         elif choice == 4:
+            print("\nPostorder Traversal:")
             tree.postorder(tree.root)
         elif choice == 5:
             break
         else:
             print("Invalid Choice")
 if __name__ == "__main__":
     main()
```

### Comparing `networke-3.0/network/program_heap.py` & `networke-4.0/network/program_heap.py`

 * *Files identical despite different names*

### Comparing `networke-3.0/network/program_prims.py` & `networke-4.0/network/program_prims.py`

 * *Files identical despite different names*

### Comparing `networke-3.0/network/program_quicksort.py` & `networke-4.0/network/program_quicksort.py`

 * *Files identical despite different names*

### Comparing `networke-3.0/network/program_stack_expr.py` & `networke-4.0/network/arith_stack_expr.py`

 * *Files identical despite different names*

### Comparing `networke-3.0/network/qu.py` & `networke-4.0/network/qu.py`

 * *Files identical despite different names*

### Comparing `networke-3.0/network/stackey.py` & `networke-4.0/network/stackey.py`

 * *Files identical despite different names*

### Comparing `networke-3.0/networke.egg-info/SOURCES.txt` & `networke-4.0/networke.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 LICENSE.txt
 README.md
 setup.py
+network/Ascending,descendign.py
 network/__init__.py
+network/arith_stack_expr.py
+network/array.py
 network/bst.py
-network/comp_sum.py
 network/doublelinky.py
+network/factorial.py
+network/fibonacci_Series.py
 network/hanoi.py
 network/krus.py
 network/linked_list.py
 network/main.py
 network/merge_sort.py
 network/poley.py
-network/pow.py
-network/progarm_factorial.py
-network/program_5_fibonacci.py
-network/program_array.py
-network/program_asc_Desc.py
+network/power.py
 network/program_dfs.py
 network/program_heap.py
 network/program_prims.py
 network/program_quicksort.py
-network/program_stack_expr.py
 network/qu.py
 network/seat.py
 network/stackey.py
+network/sum of n.py
 networke.egg-info/PKG-INFO
 networke.egg-info/SOURCES.txt
 networke.egg-info/dependency_links.txt
 networke.egg-info/top_level.txt
```

