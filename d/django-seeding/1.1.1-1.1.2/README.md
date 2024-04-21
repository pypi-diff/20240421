# Comparing `tmp/django_seeding-1.1.1.tar.gz` & `tmp/django_seeding-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_seeding-1.1.1.tar", last modified: Sun Apr 21 01:10:33 2024, max compression
+gzip compressed data, was "django_seeding-1.1.2.tar", last modified: Sun Apr 21 01:33:26 2024, max compression
```

## Comparing `django_seeding-1.1.1.tar` & `django_seeding-1.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:33.797656 django_seeding-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 01:10:29.000000 django_seeding-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17689 2024-04-21 01:10:33.797656 django_seeding-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17003 2024-04-21 01:10:29.000000 django_seeding-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:33.793656 django_seeding-1.1.1/django_seeding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/casting_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:33.793656 django_seeding-1.1.1/django_seeding/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:33.797656 django_seeding-1.1.1/django_seeding/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/management/commands/runserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/management/commands/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:33.797656 django_seeding-1.1.1/django_seeding/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/seeder_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/seeders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:33.797656 django_seeding-1.1.1/django_seeding.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17689 2024-04-21 01:10:33.000000 django_seeding-1.1.1/django_seeding.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-21 01:10:33.000000 django_seeding-1.1.1/django_seeding.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 01:10:33.000000 django_seeding-1.1.1/django_seeding.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 01:10:33.000000 django_seeding-1.1.1/django_seeding.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-21 01:10:29.000000 django_seeding-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 01:10:33.797656 django_seeding-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-21 01:10:29.000000 django_seeding-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:26.818701 django_seeding-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 01:33:20.000000 django_seeding-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17689 2024-04-21 01:33:26.818701 django_seeding-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17003 2024-04-21 01:33:20.000000 django_seeding-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:26.814701 django_seeding-1.1.2/django_seeding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/casting_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:26.814701 django_seeding-1.1.2/django_seeding/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:26.818701 django_seeding-1.1.2/django_seeding/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/management/commands/runserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/management/commands/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:26.818701 django_seeding-1.1.2/django_seeding/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/seeder_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-04-21 01:33:20.000000 django_seeding-1.1.2/django_seeding/seeders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:33:26.818701 django_seeding-1.1.2/django_seeding.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17689 2024-04-21 01:33:26.000000 django_seeding-1.1.2/django_seeding.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-21 01:33:26.000000 django_seeding-1.1.2/django_seeding.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 01:33:26.000000 django_seeding-1.1.2/django_seeding.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 01:33:26.000000 django_seeding-1.1.2/django_seeding.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-21 01:33:20.000000 django_seeding-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 01:33:26.818701 django_seeding-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-21 01:33:20.000000 django_seeding-1.1.2/setup.py
```

### Comparing `django_seeding-1.1.1/LICENSE` & `django_seeding-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_seeding-1.1.1/PKG-INFO` & `django_seeding-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-seeding
-Version: 1.1.1
+Version: 1.1.2
 Summary: Simple Django Package that helps developer to seed data from files and codes into the database automatically
 Author-email: Suliman Awad <sulimanawadstudy@gmail.com>
 Project-URL: Source, https://github.com/suliman-99/django-seeding
 Project-URL: Contributors, https://github.com/suliman-99/django-seeding/graphs/contributors
 Project-URL: License, https://github.com/suliman-99/django-seeding/blob/main/LICENSE
 Project-URL: Issues, https://github.com/suliman-99/django-seeding/issues
 Classifier: Programming Language :: Python
```

### Comparing `django_seeding-1.1.1/README.md` & `django_seeding-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django_seeding-1.1.1/django_seeding/management/commands/runserver.py` & `django_seeding-1.1.2/django_seeding/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `django_seeding-1.1.1/django_seeding/seeder_registry.py` & `django_seeding-1.1.2/django_seeding/seeder_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,18 @@
     seeders = []
 
     @classmethod
     def register(cls, seeder):
         """ Method and decorator to register the seeder-class in the seeders list to be seeded when the server is run """
         if not issubclass(seeder, Seeder):
             raise TypeError('Only subclasses of Seeder class can be registered with SeederRegistry.register')
+        
+        if seeder().get_id() in [obj.get_id() for obj in cls.seeders]:
+            return
+        
         cls.seeders.append(seeder())
 
     @classmethod
     def import_all(cls):
         """ Method that import all `seeders.py` files in the installed apps to register them in the `SeederRegistry` class """
         for app_config in apps.get_app_configs():
             app_name = app_config.name
```

### Comparing `django_seeding-1.1.1/django_seeding/seeders.py` & `django_seeding-1.1.2/django_seeding/seeders.py`

 * *Files identical despite different names*

### Comparing `django_seeding-1.1.1/django_seeding.egg-info/PKG-INFO` & `django_seeding-1.1.2/django_seeding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-seeding
-Version: 1.1.1
+Version: 1.1.2
 Summary: Simple Django Package that helps developer to seed data from files and codes into the database automatically
 Author-email: Suliman Awad <sulimanawadstudy@gmail.com>
 Project-URL: Source, https://github.com/suliman-99/django-seeding
 Project-URL: Contributors, https://github.com/suliman-99/django-seeding/graphs/contributors
 Project-URL: License, https://github.com/suliman-99/django-seeding/blob/main/LICENSE
 Project-URL: Issues, https://github.com/suliman-99/django-seeding/issues
 Classifier: Programming Language :: Python
```

### Comparing `django_seeding-1.1.1/django_seeding.egg-info/SOURCES.txt` & `django_seeding-1.1.2/django_seeding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_seeding-1.1.1/pyproject.toml` & `django_seeding-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'django-seeding'
-version = '1.1.1'
+version = '1.1.2'
 description = 'Simple Django Package that helps developer to seed data from files and codes into the database automatically'
 readme = "README.md"
 authors = [
   { name="Suliman Awad", email="sulimanawadstudy@gmail.com" },
 ]
 classifiers = [
     "Programming Language :: Python",
```

