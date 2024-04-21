# Comparing `tmp/django_seeding-1.1.2.tar.gz` & `tmp/django_seeding-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_seeding-1.1.2.tar", last modified: Sun Apr 21 01:33:26 2024, max compression
+gzip compressed data, was "django_seeding-1.2.1.tar", last modified: Sun Apr 21 01:52:25 2024, max compression
```

## Comparing `django_seeding-1.1.2.tar` & `django_seeding-1.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:26.818701 django_seeding-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 01:33:20.000000 django_seeding-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17689 2024-04-21 01:33:26.818701 django_seeding-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17003 2024-04-21 01:33:20.000000 django_seeding-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:26.814701 django_seeding-1.1.2/django_seeding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/casting_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:26.814701 django_seeding-1.1.2/django_seeding/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:26.818701 django_seeding-1.1.2/django_seeding/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/management/commands/runserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/management/commands/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:26.818701 django_seeding-1.1.2/django_seeding/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/seeder_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/seeders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:26.818701 django_seeding-1.1.2/django_seeding.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17689 2024-04-21 01:33:26.000000 django_seeding-1.1.2/django_seeding.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-21 01:33:26.000000 django_seeding-1.1.2/django_seeding.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 01:33:26.000000 django_seeding-1.1.2/django_seeding.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 01:33:26.000000 django_seeding-1.1.2/django_seeding.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-21 01:33:20.000000 django_seeding-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 01:33:26.818701 django_seeding-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-21 01:33:20.000000 django_seeding-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:52:25.536797 django_seeding-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 01:52:20.000000 django_seeding-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17689 2024-04-21 01:52:25.536797 django_seeding-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17003 2024-04-21 01:52:20.000000 django_seeding-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:52:25.536797 django_seeding-1.2.1/django_seeding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:52:20.000000 django_seeding-1.2.1/django_seeding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-21 01:52:20.000000 django_seeding-1.2.1/django_seeding/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-21 01:52:20.000000 django_seeding-1.2.1/django_seeding/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-21 01:52:20.000000 django_seeding-1.2.1/django_seeding/casting_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:52:25.536797 django_seeding-1.2.1/django_seeding/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:52:20.000000 django_seeding-1.2.1/django_seeding/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:52:25.536797 django_seeding-1.2.1/django_seeding/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:52:20.000000 django_seeding-1.2.1/django_seeding/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-21 01:52:20.000000 django_seeding-1.2.1/django_seeding/management/commands/runserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-21 01:52:20.000000 django_seeding-1.2.1/django_seeding/management/commands/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:52:25.536797 django_seeding-1.2.1/django_seeding/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 01:52:20.000000 django_seeding-1.2.1/django_seeding/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:52:20.000000 django_seeding-1.2.1/django_seeding/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-21 01:52:20.000000 django_seeding-1.2.1/django_seeding/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-21 01:52:20.000000 django_seeding-1.2.1/django_seeding/seeder_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-04-21 01:52:20.000000 django_seeding-1.2.1/django_seeding/seeders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:52:25.536797 django_seeding-1.2.1/django_seeding.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17689 2024-04-21 01:52:25.000000 django_seeding-1.2.1/django_seeding.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-21 01:52:25.000000 django_seeding-1.2.1/django_seeding.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 01:52:25.000000 django_seeding-1.2.1/django_seeding.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 01:52:25.000000 django_seeding-1.2.1/django_seeding.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-21 01:52:20.000000 django_seeding-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 01:52:25.536797 django_seeding-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-21 01:52:20.000000 django_seeding-1.2.1/setup.py
```

### Comparing `django_seeding-1.1.2/LICENSE` & `django_seeding-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_seeding-1.1.2/PKG-INFO` & `django_seeding-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-seeding
-Version: 1.1.2
+Version: 1.2.1
 Summary: Simple Django Package that helps developer to seed data from files and codes into the database automatically
 Author-email: Suliman Awad <sulimanawadstudy@gmail.com>
 Project-URL: Source, https://github.com/suliman-99/django-seeding
 Project-URL: Contributors, https://github.com/suliman-99/django-seeding/graphs/contributors
 Project-URL: License, https://github.com/suliman-99/django-seeding/blob/main/LICENSE
 Project-URL: Issues, https://github.com/suliman-99/django-seeding/issues
 Classifier: Programming Language :: Python
