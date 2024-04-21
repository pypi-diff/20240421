# Comparing `tmp/inmanta_module_files-0.2.0-py3-none-any.whl.zip` & `tmp/inmanta_module_files-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 20900 bytes, number of entries: 19
--rw-r--r--  2.0 unx      602 b- defN 24-Apr-07 17:20 inmanta_plugins/files/__init__.py
--rw-r--r--  2.0 unx     2624 b- defN 24-Apr-07 17:20 inmanta_plugins/files/base.py
--rw-r--r--  2.0 unx     2330 b- defN 24-Apr-07 17:20 inmanta_plugins/files/directory.py
--rw-r--r--  2.0 unx     6585 b- defN 24-Apr-07 17:20 inmanta_plugins/files/host.py
--rw-r--r--  2.0 unx     5848 b- defN 24-Apr-07 17:20 inmanta_plugins/files/json.py
--rw-r--r--  2.0 unx     2170 b- defN 24-Apr-07 17:21 inmanta_plugins/files/setup.cfg
--rw-r--r--  2.0 unx     2258 b- defN 24-Apr-07 17:20 inmanta_plugins/files/systemd_unit.py
--rw-r--r--  2.0 unx     2200 b- defN 24-Apr-07 17:20 inmanta_plugins/files/text.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-07 17:20 inmanta_plugins/files/files/.gitkeep
--rw-r--r--  2.0 unx     3679 b- defN 24-Apr-07 17:20 inmanta_plugins/files/model/_init.cf
--rw-r--r--  2.0 unx     1661 b- defN 24-Apr-07 17:20 inmanta_plugins/files/model/host.cf
--rw-r--r--  2.0 unx     1586 b- defN 24-Apr-07 17:20 inmanta_plugins/files/model/json.cf
--rw-r--r--  2.0 unx    10884 b- defN 24-Apr-07 17:20 inmanta_plugins/files/model/systemd_unit.cf
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-07 17:20 inmanta_plugins/files/templates/.gitkeep
--rw-r--r--  2.0 unx     2950 b- defN 24-Apr-07 17:20 inmanta_plugins/files/templates/systemd_unit.j2
--rw-r--r--  2.0 unx      742 b- defN 24-Apr-07 17:21 inmanta_module_files-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-07 17:21 inmanta_module_files-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-07 17:21 inmanta_module_files-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1721 b- defN 24-Apr-07 17:21 inmanta_module_files-0.2.0.dist-info/RECORD
-19 files, 47948 bytes uncompressed, 18028 bytes compressed:  62.4%
+Zip file size: 21124 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      602 b- defN 24-Apr-21 08:19 inmanta_plugins/files/__init__.py
+-rw-r--r--  2.0 unx     2624 b- defN 24-Apr-21 08:19 inmanta_plugins/files/base.py
+-rw-r--r--  2.0 unx     3188 b- defN 24-Apr-21 08:19 inmanta_plugins/files/directory.py
+-rw-r--r--  2.0 unx     6585 b- defN 24-Apr-21 08:19 inmanta_plugins/files/host.py
+-rw-r--r--  2.0 unx     5848 b- defN 24-Apr-21 08:19 inmanta_plugins/files/json.py
+-rw-r--r--  2.0 unx     2170 b- defN 24-Apr-21 08:19 inmanta_plugins/files/setup.cfg
+-rw-r--r--  2.0 unx     2258 b- defN 24-Apr-21 08:19 inmanta_plugins/files/systemd_unit.py
+-rw-r--r--  2.0 unx     2200 b- defN 24-Apr-21 08:19 inmanta_plugins/files/text.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-21 08:19 inmanta_plugins/files/files/.gitkeep
+-rw-r--r--  2.0 unx     3706 b- defN 24-Apr-21 08:19 inmanta_plugins/files/model/_init.cf
+-rw-r--r--  2.0 unx     1661 b- defN 24-Apr-21 08:19 inmanta_plugins/files/model/host.cf
+-rw-r--r--  2.0 unx     1586 b- defN 24-Apr-21 08:19 inmanta_plugins/files/model/json.cf
+-rw-r--r--  2.0 unx    10884 b- defN 24-Apr-21 08:19 inmanta_plugins/files/model/systemd_unit.cf
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-21 08:19 inmanta_plugins/files/templates/.gitkeep
+-rw-r--r--  2.0 unx     2950 b- defN 24-Apr-21 08:19 inmanta_plugins/files/templates/systemd_unit.j2
+-rw-r--r--  2.0 unx      742 b- defN 24-Apr-21 08:19 inmanta_module_files-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 08:19 inmanta_module_files-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-21 08:19 inmanta_module_files-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1721 b- defN 24-Apr-21 08:19 inmanta_module_files-0.2.1.dist-info/RECORD
+19 files, 48833 bytes uncompressed, 18252 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: inmanta_plugins/files/templates/.gitkeep
 Comment: 
 
 Filename: inmanta_plugins/files/templates/systemd_unit.j2
 Comment: 
 
