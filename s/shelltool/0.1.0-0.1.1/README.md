# Comparing `tmp/shelltool-0.1.0.tar.gz` & `tmp/shelltool-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shelltool-0.1.0.tar", last modified: Sun Apr 21 05:55:28 2024, max compression
+gzip compressed data, was "shelltool-0.1.1.tar", last modified: Sun Apr 21 07:33:31 2024, max compression
```

## Comparing `shelltool-0.1.0.tar` & `shelltool-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 05:55:28.820946 shelltool-0.1.0/
--rw-rw-rw-   0        0        0     1070 2024-04-21 05:33:02.000000 shelltool-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     5268 2024-04-21 05:55:28.818943 shelltool-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4742 2024-04-21 05:55:10.000000 shelltool-0.1.0/README.md
--rw-rw-rw-   0        0        0      593 2024-04-21 05:53:14.000000 shelltool-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-21 05:55:28.820946 shelltool-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-21 05:55:28.817946 shelltool-0.1.0/shelltool.egg-info/
--rw-rw-rw-   0        0        0     5268 2024-04-21 05:55:28.000000 shelltool-0.1.0/shelltool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2024-04-21 05:55:28.000000 shelltool-0.1.0/shelltool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 05:55:28.000000 shelltool-0.1.0/shelltool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-21 05:55:28.000000 shelltool-0.1.0/shelltool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4258 2024-04-21 05:55:06.000000 shelltool-0.1.0/shelltool.py
+drwxrwxrwx   0        0        0        0 2024-04-21 07:33:31.546514 shelltool-0.1.1/
+-rw-rw-rw-   0        0        0     1070 2024-04-21 05:33:02.000000 shelltool-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5901 2024-04-21 07:33:31.544515 shelltool-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5375 2024-04-21 07:32:37.000000 shelltool-0.1.1/README.md
+-rw-rw-rw-   0        0        0      593 2024-04-21 07:28:30.000000 shelltool-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-21 07:33:31.546514 shelltool-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-21 07:33:31.543504 shelltool-0.1.1/shelltool.egg-info/
+-rw-rw-rw-   0        0        0     5901 2024-04-21 07:33:31.000000 shelltool-0.1.1/shelltool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2024-04-21 07:33:31.000000 shelltool-0.1.1/shelltool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 07:33:31.000000 shelltool-0.1.1/shelltool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-21 07:33:31.000000 shelltool-0.1.1/shelltool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5080 2024-04-21 07:27:55.000000 shelltool-0.1.1/shelltool.py
```

### Comparing `shelltool-0.1.0/LICENSE` & `shelltool-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shelltool-0.1.0/PKG-INFO` & `shelltool-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: shelltool
-Version: 0.1.0
-Summary: A better way to compose shell-like commands in python.
-Author: William L.
-Project-URL: Homepage, https://github.com/FrewtyPebbles/Shellify.py
-Project-URL: Issues, https://github.com/FrewtyPebbles/Shellify.py/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Shelltool
 
 Shelltool is an api that makes dealing with and composing subprocesses in python easier, more readable, and more immediately useful.  It accomplishes this by utilizing syntax that makes it feel more like composing procedures in Bash rather than dealing with things like `Popen` or `Thread(target=lambda:subprocess.run())`.
 
 Heres an example of the syntax.  
 ```py
 if __name__ == "__main__":
@@ -167,7 +153,24 @@
 cat_to_grep_cmd = ~(SHELL.cat("./shelltool.py") | SHELL.grep("SHELL"))
 cat_to_grep_cmd.run()
 
 print(cat_to_grep_cmd.pid) # Here it is!
 
 print(cat_to_grep_cmd.stdout.decode())
 ```
+
+## Uh Oh! Race conditions! (How To Join a Concurrent Subprocess Back To It's Spawning Thread)
+
+To join a subprocess back to its spawning thread call `.finish()`:
+```py
+if __name__ == "__main__":
+    process, process_err = ~((p1 := (SHELL.echo("SHELL") | SHELL.tee("/dev/stderr"))) | SHELL.grep("SHELL")), ~(p1 @ SHELL.grep("SHELL"))
+    process.run()
+    
+    process.finish()
+    # this joins the thread/process so `p1` and the rest of `process` is evaluated at a predictable time.
+
+    process_err.run()
+    
+    print(f"p_out:\n{process.stdout.decode()}")
+    print(f"p_err:\n{process_err.stdout.decode()}")
+```
```

### Comparing `shelltool-0.1.0/pyproject.toml` & `shelltool-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "shelltool"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="William L." },
 ]
 description = "A better way to compose shell-like commands in python."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `shelltool-0.1.0/shelltool.egg-info/PKG-INFO` & `shelltool-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shelltool
-Version: 0.1.0
+Version: 0.1.1
 Summary: A better way to compose shell-like commands in python.
 Author: William L.
 Project-URL: Homepage, https://github.com/FrewtyPebbles/Shellify.py
 Project-URL: Issues, https://github.com/FrewtyPebbles/Shellify.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -167,7 +167,24 @@
 cat_to_grep_cmd = ~(SHELL.cat("./shelltool.py") | SHELL.grep("SHELL"))
 cat_to_grep_cmd.run()
 
 print(cat_to_grep_cmd.pid) # Here it is!
 
 print(cat_to_grep_cmd.stdout.decode())
 ```