```

### Comparing `django_seeding-1.1.2/README.md` & `django_seeding-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django_seeding-1.1.2/django_seeding/management/commands/runserver.py` & `django_seeding-1.2.1/django_seeding/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `django_seeding-1.1.2/django_seeding/seeder_registry.py` & `django_seeding-1.2.1/django_seeding/seeder_registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,18 @@
     seeders = []
 
     @classmethod
     def register(cls, seeder):
         """ Method and decorator to register the seeder-class in the seeders list to be seeded when the server is run """
         if not issubclass(seeder, Seeder):
             raise TypeError('Only subclasses of Seeder class can be registered with SeederRegistry.register')
-        
-        if seeder().get_id() in [obj.get_id() for obj in cls.seeders]:
-            return
+         
+        for cur_seeder in cls.seeders:
+            if cur_seeder._get_id() == seeder()._get_id():
+                return
         
         cls.seeders.append(seeder())
 
     @classmethod
     def import_all(cls):
         """ Method that import all `seeders.py` files in the installed apps to register them in the `SeederRegistry` class """
         for app_config in apps.get_app_configs():
@@ -39,47 +40,50 @@
             file_path = Path(app_config.path) / file_name
             if file_path.exists():
                 spec = importlib.util.spec_from_file_location(f"{app_name}.{module_name}", str(file_path))
                 module = importlib.util.module_from_spec(spec)
                 spec.loader.exec_module(module)
 
     @classmethod
-    def seed_all(cls, debug=None):
+    def seed_all(cls, debug=None, ids=None):
         """ 
         Method that call seed methods for all registered seeders
         
         sort the seeders depending on the `priority` (less is applied earlier)
         """
+        seeders = cls.seeders
+        if ids is not None:
+            seeders = filter(lambda seeder: seeder._get_id() in ids, seeders)
 
-        if AppliedSeeder.objects.filter(id__in=[seeder._get_id() for seeder in cls.seeders]).count() != len(cls.seeders):
+        if AppliedSeeder.objects.filter(id__in=[seeder._get_id() for seeder in seeders]).count() != len(seeders):
             BLUE_COLOR = "\033[94m"
             WHITE_COLOR = "\033[0m"
             print(BLUE_COLOR + "Running Seeders: " + WHITE_COLOR)
 
-        cls.seeders.sort(key=lambda seeder: seeder._get_priority())
-        for seeder in cls.seeders:
+        seeders.sort(key=lambda seeder: seeder._get_priority())
+        for seeder in seeders:
             seeder._seed(debug=debug)
 
     @classmethod
-    def import_all_then_seed_all(cls, debug=None):
+    def import_all_then_seed_all(cls, debug=None, ids=None):
         """
         Note: the decorator `@SeederRegistry.register` will be applied when the file is imported
 
         so, if the seeder class is written in another file (not in `seeders.py`)
         then it will not be imported
         then it will not be applied when the server is run
 
         so, to solve this problem you can import any file contains seeder inside the `AppConfig` class of your app
         """
 
         # import all `seeders.py` files from all installed apps
         cls.import_all()
 
         # call the `seed_all()` method to apply all the registered seeders
-        cls.seed_all(debug=debug)
+        cls.seed_all(debug=debug, ids=ids)
 
     @classmethod
     def on_run(cls):
         if 'runserver' not in sys.argv:
             return
         
         seed = bool(getattr(settings, 'SEEDING_ON_RUNSERVER', False))
```

### Comparing `django_seeding-1.1.2/django_seeding/seeders.py` & `django_seeding-1.2.1/django_seeding/seeders.py`

 * *Files identical despite different names*

### Comparing `django_seeding-1.1.2/django_seeding.egg-info/PKG-INFO` & `django_seeding-1.2.1/django_seeding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-seeding
-Version: 1.1.2
+Version: 1.2.1
 Summary: Simple Django Package that helps developer to seed data from files and codes into the database automatically
 Author-email: Suliman Awad <sulimanawadstudy@gmail.com>
 Project-URL: Source, https://github.com/suliman-99/django-seeding
 Project-URL: Contributors, https://github.com/suliman-99/django-seeding/graphs/contributors
 Project-URL: License, https://github.com/suliman-99/django-seeding/blob/main/LICENSE
 Project-URL: Issues, https://github.com/suliman-99/django-seeding/issues
 Classifier: Programming Language :: Python
```

### Comparing `django_seeding-1.1.2/django_seeding.egg-info/SOURCES.txt` & `django_seeding-1.2.1/django_seeding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_seeding-1.1.2/pyproject.toml` & `django_seeding-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'django-seeding'
-version = '1.1.2'
+version = '1.2.1'
 description = 'Simple Django Package that helps developer to seed data from files and codes into the database automatically'
 readme = "README.md"
 authors = [
   { name="Suliman Awad", email="sulimanawadstudy@gmail.com" },
 ]
 classifiers = [
     "Programming Language :: Python",
```

