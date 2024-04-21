# Comparing `tmp/mytot-2024.4.20.174642-py3-none-any.whl.zip` & `tmp/mytot-2024.4.21.213952-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,11 @@
-Zip file size: 27986 bytes, number of entries: 10
--rwxrwxr-x  2.0 unx     1469 b- defN 24-Apr-18 10:00 home/maxx/.local/share/mytot/TASK
+Zip file size: 27543 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-18 09:16 mytot/__init__.py
--rw-rw-r--  2.0 unx     1790 b- defN 24-Apr-20 09:44 mytot/main.py
--rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-18 09:16 mytot-2024.4.20.174642.data/data/LICENSE
--rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-20 09:46 mytot-2024.4.20.174642.dist-info/LICENSE
--rw-rw-r--  2.0 unx      777 b- defN 24-Apr-20 09:46 mytot-2024.4.20.174642.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-20 09:46 mytot-2024.4.20.174642.dist-info/WHEEL
--rw-rw-r--  2.0 unx       85 b- defN 24-Apr-20 09:46 mytot-2024.4.20.174642.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        6 b- defN 24-Apr-20 09:46 mytot-2024.4.20.174642.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      863 b- defN 24-Apr-20 09:46 mytot-2024.4.20.174642.dist-info/RECORD
-10 files, 75380 bytes uncompressed, 26492 bytes compressed:  64.9%
+-rw-rw-r--  2.0 unx     3263 b- defN 24-Apr-21 13:24 mytot/main.py
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-18 09:16 mytot-2024.4.21.213952.data/data/LICENSE
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-21 13:39 mytot-2024.4.21.213952.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      777 b- defN 24-Apr-21 13:39 mytot-2024.4.21.213952.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-21 13:39 mytot-2024.4.21.213952.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       85 b- defN 24-Apr-21 13:39 mytot-2024.4.21.213952.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        6 b- defN 24-Apr-21 13:39 mytot-2024.4.21.213952.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      773 b- defN 24-Apr-21 13:39 mytot-2024.4.21.213952.dist-info/RECORD
+9 files, 75294 bytes uncompressed, 26191 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -1,31 +1,28 @@
-Filename: home/maxx/.local/share/mytot/TASK
-Comment: 
-
 Filename: mytot/__init__.py
 Comment: 
 
 Filename: mytot/main.py
 Comment: 
 
-Filename: mytot-2024.4.20.174642.data/data/LICENSE
+Filename: mytot-2024.4.21.213952.data/data/LICENSE
 Comment: 
 
-Filename: mytot-2024.4.20.174642.dist-info/LICENSE
+Filename: mytot-2024.4.21.213952.dist-info/LICENSE
 Comment: 
 
-Filename: mytot-2024.4.20.174642.dist-info/METADATA
+Filename: mytot-2024.4.21.213952.dist-info/METADATA
 Comment: 
 
-Filename: mytot-2024.4.20.174642.dist-info/WHEEL
+Filename: mytot-2024.4.21.213952.dist-info/WHEEL
 Comment: 
 
-Filename: mytot-2024.4.20.174642.dist-info/entry_points.txt
+Filename: mytot-2024.4.21.213952.dist-info/entry_points.txt
 Comment: 
 
-Filename: mytot-2024.4.20.174642.dist-info/top_level.txt
+Filename: mytot-2024.4.21.213952.dist-info/top_level.txt
 Comment: 
 
-Filename: mytot-2024.4.20.174642.dist-info/RECORD
+Filename: mytot-2024.4.21.213952.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mytot/main.py