-Filename: inmanta_module_files-0.2.0.dist-info/METADATA
+Filename: inmanta_module_files-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_files-0.2.0.dist-info/WHEEL
+Filename: inmanta_module_files-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_files-0.2.0.dist-info/top_level.txt
+Filename: inmanta_module_files-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_files-0.2.0.dist-info/RECORD
+Filename: inmanta_module_files-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/files/directory.py

```diff
@@ -12,14 +12,16 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 Contact: edvgui@gmail.com
 """
 
+import pathlib
+
 import inmanta.agent.agent
 import inmanta.agent.handler
 import inmanta.agent.io.local
 import inmanta.const
 import inmanta.execute.proxy
 import inmanta.export
 import inmanta.resources
@@ -45,20 +47,37 @@
         self, ctx: inmanta.agent.handler.HandlerContext, resource: DirectoryResource
     ) -> None:
         super().read_resource(ctx, resource)
 
     def create_resource(
         self, ctx: inmanta.agent.handler.HandlerContext, resource: DirectoryResource
     ) -> None:
-        if not resource.create_parents:
-            # Call the basic io mkdir helper
-            self._io.mkdir(resource.path)
-        else:
-            # Call the mkdir command on the host in a subprocess
-            self._io.run("mkdir", ["-p", resource.path], timeout=10)
+        if resource.create_parents:
+            # Create all parent directories, with the owner, group and permissions of
+            # their parents
+            parent_owner = "root"
+            parent_group = "root"
+            parent_permissions = "555"
+            for parent in reversed(pathlib.Path(resource.path).parents):
+                if not self._io.file_exists(str(parent)):
+                    # Create the parent directory, and make sure it has the
+                    # right owner and permissions
+                    self._io.mkdir(str(parent))
+                    self._io.chmod(str(parent), parent_permissions)
+                    self._io.chown(str(parent), parent_owner, parent_group)
+                    continue
+
+                # Read the existing folder permissions, and save it for the next child folder
+                stat = self._io.file_stat(str(parent))
+                parent_owner = stat["owner"]
+                parent_group = stat["group"]
+                parent_permissions = str(stat["permissions"])
+
+        # Call the basic io mkdir helper
+        self._io.mkdir(resource.path)
 
         super().create_resource(ctx, resource)
 
     def update_resource(
         self,
         ctx: inmanta.agent.handler.HandlerContext,
         changes: dict[str, dict[str, object]],
```

## inmanta_plugins/files/setup.cfg

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = inmanta-module-files
-version = 0.2.0
+version = 0.2.1
 description = Simple module containing various types of resource to manage files.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Guillaume Everarts de Velp
 author_email = edvgui@gmail.com
 license = ASL 2.0
 copyright = 2023 Guillaume Everarts de Velp
