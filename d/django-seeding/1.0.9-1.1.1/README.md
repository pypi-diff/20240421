# Comparing `tmp/django-seeding-1.0.9.tar.gz` & `tmp/django_seeding-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-seeding-1.0.9.tar", last modified: Wed Oct 25 12:44:45 2023, max compression
+gzip compressed data, was "django_seeding-1.1.1.tar", last modified: Sun Apr 21 01:10:33 2024, max compression
```

## Comparing `django-seeding-1.0.9.tar` & `django_seeding-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-10-25 12:44:45.025859 django-seeding-1.0.9/
--rw-rw-rw-   0        0        0     1090 2023-10-24 17:13:48.000000 django-seeding-1.0.9/LICENSE
--rw-rw-rw-   0        0        0    17965 2023-10-25 12:44:45.025859 django-seeding-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0    17637 2023-10-25 12:44:27.000000 django-seeding-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-10-25 12:44:44.994099 django-seeding-1.0.9/django_seeding/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:34:12.000000 django-seeding-1.0.9/django_seeding/__init__.py
--rw-rw-rw-   0        0        0      160 2023-10-23 09:36:21.000000 django-seeding-1.0.9/django_seeding/admin.py
--rw-rw-rw-   0        0        0      307 2023-10-24 15:27:47.000000 django-seeding-1.0.9/django_seeding/apps.py
--rw-rw-rw-   0        0        0      421 2023-10-24 17:27:18.000000 django-seeding-1.0.9/django_seeding/asgi.py
--rw-rw-rw-   0        0        0      188 2023-10-23 09:36:29.000000 django-seeding-1.0.9/django_seeding/models.py
--rw-rw-rw-   0        0        0     3289 2023-10-24 16:18:02.000000 django-seeding-1.0.9/django_seeding/seeder_registry.py
--rw-rw-rw-   0        0        0    15208 2023-10-23 13:30:01.000000 django-seeding-1.0.9/django_seeding/seeders.py
--rw-rw-rw-   0        0        0     3368 2023-10-24 17:27:18.000000 django-seeding-1.0.9/django_seeding/settings.py
--rw-rw-rw-   0        0        0      792 2023-10-24 17:27:18.000000 django-seeding-1.0.9/django_seeding/urls.py
--rw-rw-rw-   0        0        0      421 2023-10-24 17:27:18.000000 django-seeding-1.0.9/django_seeding/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-10-25 12:44:45.025859 django-seeding-1.0.9/django_seeding.egg-info/
--rw-rw-rw-   0        0        0    17965 2023-10-25 12:44:44.000000 django-seeding-1.0.9/django_seeding.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2023-10-25 12:44:44.000000 django-seeding-1.0.9/django_seeding.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-25 12:44:44.000000 django-seeding-1.0.9/django_seeding.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-10-25 12:44:44.000000 django-seeding-1.0.9/django_seeding.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-10-25 12:44:44.000000 django-seeding-1.0.9/django_seeding.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-25 12:44:45.025859 django-seeding-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      489 2023-10-25 12:44:35.000000 django-seeding-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:33.797656 django_seeding-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 01:10:29.000000 django_seeding-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17689 2024-04-21 01:10:33.797656 django_seeding-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17003 2024-04-21 01:10:29.000000 django_seeding-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:33.793656 django_seeding-1.1.1/django_seeding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/casting_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:33.793656 django_seeding-1.1.1/django_seeding/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:33.797656 django_seeding-1.1.1/django_seeding/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/management/commands/runserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/management/commands/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:33.797656 django_seeding-1.1.1/django_seeding/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/seeder_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-04-21 01:10:29.000000 django_seeding-1.1.1/django_seeding/seeders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:10:33.797656 django_seeding-1.1.1/django_seeding.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17689 2024-04-21 01:10:33.000000 django_seeding-1.1.1/django_seeding.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-21 01:10:33.000000 django_seeding-1.1.1/django_seeding.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 01:10:33.000000 django_seeding-1.1.1/django_seeding.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 01:10:33.000000 django_seeding-1.1.1/django_seeding.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-21 01:10:29.000000 django_seeding-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 01:10:33.797656 django_seeding-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-21 01:10:29.000000 django_seeding-1.1.1/setup.py
```

### Comparing `django-seeding-1.0.9/LICENSE` & `django_seeding-1.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 suliman awad
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 suliman awad
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `django-seeding-1.0.9/PKG-INFO` & `django_seeding-1.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,647 +1,639 @@
-Metadata-Version: 2.1
-Name: django-seeding
-Version: 1.0.9
-Summary: Simple Django Package that helps developer to seed data from files and codes into the database automatically
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: django
-Requires-Dist: djangorestframework
-Requires-Dist: pandas
-
-<!-- 
-    Written By Suliman Awad
-    Email: sulimanawadstudy@gmail.com
-    Github: https://github.com/suliman-99
-    Linkedin: https://linkedin.com/in/suliman-awad-399a471b8
-    Facebook: https://www.facebook.com/suliman.awad.507
- -->
-[![repo-size][repo-size-shield]][repo-url]
-[![forks][forks-shield]][forks-url]
-[![stars][stars-shield]][stars-url]
-[![issues][issues-shield]][issues-url]
-[![contributors][contributors-shield]][contributors-url]
-[![pr][pr-shield]][contributing-url]
-[![hachtoberfest][hachtoberfest-shield]][hacktoberfest-url]
-[![license][license-shield]][license-url]
-
-
-<div align="center">
-<h3>Django Seeding</h3>
-</div>
-
-
-## Table of Contents
-
-- [Introduction](#introduction)
-- [Installation](#installation)
-- [Simple Example](#simple-example)
-- [Full Usage Documentation](#full-usage-documentation)
-    - [Seeders List](#seeders-list)
-    - [Attributes List](#attributes-list)
-    - [Run Methods](#run-methods)
-- [Full Examples](#full-examples)
-    - [CSVFileModelSeeder (Recommended)](#csvfilemodelseeder-recommended)
-    - [JSONFileModelSeeder (Recommended)](#jsonfilemodelseeder-recommended)
-    - [CSVFileSerializerSeeder](#csvfileserializerseeder)
-    - [JSONFileSerializerSeeder](#jsonfileserializerseeder)
-    - [EmptySeeder (Recommended)](#emptyseeder-recommended)
-    - [ModelSeeder (Recommended)](#modelseeder-recommended)
-    - [SerializerSeeder](#serializerseeder)
-    - [Seeder](#seeder)
-- [Contributing](#contributing)
-- [Contact](#contact)
-- [License](#license)
-
-
-## Introduction
-
-This package helps develpoers to `fill` the database with `real data` instead of filling it manually.
-
-Data can be presented as `CSV File` , `JSON File` or `in-code`.
-
-`Dependency-Injection` also available to inject your logic by specifying a `serializer_class` or writing your custom `seed` method.
-
-
-## Installation
-
-Installing using pip:
-
-```
-pip install django-seeding:
-```
-
-add `'django_seeding'` to your `INSTALLED_APPS` setting:
-
-```
-INSTALLED_APPS = [
-    ...
-    'django_seeding',
-]
-```
-
-
-## Simple Example
-
-Let's take a look at a quick example of using `CSVFileModelSeeder` seeder from `django-seeding` to build a simple seeder to insert data in the database.
-
-django_seeding_example/models.py:
-```
-from django.db import models
-
-
-class M1(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-django_seeding_example/seeders.py:
-```
-from django_seeding import seeders
-from django_seeding.seeder_registry import SeederRegistry 
-from django_seeding_example.models import M1
-
-@SeederRegistry.register
-class M1Seeder(seeders.CSVFileModelSeeder):
-    model = M1
-    csv_file_path = 'django_seeding_example/seeders_data/M1Seeder.csv'
-```
-
-django_seeding_example/seeders_data/M1Seeder.csv:
-```
-title,description
-t1,d1
-t2,d2
-```
-
-Now you just need to run this commande:
-
-```
-python manage.py seed
-```
-## Full Usage Documentation: 
-
-Now lets go deeper into the different Seeders types with its details:
-
-### Seeders List:
-- [CSVFileModelSeeder (Recommended)](#csvfilemodelseeder-recommended)
-- [JSONFileModelSeeder (Recommended)](#jsonfilemodelseeder-recommended)
-- [CSVFileSerializerSeeder](#csvfileserializerseeder)
-- [JSONFileSerializerSeeder](#jsonfileserializerseeder)
-- [EmptySeeder (Recommended)](#emptyseeder-recommended)
-- [ModelSeeder (Recommended)](#modelseeder-recommended)
-- [SerializerSeeder](#serializerseeder)
-- [Seeder](#seeder)
-
-### Attributes List
-
-#### In general there is a way to know how to deal with these seeders easily:
-
-Model..Seeder needs `model` class-attribute
-
-Serializer..Seeder needs `serializer_class` class-attribute
-
-CSVFile..Seeder needs `csv_file_path` class-attribute
-
-JSONFile..Seeder needs `json_file_path` class-attribute
-
-#### All seeders can takes these optional class-attributes:
-* `id: str` (So Recommended) 
-
-    This is what will be stored in the AppliedSeeder table to check if a seeder is already applied or not
-
-    It is recommended to set it as the seeder name
-
-    So, set it and don't change it because when the value is changed it will be considerd as a new seeder and it will be applied again even that the old seeder with the old name is applied
-
-    default value: `str(type(seeder))`
-
-
-
-* `priority: int|float` 
-
-    Seeders will be sorted depending on this attribute (lower-first)
-
-    default value: `float('inf')`
-
-
-
-
-
-* `just_debug: bool` 
-
-    This attribute specify if the seeder will be applied when the server is in the production-mode or not depending in the DEBUG variable in settings file
-
-    `DEBUG=False` & `just_debug=True` -> don't apply
-
-    `DEBUG=False` & `just_debug=False` -> apply
-
-    `DEBUG=True` & `just_debug=False` -> apply
-
-    `DEBUG=True` & `just_debug=True` -> apply
-
-    default value: `False`
-
-#### Notice:
-
-* `@SeederRegistry.register` is the decorator that register the seeder, so, if this decorator is not applied then the seeder will not be applied
-* Model seeders use bulk_create method, so, they are faster than Serializer seeders
-* CSV file reader is using pandas for a better performance and less bugs
-* Using Model seeders means the fields names must match the fields you have defined in your model
-* Using Serializer seeders means the fields names must match the fields you have defined in your serializer
-* you can define `get_` class-methods instead of class-attributes as below:
-    
-    ```
-    get_model
-    get_serializer_class
-    get_csv_file_path
-    get_json_file_path
-    get_id
-    get_priority
-    get_just_debug
-    ```
-
-
-### Run methods:
-
-* To seed with a manual command (Recommended):
-
-```
-python manage.py seed
-```
-
-
-* To seed with runserver manually just add "--seed" in runserver command:
-
-```
-python manage.py runserver --seed
-```
-
-
-* To seed on runserver automatically just set in your project settings:
-
-``` 
-SEEDING_ON_RUNSERVER = True
-``` 
-
-#### Notice: 
-* If you set `SEEDING_ON_RUNSERVER=True` in your settings file You can stop seeding in a runserver by using `--dont-seed` argument
-
-```
-python manage.py runserver --dont-seed
-```
-
-
-## Full Examples:
-
-
-Here we will go deeper in the seeders classes and its details
-
-
-#### CSVFileModelSeeder (Recommended):
-
-Fast `bulk_create` seeder
-
-notice that the titles in the `csv-file` have to match the fields name in the `model`
-
-models.py
-```
-class M1(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M1Seeder(seeders.CSVFileModelSeeder):
-    id = 'M1Seeder'
-    priopity = 1
-    model = M1
-    csv_file_path = 'django_seeding_example/seeders_data/M1Seeder.csv'
-```
-
-seeders_data/M1Seeder.csv
-```
-title,description
-t1,d1
-t2,d2
-```
-
-
-
-#### JSONFileModelSeeder (Recommended):
-
-Fast `bulk_create` seeder
-
-notice that the keys in the `json-file` have to match the fields name in the `model`
-
-models.py
-```
-class M2(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M2Seeder(seeders.JSONFileModelSeeder):
-    id = 'M2Seeder'
-    priopity = 2
-    model = M2
-    json_file_path = 'django_seeding_example/seeders_data/M2Seeder.json'
-```
-
-seeders_data/M2Seeder.json
-```
-[
-    {
-        "title": "json t1",
-        "description": "json d1"
-    },
-    {
-        "title": "json t2",
-        "description": "json d2"
-    }
-]
-```
-
-
-
-
-#### CSVFileSerializerSeeder:
-
-Slow one-by-one seeder
-
-notice that the titles in the `csv-file` have to match the fields name in the `serializer`
-
-<b> This seeder is used to inject a serializer to implement custom create logic </b>
-
-models.py
-```
-class M3(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-serializers.py
-```
-class M3Serializer(serializers.ModelSerializer):
-    class Meta:
-        model = M3
-        fields = ['title', 'description']
-
-    def create(self, validated_data):
-        validated_data['title'] = '__' + validated_data['title'] + '__'
-        validated_data['description'] = '__' + validated_data['description'] + '__'
-        return super().create(validated_data)
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M3Seeder(seeders.CSVFileSerializerSeeder):
-    id = 'M3Seeder'
-    priopity = 3
-    serializer_class = M3Serializer
-    csv_file_path = 'django_seeding_example/seeders_data/M3Seeder.csv'
-```
-
-seeders_data/M3Seeder.csv
-```
-title,description
-t1,d1
-t2,d2
-```
-
-
-
-
-#### JSONFileSerializerSeeder:
-
-Slow one-by-one seeder
-
-notice that the keys in the `json-file` have to match the fields name in the `serializer`
-
-<b> This seeder is used to inject a serializer to implement custom create logic </b>
-
-models.py
-```
-class M4(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-serializers.py
-```
-class M4Serializer(serializers.ModelSerializer):
-    class Meta:
-        model = M4
-        fields = ['title', 'description']
-
-    def create(self, validated_data):
-        validated_data['title'] = '__' + validated_data['title'] + '__'
-        validated_data['description'] = '__' + validated_data['description'] + '__'
-        return super().create(validated_data)
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M4Seeder(seeders.JSONFileSerializerSeeder):
-    id = 'M4Seeder'
-    priopity = 4
-    serializer_class = M4Serializer
-    json_file_path = 'django_seeding_example/seeders_data/M4Seeder.json'
-```
-
-seeders_data/M4Seeder.csv
-```
-[
-    {
-        "title": "json t1",
-        "description": "json d1"
-    },
-    {
-        "title": "json t2",
-        "description": "json d2"
-    }
-]
-```
-
-
-
-
-#### EmptySeeder (Recommended):
-
-Fast `bulk_create` seeder
-
-models.py
-```
-class M5(models.Model):
-    title = models.CharField(max_length=100, null=True)
-    description = models.TextField(null=True)
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M5Seeder(seeders.EmptySeeder):
-    id = 'M5Seeder'
-    priopity = 5
-    model = M5
-    records_count = 2
-```
-
-
-
-
-#### ModelSeeder (Recommended):
-
-Fast `bulk_create` seeder
-
-notice that the keys in the `data` class-attribute have to match the fields name in the `model`
-
-models.py
-```
-class M6(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M6Seeder(seeders.ModelSeeder):
-    id = 'M6Seeder'
-    priopity = 6
-    model = M6
-    data = [
-        {
-            "title": "in-code t1",
-            "description": "in-code d1"
-        },
-        {
-            "title": "in-code t2",
-            "description": "in-code d2"
-        },
-    ]
-```
-
-
-
-
-#### SerializerSeeder:
-
-Slow one-by-one seeder
-
-notice that the keys in the `data` class-attribute have to match the fields name in the `serializer`
-
-<b> This seeder is used to inject a serializer to implement custom create logic </b>
-
-models.py
-```
-class M7(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-serializer.py
-```
-class M7Serializer(serializers.ModelSerializer):
-    class Meta:
-        model = M7
-        fields = ['title', 'description']
-
-    def create(self, validated_data):
-        validated_data['title'] = '__' + validated_data['title'] + '__'
-        validated_data['description'] = '__' + validated_data['description'] + '__'
-        return super().create(validated_data)
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M7Seeder(seeders.SerializerSeeder):
-    id = 'M7Seeder'
-    priopity = 7
-    serializer_class = M7Serializer
-    data = [
-        {
-            "title": "in-code t1",
-            "description": "in-code d1"
-        },
-        {
-            "title": "in-code t2",
-            "description": "in-code d2"
-        },
-    ]
-```
-
-
-
-
-#### Seeder:
-
-Here you can write your logic as you want in the seed method
-
-models.py
-```
-class Post(models.Model):
-    content = models.TextField()
-
-
-class Comment(models.Model):
-    post = models.ForeignKey(Post, on_delete=models.CASCADE)
-    content = models.TextField()
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class CustomSeeder(seeders.Seeder):
-    id = 'CustomSeeder'
-    priopity = 8
-    
-    def seed(self):
-        post1 = Post.objects.create(content='post1')
-        post2 = Post.objects.create(content='post1')
-
-        comment1 = Comment.objects.create(post=post1, content='comment1')
-        comment2 = Comment.objects.create(post=post1, content='comment2')
-        comment3 = Comment.objects.create(post=post2, content='comment3')
-        comment4 = Comment.objects.create(post=post2, content='comment4')
-```
-
-
-
-
-
-
-## Contributing
-
-If you have suggestions for how Django Seeding could be improved, or want to report a bug, open an issue! We'd love all and any contributions.
-
-For more, check out the [Contributing Guide][contributing-url].
-
-
-## Contact
-
-Suliman Awad - [sulimanawadstudy@gmail.com][gmail-url] - [Linkedin][linkedin-account-url]
-
-Project Link: [https://github.com/suliman-99/django-seeding][repo-url]
-
-
-## License
-
-MIT License
-
-Copyright (c) 2023 Suliman Awad
-
-For more, check out the [License File][license-url].
-
-
-
-<!-- ------------------------------------ urls ------------------------------------ -->
-
-
-<!-- my urls -->
-[gmail-url]: mailto:sulimanawadstudy@gmail.com
-[linkedin-account-url]: https://linkedin.com/in/suliman-awad-399a471b8
-[facebook-account-url]: https://www.facebook.com/suliman.awad.507
-[codeforces-account-url]: https://codeforces.com/profile/Suliman_Awad
-[github-account-url]: https://github.com/suliman-99
-
-
-<!-- repo urls -->
-[repo-url]: https://github.com/suliman-99/django-seeding
-[contributors-url]: https://github.com/suliman-99/django-seeding/graphs/contributors
-[forks-url]: https://github.com/suliman-99/django-seeding/network/members
-[stars-url]: https://github.com/suliman-99/django-seeding/stargazers
-[issues-url]: https://github.com/suliman-99/django-seeding/issues
-[license-url]: ./LICENSE
-[contributing-url]: ./CONTRIBUTING.md
-[photo-url]: ./photo.png
-[demo-url]: https://github.com/suliman-99/django-seeding
-
-
-<!-- static urls -->
-[hacktoberfest-url]: https://hacktoberfest.com
-[python-url]: https://www.python.org
-[python-downloads-url]: https://www.python.org/downloads
-[django-url]: https://www.djangoproject.com
-[mysql-url]: https://www.mysql.com
-[postgresql-url]: https://www.postgresql.org
-[restful-api-url]: https://aws.amazon.com/what-is/restful-api/?nc1=h_ls
-[postman-url]: https://www.postman.com
-[git-url]: https://git-scm.com
-[git-downloads-url]: https://git-scm.com/downloads
-[github-url]: https://github.com
-[markdown-url]: https://en.wikipedia.org/wiki/Markdown
-[vscode-url]: https://code.visualstudio.com
-
-
-
-<!-- ------------------------------------ shields ------------------------------------ -->
-
-
-
-<!-- my shields -->
-[gmail-shield]: https://img.shields.io/badge/Gmail-sulimanawadstudy@gmail.com-blue?logo=gmail&style=flat-square
-[linkedin-shield]: https://img.shields.io/badge/LinkedIn-Suliman%20Awad-blue?logo=linkedin&logoColor=6688ee&style=flat-square
-[linkedin-shield2]: https://img.shields.io/badge/LinkedIn-black.svg?logo=linkedin&colorB=555&style=social
-[facebook-shield]: https://img.shields.io/badge/Facebook-Suliman%20Awad-blue?logo=Facebook&style=flat-square
-
-[codeforces-shield]: https://img.shields.io/badge/Suliman%20Awad-333333?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABMAAAAQCAYAAAD0xERiAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAAIOSURBVDhPpZHLa1NBFMa/O0naPG/E10Vb0pArunBha0C6cCVCVdwLImTnzoWIa1257J/h3+BGEN105053fRACai0Gkzbx3jt3POfMDEZss/GDjznz+s03M0G32zU4QZX4GrB6F35BeXsLw4/vXO9fKdcer9uPsXPqCnad97sP3MTxmgsr1UJXWU0yV5yg+cmMgcmddS7tPKmFhRJePFnH68075A28enoD9dqiTMpmb+YQfJ7Uxs027q0vIj5/iPjcGLeuF/Dw/mU76/d60Eyyi40Qa6fPiJfqDRlTzUaREiTklNangE5QK8ucAOz1yNpel9Wp1fF88B2PPm+Ln/W/4mo9pDczOZ1IMD2FyY6oOyWIlk0BQf5c05m0kmTIJxOpeUSnKaLRGMrQRqN/CZBoLiFB/EpOR7C/PoC51OjAGYGcJ8kEQLCcrihggsoegTDMgTxMIASgwoitLIwADJN0BOYxVs6p5HrU8TWPc9eZa9+feTObyl7TvlkmyfgwZ5dsFsIJ2ZxWGRpiACeSX9VHtNrC+Fr2Jx1oBuYhHgyq1c6AfpF+0P6iTdX/Zt8sOfhiV/IOcpnXkMaVMozAKL28H7XNJgrFSvQyKcXISssYjCJ8+BTizdYI1WoVZ9N9tFda6IQKy2qEC3tvUUwP8bNYQNBpo3IpxrTdQr+1hPc/DhD0ej0TRZGc+D8aDof4DQayYRrQETG1AAAAAElFTkSuQmCC&style=flat-square
-
-
-<!-- repo shields -->
-[repo-size-shield]: https://img.shields.io/github/repo-size/suliman-99/django-seeding.svg?label=Repo%20size&style=flat-square
-[forks-shield]: https://img.shields.io/github/forks/suliman-99/django-seeding.svg?&style=flat-square
-[stars-shield]: https://img.shields.io/github/stars/suliman-99/django-seeding.svg?&style=flat-square
-[issues-shield]: https://img.shields.io/github/issues/suliman-99/django-seeding.svg?&style=flat-square
-[contributors-shield]: https://img.shields.io/github/contributors/suliman-99/django-seeding.svg?&style=flat-square
-[pr-shield]: https://img.shields.io/badge/PR-Welcome-333333?color=0055bb&style=flat-square
-[hachtoberfest-shield]: https://img.shields.io/github/hacktoberfest/2022/suliman-99/django-seeding
-[license-shield]: https://img.shields.io/github/license/suliman-99/django-seeding.svg?&style=flat-square
-
+<!-- 
+    Written By Suliman Awad
+    Email: sulimanawadstudy@gmail.com
+    Github: https://github.com/suliman-99
+    Linkedin: https://linkedin.com/in/suliman-awad-399a471b8
+    Facebook: https://www.facebook.com/suliman.awad.507
+ -->
+[![repo-size][repo-size-shield]][repo-url]
+[![forks][forks-shield]][forks-url]
+[![stars][stars-shield]][stars-url]
+[![issues][issues-shield]][issues-url]
+[![contributors][contributors-shield]][contributors-url]
+[![pr][pr-shield]][contributing-url]
+[![hachtoberfest][hachtoberfest-shield]][hacktoberfest-url]
+[![license][license-shield]][license-url]
+
+
+<div align="center">
+<h3>Django Seeding</h3>
+</div>
+
+
+
+## Table of Contents
+
+- [Introduction](#introduction)
+- [Installation](#installation)
+- [Simple Example](#simple-example)
+- [Full Usage Documentation](#full-usage-documentation)
+    - [Seeders List](#seeders-list)
+    - [Attributes List](#attributes-list)
+    - [Run Methods](#run-methods)
+- [Full Examples](#full-examples)
+    - [CSVFileModelSeeder (Recommended)](#csvfilemodelseeder-recommended)
+    - [JSONFileModelSeeder (Recommended)](#jsonfilemodelseeder-recommended)
+    - [CSVFileSerializerSeeder](#csvfileserializerseeder)
+    - [JSONFileSerializerSeeder](#jsonfileserializerseeder)
+    - [EmptySeeder (Recommended)](#emptyseeder-recommended)
+    - [ModelSeeder (Recommended)](#modelseeder-recommended)
+    - [SerializerSeeder](#serializerseeder)
+    - [Seeder](#seeder)
+- [Contributing](#contributing)
+- [Contact](#contact)
+- [License](#license)
+
+
+## Introduction
+
+This package helps develpoers to `fill` the database with `real data` instead of filling it manually.
+
+Data can be presented as `CSV File` , `JSON File` or `in-code`.
+
+`Dependency-Injection` also available to inject your logic by specifying a `serializer_class` or writing your custom `seed` method.
+
+
+## Installation
+
+Installing using pip:
+
+```
+pip install django-seeding:
+```
+
+add `'django_seeding'` to your `INSTALLED_APPS` setting:
+
+```
+INSTALLED_APPS = [
+    ...
+    'django_seeding',
+]
+```
+
+
+## Simple Example
+
+Let's take a look at a quick example of using `CSVFileModelSeeder` seeder from `django-seeding` to build a simple seeder to insert data in the database.
+
+django_seeding_example/models.py:
+```
+from django.db import models
+
+
+class M1(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+django_seeding_example/seeders.py:
+```
+from django_seeding import seeders
+from django_seeding.seeder_registry import SeederRegistry 
+from django_seeding_example.models import M1
+
+@SeederRegistry.register
+class M1Seeder(seeders.CSVFileModelSeeder):
+    model = M1
+    csv_file_path = 'django_seeding_example/seeders_data/M1Seeder.csv'
+```
+
+django_seeding_example/seeders_data/M1Seeder.csv:
+```
+title,description
+t1,d1
+t2,d2
+```
+
+Now you just need to run this commande:
+
+```
+python manage.py seed
+```
+## Full Usage Documentation: 
+
+Now lets go deeper into the different Seeders types with its details:
+
+### Seeders List:
+- [CSVFileModelSeeder (Recommended)](#csvfilemodelseeder-recommended)
+- [JSONFileModelSeeder (Recommended)](#jsonfilemodelseeder-recommended)
+- [CSVFileSerializerSeeder](#csvfileserializerseeder)
+- [JSONFileSerializerSeeder](#jsonfileserializerseeder)
+- [EmptySeeder (Recommended)](#emptyseeder-recommended)
+- [ModelSeeder (Recommended)](#modelseeder-recommended)
+- [SerializerSeeder](#serializerseeder)
+- [Seeder](#seeder)
+
+### Attributes List
+
+#### In general there is a way to know how to deal with these seeders easily:
+
+Model..Seeder needs `model` class-attribute
+
+Serializer..Seeder needs `serializer_class` class-attribute
+
+CSVFile..Seeder needs `csv_file_path` class-attribute
+
+JSONFile..Seeder needs `json_file_path` class-attribute
+
+#### All seeders can takes these optional class-attributes:
+* `id: str` (So Recommended) 
+
+    This is what will be stored in the AppliedSeeder table to check if a seeder is already applied or not
+
+    It is recommended to set it as the seeder name
+
+    So, set it and don't change it because when the value is changed it will be considerd as a new seeder and it will be applied again even that the old seeder with the old name is applied
+
+    default value: `str(type(seeder))`
+
+
+
+* `priority: int|float` 
+
+    Seeders will be sorted depending on this attribute (lower-first)
+
+    default value: `float('inf')`
+
+
+
+
+
+* `just_debug: bool` 
+
+    This attribute specify if the seeder will be applied when the server is in the production-mode or not depending in the DEBUG variable in settings file
+
+    `DEBUG=False` & `just_debug=True` -> don't apply
+
+    `DEBUG=False` & `just_debug=False` -> apply
+
+    `DEBUG=True` & `just_debug=False` -> apply
+
+    `DEBUG=True` & `just_debug=True` -> apply
+
+    default value: `False`
+
+#### Notice:
+
+* `@SeederRegistry.register` is the decorator that register the seeder, so, if this decorator is not applied then the seeder will not be applied
+* Model seeders use bulk_create method, so, they are faster than Serializer seeders
+* CSV file reader is using pandas for a better performance and less bugs
+* Using Model seeders means the fields names must match the fields you have defined in your model
+* Using Serializer seeders means the fields names must match the fields you have defined in your serializer
+* you can define `get_` class-methods instead of class-attributes as below:
+    
+    ```
+    get_model
+    get_serializer_class
+    get_csv_file_path
+    get_json_file_path
+    get_id
+    get_priority
+    get_just_debug
+    ```
+
+
+### Run methods:
+
+* To seed with a manual command (Recommended):
+
+```
+python manage.py seed
+```
+
+
+* To seed with runserver manually just add "--seed" in runserver command:
+
+```
+python manage.py runserver --seed
+```
+
+
+* To seed on runserver automatically just set in your project settings:
+
+``` 
+SEEDING_ON_RUNSERVER = True
+``` 
+
+#### Notice: 
+* If you set `SEEDING_ON_RUNSERVER=True` in your settings file You can stop seeding in a runserver by using `--dont-seed` argument
+
+```
+python manage.py runserver --dont-seed
+```
+
+
+## Full Examples:
+
+
+Here we will go deeper in the seeders classes and its details
+
+
+#### CSVFileModelSeeder (Recommended):
+
+Fast `bulk_create` seeder
+
+notice that the titles in the `csv-file` have to match the fields name in the `model`
+
+models.py
+```
+class M1(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M1Seeder(seeders.CSVFileModelSeeder):
+    id = 'M1Seeder'
+    priopity = 1
+    model = M1
+    csv_file_path = 'django_seeding_example/seeders_data/M1Seeder.csv'
+```
+
+seeders_data/M1Seeder.csv
+```
+title,description
+t1,d1
+t2,d2
+```
+
+
+
+#### JSONFileModelSeeder (Recommended):
+
+Fast `bulk_create` seeder
+
+notice that the keys in the `json-file` have to match the fields name in the `model`
+
+models.py
+```
+class M2(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M2Seeder(seeders.JSONFileModelSeeder):
+    id = 'M2Seeder'
+    priopity = 2
+    model = M2
+    json_file_path = 'django_seeding_example/seeders_data/M2Seeder.json'
+```
+
+seeders_data/M2Seeder.json
+```
+[
+    {
+        "title": "json t1",
+        "description": "json d1"
+    },
+    {
+        "title": "json t2",
+        "description": "json d2"
+    }
+]
+```
+
+
+
+
+#### CSVFileSerializerSeeder:
+
+Slow one-by-one seeder
+
+notice that the titles in the `csv-file` have to match the fields name in the `serializer`
+
+<b> This seeder is used to inject a serializer to implement custom create logic </b>
+
+models.py
+```
+class M3(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+serializers.py
+```
+class M3Serializer(serializers.ModelSerializer):
+    class Meta:
+        model = M3
+        fields = ['title', 'description']
+
+    def create(self, validated_data):
+        validated_data['title'] = '__' + validated_data['title'] + '__'
+        validated_data['description'] = '__' + validated_data['description'] + '__'
+        return super().create(validated_data)
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M3Seeder(seeders.CSVFileSerializerSeeder):
+    id = 'M3Seeder'
+    priopity = 3
+    serializer_class = M3Serializer
+    csv_file_path = 'django_seeding_example/seeders_data/M3Seeder.csv'
+```
+
+seeders_data/M3Seeder.csv
+```
+title,description
+t1,d1
+t2,d2
+```
+
+
+
+
+#### JSONFileSerializerSeeder:
+
+Slow one-by-one seeder
+
+notice that the keys in the `json-file` have to match the fields name in the `serializer`
+
+<b> This seeder is used to inject a serializer to implement custom create logic </b>
+
+models.py
+```
+class M4(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+serializers.py
+```
+class M4Serializer(serializers.ModelSerializer):
+    class Meta:
+        model = M4
+        fields = ['title', 'description']
+
+    def create(self, validated_data):
+        validated_data['title'] = '__' + validated_data['title'] + '__'
+        validated_data['description'] = '__' + validated_data['description'] + '__'
+        return super().create(validated_data)
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M4Seeder(seeders.JSONFileSerializerSeeder):
+    id = 'M4Seeder'
+    priopity = 4
+    serializer_class = M4Serializer
+    json_file_path = 'django_seeding_example/seeders_data/M4Seeder.json'
+```
+
+seeders_data/M4Seeder.json
+```
+[
+    {
+        "title": "json t1",
+        "description": "json d1"
+    },
+    {
+        "title": "json t2",
+        "description": "json d2"
+    }
+]
+```
+
+
+
+
+#### EmptySeeder (Recommended):
+
+Fast `bulk_create` seeder
+
+models.py
+```
+class M5(models.Model):
+    title = models.CharField(max_length=100, null=True)
+    description = models.TextField(null=True)
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M5Seeder(seeders.EmptySeeder):
+    id = 'M5Seeder'
+    priopity = 5
+    model = M5
+    records_count = 2
+```
+
+
+
+
+#### ModelSeeder (Recommended):
+
+Fast `bulk_create` seeder
+
+notice that the keys in the `data` class-attribute have to match the fields name in the `model`
+
+models.py
+```
+class M6(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M6Seeder(seeders.ModelSeeder):
+    id = 'M6Seeder'
+    priopity = 6
+    model = M6
+    data = [
+        {
+            "title": "in-code t1",
+            "description": "in-code d1"
+        },
+        {
+            "title": "in-code t2",
+            "description": "in-code d2"
+        },
+    ]
+```
+
+
+
+
+#### SerializerSeeder:
+
+Slow one-by-one seeder
+
+notice that the keys in the `data` class-attribute have to match the fields name in the `serializer`
+
+<b> This seeder is used to inject a serializer to implement custom create logic </b>
+
+models.py
+```
+class M7(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+serializer.py
+```
+class M7Serializer(serializers.ModelSerializer):
+    class Meta:
+        model = M7
+        fields = ['title', 'description']
+
+    def create(self, validated_data):
+        validated_data['title'] = '__' + validated_data['title'] + '__'
+        validated_data['description'] = '__' + validated_data['description'] + '__'
+        return super().create(validated_data)
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M7Seeder(seeders.SerializerSeeder):
+    id = 'M7Seeder'
+    priopity = 7
+    serializer_class = M7Serializer
+    data = [
+        {
+            "title": "in-code t1",
+            "description": "in-code d1"
+        },
+        {
+            "title": "in-code t2",
+            "description": "in-code d2"
+        },
+    ]
+```
+
+
+
+
+#### Seeder:
+
+Here you can write your logic as you want in the seed method
+
+models.py
+```
+class Post(models.Model):
+    content = models.TextField()
+
+
+class Comment(models.Model):
+    post = models.ForeignKey(Post, on_delete=models.CASCADE)
+    content = models.TextField()
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class CustomSeeder(seeders.Seeder):
+    id = 'CustomSeeder'
+    priopity = 8
+    
+    def seed(self):
+        post1 = Post.objects.create(content='post1')
+        post2 = Post.objects.create(content='post1')
+
+        comment1 = Comment.objects.create(post=post1, content='comment1')
+        comment2 = Comment.objects.create(post=post1, content='comment2')
+        comment3 = Comment.objects.create(post=post2, content='comment3')
+        comment4 = Comment.objects.create(post=post2, content='comment4')
+```
+
+
+
+
+
+
+## Contributing
+
+If you have suggestions for how Django Seeding could be improved, or want to report a bug, open an issue! We'd love all and any contributions.
+
+For more, check out the [Contributing Guide][contributing-url].
+
+
+## Contact
+
+Suliman Awad - [sulimanawadstudy@gmail.com][gmail-url] - [Linkedin][linkedin-account-url]
+
+Project Link: [https://github.com/suliman-99/django-seeding][repo-url]
+
+
+## License
+
+MIT License
+
+Copyright (c) 2023 Suliman Awad
+
+For more, check out the [License File][license-url].
+
+
+<!-- ------------------------------------ urls ------------------------------------ -->
+
+
+
+<!-- my urls -->
+[gmail-url]: mailto:sulimanawadstudy@gmail.com
+[linkedin-account-url]: https://linkedin.com/in/suliman-awad-399a471b8
+[facebook-account-url]: https://www.facebook.com/suliman.awad.507
+[codeforces-account-url]: https://codeforces.com/profile/Suliman_Awad
+[github-account-url]: https://github.com/suliman-99
+
+
+<!-- repo urls -->
+[repo-url]: https://github.com/suliman-99/django-seeding
+[contributors-url]: https://github.com/suliman-99/django-seeding/graphs/contributors
+[forks-url]: https://github.com/suliman-99/django-seeding/network/members
+[stars-url]: https://github.com/suliman-99/django-seeding/stargazers
+[issues-url]: https://github.com/suliman-99/django-seeding/issues
+[license-url]: ./LICENSE
+[contributing-url]: ./CONTRIBUTING.md
+[photo-url]: ./photo.png
+[demo-url]: https://github.com/suliman-99/django-seeding
+
+
+<!-- static urls -->
+[hacktoberfest-url]: https://hacktoberfest.com
+[python-url]: https://www.python.org
+[python-downloads-url]: https://www.python.org/downloads
+[django-url]: https://www.djangoproject.com
+[mysql-url]: https://www.mysql.com
+[postgresql-url]: https://www.postgresql.org
+[restful-api-url]: https://aws.amazon.com/what-is/restful-api/?nc1=h_ls
+[postman-url]: https://www.postman.com
+[git-url]: https://git-scm.com
+[git-downloads-url]: https://git-scm.com/downloads
+[github-url]: https://github.com
+[markdown-url]: https://en.wikipedia.org/wiki/Markdown
+[vscode-url]: https://code.visualstudio.com
+
+
+
+<!-- ------------------------------------ shields ------------------------------------ -->
+
+
+
+<!-- my shields -->
+[gmail-shield]: https://img.shields.io/badge/Gmail-sulimanawadstudy@gmail.com-blue?logo=gmail&style=flat-square
+[linkedin-shield]: https://img.shields.io/badge/LinkedIn-Suliman%20Awad-blue?logo=linkedin&logoColor=6688ee&style=flat-square
+[linkedin-shield2]: https://img.shields.io/badge/LinkedIn-black.svg?logo=linkedin&colorB=555&style=social
+[facebook-shield]: https://img.shields.io/badge/Facebook-Suliman%20Awad-blue?logo=Facebook&style=flat-square
+
+[codeforces-shield]: https://img.shields.io/badge/Suliman%20Awad-333333?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABMAAAAQCAYAAAD0xERiAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAAIOSURBVDhPpZHLa1NBFMa/O0naPG/E10Vb0pArunBha0C6cCVCVdwLImTnzoWIa1257J/h3+BGEN105053fRACai0Gkzbx3jt3POfMDEZss/GDjznz+s03M0G32zU4QZX4GrB6F35BeXsLw4/vXO9fKdcer9uPsXPqCnad97sP3MTxmgsr1UJXWU0yV5yg+cmMgcmddS7tPKmFhRJePFnH68075A28enoD9dqiTMpmb+YQfJ7Uxs027q0vIj5/iPjcGLeuF/Dw/mU76/d60Eyyi40Qa6fPiJfqDRlTzUaREiTklNangE5QK8ucAOz1yNpel9Wp1fF88B2PPm+Ln/W/4mo9pDczOZ1IMD2FyY6oOyWIlk0BQf5c05m0kmTIJxOpeUSnKaLRGMrQRqN/CZBoLiFB/EpOR7C/PoC51OjAGYGcJ8kEQLCcrihggsoegTDMgTxMIASgwoitLIwADJN0BOYxVs6p5HrU8TWPc9eZa9+feTObyl7TvlkmyfgwZ5dsFsIJ2ZxWGRpiACeSX9VHtNrC+Fr2Jx1oBuYhHgyq1c6AfpF+0P6iTdX/Zt8sOfhiV/IOcpnXkMaVMozAKL28H7XNJgrFSvQyKcXISssYjCJ8+BTizdYI1WoVZ9N9tFda6IQKy2qEC3tvUUwP8bNYQNBpo3IpxrTdQr+1hPc/DhD0ej0TRZGc+D8aDof4DQayYRrQETG1AAAAAElFTkSuQmCC&style=flat-square
+
+
+<!-- repo shields -->
+[repo-size-shield]: https://img.shields.io/github/repo-size/suliman-99/django-seeding.svg?label=Repo%20size&style=flat-square
+[forks-shield]: https://img.shields.io/github/forks/suliman-99/django-seeding.svg?&style=flat-square
+[stars-shield]: https://img.shields.io/github/stars/suliman-99/django-seeding.svg?&style=flat-square
+[issues-shield]: https://img.shields.io/github/issues/suliman-99/django-seeding.svg?&style=flat-square
+[contributors-shield]: https://img.shields.io/github/contributors/suliman-99/django-seeding.svg?&style=flat-square
+[pr-shield]: https://img.shields.io/badge/PR-Welcome-333333?color=0055bb&style=flat-square
+[hachtoberfest-shield]: https://img.shields.io/github/hacktoberfest/2022/suliman-99/django-seeding
+[license-shield]: https://img.shields.io/github/license/suliman-99/django-seeding.svg?&style=flat-square
+
+
```

### Comparing `django-seeding-1.0.9/README.md` & `django_seeding-1.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,637 +1,653 @@
-<!-- 
-    Written By Suliman Awad
-    Email: sulimanawadstudy@gmail.com
-    Github: https://github.com/suliman-99
-    Linkedin: https://linkedin.com/in/suliman-awad-399a471b8
-    Facebook: https://www.facebook.com/suliman.awad.507
- -->
-[![repo-size][repo-size-shield]][repo-url]
-[![forks][forks-shield]][forks-url]
-[![stars][stars-shield]][stars-url]
-[![issues][issues-shield]][issues-url]
-[![contributors][contributors-shield]][contributors-url]
-[![pr][pr-shield]][contributing-url]
-[![hachtoberfest][hachtoberfest-shield]][hacktoberfest-url]
-[![license][license-shield]][license-url]
-
-
-<div align="center">
-<h3>Django Seeding</h3>
-</div>
-
-
-## Table of Contents
-
-- [Introduction](#introduction)
-- [Installation](#installation)
-- [Simple Example](#simple-example)
-- [Full Usage Documentation](#full-usage-documentation)
-    - [Seeders List](#seeders-list)
-    - [Attributes List](#attributes-list)
-    - [Run Methods](#run-methods)
-- [Full Examples](#full-examples)
-    - [CSVFileModelSeeder (Recommended)](#csvfilemodelseeder-recommended)
-    - [JSONFileModelSeeder (Recommended)](#jsonfilemodelseeder-recommended)
-    - [CSVFileSerializerSeeder](#csvfileserializerseeder)
-    - [JSONFileSerializerSeeder](#jsonfileserializerseeder)
-    - [EmptySeeder (Recommended)](#emptyseeder-recommended)
-    - [ModelSeeder (Recommended)](#modelseeder-recommended)
-    - [SerializerSeeder](#serializerseeder)
-    - [Seeder](#seeder)
-- [Contributing](#contributing)
-- [Contact](#contact)
-- [License](#license)
-
-
-## Introduction
-
-This package helps develpoers to `fill` the database with `real data` instead of filling it manually.
-
-Data can be presented as `CSV File` , `JSON File` or `in-code`.
-
-`Dependency-Injection` also available to inject your logic by specifying a `serializer_class` or writing your custom `seed` method.
-
-
-## Installation
-
-Installing using pip:
-
-```
-pip install django-seeding:
-```
-
-add `'django_seeding'` to your `INSTALLED_APPS` setting:
-
-```
-INSTALLED_APPS = [
-    ...
-    'django_seeding',
-]
-```
-
-
-## Simple Example
-
-Let's take a look at a quick example of using `CSVFileModelSeeder` seeder from `django-seeding` to build a simple seeder to insert data in the database.
-
-django_seeding_example/models.py:
-```
-from django.db import models
-
-
-class M1(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-django_seeding_example/seeders.py:
-```
-from django_seeding import seeders
-from django_seeding.seeder_registry import SeederRegistry 
-from django_seeding_example.models import M1
-
-@SeederRegistry.register
-class M1Seeder(seeders.CSVFileModelSeeder):
-    model = M1
-    csv_file_path = 'django_seeding_example/seeders_data/M1Seeder.csv'
-```
-
-django_seeding_example/seeders_data/M1Seeder.csv:
-```
-title,description
-t1,d1
-t2,d2
-```
-
-Now you just need to run this commande:
-
-```
-python manage.py seed
-```
-## Full Usage Documentation: 
-
-Now lets go deeper into the different Seeders types with its details:
-
-### Seeders List:
-- [CSVFileModelSeeder (Recommended)](#csvfilemodelseeder-recommended)
-- [JSONFileModelSeeder (Recommended)](#jsonfilemodelseeder-recommended)
-- [CSVFileSerializerSeeder](#csvfileserializerseeder)
-- [JSONFileSerializerSeeder](#jsonfileserializerseeder)
-- [EmptySeeder (Recommended)](#emptyseeder-recommended)
-- [ModelSeeder (Recommended)](#modelseeder-recommended)
-- [SerializerSeeder](#serializerseeder)
-- [Seeder](#seeder)
-
-### Attributes List
-
-#### In general there is a way to know how to deal with these seeders easily:
-
-Model..Seeder needs `model` class-attribute
-
-Serializer..Seeder needs `serializer_class` class-attribute
-
-CSVFile..Seeder needs `csv_file_path` class-attribute
-
-JSONFile..Seeder needs `json_file_path` class-attribute
-
-#### All seeders can takes these optional class-attributes:
-* `id: str` (So Recommended) 
-
-    This is what will be stored in the AppliedSeeder table to check if a seeder is already applied or not
-
-    It is recommended to set it as the seeder name
-
-    So, set it and don't change it because when the value is changed it will be considerd as a new seeder and it will be applied again even that the old seeder with the old name is applied
-
-    default value: `str(type(seeder))`
-
-
-
-* `priority: int|float` 
-
-    Seeders will be sorted depending on this attribute (lower-first)
-
-    default value: `float('inf')`
-
-
-
-
-
-* `just_debug: bool` 
-
-    This attribute specify if the seeder will be applied when the server is in the production-mode or not depending in the DEBUG variable in settings file
-
-    `DEBUG=False` & `just_debug=True` -> don't apply
-
-    `DEBUG=False` & `just_debug=False` -> apply
-
-    `DEBUG=True` & `just_debug=False` -> apply
-
-    `DEBUG=True` & `just_debug=True` -> apply
-
-    default value: `False`
-
-#### Notice:
-
-* `@SeederRegistry.register` is the decorator that register the seeder, so, if this decorator is not applied then the seeder will not be applied
-* Model seeders use bulk_create method, so, they are faster than Serializer seeders
-* CSV file reader is using pandas for a better performance and less bugs
-* Using Model seeders means the fields names must match the fields you have defined in your model
-* Using Serializer seeders means the fields names must match the fields you have defined in your serializer
-* you can define `get_` class-methods instead of class-attributes as below:
-    
-    ```
-    get_model
-    get_serializer_class
-    get_csv_file_path
-    get_json_file_path
-    get_id
-    get_priority
-    get_just_debug
-    ```
-
-
-### Run methods:
-
-* To seed with a manual command (Recommended):
-
-```
-python manage.py seed
-```
-
-
-* To seed with runserver manually just add "--seed" in runserver command:
-
-```
-python manage.py runserver --seed
-```
-
-
-* To seed on runserver automatically just set in your project settings:
-
-``` 
-SEEDING_ON_RUNSERVER = True
-``` 
-
-#### Notice: 
-* If you set `SEEDING_ON_RUNSERVER=True` in your settings file You can stop seeding in a runserver by using `--dont-seed` argument
-
-```
-python manage.py runserver --dont-seed
-```
-
-
-## Full Examples:
-
-
-Here we will go deeper in the seeders classes and its details
-
-
-#### CSVFileModelSeeder (Recommended):
-
-Fast `bulk_create` seeder
-
-notice that the titles in the `csv-file` have to match the fields name in the `model`
-
-models.py
-```
-class M1(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M1Seeder(seeders.CSVFileModelSeeder):
-    id = 'M1Seeder'
-    priopity = 1
-    model = M1
-    csv_file_path = 'django_seeding_example/seeders_data/M1Seeder.csv'
-```
-
-seeders_data/M1Seeder.csv
-```
-title,description
-t1,d1
-t2,d2
-```
-
-
-
-#### JSONFileModelSeeder (Recommended):
-
-Fast `bulk_create` seeder
-
-notice that the keys in the `json-file` have to match the fields name in the `model`
-
-models.py
-```
-class M2(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M2Seeder(seeders.JSONFileModelSeeder):
-    id = 'M2Seeder'
-    priopity = 2
-    model = M2
-    json_file_path = 'django_seeding_example/seeders_data/M2Seeder.json'
-```
-
-seeders_data/M2Seeder.json
-```
-[
-    {
-        "title": "json t1",
-        "description": "json d1"
-    },
-    {
-        "title": "json t2",
-        "description": "json d2"
-    }
-]
-```
-
-
-
-
-#### CSVFileSerializerSeeder:
-
-Slow one-by-one seeder
-
-notice that the titles in the `csv-file` have to match the fields name in the `serializer`
-
-<b> This seeder is used to inject a serializer to implement custom create logic </b>
-
-models.py
-```
-class M3(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-serializers.py
-```
-class M3Serializer(serializers.ModelSerializer):
-    class Meta:
-        model = M3
-        fields = ['title', 'description']
-
-    def create(self, validated_data):
-        validated_data['title'] = '__' + validated_data['title'] + '__'
-        validated_data['description'] = '__' + validated_data['description'] + '__'
-        return super().create(validated_data)
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M3Seeder(seeders.CSVFileSerializerSeeder):
-    id = 'M3Seeder'
-    priopity = 3
-    serializer_class = M3Serializer
-    csv_file_path = 'django_seeding_example/seeders_data/M3Seeder.csv'
-```
-
-seeders_data/M3Seeder.csv
-```
-title,description
-t1,d1
-t2,d2
-```
-
-
-
-
-#### JSONFileSerializerSeeder:
-
-Slow one-by-one seeder
-
-notice that the keys in the `json-file` have to match the fields name in the `serializer`
-
-<b> This seeder is used to inject a serializer to implement custom create logic </b>
-
-models.py
-```
-class M4(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-serializers.py
-```
-class M4Serializer(serializers.ModelSerializer):
-    class Meta:
-        model = M4
-        fields = ['title', 'description']
-
-    def create(self, validated_data):
-        validated_data['title'] = '__' + validated_data['title'] + '__'
-        validated_data['description'] = '__' + validated_data['description'] + '__'
-        return super().create(validated_data)
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M4Seeder(seeders.JSONFileSerializerSeeder):
-    id = 'M4Seeder'
-    priopity = 4
-    serializer_class = M4Serializer
-    json_file_path = 'django_seeding_example/seeders_data/M4Seeder.json'
-```
-
-seeders_data/M4Seeder.csv
-```
-[
-    {
-        "title": "json t1",
-        "description": "json d1"
-    },
-    {
-        "title": "json t2",
-        "description": "json d2"
-    }
-]
-```
-
-
-
-
-#### EmptySeeder (Recommended):
-
-Fast `bulk_create` seeder
-
-models.py
-```
-class M5(models.Model):
-    title = models.CharField(max_length=100, null=True)
-    description = models.TextField(null=True)
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M5Seeder(seeders.EmptySeeder):
-    id = 'M5Seeder'
-    priopity = 5
-    model = M5
-    records_count = 2
-```
-
-
-
-
-#### ModelSeeder (Recommended):
-
-Fast `bulk_create` seeder
-
-notice that the keys in the `data` class-attribute have to match the fields name in the `model`
-
-models.py
-```
-class M6(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M6Seeder(seeders.ModelSeeder):
-    id = 'M6Seeder'
-    priopity = 6
-    model = M6
-    data = [
-        {
-            "title": "in-code t1",
-            "description": "in-code d1"
-        },
-        {
-            "title": "in-code t2",
-            "description": "in-code d2"
-        },
-    ]
-```
-
-
-
-
-#### SerializerSeeder:
-
-Slow one-by-one seeder
-
-notice that the keys in the `data` class-attribute have to match the fields name in the `serializer`
-
-<b> This seeder is used to inject a serializer to implement custom create logic </b>
-
-models.py
-```
-class M7(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-serializer.py
-```
-class M7Serializer(serializers.ModelSerializer):
-    class Meta:
-        model = M7
-        fields = ['title', 'description']
-
-    def create(self, validated_data):
-        validated_data['title'] = '__' + validated_data['title'] + '__'
-        validated_data['description'] = '__' + validated_data['description'] + '__'
-        return super().create(validated_data)
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M7Seeder(seeders.SerializerSeeder):
-    id = 'M7Seeder'
-    priopity = 7
-    serializer_class = M7Serializer
-    data = [
-        {
-            "title": "in-code t1",
-            "description": "in-code d1"
-        },
-        {
-            "title": "in-code t2",
-            "description": "in-code d2"
-        },
-    ]
-```
-
-
-
-
-#### Seeder:
-
-Here you can write your logic as you want in the seed method
-
-models.py
-```
-class Post(models.Model):
-    content = models.TextField()
-
-
-class Comment(models.Model):
-    post = models.ForeignKey(Post, on_delete=models.CASCADE)
-    content = models.TextField()
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class CustomSeeder(seeders.Seeder):
-    id = 'CustomSeeder'
-    priopity = 8
-    
-    def seed(self):
-        post1 = Post.objects.create(content='post1')
-        post2 = Post.objects.create(content='post1')
-
-        comment1 = Comment.objects.create(post=post1, content='comment1')
-        comment2 = Comment.objects.create(post=post1, content='comment2')
-        comment3 = Comment.objects.create(post=post2, content='comment3')
-        comment4 = Comment.objects.create(post=post2, content='comment4')
-```
-
-
-
-
-
-
-## Contributing
-
-If you have suggestions for how Django Seeding could be improved, or want to report a bug, open an issue! We'd love all and any contributions.
-
-For more, check out the [Contributing Guide][contributing-url].
-
-
-## Contact
-
-Suliman Awad - [sulimanawadstudy@gmail.com][gmail-url] - [Linkedin][linkedin-account-url]
-
-Project Link: [https://github.com/suliman-99/django-seeding][repo-url]
-
-
-## License
-
-MIT License
-
-Copyright (c) 2023 Suliman Awad
-
-For more, check out the [License File][license-url].
-
-
-
-<!-- ------------------------------------ urls ------------------------------------ -->
-
-
-<!-- my urls -->
-[gmail-url]: mailto:sulimanawadstudy@gmail.com
-[linkedin-account-url]: https://linkedin.com/in/suliman-awad-399a471b8
-[facebook-account-url]: https://www.facebook.com/suliman.awad.507
-[codeforces-account-url]: https://codeforces.com/profile/Suliman_Awad
-[github-account-url]: https://github.com/suliman-99
-
-
-<!-- repo urls -->
-[repo-url]: https://github.com/suliman-99/django-seeding
-[contributors-url]: https://github.com/suliman-99/django-seeding/graphs/contributors
-[forks-url]: https://github.com/suliman-99/django-seeding/network/members
-[stars-url]: https://github.com/suliman-99/django-seeding/stargazers
-[issues-url]: https://github.com/suliman-99/django-seeding/issues
-[license-url]: ./LICENSE
-[contributing-url]: ./CONTRIBUTING.md
-[photo-url]: ./photo.png
-[demo-url]: https://github.com/suliman-99/django-seeding
-
-
-<!-- static urls -->
-[hacktoberfest-url]: https://hacktoberfest.com
-[python-url]: https://www.python.org
-[python-downloads-url]: https://www.python.org/downloads
-[django-url]: https://www.djangoproject.com
-[mysql-url]: https://www.mysql.com
-[postgresql-url]: https://www.postgresql.org
-[restful-api-url]: https://aws.amazon.com/what-is/restful-api/?nc1=h_ls
-[postman-url]: https://www.postman.com
-[git-url]: https://git-scm.com
-[git-downloads-url]: https://git-scm.com/downloads
-[github-url]: https://github.com
-[markdown-url]: https://en.wikipedia.org/wiki/Markdown
-[vscode-url]: https://code.visualstudio.com
-
-
-
-<!-- ------------------------------------ shields ------------------------------------ -->
-
-
-
-<!-- my shields -->
-[gmail-shield]: https://img.shields.io/badge/Gmail-sulimanawadstudy@gmail.com-blue?logo=gmail&style=flat-square
-[linkedin-shield]: https://img.shields.io/badge/LinkedIn-Suliman%20Awad-blue?logo=linkedin&logoColor=6688ee&style=flat-square
-[linkedin-shield2]: https://img.shields.io/badge/LinkedIn-black.svg?logo=linkedin&colorB=555&style=social
-[facebook-shield]: https://img.shields.io/badge/Facebook-Suliman%20Awad-blue?logo=Facebook&style=flat-square
-
-[codeforces-shield]: https://img.shields.io/badge/Suliman%20Awad-333333?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABMAAAAQCAYAAAD0xERiAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAAIOSURBVDhPpZHLa1NBFMa/O0naPG/E10Vb0pArunBha0C6cCVCVdwLImTnzoWIa1257J/h3+BGEN105053fRACai0Gkzbx3jt3POfMDEZss/GDjznz+s03M0G32zU4QZX4GrB6F35BeXsLw4/vXO9fKdcer9uPsXPqCnad97sP3MTxmgsr1UJXWU0yV5yg+cmMgcmddS7tPKmFhRJePFnH68075A28enoD9dqiTMpmb+YQfJ7Uxs027q0vIj5/iPjcGLeuF/Dw/mU76/d60Eyyi40Qa6fPiJfqDRlTzUaREiTklNangE5QK8ucAOz1yNpel9Wp1fF88B2PPm+Ln/W/4mo9pDczOZ1IMD2FyY6oOyWIlk0BQf5c05m0kmTIJxOpeUSnKaLRGMrQRqN/CZBoLiFB/EpOR7C/PoC51OjAGYGcJ8kEQLCcrihggsoegTDMgTxMIASgwoitLIwADJN0BOYxVs6p5HrU8TWPc9eZa9+feTObyl7TvlkmyfgwZ5dsFsIJ2ZxWGRpiACeSX9VHtNrC+Fr2Jx1oBuYhHgyq1c6AfpF+0P6iTdX/Zt8sOfhiV/IOcpnXkMaVMozAKL28H7XNJgrFSvQyKcXISssYjCJ8+BTizdYI1WoVZ9N9tFda6IQKy2qEC3tvUUwP8bNYQNBpo3IpxrTdQr+1hPc/DhD0ej0TRZGc+D8aDof4DQayYRrQETG1AAAAAElFTkSuQmCC&style=flat-square
-
-
-<!-- repo shields -->
-[repo-size-shield]: https://img.shields.io/github/repo-size/suliman-99/django-seeding.svg?label=Repo%20size&style=flat-square
-[forks-shield]: https://img.shields.io/github/forks/suliman-99/django-seeding.svg?&style=flat-square
-[stars-shield]: https://img.shields.io/github/stars/suliman-99/django-seeding.svg?&style=flat-square
-[issues-shield]: https://img.shields.io/github/issues/suliman-99/django-seeding.svg?&style=flat-square
-[contributors-shield]: https://img.shields.io/github/contributors/suliman-99/django-seeding.svg?&style=flat-square
-[pr-shield]: https://img.shields.io/badge/PR-Welcome-333333?color=0055bb&style=flat-square
-[hachtoberfest-shield]: https://img.shields.io/github/hacktoberfest/2022/suliman-99/django-seeding
-[license-shield]: https://img.shields.io/github/license/suliman-99/django-seeding.svg?&style=flat-square
-
+Metadata-Version: 2.1
+Name: django-seeding
+Version: 1.1.1
+Summary: Simple Django Package that helps developer to seed data from files and codes into the database automatically
+Author-email: Suliman Awad <sulimanawadstudy@gmail.com>
+Project-URL: Source, https://github.com/suliman-99/django-seeding
+Project-URL: Contributors, https://github.com/suliman-99/django-seeding/graphs/contributors
+Project-URL: License, https://github.com/suliman-99/django-seeding/blob/main/LICENSE
+Project-URL: Issues, https://github.com/suliman-99/django-seeding/issues
+Classifier: Programming Language :: Python
+Classifier: Framework :: Django
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<!-- 
+    Written By Suliman Awad
+    Email: sulimanawadstudy@gmail.com
+    Github: https://github.com/suliman-99
+    Linkedin: https://linkedin.com/in/suliman-awad-399a471b8
+    Facebook: https://www.facebook.com/suliman.awad.507
+ -->
+[![repo-size][repo-size-shield]][repo-url]
+[![forks][forks-shield]][forks-url]
+[![stars][stars-shield]][stars-url]
+[![issues][issues-shield]][issues-url]
+[![contributors][contributors-shield]][contributors-url]
+[![pr][pr-shield]][contributing-url]
+[![hachtoberfest][hachtoberfest-shield]][hacktoberfest-url]
+[![license][license-shield]][license-url]
+
+
+<div align="center">
+<h3>Django Seeding</h3>
+</div>
+
+
+
+## Table of Contents
+
+- [Introduction](#introduction)
+- [Installation](#installation)
+- [Simple Example](#simple-example)
+- [Full Usage Documentation](#full-usage-documentation)
+    - [Seeders List](#seeders-list)
+    - [Attributes List](#attributes-list)
+    - [Run Methods](#run-methods)
+- [Full Examples](#full-examples)
+    - [CSVFileModelSeeder (Recommended)](#csvfilemodelseeder-recommended)
+    - [JSONFileModelSeeder (Recommended)](#jsonfilemodelseeder-recommended)
+    - [CSVFileSerializerSeeder](#csvfileserializerseeder)
+    - [JSONFileSerializerSeeder](#jsonfileserializerseeder)
+    - [EmptySeeder (Recommended)](#emptyseeder-recommended)
+    - [ModelSeeder (Recommended)](#modelseeder-recommended)
+    - [SerializerSeeder](#serializerseeder)
+    - [Seeder](#seeder)
+- [Contributing](#contributing)
+- [Contact](#contact)
+- [License](#license)
+
+
+## Introduction
+
+This package helps develpoers to `fill` the database with `real data` instead of filling it manually.
+
+Data can be presented as `CSV File` , `JSON File` or `in-code`.
+
+`Dependency-Injection` also available to inject your logic by specifying a `serializer_class` or writing your custom `seed` method.
+
+
+## Installation
+
+Installing using pip:
+
+```
+pip install django-seeding:
+```
+
+add `'django_seeding'` to your `INSTALLED_APPS` setting:
+
+```
+INSTALLED_APPS = [
+    ...
+    'django_seeding',
+]
+```
+
+
+## Simple Example
+
+Let's take a look at a quick example of using `CSVFileModelSeeder` seeder from `django-seeding` to build a simple seeder to insert data in the database.
+
+django_seeding_example/models.py:
+```
+from django.db import models
+
+
+class M1(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+django_seeding_example/seeders.py:
+```
+from django_seeding import seeders
+from django_seeding.seeder_registry import SeederRegistry 
+from django_seeding_example.models import M1
+
+@SeederRegistry.register
+class M1Seeder(seeders.CSVFileModelSeeder):
+    model = M1
+    csv_file_path = 'django_seeding_example/seeders_data/M1Seeder.csv'
+```
+
+django_seeding_example/seeders_data/M1Seeder.csv:
+```
+title,description
+t1,d1
+t2,d2
+```
+
+Now you just need to run this commande:
+
+```
+python manage.py seed
+```
+## Full Usage Documentation: 
+
+Now lets go deeper into the different Seeders types with its details:
+
+### Seeders List:
+- [CSVFileModelSeeder (Recommended)](#csvfilemodelseeder-recommended)
+- [JSONFileModelSeeder (Recommended)](#jsonfilemodelseeder-recommended)
+- [CSVFileSerializerSeeder](#csvfileserializerseeder)
+- [JSONFileSerializerSeeder](#jsonfileserializerseeder)
+- [EmptySeeder (Recommended)](#emptyseeder-recommended)
+- [ModelSeeder (Recommended)](#modelseeder-recommended)
+- [SerializerSeeder](#serializerseeder)
+- [Seeder](#seeder)
+
+### Attributes List
+
+#### In general there is a way to know how to deal with these seeders easily:
+
+Model..Seeder needs `model` class-attribute
+
+Serializer..Seeder needs `serializer_class` class-attribute
+
+CSVFile..Seeder needs `csv_file_path` class-attribute
+
+JSONFile..Seeder needs `json_file_path` class-attribute
+
+#### All seeders can takes these optional class-attributes:
+* `id: str` (So Recommended) 
+
+    This is what will be stored in the AppliedSeeder table to check if a seeder is already applied or not
+
+    It is recommended to set it as the seeder name
+
+    So, set it and don't change it because when the value is changed it will be considerd as a new seeder and it will be applied again even that the old seeder with the old name is applied
+
+    default value: `str(type(seeder))`
+
+
+
+* `priority: int|float` 
+
+    Seeders will be sorted depending on this attribute (lower-first)
+
+    default value: `float('inf')`
+
+
+
+
+
+* `just_debug: bool` 
+
+    This attribute specify if the seeder will be applied when the server is in the production-mode or not depending in the DEBUG variable in settings file
+
+    `DEBUG=False` & `just_debug=True` -> don't apply
+
+    `DEBUG=False` & `just_debug=False` -> apply
+
+    `DEBUG=True` & `just_debug=False` -> apply
+
+    `DEBUG=True` & `just_debug=True` -> apply
+
+    default value: `False`
+
+#### Notice:
+
+* `@SeederRegistry.register` is the decorator that register the seeder, so, if this decorator is not applied then the seeder will not be applied
+* Model seeders use bulk_create method, so, they are faster than Serializer seeders
+* CSV file reader is using pandas for a better performance and less bugs
+* Using Model seeders means the fields names must match the fields you have defined in your model
+* Using Serializer seeders means the fields names must match the fields you have defined in your serializer
+* you can define `get_` class-methods instead of class-attributes as below:
+    
+    ```
+    get_model
+    get_serializer_class
+    get_csv_file_path
+    get_json_file_path
+    get_id
+    get_priority
+    get_just_debug
+    ```
+
+
+### Run methods:
+
+* To seed with a manual command (Recommended):
+
+```
+python manage.py seed
+```
+
+
+* To seed with runserver manually just add "--seed" in runserver command:
+
+```
+python manage.py runserver --seed
+```
+
+
+* To seed on runserver automatically just set in your project settings:
+
+``` 
+SEEDING_ON_RUNSERVER = True
+``` 
+
+#### Notice: 
+* If you set `SEEDING_ON_RUNSERVER=True` in your settings file You can stop seeding in a runserver by using `--dont-seed` argument
+
+```
+python manage.py runserver --dont-seed
+```
+
+
+## Full Examples:
+
+
+Here we will go deeper in the seeders classes and its details
+
+
+#### CSVFileModelSeeder (Recommended):
+
+Fast `bulk_create` seeder
+
+notice that the titles in the `csv-file` have to match the fields name in the `model`
+
+models.py
+```
+class M1(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M1Seeder(seeders.CSVFileModelSeeder):
+    id = 'M1Seeder'
+    priopity = 1
+    model = M1
+    csv_file_path = 'django_seeding_example/seeders_data/M1Seeder.csv'
+```
+
+seeders_data/M1Seeder.csv
+```
+title,description
+t1,d1
+t2,d2
+```
+
+
+
+#### JSONFileModelSeeder (Recommended):
+
+Fast `bulk_create` seeder
+
+notice that the keys in the `json-file` have to match the fields name in the `model`
+
+models.py
+```
+class M2(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M2Seeder(seeders.JSONFileModelSeeder):
+    id = 'M2Seeder'
+    priopity = 2
+    model = M2
+    json_file_path = 'django_seeding_example/seeders_data/M2Seeder.json'
+```
+
+seeders_data/M2Seeder.json
+```
+[
+    {
+        "title": "json t1",
+        "description": "json d1"
+    },
+    {
+        "title": "json t2",
+        "description": "json d2"
+    }
+]
+```
+
+
+
+
+#### CSVFileSerializerSeeder:
+
+Slow one-by-one seeder
+
+notice that the titles in the `csv-file` have to match the fields name in the `serializer`
+
+<b> This seeder is used to inject a serializer to implement custom create logic </b>
+
+models.py
+```
+class M3(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+serializers.py
+```
+class M3Serializer(serializers.ModelSerializer):
+    class Meta:
+        model = M3
+        fields = ['title', 'description']
+
+    def create(self, validated_data):
+        validated_data['title'] = '__' + validated_data['title'] + '__'
+        validated_data['description'] = '__' + validated_data['description'] + '__'
+        return super().create(validated_data)
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M3Seeder(seeders.CSVFileSerializerSeeder):
+    id = 'M3Seeder'
+    priopity = 3
+    serializer_class = M3Serializer
+    csv_file_path = 'django_seeding_example/seeders_data/M3Seeder.csv'
+```
+
+seeders_data/M3Seeder.csv
+```
+title,description
+t1,d1
+t2,d2
+```
+
+
+
+
+#### JSONFileSerializerSeeder:
+
+Slow one-by-one seeder
+
+notice that the keys in the `json-file` have to match the fields name in the `serializer`
+
+<b> This seeder is used to inject a serializer to implement custom create logic </b>
+
+models.py
+```
+class M4(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+serializers.py
+```
+class M4Serializer(serializers.ModelSerializer):
+    class Meta:
+        model = M4
+        fields = ['title', 'description']
+
+    def create(self, validated_data):
+        validated_data['title'] = '__' + validated_data['title'] + '__'
+        validated_data['description'] = '__' + validated_data['description'] + '__'
+        return super().create(validated_data)
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M4Seeder(seeders.JSONFileSerializerSeeder):
+    id = 'M4Seeder'
+    priopity = 4
+    serializer_class = M4Serializer
+    json_file_path = 'django_seeding_example/seeders_data/M4Seeder.json'
+```
+
+seeders_data/M4Seeder.json
+```
+[
+    {
+        "title": "json t1",
+        "description": "json d1"
+    },
+    {
+        "title": "json t2",
+        "description": "json d2"
+    }
+]
+```
+
+
+
+
+#### EmptySeeder (Recommended):
+
+Fast `bulk_create` seeder
+
+models.py
+```
+class M5(models.Model):
+    title = models.CharField(max_length=100, null=True)
+    description = models.TextField(null=True)
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M5Seeder(seeders.EmptySeeder):
+    id = 'M5Seeder'
+    priopity = 5
+    model = M5
+    records_count = 2
+```
+
+
+
+
+#### ModelSeeder (Recommended):
+
+Fast `bulk_create` seeder
+
+notice that the keys in the `data` class-attribute have to match the fields name in the `model`
+
+models.py
+```
+class M6(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M6Seeder(seeders.ModelSeeder):
+    id = 'M6Seeder'
+    priopity = 6
+    model = M6
+    data = [
+        {
+            "title": "in-code t1",
+            "description": "in-code d1"
+        },
+        {
+            "title": "in-code t2",
+            "description": "in-code d2"
+        },
+    ]
+```
+
+
+
+
+#### SerializerSeeder:
+
+Slow one-by-one seeder
+
+notice that the keys in the `data` class-attribute have to match the fields name in the `serializer`
+
+<b> This seeder is used to inject a serializer to implement custom create logic </b>
+
+models.py
+```
+class M7(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+serializer.py
+```
+class M7Serializer(serializers.ModelSerializer):
+    class Meta:
+        model = M7
+        fields = ['title', 'description']
+
+    def create(self, validated_data):
+        validated_data['title'] = '__' + validated_data['title'] + '__'
+        validated_data['description'] = '__' + validated_data['description'] + '__'
+        return super().create(validated_data)
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M7Seeder(seeders.SerializerSeeder):
+    id = 'M7Seeder'
+    priopity = 7
+    serializer_class = M7Serializer
+    data = [
+        {
+            "title": "in-code t1",
+            "description": "in-code d1"
+        },
+        {
+            "title": "in-code t2",
+            "description": "in-code d2"
+        },
+    ]
+```
+
+
+
+
+#### Seeder:
+
+Here you can write your logic as you want in the seed method
+
+models.py
+```
+class Post(models.Model):
+    content = models.TextField()
+
+
+class Comment(models.Model):
+    post = models.ForeignKey(Post, on_delete=models.CASCADE)
+    content = models.TextField()
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class CustomSeeder(seeders.Seeder):
+    id = 'CustomSeeder'
+    priopity = 8
+    
+    def seed(self):
+        post1 = Post.objects.create(content='post1')
+        post2 = Post.objects.create(content='post1')
+
+        comment1 = Comment.objects.create(post=post1, content='comment1')
+        comment2 = Comment.objects.create(post=post1, content='comment2')
+        comment3 = Comment.objects.create(post=post2, content='comment3')
+        comment4 = Comment.objects.create(post=post2, content='comment4')
+```
+
+
+
+
+
+
+## Contributing
+
+If you have suggestions for how Django Seeding could be improved, or want to report a bug, open an issue! We'd love all and any contributions.
+
+For more, check out the [Contributing Guide][contributing-url].
+
+
+## Contact
+
+Suliman Awad - [sulimanawadstudy@gmail.com][gmail-url] - [Linkedin][linkedin-account-url]
+
+Project Link: [https://github.com/suliman-99/django-seeding][repo-url]
+
+
+## License
+
+MIT License
+
+Copyright (c) 2023 Suliman Awad
+
+For more, check out the [License File][license-url].
+
+
+<!-- ------------------------------------ urls ------------------------------------ -->
+
+
+
+<!-- my urls -->
+[gmail-url]: mailto:sulimanawadstudy@gmail.com
+[linkedin-account-url]: https://linkedin.com/in/suliman-awad-399a471b8
+[facebook-account-url]: https://www.facebook.com/suliman.awad.507
+[codeforces-account-url]: https://codeforces.com/profile/Suliman_Awad
+[github-account-url]: https://github.com/suliman-99
+
+
+<!-- repo urls -->
+[repo-url]: https://github.com/suliman-99/django-seeding
+[contributors-url]: https://github.com/suliman-99/django-seeding/graphs/contributors
+[forks-url]: https://github.com/suliman-99/django-seeding/network/members
+[stars-url]: https://github.com/suliman-99/django-seeding/stargazers
+[issues-url]: https://github.com/suliman-99/django-seeding/issues
+[license-url]: ./LICENSE
+[contributing-url]: ./CONTRIBUTING.md
+[photo-url]: ./photo.png
+[demo-url]: https://github.com/suliman-99/django-seeding
+
+
+<!-- static urls -->
+[hacktoberfest-url]: https://hacktoberfest.com
+[python-url]: https://www.python.org
+[python-downloads-url]: https://www.python.org/downloads
+[django-url]: https://www.djangoproject.com
+[mysql-url]: https://www.mysql.com
+[postgresql-url]: https://www.postgresql.org
+[restful-api-url]: https://aws.amazon.com/what-is/restful-api/?nc1=h_ls
+[postman-url]: https://www.postman.com
+[git-url]: https://git-scm.com
+[git-downloads-url]: https://git-scm.com/downloads
+[github-url]: https://github.com
+[markdown-url]: https://en.wikipedia.org/wiki/Markdown
+[vscode-url]: https://code.visualstudio.com
+
+
+
+<!-- ------------------------------------ shields ------------------------------------ -->
+
+
+
+<!-- my shields -->
+[gmail-shield]: https://img.shields.io/badge/Gmail-sulimanawadstudy@gmail.com-blue?logo=gmail&style=flat-square
+[linkedin-shield]: https://img.shields.io/badge/LinkedIn-Suliman%20Awad-blue?logo=linkedin&logoColor=6688ee&style=flat-square
+[linkedin-shield2]: https://img.shields.io/badge/LinkedIn-black.svg?logo=linkedin&colorB=555&style=social
+[facebook-shield]: https://img.shields.io/badge/Facebook-Suliman%20Awad-blue?logo=Facebook&style=flat-square
+
+[codeforces-shield]: https://img.shields.io/badge/Suliman%20Awad-333333?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABMAAAAQCAYAAAD0xERiAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAAIOSURBVDhPpZHLa1NBFMa/O0naPG/E10Vb0pArunBha0C6cCVCVdwLImTnzoWIa1257J/h3+BGEN105053fRACai0Gkzbx3jt3POfMDEZss/GDjznz+s03M0G32zU4QZX4GrB6F35BeXsLw4/vXO9fKdcer9uPsXPqCnad97sP3MTxmgsr1UJXWU0yV5yg+cmMgcmddS7tPKmFhRJePFnH68075A28enoD9dqiTMpmb+YQfJ7Uxs027q0vIj5/iPjcGLeuF/Dw/mU76/d60Eyyi40Qa6fPiJfqDRlTzUaREiTklNangE5QK8ucAOz1yNpel9Wp1fF88B2PPm+Ln/W/4mo9pDczOZ1IMD2FyY6oOyWIlk0BQf5c05m0kmTIJxOpeUSnKaLRGMrQRqN/CZBoLiFB/EpOR7C/PoC51OjAGYGcJ8kEQLCcrihggsoegTDMgTxMIASgwoitLIwADJN0BOYxVs6p5HrU8TWPc9eZa9+feTObyl7TvlkmyfgwZ5dsFsIJ2ZxWGRpiACeSX9VHtNrC+Fr2Jx1oBuYhHgyq1c6AfpF+0P6iTdX/Zt8sOfhiV/IOcpnXkMaVMozAKL28H7XNJgrFSvQyKcXISssYjCJ8+BTizdYI1WoVZ9N9tFda6IQKy2qEC3tvUUwP8bNYQNBpo3IpxrTdQr+1hPc/DhD0ej0TRZGc+D8aDof4DQayYRrQETG1AAAAAElFTkSuQmCC&style=flat-square
+
+
+<!-- repo shields -->
+[repo-size-shield]: https://img.shields.io/github/repo-size/suliman-99/django-seeding.svg?label=Repo%20size&style=flat-square
+[forks-shield]: https://img.shields.io/github/forks/suliman-99/django-seeding.svg?&style=flat-square
+[stars-shield]: https://img.shields.io/github/stars/suliman-99/django-seeding.svg?&style=flat-square
+[issues-shield]: https://img.shields.io/github/issues/suliman-99/django-seeding.svg?&style=flat-square
+[contributors-shield]: https://img.shields.io/github/contributors/suliman-99/django-seeding.svg?&style=flat-square
+[pr-shield]: https://img.shields.io/badge/PR-Welcome-333333?color=0055bb&style=flat-square
+[hachtoberfest-shield]: https://img.shields.io/github/hacktoberfest/2022/suliman-99/django-seeding
+[license-shield]: https://img.shields.io/github/license/suliman-99/django-seeding.svg?&style=flat-square
+
+
```

### Comparing `django-seeding-1.0.9/django_seeding.egg-info/PKG-INFO` & `django_seeding-1.1.1/django_seeding.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,647 +1,653 @@
-Metadata-Version: 2.1
-Name: django-seeding
-Version: 1.0.9
-Summary: Simple Django Package that helps developer to seed data from files and codes into the database automatically
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: django
-Requires-Dist: djangorestframework
-Requires-Dist: pandas
-
-<!-- 
-    Written By Suliman Awad
-    Email: sulimanawadstudy@gmail.com
-    Github: https://github.com/suliman-99
-    Linkedin: https://linkedin.com/in/suliman-awad-399a471b8
-    Facebook: https://www.facebook.com/suliman.awad.507
- -->
-[![repo-size][repo-size-shield]][repo-url]
-[![forks][forks-shield]][forks-url]
-[![stars][stars-shield]][stars-url]
-[![issues][issues-shield]][issues-url]
-[![contributors][contributors-shield]][contributors-url]
-[![pr][pr-shield]][contributing-url]
-[![hachtoberfest][hachtoberfest-shield]][hacktoberfest-url]
-[![license][license-shield]][license-url]
-
-
-<div align="center">
-<h3>Django Seeding</h3>
-</div>
-
-
-## Table of Contents
-
-- [Introduction](#introduction)
-- [Installation](#installation)
-- [Simple Example](#simple-example)
-- [Full Usage Documentation](#full-usage-documentation)
-    - [Seeders List](#seeders-list)
-    - [Attributes List](#attributes-list)
-    - [Run Methods](#run-methods)
-- [Full Examples](#full-examples)
-    - [CSVFileModelSeeder (Recommended)](#csvfilemodelseeder-recommended)
-    - [JSONFileModelSeeder (Recommended)](#jsonfilemodelseeder-recommended)
-    - [CSVFileSerializerSeeder](#csvfileserializerseeder)
-    - [JSONFileSerializerSeeder](#jsonfileserializerseeder)
-    - [EmptySeeder (Recommended)](#emptyseeder-recommended)
-    - [ModelSeeder (Recommended)](#modelseeder-recommended)
-    - [SerializerSeeder](#serializerseeder)
-    - [Seeder](#seeder)
-- [Contributing](#contributing)
-- [Contact](#contact)
-- [License](#license)
-
-
-## Introduction
-
-This package helps develpoers to `fill` the database with `real data` instead of filling it manually.
-
-Data can be presented as `CSV File` , `JSON File` or `in-code`.
-
-`Dependency-Injection` also available to inject your logic by specifying a `serializer_class` or writing your custom `seed` method.
-
-
-## Installation
-
-Installing using pip:
-
-```
-pip install django-seeding:
-```
-
-add `'django_seeding'` to your `INSTALLED_APPS` setting:
-
-```
-INSTALLED_APPS = [
-    ...
-    'django_seeding',
-]
-```
-
-
-## Simple Example
-
-Let's take a look at a quick example of using `CSVFileModelSeeder` seeder from `django-seeding` to build a simple seeder to insert data in the database.
-
-django_seeding_example/models.py:
-```
-from django.db import models
-
-
-class M1(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-django_seeding_example/seeders.py:
-```
-from django_seeding import seeders
-from django_seeding.seeder_registry import SeederRegistry 
-from django_seeding_example.models import M1
-
-@SeederRegistry.register
-class M1Seeder(seeders.CSVFileModelSeeder):
-    model = M1
-    csv_file_path = 'django_seeding_example/seeders_data/M1Seeder.csv'
-```
-
-django_seeding_example/seeders_data/M1Seeder.csv:
-```
-title,description
-t1,d1
-t2,d2
-```
-
-Now you just need to run this commande:
-
-```
-python manage.py seed
-```
-## Full Usage Documentation: 
-
-Now lets go deeper into the different Seeders types with its details:
-
-### Seeders List:
-- [CSVFileModelSeeder (Recommended)](#csvfilemodelseeder-recommended)
-- [JSONFileModelSeeder (Recommended)](#jsonfilemodelseeder-recommended)
-- [CSVFileSerializerSeeder](#csvfileserializerseeder)
-- [JSONFileSerializerSeeder](#jsonfileserializerseeder)
-- [EmptySeeder (Recommended)](#emptyseeder-recommended)
-- [ModelSeeder (Recommended)](#modelseeder-recommended)
-- [SerializerSeeder](#serializerseeder)
-- [Seeder](#seeder)
-
-### Attributes List
-
-#### In general there is a way to know how to deal with these seeders easily:
-
-Model..Seeder needs `model` class-attribute
-
-Serializer..Seeder needs `serializer_class` class-attribute
-
-CSVFile..Seeder needs `csv_file_path` class-attribute
-
-JSONFile..Seeder needs `json_file_path` class-attribute
-
-#### All seeders can takes these optional class-attributes:
-* `id: str` (So Recommended) 
-
-    This is what will be stored in the AppliedSeeder table to check if a seeder is already applied or not
-
-    It is recommended to set it as the seeder name
-
-    So, set it and don't change it because when the value is changed it will be considerd as a new seeder and it will be applied again even that the old seeder with the old name is applied
-
-    default value: `str(type(seeder))`
-
-
-
-* `priority: int|float` 
-
-    Seeders will be sorted depending on this attribute (lower-first)
-
-    default value: `float('inf')`
-
-
-
-
-
-* `just_debug: bool` 
-
-    This attribute specify if the seeder will be applied when the server is in the production-mode or not depending in the DEBUG variable in settings file
-
-    `DEBUG=False` & `just_debug=True` -> don't apply
-
-    `DEBUG=False` & `just_debug=False` -> apply
-
-    `DEBUG=True` & `just_debug=False` -> apply
-
-    `DEBUG=True` & `just_debug=True` -> apply
-
-    default value: `False`
-
-#### Notice:
-
-* `@SeederRegistry.register` is the decorator that register the seeder, so, if this decorator is not applied then the seeder will not be applied
-* Model seeders use bulk_create method, so, they are faster than Serializer seeders
-* CSV file reader is using pandas for a better performance and less bugs
-* Using Model seeders means the fields names must match the fields you have defined in your model
-* Using Serializer seeders means the fields names must match the fields you have defined in your serializer
-* you can define `get_` class-methods instead of class-attributes as below:
-    
-    ```
-    get_model
-    get_serializer_class
-    get_csv_file_path
-    get_json_file_path
-    get_id
-    get_priority
-    get_just_debug
-    ```
-
-
-### Run methods:
-
-* To seed with a manual command (Recommended):
-
-```
-python manage.py seed
-```
-
-
-* To seed with runserver manually just add "--seed" in runserver command:
-
-```
-python manage.py runserver --seed
-```
-
-
-* To seed on runserver automatically just set in your project settings:
-
-``` 
-SEEDING_ON_RUNSERVER = True
-``` 
-
-#### Notice: 
-* If you set `SEEDING_ON_RUNSERVER=True` in your settings file You can stop seeding in a runserver by using `--dont-seed` argument
-
-```
-python manage.py runserver --dont-seed
-```
-
-
-## Full Examples:
-
-
-Here we will go deeper in the seeders classes and its details
-
-
-#### CSVFileModelSeeder (Recommended):
-
-Fast `bulk_create` seeder
-
-notice that the titles in the `csv-file` have to match the fields name in the `model`
-
-models.py
-```
-class M1(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M1Seeder(seeders.CSVFileModelSeeder):
-    id = 'M1Seeder'
-    priopity = 1
-    model = M1
-    csv_file_path = 'django_seeding_example/seeders_data/M1Seeder.csv'
-```
-
-seeders_data/M1Seeder.csv
-```
-title,description
-t1,d1
-t2,d2
-```
-
-
-
-#### JSONFileModelSeeder (Recommended):
-
-Fast `bulk_create` seeder
-
-notice that the keys in the `json-file` have to match the fields name in the `model`
-
-models.py
-```
-class M2(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M2Seeder(seeders.JSONFileModelSeeder):
-    id = 'M2Seeder'
-    priopity = 2
-    model = M2
-    json_file_path = 'django_seeding_example/seeders_data/M2Seeder.json'
-```
-
-seeders_data/M2Seeder.json
-```
-[
-    {
-        "title": "json t1",
-        "description": "json d1"
-    },
-    {
-        "title": "json t2",
-        "description": "json d2"
-    }
-]
-```
-
-
-
-
-#### CSVFileSerializerSeeder:
-
-Slow one-by-one seeder
-
-notice that the titles in the `csv-file` have to match the fields name in the `serializer`
-
-<b> This seeder is used to inject a serializer to implement custom create logic </b>
-
-models.py
-```
-class M3(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-serializers.py
-```
-class M3Serializer(serializers.ModelSerializer):
-    class Meta:
-        model = M3
-        fields = ['title', 'description']
-
-    def create(self, validated_data):
-        validated_data['title'] = '__' + validated_data['title'] + '__'
-        validated_data['description'] = '__' + validated_data['description'] + '__'
-        return super().create(validated_data)
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M3Seeder(seeders.CSVFileSerializerSeeder):
-    id = 'M3Seeder'
-    priopity = 3
-    serializer_class = M3Serializer
-    csv_file_path = 'django_seeding_example/seeders_data/M3Seeder.csv'
-```
-
-seeders_data/M3Seeder.csv
-```
-title,description
-t1,d1
-t2,d2
-```
-
-
-
-
-#### JSONFileSerializerSeeder:
-
-Slow one-by-one seeder
-
-notice that the keys in the `json-file` have to match the fields name in the `serializer`
-
-<b> This seeder is used to inject a serializer to implement custom create logic </b>
-
-models.py
-```
-class M4(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-serializers.py
-```
-class M4Serializer(serializers.ModelSerializer):
-    class Meta:
-        model = M4
-        fields = ['title', 'description']
-
-    def create(self, validated_data):
-        validated_data['title'] = '__' + validated_data['title'] + '__'
-        validated_data['description'] = '__' + validated_data['description'] + '__'
-        return super().create(validated_data)
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M4Seeder(seeders.JSONFileSerializerSeeder):
-    id = 'M4Seeder'
-    priopity = 4
-    serializer_class = M4Serializer
-    json_file_path = 'django_seeding_example/seeders_data/M4Seeder.json'
-```
-
-seeders_data/M4Seeder.csv
-```
-[
-    {
-        "title": "json t1",
-        "description": "json d1"
-    },
-    {
-        "title": "json t2",
-        "description": "json d2"
-    }
-]
-```
-
-
-
-
-#### EmptySeeder (Recommended):
-
-Fast `bulk_create` seeder
-
-models.py
-```
-class M5(models.Model):
-    title = models.CharField(max_length=100, null=True)
-    description = models.TextField(null=True)
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M5Seeder(seeders.EmptySeeder):
-    id = 'M5Seeder'
-    priopity = 5
-    model = M5
-    records_count = 2
-```
-
-
-
-
-#### ModelSeeder (Recommended):
-
-Fast `bulk_create` seeder
-
-notice that the keys in the `data` class-attribute have to match the fields name in the `model`
-
-models.py
-```
-class M6(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M6Seeder(seeders.ModelSeeder):
-    id = 'M6Seeder'
-    priopity = 6
-    model = M6
-    data = [
-        {
-            "title": "in-code t1",
-            "description": "in-code d1"
-        },
-        {
-            "title": "in-code t2",
-            "description": "in-code d2"
-        },
-    ]
-```
-
-
-
-
-#### SerializerSeeder:
-
-Slow one-by-one seeder
-
-notice that the keys in the `data` class-attribute have to match the fields name in the `serializer`
-
-<b> This seeder is used to inject a serializer to implement custom create logic </b>
-
-models.py
-```
-class M7(models.Model):
-    title = models.CharField(max_length=100)
-    description = models.TextField()
-```
-
-serializer.py
-```
-class M7Serializer(serializers.ModelSerializer):
-    class Meta:
-        model = M7
-        fields = ['title', 'description']
-
-    def create(self, validated_data):
-        validated_data['title'] = '__' + validated_data['title'] + '__'
-        validated_data['description'] = '__' + validated_data['description'] + '__'
-        return super().create(validated_data)
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class M7Seeder(seeders.SerializerSeeder):
-    id = 'M7Seeder'
-    priopity = 7
-    serializer_class = M7Serializer
-    data = [
-        {
-            "title": "in-code t1",
-            "description": "in-code d1"
-        },
-        {
-            "title": "in-code t2",
-            "description": "in-code d2"
-        },
-    ]
-```
-
-
-
-
-#### Seeder:
-
-Here you can write your logic as you want in the seed method
-
-models.py
-```
-class Post(models.Model):
-    content = models.TextField()
-
-
-class Comment(models.Model):
-    post = models.ForeignKey(Post, on_delete=models.CASCADE)
-    content = models.TextField()
-```
-
-seeders.py
-```
-@SeederRegistry.register
-class CustomSeeder(seeders.Seeder):
-    id = 'CustomSeeder'
-    priopity = 8
-    
-    def seed(self):
-        post1 = Post.objects.create(content='post1')
-        post2 = Post.objects.create(content='post1')
-
-        comment1 = Comment.objects.create(post=post1, content='comment1')
-        comment2 = Comment.objects.create(post=post1, content='comment2')
-        comment3 = Comment.objects.create(post=post2, content='comment3')
-        comment4 = Comment.objects.create(post=post2, content='comment4')
-```
-
-
-
-
-
-
-## Contributing
-
-If you have suggestions for how Django Seeding could be improved, or want to report a bug, open an issue! We'd love all and any contributions.
-
-For more, check out the [Contributing Guide][contributing-url].
-
-
-## Contact
-
-Suliman Awad - [sulimanawadstudy@gmail.com][gmail-url] - [Linkedin][linkedin-account-url]
-
-Project Link: [https://github.com/suliman-99/django-seeding][repo-url]
-
-
-## License
-
-MIT License
-
-Copyright (c) 2023 Suliman Awad
-
-For more, check out the [License File][license-url].
-
-
-
-<!-- ------------------------------------ urls ------------------------------------ -->
-
-
-<!-- my urls -->
-[gmail-url]: mailto:sulimanawadstudy@gmail.com
-[linkedin-account-url]: https://linkedin.com/in/suliman-awad-399a471b8
-[facebook-account-url]: https://www.facebook.com/suliman.awad.507
-[codeforces-account-url]: https://codeforces.com/profile/Suliman_Awad
-[github-account-url]: https://github.com/suliman-99
-
-
-<!-- repo urls -->
-[repo-url]: https://github.com/suliman-99/django-seeding
-[contributors-url]: https://github.com/suliman-99/django-seeding/graphs/contributors
-[forks-url]: https://github.com/suliman-99/django-seeding/network/members
-[stars-url]: https://github.com/suliman-99/django-seeding/stargazers
-[issues-url]: https://github.com/suliman-99/django-seeding/issues
-[license-url]: ./LICENSE
-[contributing-url]: ./CONTRIBUTING.md
-[photo-url]: ./photo.png
-[demo-url]: https://github.com/suliman-99/django-seeding
-
-
-<!-- static urls -->
-[hacktoberfest-url]: https://hacktoberfest.com
-[python-url]: https://www.python.org
-[python-downloads-url]: https://www.python.org/downloads
-[django-url]: https://www.djangoproject.com
-[mysql-url]: https://www.mysql.com
-[postgresql-url]: https://www.postgresql.org
-[restful-api-url]: https://aws.amazon.com/what-is/restful-api/?nc1=h_ls
-[postman-url]: https://www.postman.com
-[git-url]: https://git-scm.com
-[git-downloads-url]: https://git-scm.com/downloads
-[github-url]: https://github.com
-[markdown-url]: https://en.wikipedia.org/wiki/Markdown
-[vscode-url]: https://code.visualstudio.com
-
-
-
-<!-- ------------------------------------ shields ------------------------------------ -->
-
-
-
-<!-- my shields -->
-[gmail-shield]: https://img.shields.io/badge/Gmail-sulimanawadstudy@gmail.com-blue?logo=gmail&style=flat-square
-[linkedin-shield]: https://img.shields.io/badge/LinkedIn-Suliman%20Awad-blue?logo=linkedin&logoColor=6688ee&style=flat-square
-[linkedin-shield2]: https://img.shields.io/badge/LinkedIn-black.svg?logo=linkedin&colorB=555&style=social
-[facebook-shield]: https://img.shields.io/badge/Facebook-Suliman%20Awad-blue?logo=Facebook&style=flat-square
-
-[codeforces-shield]: https://img.shields.io/badge/Suliman%20Awad-333333?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABMAAAAQCAYAAAD0xERiAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAAIOSURBVDhPpZHLa1NBFMa/O0naPG/E10Vb0pArunBha0C6cCVCVdwLImTnzoWIa1257J/h3+BGEN105053fRACai0Gkzbx3jt3POfMDEZss/GDjznz+s03M0G32zU4QZX4GrB6F35BeXsLw4/vXO9fKdcer9uPsXPqCnad97sP3MTxmgsr1UJXWU0yV5yg+cmMgcmddS7tPKmFhRJePFnH68075A28enoD9dqiTMpmb+YQfJ7Uxs027q0vIj5/iPjcGLeuF/Dw/mU76/d60Eyyi40Qa6fPiJfqDRlTzUaREiTklNangE5QK8ucAOz1yNpel9Wp1fF88B2PPm+Ln/W/4mo9pDczOZ1IMD2FyY6oOyWIlk0BQf5c05m0kmTIJxOpeUSnKaLRGMrQRqN/CZBoLiFB/EpOR7C/PoC51OjAGYGcJ8kEQLCcrihggsoegTDMgTxMIASgwoitLIwADJN0BOYxVs6p5HrU8TWPc9eZa9+feTObyl7TvlkmyfgwZ5dsFsIJ2ZxWGRpiACeSX9VHtNrC+Fr2Jx1oBuYhHgyq1c6AfpF+0P6iTdX/Zt8sOfhiV/IOcpnXkMaVMozAKL28H7XNJgrFSvQyKcXISssYjCJ8+BTizdYI1WoVZ9N9tFda6IQKy2qEC3tvUUwP8bNYQNBpo3IpxrTdQr+1hPc/DhD0ej0TRZGc+D8aDof4DQayYRrQETG1AAAAAElFTkSuQmCC&style=flat-square
-
-
-<!-- repo shields -->
-[repo-size-shield]: https://img.shields.io/github/repo-size/suliman-99/django-seeding.svg?label=Repo%20size&style=flat-square
-[forks-shield]: https://img.shields.io/github/forks/suliman-99/django-seeding.svg?&style=flat-square
-[stars-shield]: https://img.shields.io/github/stars/suliman-99/django-seeding.svg?&style=flat-square
-[issues-shield]: https://img.shields.io/github/issues/suliman-99/django-seeding.svg?&style=flat-square
-[contributors-shield]: https://img.shields.io/github/contributors/suliman-99/django-seeding.svg?&style=flat-square
-[pr-shield]: https://img.shields.io/badge/PR-Welcome-333333?color=0055bb&style=flat-square
-[hachtoberfest-shield]: https://img.shields.io/github/hacktoberfest/2022/suliman-99/django-seeding
-[license-shield]: https://img.shields.io/github/license/suliman-99/django-seeding.svg?&style=flat-square
-
+Metadata-Version: 2.1
+Name: django-seeding
+Version: 1.1.1
+Summary: Simple Django Package that helps developer to seed data from files and codes into the database automatically
+Author-email: Suliman Awad <sulimanawadstudy@gmail.com>
+Project-URL: Source, https://github.com/suliman-99/django-seeding
+Project-URL: Contributors, https://github.com/suliman-99/django-seeding/graphs/contributors
+Project-URL: License, https://github.com/suliman-99/django-seeding/blob/main/LICENSE
+Project-URL: Issues, https://github.com/suliman-99/django-seeding/issues
+Classifier: Programming Language :: Python
+Classifier: Framework :: Django
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<!-- 
+    Written By Suliman Awad
+    Email: sulimanawadstudy@gmail.com
+    Github: https://github.com/suliman-99
+    Linkedin: https://linkedin.com/in/suliman-awad-399a471b8
+    Facebook: https://www.facebook.com/suliman.awad.507
+ -->
+[![repo-size][repo-size-shield]][repo-url]
+[![forks][forks-shield]][forks-url]
+[![stars][stars-shield]][stars-url]
+[![issues][issues-shield]][issues-url]
+[![contributors][contributors-shield]][contributors-url]
+[![pr][pr-shield]][contributing-url]
+[![hachtoberfest][hachtoberfest-shield]][hacktoberfest-url]
+[![license][license-shield]][license-url]
+
+
+<div align="center">
+<h3>Django Seeding</h3>
+</div>
+
+
+
+## Table of Contents
+
+- [Introduction](#introduction)
+- [Installation](#installation)
+- [Simple Example](#simple-example)
+- [Full Usage Documentation](#full-usage-documentation)
+    - [Seeders List](#seeders-list)
+    - [Attributes List](#attributes-list)
+    - [Run Methods](#run-methods)
+- [Full Examples](#full-examples)
+    - [CSVFileModelSeeder (Recommended)](#csvfilemodelseeder-recommended)
+    - [JSONFileModelSeeder (Recommended)](#jsonfilemodelseeder-recommended)
+    - [CSVFileSerializerSeeder](#csvfileserializerseeder)
+    - [JSONFileSerializerSeeder](#jsonfileserializerseeder)
+    - [EmptySeeder (Recommended)](#emptyseeder-recommended)
+    - [ModelSeeder (Recommended)](#modelseeder-recommended)
+    - [SerializerSeeder](#serializerseeder)
+    - [Seeder](#seeder)
+- [Contributing](#contributing)
+- [Contact](#contact)
+- [License](#license)
+
+
+## Introduction
+
+This package helps develpoers to `fill` the database with `real data` instead of filling it manually.
+
+Data can be presented as `CSV File` , `JSON File` or `in-code`.
+
+`Dependency-Injection` also available to inject your logic by specifying a `serializer_class` or writing your custom `seed` method.
+
+
+## Installation
+
+Installing using pip:
+
+```
+pip install django-seeding:
+```
+
+add `'django_seeding'` to your `INSTALLED_APPS` setting:
+
+```
+INSTALLED_APPS = [
+    ...
+    'django_seeding',
+]
+```
+
+
+## Simple Example
+
+Let's take a look at a quick example of using `CSVFileModelSeeder` seeder from `django-seeding` to build a simple seeder to insert data in the database.
+
+django_seeding_example/models.py:
+```
+from django.db import models
+
+
+class M1(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+django_seeding_example/seeders.py:
+```
+from django_seeding import seeders
+from django_seeding.seeder_registry import SeederRegistry 
+from django_seeding_example.models import M1
+
+@SeederRegistry.register
+class M1Seeder(seeders.CSVFileModelSeeder):
+    model = M1
+    csv_file_path = 'django_seeding_example/seeders_data/M1Seeder.csv'
+```
+
+django_seeding_example/seeders_data/M1Seeder.csv:
+```
+title,description
+t1,d1
+t2,d2
+```
+
+Now you just need to run this commande:
+
+```
+python manage.py seed
+```
+## Full Usage Documentation: 
+
+Now lets go deeper into the different Seeders types with its details:
+
+### Seeders List:
+- [CSVFileModelSeeder (Recommended)](#csvfilemodelseeder-recommended)
+- [JSONFileModelSeeder (Recommended)](#jsonfilemodelseeder-recommended)
+- [CSVFileSerializerSeeder](#csvfileserializerseeder)
+- [JSONFileSerializerSeeder](#jsonfileserializerseeder)
+- [EmptySeeder (Recommended)](#emptyseeder-recommended)
+- [ModelSeeder (Recommended)](#modelseeder-recommended)
+- [SerializerSeeder](#serializerseeder)
+- [Seeder](#seeder)
+
+### Attributes List
+
+#### In general there is a way to know how to deal with these seeders easily:
+
+Model..Seeder needs `model` class-attribute
+
+Serializer..Seeder needs `serializer_class` class-attribute
+
+CSVFile..Seeder needs `csv_file_path` class-attribute
+
+JSONFile..Seeder needs `json_file_path` class-attribute
+
+#### All seeders can takes these optional class-attributes:
+* `id: str` (So Recommended) 
+
+    This is what will be stored in the AppliedSeeder table to check if a seeder is already applied or not
+
+    It is recommended to set it as the seeder name
+
+    So, set it and don't change it because when the value is changed it will be considerd as a new seeder and it will be applied again even that the old seeder with the old name is applied
+
+    default value: `str(type(seeder))`
+
+
+
+* `priority: int|float` 
+
+    Seeders will be sorted depending on this attribute (lower-first)
+
+    default value: `float('inf')`
+
+
+
+
+
+* `just_debug: bool` 
+
+    This attribute specify if the seeder will be applied when the server is in the production-mode or not depending in the DEBUG variable in settings file
+
+    `DEBUG=False` & `just_debug=True` -> don't apply
+
+    `DEBUG=False` & `just_debug=False` -> apply
+
+    `DEBUG=True` & `just_debug=False` -> apply
+
+    `DEBUG=True` & `just_debug=True` -> apply
+
+    default value: `False`
+
+#### Notice:
+
+* `@SeederRegistry.register` is the decorator that register the seeder, so, if this decorator is not applied then the seeder will not be applied
+* Model seeders use bulk_create method, so, they are faster than Serializer seeders
+* CSV file reader is using pandas for a better performance and less bugs
+* Using Model seeders means the fields names must match the fields you have defined in your model
+* Using Serializer seeders means the fields names must match the fields you have defined in your serializer
+* you can define `get_` class-methods instead of class-attributes as below:
+    
+    ```
+    get_model
+    get_serializer_class
+    get_csv_file_path
+    get_json_file_path
+    get_id
+    get_priority
+    get_just_debug
+    ```
+
+
+### Run methods:
+
+* To seed with a manual command (Recommended):
+
+```
+python manage.py seed
+```
+
+
+* To seed with runserver manually just add "--seed" in runserver command:
+
+```
+python manage.py runserver --seed
+```
+
+
+* To seed on runserver automatically just set in your project settings:
+
+``` 
+SEEDING_ON_RUNSERVER = True
+``` 
+
+#### Notice: 
+* If you set `SEEDING_ON_RUNSERVER=True` in your settings file You can stop seeding in a runserver by using `--dont-seed` argument
+
+```
+python manage.py runserver --dont-seed
+```
+
+
+## Full Examples:
+
+
+Here we will go deeper in the seeders classes and its details
+
+
+#### CSVFileModelSeeder (Recommended):
+
+Fast `bulk_create` seeder
+
+notice that the titles in the `csv-file` have to match the fields name in the `model`
+
+models.py
+```
+class M1(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M1Seeder(seeders.CSVFileModelSeeder):
+    id = 'M1Seeder'
+    priopity = 1
+    model = M1
+    csv_file_path = 'django_seeding_example/seeders_data/M1Seeder.csv'
+```
+
+seeders_data/M1Seeder.csv
+```
+title,description
+t1,d1
+t2,d2
+```
+
+
+
+#### JSONFileModelSeeder (Recommended):
+
+Fast `bulk_create` seeder
+
+notice that the keys in the `json-file` have to match the fields name in the `model`
+
+models.py
+```
+class M2(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M2Seeder(seeders.JSONFileModelSeeder):
+    id = 'M2Seeder'
+    priopity = 2
+    model = M2
+    json_file_path = 'django_seeding_example/seeders_data/M2Seeder.json'
+```
+
+seeders_data/M2Seeder.json
+```
+[
+    {
+        "title": "json t1",
+        "description": "json d1"
+    },
+    {
+        "title": "json t2",
+        "description": "json d2"
+    }
+]
+```
+
+
+
+
+#### CSVFileSerializerSeeder:
+
+Slow one-by-one seeder
+
+notice that the titles in the `csv-file` have to match the fields name in the `serializer`
+
+<b> This seeder is used to inject a serializer to implement custom create logic </b>
+
+models.py
+```
+class M3(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+serializers.py
+```
+class M3Serializer(serializers.ModelSerializer):
+    class Meta:
+        model = M3
+        fields = ['title', 'description']
+
+    def create(self, validated_data):
+        validated_data['title'] = '__' + validated_data['title'] + '__'
+        validated_data['description'] = '__' + validated_data['description'] + '__'
+        return super().create(validated_data)
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M3Seeder(seeders.CSVFileSerializerSeeder):
+    id = 'M3Seeder'
+    priopity = 3
+    serializer_class = M3Serializer
+    csv_file_path = 'django_seeding_example/seeders_data/M3Seeder.csv'
+```
+
+seeders_data/M3Seeder.csv
+```
+title,description
+t1,d1
+t2,d2
+```
+
+
+
+
+#### JSONFileSerializerSeeder:
+
+Slow one-by-one seeder
+
+notice that the keys in the `json-file` have to match the fields name in the `serializer`
+
+<b> This seeder is used to inject a serializer to implement custom create logic </b>
+
+models.py
+```
+class M4(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+serializers.py
+```
+class M4Serializer(serializers.ModelSerializer):
+    class Meta:
+        model = M4
+        fields = ['title', 'description']
+
+    def create(self, validated_data):
+        validated_data['title'] = '__' + validated_data['title'] + '__'
+        validated_data['description'] = '__' + validated_data['description'] + '__'
+        return super().create(validated_data)
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M4Seeder(seeders.JSONFileSerializerSeeder):
+    id = 'M4Seeder'
+    priopity = 4
+    serializer_class = M4Serializer
+    json_file_path = 'django_seeding_example/seeders_data/M4Seeder.json'
+```
+
+seeders_data/M4Seeder.json
+```
+[
+    {
+        "title": "json t1",
+        "description": "json d1"
+    },
+    {
+        "title": "json t2",
+        "description": "json d2"
+    }
+]
+```
+
+
+
+
+#### EmptySeeder (Recommended):
+
+Fast `bulk_create` seeder
+
+models.py
+```
+class M5(models.Model):
+    title = models.CharField(max_length=100, null=True)
+    description = models.TextField(null=True)
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M5Seeder(seeders.EmptySeeder):
+    id = 'M5Seeder'
+    priopity = 5
+    model = M5
+    records_count = 2
+```
+
+
+
+
+#### ModelSeeder (Recommended):
+
+Fast `bulk_create` seeder
+
+notice that the keys in the `data` class-attribute have to match the fields name in the `model`
+
+models.py
+```
+class M6(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M6Seeder(seeders.ModelSeeder):
+    id = 'M6Seeder'
+    priopity = 6
+    model = M6
+    data = [
+        {
+            "title": "in-code t1",
+            "description": "in-code d1"
+        },
+        {
+            "title": "in-code t2",
+            "description": "in-code d2"
+        },
+    ]
+```
+
+
+
+
+#### SerializerSeeder:
+
+Slow one-by-one seeder
+
+notice that the keys in the `data` class-attribute have to match the fields name in the `serializer`
+
+<b> This seeder is used to inject a serializer to implement custom create logic </b>
+
+models.py
+```
+class M7(models.Model):
+    title = models.CharField(max_length=100)
+    description = models.TextField()
+```
+
+serializer.py
+```
+class M7Serializer(serializers.ModelSerializer):
+    class Meta:
+        model = M7
+        fields = ['title', 'description']
+
+    def create(self, validated_data):
+        validated_data['title'] = '__' + validated_data['title'] + '__'
+        validated_data['description'] = '__' + validated_data['description'] + '__'
+        return super().create(validated_data)
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class M7Seeder(seeders.SerializerSeeder):
+    id = 'M7Seeder'
+    priopity = 7
+    serializer_class = M7Serializer
+    data = [
+        {
+            "title": "in-code t1",
+            "description": "in-code d1"
+        },
+        {
+            "title": "in-code t2",
+            "description": "in-code d2"
+        },
+    ]
+```
+
+
+
+
+#### Seeder:
+
+Here you can write your logic as you want in the seed method
+
+models.py
+```
+class Post(models.Model):
+    content = models.TextField()
+
+
+class Comment(models.Model):
+    post = models.ForeignKey(Post, on_delete=models.CASCADE)
+    content = models.TextField()
+```
+
+seeders.py
+```
+@SeederRegistry.register
+class CustomSeeder(seeders.Seeder):
+    id = 'CustomSeeder'
+    priopity = 8
+    
+    def seed(self):
+        post1 = Post.objects.create(content='post1')
+        post2 = Post.objects.create(content='post1')
+
+        comment1 = Comment.objects.create(post=post1, content='comment1')
+        comment2 = Comment.objects.create(post=post1, content='comment2')
+        comment3 = Comment.objects.create(post=post2, content='comment3')
+        comment4 = Comment.objects.create(post=post2, content='comment4')
+```
+
+
+
+
+
+
+## Contributing
+
+If you have suggestions for how Django Seeding could be improved, or want to report a bug, open an issue! We'd love all and any contributions.
+
+For more, check out the [Contributing Guide][contributing-url].
+
+
+## Contact
+
+Suliman Awad - [sulimanawadstudy@gmail.com][gmail-url] - [Linkedin][linkedin-account-url]
+
+Project Link: [https://github.com/suliman-99/django-seeding][repo-url]
+
+
+## License
+
+MIT License
+
+Copyright (c) 2023 Suliman Awad
+
+For more, check out the [License File][license-url].
+
+
+<!-- ------------------------------------ urls ------------------------------------ -->
+
+
+
+<!-- my urls -->
+[gmail-url]: mailto:sulimanawadstudy@gmail.com
+[linkedin-account-url]: https://linkedin.com/in/suliman-awad-399a471b8
+[facebook-account-url]: https://www.facebook.com/suliman.awad.507
+[codeforces-account-url]: https://codeforces.com/profile/Suliman_Awad
+[github-account-url]: https://github.com/suliman-99
+
+
+<!-- repo urls -->
+[repo-url]: https://github.com/suliman-99/django-seeding
+[contributors-url]: https://github.com/suliman-99/django-seeding/graphs/contributors
+[forks-url]: https://github.com/suliman-99/django-seeding/network/members
+[stars-url]: https://github.com/suliman-99/django-seeding/stargazers
+[issues-url]: https://github.com/suliman-99/django-seeding/issues
+[license-url]: ./LICENSE
+[contributing-url]: ./CONTRIBUTING.md
+[photo-url]: ./photo.png
+[demo-url]: https://github.com/suliman-99/django-seeding
+
+
+<!-- static urls -->
+[hacktoberfest-url]: https://hacktoberfest.com
+[python-url]: https://www.python.org
+[python-downloads-url]: https://www.python.org/downloads
+[django-url]: https://www.djangoproject.com
+[mysql-url]: https://www.mysql.com
+[postgresql-url]: https://www.postgresql.org
+[restful-api-url]: https://aws.amazon.com/what-is/restful-api/?nc1=h_ls
+[postman-url]: https://www.postman.com
+[git-url]: https://git-scm.com
+[git-downloads-url]: https://git-scm.com/downloads
+[github-url]: https://github.com
+[markdown-url]: https://en.wikipedia.org/wiki/Markdown
+[vscode-url]: https://code.visualstudio.com
+
+
+
+<!-- ------------------------------------ shields ------------------------------------ -->
+
+
+
+<!-- my shields -->
+[gmail-shield]: https://img.shields.io/badge/Gmail-sulimanawadstudy@gmail.com-blue?logo=gmail&style=flat-square
+[linkedin-shield]: https://img.shields.io/badge/LinkedIn-Suliman%20Awad-blue?logo=linkedin&logoColor=6688ee&style=flat-square
+[linkedin-shield2]: https://img.shields.io/badge/LinkedIn-black.svg?logo=linkedin&colorB=555&style=social
+[facebook-shield]: https://img.shields.io/badge/Facebook-Suliman%20Awad-blue?logo=Facebook&style=flat-square
+
+[codeforces-shield]: https://img.shields.io/badge/Suliman%20Awad-333333?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABMAAAAQCAYAAAD0xERiAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAAIOSURBVDhPpZHLa1NBFMa/O0naPG/E10Vb0pArunBha0C6cCVCVdwLImTnzoWIa1257J/h3+BGEN105053fRACai0Gkzbx3jt3POfMDEZss/GDjznz+s03M0G32zU4QZX4GrB6F35BeXsLw4/vXO9fKdcer9uPsXPqCnad97sP3MTxmgsr1UJXWU0yV5yg+cmMgcmddS7tPKmFhRJePFnH68075A28enoD9dqiTMpmb+YQfJ7Uxs027q0vIj5/iPjcGLeuF/Dw/mU76/d60Eyyi40Qa6fPiJfqDRlTzUaREiTklNangE5QK8ucAOz1yNpel9Wp1fF88B2PPm+Ln/W/4mo9pDczOZ1IMD2FyY6oOyWIlk0BQf5c05m0kmTIJxOpeUSnKaLRGMrQRqN/CZBoLiFB/EpOR7C/PoC51OjAGYGcJ8kEQLCcrihggsoegTDMgTxMIASgwoitLIwADJN0BOYxVs6p5HrU8TWPc9eZa9+feTObyl7TvlkmyfgwZ5dsFsIJ2ZxWGRpiACeSX9VHtNrC+Fr2Jx1oBuYhHgyq1c6AfpF+0P6iTdX/Zt8sOfhiV/IOcpnXkMaVMozAKL28H7XNJgrFSvQyKcXISssYjCJ8+BTizdYI1WoVZ9N9tFda6IQKy2qEC3tvUUwP8bNYQNBpo3IpxrTdQr+1hPc/DhD0ej0TRZGc+D8aDof4DQayYRrQETG1AAAAAElFTkSuQmCC&style=flat-square
+
+
+<!-- repo shields -->
+[repo-size-shield]: https://img.shields.io/github/repo-size/suliman-99/django-seeding.svg?label=Repo%20size&style=flat-square
+[forks-shield]: https://img.shields.io/github/forks/suliman-99/django-seeding.svg?&style=flat-square
+[stars-shield]: https://img.shields.io/github/stars/suliman-99/django-seeding.svg?&style=flat-square
+[issues-shield]: https://img.shields.io/github/issues/suliman-99/django-seeding.svg?&style=flat-square
+[contributors-shield]: https://img.shields.io/github/contributors/suliman-99/django-seeding.svg?&style=flat-square
+[pr-shield]: https://img.shields.io/badge/PR-Welcome-333333?color=0055bb&style=flat-square
+[hachtoberfest-shield]: https://img.shields.io/github/hacktoberfest/2022/suliman-99/django-seeding
+[license-shield]: https://img.shields.io/github/license/suliman-99/django-seeding.svg?&style=flat-square
+
+
```