```diff
@@ -12,26 +12,30 @@
         os.makedirs(path)
 
 
 def RUN():
     if len(sys.argv) < 2:
         print("usage RUN [script_file]")
         return
+    if len(sys.argv) >= 3:
+        args = " ".join(sys.argv[2:])
+    else:
+        args = ""
     script_file = os.path.abspath(sys.argv[1])
     path, name = os.path.split(script_file)
     log_path = os.path.join(path, "log")
-    log_file = os.path.join(path, "log", f"{name}.run")
+    log_file = os.path.join(path, "log", f"{name}.log")
     mkdir(log_path)
     now = datetime.datetime.now()
     if name.endswith(".py"):
-        cmd = f"nohup python -Wignore {script_file} &"
+        cmd = f"nohup python -Wignore {script_file} {args} &"
     elif name.endswith(".sh"):
-        cmd = f"nohup bash {script_file} &"
+        cmd = f"nohup bash {script_file} {args} &"
     else:
-        cmd = f"nohup {script_file} &"
+        cmd = f"nohup {script_file} {args} &"
 
     with open(log_file, "a") as f:
         f.write(f"{now} | start run {name}\n")
     subprocess.Popen(
         cmd,
         cwd=path,
         stdout=open(log_file, "a"),
@@ -52,19 +56,60 @@
             continue
         key = arg
         break
     for process in psutil.process_iter(["pid", "name", "cmdline"]):
         if process.info["cmdline"] is None:
             continue
         cmdline = " ".join(list(process.info["cmdline"]))
+        if "KILL" in cmdline:
+            continue
         if key in cmdline:
             pid = process.info["pid"]
-            print("kill -{signal} {pid}")
+            print(f"kill -{signal} {pid}")
             os.kill(pid, signal)
 
 
+def today():
+    return datetime.datetime.now().strftime("%Y%m%d")
+
+
 def TASK():
     if len(sys.argv) < 2:
         print("usage TASK [script_file]")
         return
-    bash_file = os.path.expanduser("~/.local/share/mytot/TASK")
-    subprocess.run(["bash", bash_file] + sys.argv[1:], check=False)
+    script_file = os.path.abspath(sys.argv[1])
+    # check the pragma
+    date = today()
+    mkdir(os.path.expanduser("~/.cache/task_log/"))
+    task_log = os.path.expanduser(f"~/.cache/task_log/out.{date}")
+    for process in psutil.process_iter(["pid", "name", "cmdline"]):
+        if process.info["cmdline"] is None:
+            continue
+        cmdline = " ".join(list(process.info["cmdline"]))
+        if script_file in cmdline:
+            with open(task_log, "a") as f:
+                now = datetime.datetime.now()
+                f.write(f"{now} | {script_file} is running\n")
+            return
+    path, name = os.path.split(script_file)
+    log_path = os.path.join(path, "log")
+    mkdir(log_path)
+    if script_file.endswith(".py"):
+        cmd = ["python", "-Wignore", script_file]
+    elif script_file.endswith(".sh"):
+        cmd = ["bash", script_file]
+    else:
+        cmd = [script_file]
+    if len(sys.argv) >= 3:
+        cmd += sys.argv[2:]
+
+    with open(task_log, "a") as f:
+        f.write("{} | start run {}\n".format(datetime.datetime.now(), script_file))
+        f.write("{} | cmd: {}\n".format(datetime.datetime.now(), " ".join(cmd)))
+    log_file = os.path.join(path, "log", f"{name}.log")
+    subprocess.run(
+        cmd,
+        cwd=path,
+        stdout=open(log_file, "a"),
+        stderr=open(log_file, "a"),
+        check=False,
+    )
```

## Comparing `mytot-2024.4.20.174642.data/data/LICENSE` & `mytot-2024.4.21.213952.data/data/LICENSE`

 * *Files identical despite different names*

## Comparing `mytot-2024.4.20.174642.dist-info/LICENSE` & `mytot-2024.4.21.213952.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mytot-2024.4.20.174642.dist-info/METADATA` & `mytot-2024.4.21.213952.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mytot
-Version: 2024.4.20.174642
+Version: 2024.4.21.213952
 Summary: Tool of Tool
 Author: Xin-Xin Ma
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
 Requires-Dist: psutil
```