+
+## Uh Oh! Race conditions! (How To Join a Concurrent Subprocess Back To It's Spawning Thread)
+
+To join a subprocess back to its spawning thread call `.finish()`:
+```py
+if __name__ == "__main__":
+    process, process_err = ~((p1 := (SHELL.echo("SHELL") | SHELL.tee("/dev/stderr"))) | SHELL.grep("SHELL")), ~(p1 @ SHELL.grep("SHELL"))
+    process.run()
+    
+    process.finish()
+    # this joins the thread/process so `p1` and the rest of `process` is evaluated at a predictable time.
+
+    process_err.run()
+    
+    print(f"p_out:\n{process.stdout.decode()}")
+    print(f"p_err:\n{process_err.stdout.decode()}")
+```
```

### Comparing `shelltool-0.1.0/shelltool.py` & `shelltool-0.1.1/shelltool.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,40 +18,55 @@
         self.pipe_in:bytes | CLITool = None
         self.args = []
         self.thread:th.Thread = None
         self._stderr:bytes = None
         self._stdout:bytes = None
         self.pipe_err = False
         self.concurrent = False
+        self.has_run = False
 
     def __call__(self, *args: Any) -> CLITool:
         self.args = [self.name, *[str(arg) for arg in args]]
         return self
     
+    def finish(self):
+        "Blocks code untill process is finished.  Basically the same as `.join()`ing the thread."
+        if self.thread != None:
+            self.thread.join()
+        else:
+            raise RuntimeError("Concurrent process is not running.")
+
+    
     def _run(self):
         "Run the command."
         self.process = subp.Popen(" ".join(self.args), shell=True,
             stdout=subp.PIPE, stderr=subp.PIPE, stdin=subp.PIPE)
         
         pipe_in = b''
 
         if isinstance(self.pipe_in, CLITool):
             if self.pipe_err:
-                pipe_in = self.pipe_in.run().stderr
+                if not self.pipe_in.has_run:
+                    self.pipe_in.run()
+                pipe_in = self.pipe_in.stderr
             else:
-                pipe_in = self.pipe_in.run().stdout
+                if not self.pipe_in.has_run:
+                    self.pipe_in.run()
+                pipe_in = self.pipe_in.stdout
         else:
             pipe_in = self.pipe_in
 
+        #print(self.name, "RUNNING")
         self._stdout, self._stderr = self.process.communicate(pipe_in)
 
         return self
     
     def run(self):
         "Runs the process."
+        self.has_run = True
         if self.concurrent:
             return self._run_concurrent()
         else:
             return self._run()
     
     def _run_concurrent(self):
         "Runs process on a separate thread."
@@ -107,25 +122,25 @@
             return self.process.pid
         return None
     
     @property
     def stdout(self):
         if self._stdout != None:
             return self._stdout
-        if self.concurrent:
+        elif self.thread != None:
             self.thread.join()
-            return self._stdout
+        return self._stdout
     
     @property
     def stderr(self):
         if self._stderr != None:
             return self._stderr
-        if self.concurrent:
+        elif self.thread != None:
             self.thread.join()
-            return self._stderr
+        return self._stderr
 
 class Shell:
     def __getattribute__(self, name: str) -> CLITool:
         "Shell command."
         return CLITool(name)
     def __getitem__(self, name: str) -> CLITool:
         "Shell command."
@@ -133,12 +148,17 @@
     def __getattr__(self, name: str) -> CLITool:
         "Shell command."
         return CLITool(name)
     
 SHELL = Shell()
 
 if __name__ == "__main__":
-    
-    process = ~(SHELL.cat("./shelltool.py") | SHELL.grep("SHELL"))
+    process, process_err = ~((p1 := (SHELL.echo("SHELL") | SHELL.tee("/dev/stderr"))) | SHELL.grep("SHELL")), ~(p1 @ SHELL.grep("SHELL"))
     process.run()
+    
+    process.finish()
+    # this joins the thread/process so `p1` and the rest of `process` is evaluated at a predictable time.
 
-    print(f"result:\n{process.stdout.decode()}")
+    process_err.run()
+    
+    print(f"p_out:\n{process.stdout.decode()}")
+    print(f"p_err:\n{process_err.stdout.decode()}")
```

