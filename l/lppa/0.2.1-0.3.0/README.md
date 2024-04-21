# Comparing `tmp/lppa-0.2.1.tar.gz` & `tmp/lppa-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lppa-0.2.1.tar", last modified: Sun Jan 30 15:40:05 2022, max compression
+gzip compressed data, was "lppa-0.3.0.tar", last modified: Sun Apr 21 12:31:31 2024, max compression
```

## Comparing `lppa-0.2.1.tar` & `lppa-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,32 @@
-drwxrwxr-x   0 athos     (1000) athos     (1000)        0 2022-01-30 15:40:05.194732 lppa-0.2.1/
--rw-rw-r--   0 athos     (1000) athos     (1000)    35149 2021-08-10 20:34:46.000000 lppa-0.2.1/LICENSE
--rw-rw-r--   0 athos     (1000) athos     (1000)     2697 2022-01-30 15:40:05.194732 lppa-0.2.1/PKG-INFO
--rw-rw-r--   0 athos     (1000) athos     (1000)     1962 2021-08-26 18:16:54.000000 lppa-0.2.1/README.md
-drwxrwxr-x   0 athos     (1000) athos     (1000)        0 2022-01-30 15:40:05.194732 lppa-0.2.1/lppa/
--rw-rw-r--   0 athos     (1000) athos     (1000)     1714 2022-01-30 15:30:01.000000 lppa-0.2.1/lppa/__init__.py
--rw-rw-r--   0 athos     (1000) athos     (1000)      718 2021-08-26 18:16:54.000000 lppa-0.2.1/lppa/__main__.py
--rw-rw-r--   0 athos     (1000) athos     (1000)     3097 2021-08-26 18:16:54.000000 lppa-0.2.1/lppa/auth.py
--rw-rw-r--   0 athos     (1000) athos     (1000)     3792 2022-01-28 14:08:33.000000 lppa-0.2.1/lppa/cli.py
--rw-rw-r--   0 athos     (1000) athos     (1000)     5163 2022-01-28 13:56:28.000000 lppa-0.2.1/lppa/ppa.py
--rw-rw-r--   0 athos     (1000) athos     (1000)     2188 2021-08-26 18:16:54.000000 lppa-0.2.1/lppa/processors.py
--rw-rw-r--   0 athos     (1000) athos     (1000)      954 2021-08-26 18:16:54.000000 lppa-0.2.1/lppa/utils.py
-drwxrwxr-x   0 athos     (1000) athos     (1000)        0 2022-01-30 15:40:05.194732 lppa-0.2.1/lppa.egg-info/
--rw-rw-r--   0 athos     (1000) athos     (1000)     2697 2022-01-30 15:40:05.000000 lppa-0.2.1/lppa.egg-info/PKG-INFO
--rw-rw-r--   0 athos     (1000) athos     (1000)      316 2022-01-30 15:40:05.000000 lppa-0.2.1/lppa.egg-info/SOURCES.txt
--rw-rw-r--   0 athos     (1000) athos     (1000)        1 2022-01-30 15:40:05.000000 lppa-0.2.1/lppa.egg-info/dependency_links.txt
--rw-rw-r--   0 athos     (1000) athos     (1000)       39 2022-01-30 15:40:05.000000 lppa-0.2.1/lppa.egg-info/entry_points.txt
--rw-rw-r--   0 athos     (1000) athos     (1000)       22 2022-01-30 15:40:05.000000 lppa-0.2.1/lppa.egg-info/requires.txt
--rw-rw-r--   0 athos     (1000) athos     (1000)        5 2022-01-30 15:40:05.000000 lppa-0.2.1/lppa.egg-info/top_level.txt
--rw-rw-r--   0 athos     (1000) athos     (1000)      250 2021-08-30 21:04:13.000000 lppa-0.2.1/pyproject.toml
--rw-rw-r--   0 athos     (1000) athos     (1000)      954 2022-01-30 15:40:05.198732 lppa-0.2.1/setup.cfg
+drwxrwxr-x   0 athos     (1000) athos     (1000)        0 2024-04-21 12:31:31.876019 lppa-0.3.0/
+-rw-rw-r--   0 athos     (1000) athos     (1000)     1676 2024-04-21 12:31:28.000000 lppa-0.3.0/CHANGELOG.md
+-rw-rw-r--   0 athos     (1000) athos     (1000)    35149 2021-04-28 01:25:44.000000 lppa-0.3.0/LICENSE
+-rw-rw-r--   0 athos     (1000) athos     (1000)       59 2022-02-04 09:13:19.000000 lppa-0.3.0/MANIFEST.in
+-rw-rw-r--   0 athos     (1000) athos     (1000)     1777 2022-09-12 19:41:41.000000 lppa-0.3.0/Makefile
+-rw-r--r--   0 athos     (1000) athos     (1000)     3945 2024-04-21 12:31:31.876019 lppa-0.3.0/PKG-INFO
+-rw-rw-r--   0 athos     (1000) athos     (1000)     2788 2024-04-21 04:44:47.000000 lppa-0.3.0/README.md
+drwxrwxr-x   0 athos     (1000) athos     (1000)        0 2024-04-21 12:31:31.875019 lppa-0.3.0/lppa/
+-rw-rw-r--   0 athos     (1000) athos     (1000)     1714 2024-04-21 12:31:28.000000 lppa-0.3.0/lppa/__init__.py
+-rw-rw-r--   0 athos     (1000) athos     (1000)      718 2021-08-24 12:10:55.000000 lppa-0.3.0/lppa/__main__.py
+-rw-rw-r--   0 athos     (1000) athos     (1000)     3097 2021-08-24 12:09:30.000000 lppa-0.3.0/lppa/auth.py
+-rw-rw-r--   0 athos     (1000) athos     (1000)     3856 2024-04-21 04:50:22.000000 lppa-0.3.0/lppa/cli.py
+-rw-rw-r--   0 athos     (1000) athos     (1000)      943 2023-11-28 22:14:03.000000 lppa-0.3.0/lppa/constants.py
+-rw-rw-r--   0 athos     (1000) athos     (1000)     5123 2022-02-08 18:19:08.000000 lppa-0.3.0/lppa/ppa.py
+-rw-rw-r--   0 athos     (1000) athos     (1000)     2188 2021-08-24 12:11:33.000000 lppa-0.3.0/lppa/processors.py
+-rw-rw-r--   0 athos     (1000) athos     (1000)     1014 2024-04-05 12:58:30.000000 lppa-0.3.0/lppa/utils.py
+drwxrwxr-x   0 athos     (1000) athos     (1000)        0 2024-04-21 12:31:31.876019 lppa-0.3.0/lppa.egg-info/
+-rw-r--r--   0 athos     (1000) athos     (1000)     3945 2024-04-21 12:31:31.000000 lppa-0.3.0/lppa.egg-info/PKG-INFO
+-rw-rw-r--   0 athos     (1000) athos     (1000)      489 2024-04-21 12:31:31.000000 lppa-0.3.0/lppa.egg-info/SOURCES.txt
+-rw-rw-r--   0 athos     (1000) athos     (1000)        1 2024-04-21 12:31:31.000000 lppa-0.3.0/lppa.egg-info/dependency_links.txt
+-rw-rw-r--   0 athos     (1000) athos     (1000)       38 2024-04-21 12:31:31.000000 lppa-0.3.0/lppa.egg-info/entry_points.txt
+-rw-rw-r--   0 athos     (1000) athos     (1000)       22 2024-04-21 12:31:31.000000 lppa-0.3.0/lppa.egg-info/requires.txt
+-rw-rw-r--   0 athos     (1000) athos     (1000)        5 2024-04-21 12:31:31.000000 lppa-0.3.0/lppa.egg-info/top_level.txt
+-rw-rw-r--   0 athos     (1000) athos     (1000)      333 2022-02-04 09:13:19.000000 lppa-0.3.0/pyproject.toml
+-rw-rw-r--   0 athos     (1000) athos     (1000)       45 2024-04-20 13:16:59.000000 lppa-0.3.0/requirements-dev.txt
+-rw-rw-r--   0 athos     (1000) athos     (1000)     1276 2024-04-21 12:31:31.877019 lppa-0.3.0/setup.cfg
+drwxrwxr-x   0 athos     (1000) athos     (1000)        0 2024-04-21 12:31:31.876019 lppa-0.3.0/tests/
+-rw-rw-r--   0 athos     (1000) athos     (1000)     2089 2021-08-24 12:12:59.000000 lppa-0.3.0/tests/test_auth.py
+-rw-rw-r--   0 athos     (1000) athos     (1000)     1971 2024-04-21 04:36:46.000000 lppa-0.3.0/tests/test_cli.py
+-rw-rw-r--   0 athos     (1000) athos     (1000)     2174 2024-04-20 23:45:21.000000 lppa-0.3.0/tests/test_ppa.py
+-rw-rw-r--   0 athos     (1000) athos     (1000)     2997 2021-08-24 12:13:39.000000 lppa-0.3.0/tests/test_processors.py
+-rw-rw-r--   0 athos     (1000) athos     (1000)     1217 2024-04-05 13:09:26.000000 lppa-0.3.0/tests/test_utils.py
```

### Comparing `lppa-0.2.1/LICENSE` & `lppa-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lppa-0.2.1/PKG-INFO` & `lppa-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,24 @@
-Metadata-Version: 2.1
-Name: lppa
-Version: 0.2.1
-Summary: Request PPAs for deb source packages
-Home-page: https://github.com/athos-ribeiro/lppa
-Author: Athos Ribeiro
-Author-email: athos.ribeiro@canonical.com
-License: GPLv3+
-Keywords: PPA,Ubuntu,Launchpad
-Platform: any
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# DISCONTINUED
+
+This has been discontinued in favor of
+[ppa-dev-tools](https://code.launchpad.net/~bryce/ppa-dev-tools/+git/ppa-dev-tools-1).
+
+While this is still useful for examples, I no longer intend to proceed with
+development for this tool. Please, use ppa-dev-tools instead.
 
 # lppa
 
-Command line tool to create Launchpad PPAs and push deb source packages to them
+Command line tool to create Launchpad PPAs and push deb source packages to them.
+
+While this tool is intended to be used by distribution developers who often
+need to prepare and push packages to test PPAs, this can also be used by
+developers who wish to distribute their software through PPAs. For the latter,
+please make sure to check the documentation since the default values are
+designed to enhance the former use cases.
 
 ## Installation
 
 ```
 pip install lppa
 ```
 
@@ -45,26 +38,28 @@
 To create a new PPA, run
 
 ```
 lppa create PPA_NAME [all|arch, ...]
 ```
 
 where arch is a Launchpad processor (you can pass multiple architectures here)
-or `all` to enable all available architectures.
+or `all` to enable all available architectures. If no architecture is passed,
+`all` is assumed.
 
 The currently available Launchpad processors are
 
 - amd64
 - arm64
 - s390x
 - ppc64el
 - armhf
 - armel
 - i386
 - powerpc
+- riscv64
 
 ### Delete an existing PPA
 
 ```
 lppa delete PPA_NAME
 ```
 
@@ -108,13 +103,16 @@
 $ workon lppa
 $ make devel
 $ make check
 ```
 
 ### Releasing
 
-- Change `lppa/__init__.py` to set the version to be published
-- Create a new git tag for the new version
-- Run `make publish` to build a new version and push it to PyPI
-- Change `lppa/__init__.py` to set the version to the next development version
+There is a `make release` target which will
 
+- Change `lppa/__init__.py` to set the version to be published
+- Update the CHANGELOG.md file with towncrier entries
+- Commit the changes above and tag the repository
+- Push the changes to PyPI (login required)
+- Add a final commit bumping the package version to a new development one
 
+Finally, a manual `git push` (including tags) is required.
```

### Comparing `lppa-0.2.1/lppa/__init__.py` & `lppa-0.3.0/lppa/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 import configparser
 import logging
 import sys
 
-__version__ = '0.2.1'
+__version__ = '0.3.0'
 
 _defaults = {
     'log_level': 'warning',
     'log_file': 'stderr',
     'api_version': 'devel',
     'app_name': 'lppa',
     'lp_env': 'production'  # or staging
```

### Comparing `lppa-0.2.1/lppa/__main__.py` & `lppa-0.3.0/lppa/__main__.py`

 * *Files identical despite different names*

### Comparing `lppa-0.2.1/lppa/auth.py` & `lppa-0.3.0/lppa/auth.py`

 * *Files identical despite different names*

### Comparing `lppa-0.2.1/lppa/cli.py` & `lppa-0.3.0/lppa/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,45 +13,44 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 import argparse
 
 from lppa.ppa import PPA
+import lppa.constants
 import lppa.utils
 
-DESCRIPTION = 'CLI for Handling launchpad PPAs'
-PROCESSORS = ['amd64', 'arm64', 's390x', 'ppc64el', 'armhf', 'armel', 'i386', 'powerpc']
-
 
 def create(args):
     pocket = 'Updates'
     if args.proposed:
         pocket = 'Proposed'
-    arches = args.processors or ['amd64', 'i386']
+    arches = args.processors or ['all']
     if 'all' in arches:
-        arches = PROCESSORS
-    elif any(arch not in PROCESSORS for arch in arches):
-        argparse.ArgumentParser.exit(-1, f'Invalid "{arches}" is not a subset of "{PROCESSORS}"')
+        arches = lppa.constants.PROCESSORS
+    elif any(arch not in lppa.constants.PROCESSORS for arch in arches):
+        argparse.ArgumentParser.exit(
+            -1, f'Invalid "{arches}" is not a subset of "{lppa.constants.PROCESSORS}"'
+        )
     archive = PPA(args.name, arches, pocket=pocket)
     archive.create()
     print(f'New PPA created: {args.name}')
     print(f'PPA Packages page: {archive.archive.web_link}/+packages')
     print('You can upload packages to this PPA using:')
     print(f'\t{archive.get_dput_str()}')
 
 
 def delete(args):
     archive = PPA(args.name, None)
     archive.delete()
 
 
 def list(args):
-    ppas = lppa.utils.ppa_list()
-    for ppa_name in ppas:
+    for ppa_name in lppa.utils.ppa_list():
         print(ppa_name)
 
 
 def info(args):
     archive = PPA(args.name, None)
     archive.set_existing_archive()
     if not archive.archive:
@@ -60,33 +59,35 @@
     print('You can upload packages to this PPA using:')
     print(f'\t{archive.get_dput_str()}')
     if args.verbose:
         print(f'"{archive.name}" is available for arches: {archive.get_processors()}')
 
 
 def run():
-    parser = argparse.ArgumentParser(description=DESCRIPTION)
+    parser = argparse.ArgumentParser(description=lppa.constants.CLI_DESCRIPTION)
+    parser.add_argument('--version', action='version', version=lppa.__version__)
 
     subparsers = parser.add_subparsers(help='sub-command help')
 
     parser_create = subparsers.add_parser('create', help='Create new PPA')
     parser_create.add_argument('name', help='Name of the PPA to be created')
     parser_create.add_argument(
         'processors',
         nargs='*',
-        # choices=PROCESSORS,
+        # choices=constants.PROCESSORS,
         help=(
             'List of launchpad processors to be enabled in the new PPA. Use "all" to enable all '
-            'architectures. If no value is provided, assume amd64 and i386'
+            'architectures. If no value is provided, assume all'
         )
     )
     parser_create.add_argument(
         '--proposed',
         help='Prefer build dependencies from the -proposed pocket',
-        action='store_true'
+        action=argparse.BooleanOptionalAction,
+        default=True
     )
     parser_create.set_defaults(func=create)
 
     parser_delete = subparsers.add_parser('delete', help='Delete existing PPA')
     parser_delete.add_argument('name', help='Name of the PPA to be deleted')
     parser_delete.set_defaults(func=delete)
```

### Comparing `lppa-0.2.1/lppa/ppa.py` & `lppa-0.3.0/lppa/ppa.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,43 +16,40 @@
 """
 import logging
 
 from lazr.restfulclient.errors import BadRequest, NotFound
 
 from lppa.auth import Session
 from lppa.processors import Processors
+import lppa.constants
 
 
 logger = logging.getLogger(__name__)
 
-DEFAULT_COMPONENT = 'multiverse'
-DEFAULT_POCKET = 'Updates'
-VALID_POCKETS = ('Updates', 'Proposed', 'Backports', 'Security', 'Release')
-
 
 class PPA():
     """Launchpad PPA manager class"""
-    def __init__(self, name, architectures, pocket=DEFAULT_POCKET):
+    def __init__(self, name, architectures, pocket=lppa.constants.DEFAULT_POCKET):
         """Initializer
 
         param name: str, the name for the PPA to be managed
         param architectures: list[str], list of launchpad processors, such as arm64
         param pocket: str, pocket for fetching build-dependencies from
         """
-        if pocket not in VALID_POCKETS:
-            raise ValueError(f'{pocket} not in {VALID_POCKETS}')
+        if pocket not in lppa.constants.VALID_POCKETS:
+            raise ValueError(f'{pocket} not in {lppa.constants.VALID_POCKETS}')
 
         self.name = name
         self.session = Session().get_session()
         self.me = self.session.me
         self.team = self.session.people[self.me.name]
         self.architectures = architectures
         self.archive = None
         self.pocket = pocket
-        self.component = DEFAULT_COMPONENT
+        self.component = lppa.constants.DEFAULT_COMPONENT
 
     def set_existing_archive(self):
         """Set the PPA archive interface if one already exists with the requested name"""
         try:
             self.archive = self.me.getPPAByName(name=self.name)
         except NotFound:
             logger.debug(
@@ -78,15 +75,15 @@
             )
         processors_api = Processors(session=self.session)
         processor_urls = []
         for arch in self.architectures:
             logger.debug('Fetching processor url for "%s"', arch)
             processor_urls.append(processors_api.get_by_name(arch).self_link)
         self.archive.setProcessors(processors=processor_urls)
-        if self.pocket != DEFAULT_POCKET:
+        if self.pocket != lppa.constants.DEFAULT_POCKET:
             ubuntu = self.archive.distribution
             self.archive.addArchiveDependency(
                 dependency=ubuntu.main_archive,
                 component=self.component,
                 pocket=self.pocket
             )
         logger.info(
```

### Comparing `lppa-0.2.1/lppa/processors.py` & `lppa-0.3.0/lppa/processors.py`

 * *Files identical despite different names*

### Comparing `lppa-0.2.1/lppa/utils.py` & `lppa-0.3.0/lppa/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,11 +19,13 @@
 from lppa.auth import Session
 
 
 def ppa_list():
     session = Session().get_session()
     me = session.me
     ppas_url = me.ppas_collection_link
-    r = requests.get(ppas_url)
-    ppas = r.json()
-    ppa_names = [ppa['name'] for ppa in ppas['entries']]
-    return sorted(ppa_names)
+    while ppas_url:
+        r = requests.get(ppas_url)
+        ppas = r.json()
+        ppas_url = ppas.get('next_collection_link')
+        for ppa in ppas['entries']:
+            yield ppa['name']
```

### Comparing `lppa-0.2.1/setup.cfg` & `lppa-0.3.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 [metadata]
 name = lppa
 version = attr: lppa.__version__
 description = Request PPAs for deb source packages
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/athos-ribeiro/lppa
+project_urls = 
+	Changelog = https://github.com/athos-ribeiro/lppa/blob/main/CHANGELOG.md
+	Bug Tracker = https://github.com/athos-ribeiro/lppa/issues
+	Source Code = https://github.com/athos-ribeiro/lppa
 license = GPLv3+
 license_files = LICENSE
 platform = any
 author = Athos Ribeiro
 author_email = athos.ribeiro@canonical.com
 keywords = 
 	PPA
 	Ubuntu
 	Launchpad
 classifiers = 
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: 3 :: Only
 
 [options.entry_points]
 console_scripts = 
 	lppa = lppa.cli:run
 
 [options]
```