```

## inmanta_plugins/files/model/_init.cf

```diff
@@ -41,14 +41,15 @@
     :attr group: The name of the group owning the file
         (null if you don't want to manage this).
     """
     string path
     int? permissions = 744
     string? owner
     string? group
+    bool send_event = true
 end
 BaseFile.host [1] -- std::Host
 """
 The host that this file is managed on.
 """
```

## Comparing `inmanta_module_files-0.2.0.dist-info/METADATA` & `inmanta_module_files-0.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmanta-module-files
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple module containing various types of resource to manage files.
 Author: Guillaume Everarts de Velp
 Author-email: edvgui@gmail.com
 License: ASL 2.0
 Description-Content-Type: text/markdown
 Requires-Dist: inmanta-module-std
```

## Comparing `inmanta_module_files-0.2.0.dist-info/RECORD` & `inmanta_module_files-0.2.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 inmanta_plugins/files/__init__.py,sha256=BUgfj_qgct0U3NELQUglCpB81sjkDRMCrHtloSL4ylM,602
 inmanta_plugins/files/base.py,sha256=nIuZ5q3mj876P6n6aeZ_ramQUHzR7NjJ4G_tsuRPKrc,2624
-inmanta_plugins/files/directory.py,sha256=2vQ4Torn5NpA55-uDXcqgkPM9VmBq0zJaBdUz31PyL4,2330
+inmanta_plugins/files/directory.py,sha256=pqCVFBLz_zQUHQ6e5rG43ht0njicMop-4GCXBsWYo_w,3188
 inmanta_plugins/files/host.py,sha256=c4pcP8zroNLc2RbVgOnQYlA5mdqQnP45cnS8941cMHk,6585
 inmanta_plugins/files/json.py,sha256=kY6ql6QB9BUA2bPTrX7LSgYrNcIlJlYzTQDoIMrahNg,5848
-inmanta_plugins/files/setup.cfg,sha256=bT0c2t7rseq8G4c2vDrxM6Nd3rsphKxt8C_Q_sXCe3o,2170
+inmanta_plugins/files/setup.cfg,sha256=j2-IfC8YZzA4JxNieMmTkObetLmSnpAmBJJvRXXiBi8,2170
 inmanta_plugins/files/systemd_unit.py,sha256=x_-yy9Bl_8O_SNViIkwtpH8ma-NZskmqlGkGBzkSoN4,2258
 inmanta_plugins/files/text.py,sha256=h6ZoDGtZYlC2yEGiLpopL96rOMKUrw-AxPULEysO8-I,2200
 inmanta_plugins/files/files/.gitkeep,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-inmanta_plugins/files/model/_init.cf,sha256=FB0UFvCiAqpBFx_RFS0zA2V0oja532hfEOpqFx7o89Q,3679
+inmanta_plugins/files/model/_init.cf,sha256=rCoI_LIQxT6xgGzNixEnl3OgI8NfaBm7bEUgAqqjGxM,3706
 inmanta_plugins/files/model/host.cf,sha256=tpW8EhP9ECeZ_Q97Q7giwIrjj6HlVd9XzvchFkCS4XA,1661
 inmanta_plugins/files/model/json.cf,sha256=6Om8bihPKrZX7-hfyZLZ_rn7G-CLwf0BNvggJOdkTx8,1586
 inmanta_plugins/files/model/systemd_unit.cf,sha256=prsWy4r9ofpeQoHcszIc89usgkGl_UtC3gcRILpQ4QQ,10884
 inmanta_plugins/files/templates/.gitkeep,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inmanta_plugins/files/templates/systemd_unit.j2,sha256=fp-_5ggm2U_YPCGhPzKWrOigQZMbqTJ6AdhwUd7nQ9A,2950
-inmanta_module_files-0.2.0.dist-info/METADATA,sha256=5idxLTn4iNX6rMNPVT48A7J_5CdZ4mBYZWJH7W-hZIk,742
-inmanta_module_files-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-inmanta_module_files-0.2.0.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
-inmanta_module_files-0.2.0.dist-info/RECORD,,
+inmanta_module_files-0.2.1.dist-info/METADATA,sha256=9T2Sd6HqAYwdlsYiySNq7U-qHG0tjrBZ7CyF8FWR1wI,742
+inmanta_module_files-0.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+inmanta_module_files-0.2.1.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
+inmanta_module_files-0.2.1.dist-info/RECORD,,
```

