# Comparing `tmp/sedrila-0.7.0.tar.gz` & `tmp/sedrila-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sedrila-0.7.0.tar", max compression
+gzip compressed data, was "sedrila-1.0.0.tar", max compression
```

## Comparing `sedrila-0.7.0.tar` & `sedrila-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1108 2022-11-04 08:14:04.746613 sedrila-0.7.0/LICENSE
--rwxr-xr-x   0        0        0     4087 2024-03-25 11:31:56.923322 sedrila-0.7.0/README.md
--rwxr-xr-x   0        0        0      622 2024-01-16 08:42:09.535422 sedrila-0.7.0/baseresources/favicon-32x32.png
--rwxr-xr-x   0        0        0       79 2024-01-06 12:00:53.054430 sedrila-0.7.0/baseresources/local.css
--rwxr-xr-x   0        0        0     8057 2024-02-17 09:50:19.451320 sedrila-0.7.0/baseresources/sedrila.css
--rwxr-xr-x   0        0        0     1929 2023-12-21 08:14:44.888758 sedrila-0.7.0/baseresources/sidebar.js
--rwxr-xr-x   0        0        0     6607 2024-04-02 17:14:14.148211 sedrila-0.7.0/py/base.py
--rwxr-xr-x   0        0        0     3343 2024-03-19 08:47:22.086143 sedrila-0.7.0/py/git.py
--rwxr-xr-x   0        0        0       34 2022-11-17 11:17:31.396262 sedrila-0.7.0/py/sdrl/__init__.py
--rwxr-xr-x   0        0        0    24154 2024-03-26 13:26:44.008028 sedrila-0.7.0/py/sdrl/course.py
--rwxr-xr-x   0        0        0     9777 2024-03-14 17:40:26.435091 sedrila-0.7.0/py/sdrl/glossary.py
--rwxr-xr-x   0        0        0     1209 2024-03-28 09:55:55.453116 sedrila-0.7.0/py/sdrl/html.py
--rwxr-xr-x   0        0        0     3901 2024-04-02 13:32:41.301782 sedrila-0.7.0/py/sdrl/interactive.py
--rwxr-xr-x   0        0        0     8274 2024-03-27 15:01:39.014198 sedrila-0.7.0/py/sdrl/macros.py
--rwxr-xr-x   0        0        0     4604 2024-03-14 17:40:29.403549 sedrila-0.7.0/py/sdrl/markdown.py
--rwxr-xr-x   0        0        0     6059 2024-03-20 16:23:20.848908 sedrila-0.7.0/py/sdrl/part.py
--rwxr-xr-x   0        0        0     1504 2024-02-23 11:01:27.759372 sedrila-0.7.0/py/sdrl/participant.py
--rwxr-xr-x   0        0        0     1334 2023-11-22 14:11:46.025037 sedrila-0.7.0/py/sdrl/replacements.py
--rwxr-xr-x   0        0        0     8344 2024-04-02 17:08:18.901707 sedrila-0.7.0/py/sdrl/repo.py
--rwxr-xr-x   0        0        0       31 2024-01-24 12:48:05.392624 sedrila-0.7.0/py/sdrl/subcmd/__init__.py
--rwxr-xr-x   0        0        0    26282 2024-04-02 16:56:24.340593 sedrila-0.7.0/py/sdrl/subcmd/author.py
--rwxr-xr-x   0        0        0     8508 2024-04-02 13:32:41.354363 sedrila-0.7.0/py/sdrl/subcmd/instructor.py
--rwxr-xr-x   0        0        0     5959 2024-03-26 13:02:02.723848 sedrila-0.7.0/py/sdrl/subcmd/student.py
--rwxr-xr-x   0        0        0      975 2024-02-24 16:55:02.006852 sedrila-0.7.0/py/sedrila.py
--rwxr-xr-x   0        0        0     2329 2024-04-02 17:14:14.141110 sedrila-0.7.0/pyproject.toml
--rwxr-xr-x   0        0        0     1546 2024-03-20 16:45:46.286389 sedrila-0.7.0/templates/base.html
--rwxr-xr-x   0        0        0      198 2023-12-21 08:24:47.653800 sedrila-0.7.0/templates/chapter.html
--rwxr-xr-x   0        0        0      154 2024-01-05 15:47:36.097811 sedrila-0.7.0/templates/glossary.html
--rwxr-xr-x   0        0        0      158 2023-12-21 08:24:47.628801 sedrila-0.7.0/templates/homepage.html
--rwxr-xr-x   0        0        0      312 2024-03-20 16:41:25.421337 sedrila-0.7.0/templates/task.html
--rwxr-xr-x   0        0        0      159 2023-12-21 08:24:47.660799 sedrila-0.7.0/templates/taskgroup.html
--rw-r--r--   0        0        0    11173 1970-01-01 00:00:00.000000 sedrila-0.7.0/setup.py
--rw-r--r--   0        0        0     5519 1970-01-01 00:00:00.000000 sedrila-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2022-11-04 08:14:04.746613 sedrila-1.0.0/LICENSE
+-rwxr-xr-x   0        0        0     4087 2024-03-25 11:31:56.923322 sedrila-1.0.0/README.md
+-rwxr-xr-x   0        0        0      622 2024-01-16 08:42:09.535422 sedrila-1.0.0/baseresources/favicon-32x32.png
+-rwxr-xr-x   0        0        0       79 2024-01-06 12:00:53.054430 sedrila-1.0.0/baseresources/local.css
+-rwxr-xr-x   0        0        0     7882 2024-04-04 09:44:27.185644 sedrila-1.0.0/baseresources/sedrila.css
+-rwxr-xr-x   0        0        0     1929 2023-12-21 08:14:44.888758 sedrila-1.0.0/baseresources/sidebar.js
+-rwxr-xr-x   0        0        0     6607 2024-04-21 11:40:26.114889 sedrila-1.0.0/py/base.py
+-rwxr-xr-x   0        0        0     3501 2024-04-09 14:20:20.887078 sedrila-1.0.0/py/git.py
+-rwxr-xr-x   0        0        0       34 2022-11-17 11:17:31.396262 sedrila-1.0.0/py/sdrl/__init__.py
+-rwxr-xr-x   0        0        0    23598 2024-04-19 08:43:39.210978 sedrila-1.0.0/py/sdrl/course.py
+-rwxr-xr-x   0        0        0     9777 2024-03-14 17:40:26.435091 sedrila-1.0.0/py/sdrl/glossary.py
+-rwxr-xr-x   0        0        0     1209 2024-03-28 09:55:55.453116 sedrila-1.0.0/py/sdrl/html.py
+-rwxr-xr-x   0        0        0     3901 2024-04-02 13:32:41.301782 sedrila-1.0.0/py/sdrl/interactive.py
+-rwxr-xr-x   0        0        0     8274 2024-03-27 15:01:39.014198 sedrila-1.0.0/py/sdrl/macros.py
+-rwxr-xr-x   0        0        0     3889 2024-04-03 09:22:13.806872 sedrila-1.0.0/py/sdrl/markdown.py
+-rwxr-xr-x   0        0        0     6222 2024-04-09 14:20:22.676239 sedrila-1.0.0/py/sdrl/part.py
+-rwxr-xr-x   0        0        0     1504 2024-02-23 11:01:27.759372 sedrila-1.0.0/py/sdrl/participant.py
+-rwxr-xr-x   0        0        0     1334 2023-11-22 14:11:46.025037 sedrila-1.0.0/py/sdrl/replacements.py
+-rwxr-xr-x   0        0        0     8344 2024-04-02 17:08:18.901707 sedrila-1.0.0/py/sdrl/repo.py
+-rwxr-xr-x   0        0        0       31 2024-01-24 12:48:05.392624 sedrila-1.0.0/py/sdrl/subcmd/__init__.py
+-rwxr-xr-x   0        0        0    28066 2024-04-19 14:16:39.062499 sedrila-1.0.0/py/sdrl/subcmd/author.py
+-rwxr-xr-x   0        0        0     8890 2024-04-09 14:20:20.925497 sedrila-1.0.0/py/sdrl/subcmd/instructor.py
+-rwxr-xr-x   0        0        0     5959 2024-03-26 13:02:02.723848 sedrila-1.0.0/py/sdrl/subcmd/student.py
+-rwxr-xr-x   0        0        0      975 2024-02-24 16:55:02.006852 sedrila-1.0.0/py/sedrila.py
+-rwxr-xr-x   0        0        0     2329 2024-04-21 11:40:26.103419 sedrila-1.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1546 2024-03-20 16:45:46.286389 sedrila-1.0.0/templates/base.html
+-rwxr-xr-x   0        0        0      198 2023-12-21 08:24:47.653800 sedrila-1.0.0/templates/chapter.html
+-rwxr-xr-x   0        0        0      154 2024-01-05 15:47:36.097811 sedrila-1.0.0/templates/glossary.html
+-rwxr-xr-x   0        0        0      158 2023-12-21 08:24:47.628801 sedrila-1.0.0/templates/homepage.html
+-rwxr-xr-x   0        0        0      312 2024-03-20 16:41:25.421337 sedrila-1.0.0/templates/task.html
+-rwxr-xr-x   0        0        0      159 2023-12-21 08:24:47.660799 sedrila-1.0.0/templates/taskgroup.html
+-rw-r--r--   0        0        0    11173 1970-01-01 00:00:00.000000 sedrila-1.0.0/setup.py
+-rw-r--r--   0        0        0     5519 1970-01-01 00:00:00.000000 sedrila-1.0.0/PKG-INFO
```

### Comparing `sedrila-0.7.0/LICENSE` & `sedrila-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sedrila-0.7.0/README.md` & `sedrila-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sedrila-0.7.0/baseresources/favicon-32x32.png` & `sedrila-1.0.0/baseresources/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `sedrila-0.7.0/baseresources/sedrila.css` & `sedrila-1.0.0/baseresources/sedrila.css`

 * *Files 2% similar despite different names*

```diff
@@ -245,27 +245,14 @@
     content: " R";
 }
 
 .required-by-decoration::before {
     content: " r";
 }
 
-.profiles-decoration {
-    font-size: 90%;
-    font-style: oblique;
-}
-
-.profiles-decoration::before {
-    content: " (";
-}
-
-.profiles-decoration::after {
-    content: ")";
-}
-
 .nostage {}
 
 .stage-draft {
     background-color: #999;
 }
 
 .stage-alpha {
```

### Comparing `sedrila-0.7.0/baseresources/sidebar.js` & `sedrila-1.0.0/baseresources/sidebar.js`

 * *Files identical despite different names*

### Comparing `sedrila-0.7.0/py/base.py` & `sedrila-1.0.0/py/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import requests
 import rich
 import rich.table
 import yaml
 
 
-SEDRILA_VERSION = "0.7.0"  # keep in sync with pyproject.toml
+SEDRILA_VERSION = "1.0.0"  # keep in sync with pyproject.toml
 CONFIG_FILENAME = "sedrila.yaml"  # at top-level of source dir
 GLOSSARY_BASENAME = "glossary"  # .md at top-level of chapterdir, .html in build directory
 METADATA_FILE = "course.json"  # at top-level of build directory
 CACHE_FILE = "course.pickle"  # at top-level of instructor build directory
 TEMPLATES_DIR = "templates"
 SEDRILA_COMMAND_ENV = "SEDRILA_COMMAND"
```

### Comparing `sedrila-0.7.0/py/git.py` & `sedrila-1.0.0/py/git.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,14 +77,19 @@
     os.system("git pull --ff-only")
 
 
 def push():
     os.system("git push")
 
 
+def remote_url():
+    result = sp.run(["git", "config", "--get", "remote.origin.url"], stdout=sp.PIPE)
+    return result.stdout.decode("utf-8").strip()
+
+    
 def username_from_repo_url(repo_url: str) -> str:
     # a repo_url is git@server:useraccount/reponame.git or git@server:useraccount/subset/reponame.git
     repo_url_regexp = r":([\w_\.-]+)/"
     mm = re.search(repo_url_regexp, repo_url)
     if repo_url.startswith("http") or not mm:
         #for testing purposes, local paths are allowed but default to the current user
         if os.path.isdir(repo_url):
```

### Comparing `sedrila-0.7.0/py/sdrl/course.py` & `sedrila-1.0.0/py/sdrl/course.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 Otherwise, 'read_contentfiles' is false and metadata comes from METADATA_FILE. 
 """
 import dataclasses
 import enum
 import functools
 import glob
 import graphlib
-import math
 import numbers
 import os
 import re
 import typing as tg
 
 import base as b
 import sdrl.glossary as glossary
@@ -35,15 +34,14 @@
     timevalue: tg.Union[int, float]  # task timevalue: (in hours)
     difficulty: int  # difficulty: int from DIFFICULTY_RANGE
     explains: list[str] = []  # terms (for backlinks in glossary)
     assumes: list[str] = []  # tasknames: This knowledge is assumed to be present
     requires: list[str] = []  # tasknames: These specific results will be reused here
     assumed_by: list[str] = []  # tasknames: inverse of assumes
     required_by: list[str] = []  # tasknames: inverse of requires
-    profiles: list[str] = []  # profile shortnames: specialty areas task pertains to
     workhours: float = 0.0  # time student has worked on this according to commit msgs
     accepted: bool = False  # whether instructor has ever marked it 'accept'
     rejections: int = 0  # how often instructor has marked it 'reject'
 
     taskgroup: 'Taskgroup'  # where the task belongs
 
     @property
@@ -74,49 +72,48 @@
         refs = (self._taskrefs('assumed_by') + self._taskrefs('required_by') +
                 self._taskrefs('assumes') + self._taskrefs('requires'))
         return f"<a {href} {titleattr}>{self.slug}</a> {diffsymbol} {timevalue}{refs}"
 
     def as_json(self) -> b.StrAnyDict:
         return dict(slug=self.slug,
                     title=self.title, timevalue=self.timevalue, difficulty=self.difficulty,
-                    assumes=self.assumes, requires=self.requires, profiles=self.profiles)
+                    assumes=self.assumes, requires=self.requires)
 
     def from_file(self, file: str, taskgroup: 'Taskgroup') -> 'Task':
         """Initializer used in author mode"""
         self.read_partsfile(file)
         # ----- get taskdata from file:
         nameparts = os.path.basename(self.sourcefile).split('.')
         assert len(nameparts) == 2  # taskname, suffix 'md'
         self.slug = nameparts[0]  # must be globally unique
         self.outputfile = f"{self.slug}.html"
         b.copyattrs(file,
                     self.metadata, self,
                     mustcopy_attrs='title, timevalue, difficulty',
-                    cancopy_attrs='stage, explains, assumes, requires, profiles',  # TODO 2: check profiles against sedrila.yaml
+                    cancopy_attrs='stage, explains, assumes, requires',
                     mustexist_attrs='',
                     typecheck=dict(timevalue=numbers.Number, difficulty=int))
         self.evaluate_stage(file, taskgroup.chapter.course)
         taskgroup.chapter.course.namespace_add(self.sourcefile, self)
 
-        # ----- ensure assumes/requires/profiles are lists:
+        # ----- ensure explains/assumes/requires are lists:
         def _handle_strlist(attrname: str):
             attrvalue = getattr(self, attrname)
             if isinstance(attrvalue, str):
                 setattr(self, attrname, re.split(r", *", attrvalue))
             elif not attrvalue:
                 setattr(self, attrname, [])
             else:
                 msg = f"'{file}': value of '%s:' must be a (non-empty) string"
                 b.error(msg % attrname)
                 setattr(self, attrname, [])
 
-        _handle_strlist('assumes')
         _handle_strlist('explains')
+        _handle_strlist('assumes')
         _handle_strlist('requires')
-        _handle_strlist('profiles')
 
         # ----- add to glossary:
         if self.explains:
             for term in self.explains:
                 taskgroup.chapter.course.glossary.explains(self.slug, term)
                 
         # ----- done:
@@ -127,15 +124,14 @@
         self.taskgroup = taskgroup
         self.slug = task['slug']
         self.title = task['title']
         self.timevalue = task['timevalue']
         self.difficulty = task['difficulty']
         self.assumes = task['assumes']
         self.requires = task['requires']
-        self.profiles = task['profiles']
         return self
 
     def _taskrefs(self, attr_name: str) -> str:
         """Create a toc link dedoration for one set of related tasks."""
         attr_cssclass = "%s-decoration" % attr_name.replace("_", "-")
         attr_label = attr_name.replace("_", " ")
         refslist = getattr(self, attr_name)
@@ -182,20 +178,20 @@
       Will then read all content for a build.
     - From a metadata file generated during build (read_contentfiles=False)
       for bookkeeping/reporting.
     """
     configfile: str
     breadcrumb_title: str
     baseresourcedir: str = f"{sedrila_libdir}/baseresources"
-    chapterdir: str = 'ch'
+    chapterdir: str
+    altdir: str
     templatedir: str = f"{sedrila_libdir}/templates"
     blockmacro_topmatter: dict[str, str]
     instructors: list[b.StrAnyDict]
     htaccess_template: str = None  # structure of .htaccess file generated in instructor website
-    profiles: list[str]  # list of all allowed profile shortnames
     chapters: list['Chapter']
     stages: list[str]  # list of allowed values of stage in parts 
 
     namespace: dict[str, part.Structurepart]  # the parts known so far
     include_stage: str  # lowest stage that parts must have to be included in output
     include_stage_index: int  # index in stages list, or len(stages) if include_stage is ""
     cache_mode: CacheMode
@@ -212,16 +208,17 @@
     glossary: glossary.Glossary
 
     def __init__(self, configfile: str, read_contentfiles: bool, include_stage: str):
         self.configfile = self.sourcefile = configfile
         configdict = b.slurp_yaml(configfile)
         b.copyattrs(configfile, 
                     configdict, self,
-                    mustcopy_attrs='title, breadcrumb_title, instructors, profiles, stages, allowed_attempts',
-                    cancopy_attrs=('baseresourcedir, chapterdir, templatedir, '
+                    mustcopy_attrs=('title, breadcrumb_title, chapterdir, altdir, '
+                                    'instructors, stages, allowed_attempts'),
+                    cancopy_attrs=('baseresourcedir, templatedir, '
                                    'blockmacro_topmatter, htaccess_template, init_data'),
                     mustexist_attrs='chapters')
         self.allowed_attempts_base, self.allowed_attempts_hourly = self._parse_allowed_attempts()
         self.slug = self.breadcrumb_title
         self.outputfile = "index.html"
         self.namespace = dict()
         self.namespace_add(configfile, self)
@@ -265,21 +262,18 @@
             if t.slug in result:
                 b.error(f"duplicate task: '{t.sourcefile}'\t'{result[t.slug].sourcefile}'")
             else:
                 result[t.slug] = t
         return result
 
     def as_json(self) -> b.StrAnyDict:
-        result = dict(baseresourcedir=self.baseresourcedir, 
+        result = dict(title=self.title,
                       breadcrumb_title=self.breadcrumb_title,
-                      stages=self.stages,
-                      chapterdir=self.chapterdir,
-                      templatedir=self.templatedir,
+                      chapterdir="", altdir="",  stages=[],  # are mustcopy_attrs but are not needed
                       instructors=self.instructors,
-                      profiles=self.profiles,
                       init_data=self.init_data,
                       allowed_attempts=self.allowed_attempts,
                       chapters=[chapter.as_json() for chapter in self.chapters])
         result.update(super().as_json())
         return result
 
     def chapter(self, slug: str) -> tg.Optional['Chapter']:
@@ -382,17 +376,14 @@
             b.debug(f"Task '{task.slug}'\tassumes {task.assumes},\trequires {task.requires}")
             for assumed in task.assumes:
                 if not self._task_or_taskgroup_exists(assumed):
                     b.error(f"{task.slug}:\t assumed task or taskgroup '{assumed}' does not exist")
             for required in task.requires:
                 if not self._task_or_taskgroup_exists(required):
                     b.error(f"{task.slug}:\t required task or taskgroup '{required}' does not exist")
-            for profile in task.profiles:
-                if profile not in self.profiles:
-                    b.error(f"{task.slug}:\t profile '{profile}' does not exist")
 
     def _compute_taskorder(self):
         """
         Set self.taskorder such that it respects the 'assumes' and 'requires'
         dependencies globally (across all taskgroups and chapters).
         The attribute will be used for ordering the tasks when rendering a taskgroup.
         """
```

### Comparing `sedrila-0.7.0/py/sdrl/glossary.py` & `sedrila-1.0.0/py/sdrl/glossary.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.7.0/py/sdrl/html.py` & `sedrila-1.0.0/py/sdrl/html.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.7.0/py/sdrl/interactive.py` & `sedrila-1.0.0/py/sdrl/interactive.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.7.0/py/sdrl/macros.py` & `sedrila-1.0.0/py/sdrl/macros.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.7.0/py/sdrl/markdown.py` & `sedrila-1.0.0/py/sdrl/markdown.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 # see bottom for initialization code
 
 
 class SedrilaExtension(mde.Extension):
     def extendMarkdown(self, md):
         md.preprocessors.register(SedrilaPreprocessor(md), 'sedrila_preprocessor', 50)
-        md.treeprocessors.register(AdmonitionFilter(md), "admonition_filter", 100)
         md.postprocessors.register(SedrilaPostprocessor(md), 'sedrila_postprocessor', 10)
 
 
 class SedrilaPreprocessor(mdpre.Preprocessor):
     def run(self, lines: list[str]) -> list[str]:
         content = "\n".join(lines)  # we work on the entire markup at once
         content = self.perhaps_suppress_instructorinfo(content)  
@@ -49,24 +48,14 @@
 
 class SedrilaPostprocessor(mdpost.Postprocessor):
     def run(self, text: str) -> str:
         text = macros.expand_macros(self.md.context_sourcefile, self.md.partname, text)
         return text
 
 
-class AdmonitionFilter(mdt.Treeprocessor):
-    def run(self, root):
-        """Removes admonition div blocks not to be shown in current self.mode."""
-        for divparent in root.findall('.//div/..'):  # sadly, etree does not support contains()
-            for div in divparent.findall('div'):
-                classes = div.attrib.get('class', '')
-                if 'admonition' in classes and 'instructor' in classes and self.md.mode != b.Mode.INSTRUCTOR:
-                    divparent.remove(div)  # show  !!! instructor  blocks only in instructor mode
-
-
 class SedrilaMarkdown(markdown.Markdown):
     mode: macros.MM
     context_sourcefile: str
     partname: str
     blockmacro_topmatter: dict[str, str]
 
 
@@ -82,18 +71,17 @@
     md.blockmacro_topmatter = blockmacro_topmatter
     return md.reset().convert(markdown_markup)
 
 
 # ######### initialization:
 
 extensions = [SedrilaExtension(), 
-              'admonition', 'attr_list', 'codehilite', 'fenced_code',
+              'attr_list', 'codehilite', 'fenced_code',
               'sane_lists', 'toc', 'smarty',
              ]
-# https://python-markdown.github.io/extensions/admonition/
 # https://python-markdown.github.io/extensions/attr_list/
 # https://python-markdown.github.io/extensions/code_hilite/
 # https://python-markdown.github.io/extensions/fenced_code_blocks/
 # https://python-markdown.github.io/extensions/sane_lists/
 # https://python-markdown.github.io/extensions/smarty/
 # https://python-markdown.github.io/extensions/toc/
 # https://github.com/daGrevis/mdx_linkify  breaks the correct handling of `a < b` and cannot be used
```

### Comparing `sedrila-0.7.0/py/sdrl/part.py` & `sedrila-1.0.0/py/sdrl/part.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,19 +30,26 @@
     title: str  # title: value
     linkslist_top: str = ''  # generated HTML of cross reference links
     linkslist_bottom: str = ''  # generated HTML of cross reference links
     stage: str = ''  # stage: value
     skipthis: bool  # do not include this chapter/taskgroup/task in generated site
     toc: str  # table of contents
 
+    def __repr__(self):
+        return self.slug
+
     @property
     def breadcrumb_item(self) -> str:
         return "(undefined)"
 
     @property
+    def to_be_skipped(self) -> bool:
+        return ...  # defined in concrete part classes
+
+    @property
     def toc_entry(self) -> str:
         classes = f"stage-{self.stage}" if self.stage else "no-stage"
         return h.indented_block(self.toc_link_text, self.TOC_LEVEL, classes)
 
     @property
     def toc_link_text(self) -> str:
         titleattr = f"title=\"{self.title}\""
@@ -95,26 +102,28 @@
 
 
 class Zipdir(Structurepart):
     """
     Turn directories named ch/mychapter/mytaskgroup/myzipdir.zip 
     containing a tree of files, say, myfile.txt
     into an output file myzipdir.zip
-    that contains mychapter/mytaskgroup/myzipdir/myfile.txt.  
+    that contains myzipdir/myfile.txt.  
     """
     innerpath: str  # relative pathname of the zipdir, to be re-created in the ZIP archive
 
     def __init__(self, dirprefix: str, dirname: str, outputdir: str):
         assert dirname.startswith(dirprefix)
         assert dirname[-1] != '/'  # dirprefix must not end with a slash, else our logic would break
         self.sourcefile = dirname
         self.slug = self.title = self.outputfile = os.path.basename(dirname)  # e.g. myfile.zip
-        bareslug = self.slug[:-4]  # e.g. myfile
-        innerpath1 = os.path.dirname(dirname).replace(dirprefix+'/', '', 1)
-        self.innerpath = f"{innerpath1}/{bareslug}"
+        self.innerpath = self.slug[:-len(".zip")]  # e.g. myfile
+
+    @property
+    def to_be_skipped(self) -> bool:
+        return False  # TODO 3: should be skipped if no [PARTREF] to it exists anywhere
 
     def render(self, targetdir: str):
         with zipfile.ZipFile(f"{targetdir}/{self.outputfile}", mode='w') as archive:
             self._zip_the_files(archive)
 
     def _zip_the_files(self, archive: zipfile.ZipFile):
         for dirpath, dirnames, filenames in os.walk(self.sourcefile):
```

### Comparing `sedrila-0.7.0/py/sdrl/participant.py` & `sedrila-1.0.0/py/sdrl/participant.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.7.0/py/sdrl/replacements.py` & `sedrila-1.0.0/py/sdrl/replacements.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.7.0/py/sdrl/repo.py` & `sedrila-1.0.0/py/sdrl/repo.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.7.0/py/sdrl/subcmd/author.py` & `sedrila-1.0.0/py/sdrl/subcmd/author.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import functools
 import glob
 import html
 import json
 import os
 import os.path
 import pickle
+import re
 import shutil
 import typing as tg
 
 import jinja2
 
 import base as b
 import sdrl.course
@@ -20,15 +21,15 @@
 import sdrl.part
 
 meaning = """Creates and renders an instance of a SeDriLa course.
 Checks consistency of the course description beforehands.
 """
 
 OUTPUT_INSTRUCTORS_DEFAULT_SUBDIR = "instructor"
-
+ALTDIR_KEYWORD = "ALT:"
 
 def add_arguments(subparser: argparse.ArgumentParser):
     subparser.add_argument('--config', metavar="configfile", default=b.CONFIG_FILENAME,
                            help="SeDriLa configuration description YAML file")
     subparser.add_argument('--include_stage', metavar="stage", default='',
                            help="include parts with this and higher 'stage:' entries in the generated output "
                                 "(default: only those with no stage)")
@@ -259,15 +260,15 @@
 def register_macros(course):
     MM = macros.MM
     b.info("registering macros")
     if course.cache_mode == sdrl.course.CacheMode.READ:
         course.glossary._register_macros_phase1()  # modifies state in module 'mocros'! 
     # ----- register EARLY-mode macros:
     macros.register_macro('INCLUDE', 1, MM.EARLY,
-                          expand_include)
+                          functools.partial(expand_include, course))
     # ----- register INNER-mode macros:
     macros.register_macro('HREF', 1, MM.INNER,
                           functools.partial(expand_href, course))  # show and link a URL
     macros.register_macro('PARTREF', 1, MM.INNER, 
                           functools.partial(expand_partref, course))  # slug as linktext
     macros.register_macro('PARTREFTITLE', 1, MM.INNER, 
                           functools.partial(expand_partref, course))  # title as linktext
@@ -390,35 +391,65 @@
     # markup matches that of expand_enumeration(), argument is not checked in any way
     macroname = macrocall.macroname
     classname = f"enumeration-{macroname.lower()}"
     value = macrocall.arg1
     return f"<span class='{classname}'>{value}</span>"
 
 
-def expand_include(macrocall: macros.Macrocall) -> str:
+def expand_include(course: sdrl.course.Course, macrocall: macros.Macrocall) -> str:
     """
     [INCLUDE::filename] inserts file contents into the Markdown text.
-    If the file has suffix *.md or *.md.inc, it is macro-expanded beforehands,
+    If the file has suffix *.md, it is macro-expanded beforehands,
     contents of all other files are inserted verbatim.
-    The filename is relative to the location of the file containing the macro call.
+    A relative filename is relative to the location of the file containing the macro call.
+    An absolute filename is relative to course.chapterdir.
+    The format [INCLUDE::ALT:filename] refers to files in course.altdir,
+    for relative names, the path from chapterdir to filename's dir is used below altdir.
+    In the special case [INCLUDE::ALT:] with no filename at all, the filename is reused as well.
     """
-    filename = macrocall.arg1
-    path = os.path.dirname(macrocall.filename)
-    fullfilename = os.path.join(path, filename)
+    fullfilename = includefile_path(course, macrocall)
+    # print(f"## fullfilename: {fullfilename} ({macrocall.filename})")
     if not os.path.exists(fullfilename):
-        macrocall.error(f"file '{fullfilename}' does not exist")
+        msgfunc = macrocall.warning if macrocall.arg1.startswith(ALTDIR_KEYWORD) else macrocall.error
+        msgfunc(f"file '{fullfilename}' does not exist")
         return ""
     with open(fullfilename, "rt", encoding='utf8') as f:
         rawcontent = f.read()
-    if filename.endswith('.md') or filename.endswith('.md.inc'):
+    if fullfilename.endswith('.md'):
         return macros.expand_macros(md.md.context_sourcefile, md.md.partname, rawcontent)
     else:
         return rawcontent
 
 
+def includefile_path(course: sdrl.course.Course, macrocall: macros.Macrocall) -> str:
+    arg_re = r"(?P<alt>" + ALTDIR_KEYWORD + r")?(?P<slash>/)?(?P<incfile>.*)"
+    mm = re.fullmatch(arg_re, macrocall.arg1)
+    is_alt = mm.group("alt") is not None
+    is_abs = mm.group("slash") is not None
+    inc_filepath = mm.group("incfile")
+    ctx_filepath = macrocall.filename  # e.g. ch/chapter/group/task.md
+    ctx_dirpath = os.path.dirname(ctx_filepath)  # e.g. ch/chapter/group
+    ctx_basename = os.path.basename(ctx_filepath)  # e.g. task.md
+    # print(f"## {macrocall.arg1} -> alt:{is_alt}, abs:{is_abs}, inc:{inc_filepath}, ctx:{ctx_dirpath}, {course.altdir}")
+    if is_alt:  # construct path in altdir tree:
+        abs_filepath = macrocall.filename.replace(course.chapterdir, course.altdir, 1)
+        abs_dirpath = os.path.dirname(abs_filepath)
+        # print(f"### is_alt: {abs_dirpath}")
+        if is_abs:
+            fullfilename = os.path.join(course.altdir, inc_filepath)
+        else:
+            fullfilename = os.path.join(abs_dirpath, inc_filepath or ctx_basename)
+    else:  # in chapterdir tree:
+        if is_abs:
+            fullfilename = os.path.join(course.chapterdir, inc_filepath)
+        else:
+            fullfilename = os.path.join(ctx_dirpath, inc_filepath)
+    return fullfilename
+
+
 def render_homepage(course: sdrl.course.Course, env, targetdir: str, mode: b.Mode):
     template = env.get_template("homepage.html")
     render_structure(course, template, course, targetdir, mode)
     course.render_zipdirs(targetdir)
 
 
 def render_chapter(chapter: sdrl.course.Chapter, env, targetdir: str, mode: b.Mode):
```

### Comparing `sedrila-0.7.0/py/sdrl/subcmd/instructor.py` & `sedrila-1.0.0/py/sdrl/subcmd/instructor.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     home_fallback = "."
     if os.environ.get(REPOS_HOME_VAR) is None:
         b.warning(f"Environment variable {REPOS_HOME_VAR} is not set. Assume current directory as student workdirs directory")
         if pargs.repo_url and os.path.isfile(sdrl.participant.PARTICIPANT_FILE):
             b.warning("It looks like you are already inside a student dir. Assuming parent directory instead.")
             home_fallback = ".."
     home = os.environ.get(REPOS_HOME_VAR) or home_fallback
-    checkout_student_repo(pargs.repo_url, home, pargs.get)
-    if not(pargs.put) and not(pargs.check):
+    checkout_success = checkout_student_repo(pargs.repo_url, home, pargs.get)
+    if not(pargs.put) and not(pargs.check) or not(checkout_success):
         os.chdir("..")
         return
     student = sdrl.participant.Student()
     metadatafile = f"{student.course_url}/{b.METADATA_FILE}"
     course = sdrl.course.Course(metadatafile, read_contentfiles=False, include_stage="")
     r.compute_student_work_so_far(course)
     entries, workhours_total, timevalue_total = r.student_work_so_far(course)
@@ -82,24 +82,32 @@
         username = git.username_from_repo_url(repo_url)
         os.chdir(home)
     if os.path.exists(username) or inrepo:
         if not(inrepo):
             os.chdir(username)
         b.info(f"**** pulling repo in existing directory '{os.getcwd()}'")
         if pull:
+            if repo_url:
+                existing = git.remote_url()
+                if repo_url != existing:
+                    print(repo_url)
+                    print(existing)
+                    b.error("user repo with other url already present. please resolve manually. aborting")
+                    return False
             git.pull()
         else:
             b.warning("not pulling user repo, relying on existing state")
     else:
         if not(pull):
             b.warning("attempted to grade non-existing user without pulling.")
             b.warning("ignore and clone regardless.")
         git.clone(repo_url, username)
         os.chdir(username)
         b.info(f"**** cloned repo into new directory '{os.getcwd()}'")
+    return True
 
 
 def rewrite_submission_file(course: sdrl.course.Course, filename: str):
     """Checks status of entries and inserts different marks where needed."""
     entries = b.slurp_yaml(filename)
     rewrite_submission_entries(course, entries)
     b.spit_yaml(filename, entries)
```

### Comparing `sedrila-0.7.0/py/sdrl/subcmd/student.py` & `sedrila-1.0.0/py/sdrl/subcmd/student.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.7.0/py/sedrila.py` & `sedrila-1.0.0/py/sedrila.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.7.0/pyproject.toml` & `sedrila-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # https://packaging.python.org/en/latest/
 # https://packaging.python.org/en/latest/specifications/pyproject-toml/
 # https://packaging.python.org/en/latest/guides/writing-pyproject-toml/
 # https://python-poetry.org/docs/pyproject/
 [tool.poetry]
 name = "sedrila"
-version = "0.7.0"  # keep in sync with base.py
+version = "1.0.0"  # keep in sync with base.py
 description = "Tool infrastructure for building and running \"self-driven lab\" courses"
 license = "MIT"
 authors = ["Lutz Prechelt <prechelt@inf.fu-berlin.de>"]
 readme = "README.md"
 homepage = "https://github.com/fubinf/sedrila"
 repository = "https://github.com/fubinf/sedrila"
 keywords = ["static site generator"]
```

### Comparing `sedrila-0.7.0/templates/base.html` & `sedrila-1.0.0/templates/base.html`

 * *Files identical despite different names*

### Comparing `sedrila-0.7.0/setup.py` & `sedrila-1.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
  'rich>=13.7,<14.0']
 
 entry_points = \
 {'console_scripts': ['sedrila = sedrila:main']}
 
 setup_kwargs = {
     'name': 'sedrila',
-    'version': '0.7.0',
+    'version': '1.0.0',
     'description': 'Tool infrastructure for building and running "self-driven lab" courses',
     'long_description': '[![Documentation Status](https://readthedocs.org/projects/sedrila/badge/?version=latest)](https://sedrila.readthedocs.io/en/latest/?badge=latest)\n\n# `sedrila`: Tool infrastructure for building and running "self-driven lab" courses\n\nA "self-driven lab" (SeDriLa) course is one where students select freely \na subset from a large set of tasks.\nThe tasks are described with sufficient detail that no guidance from an instructor\nis needed most of the time.\n\nsedrila is a command-line tool supporting course authors for authoring a course\nand then course instructors and students for executing it.\n\nFind the [documentation at readthedocs](https://sedrila.readthedocs.io).\n\n\n## Ideas for future versions\n\n- Process `SEDRILA_INSTRUCTOR_COURSE_URLS` as described in the instructor documentation.\n- `sedrila instructor` should keep a JSON file `student_course_urls.json` that maps student usernames\n  to the course URL first seen for that student, because if a student ever changed\n  the URL in the `student.yaml`, prior signed commits of instructors might become \n  invalid semantically if the new course has a different set of tasks.  \n  The map is added to when a `student.yaml` is first seen\n  and checked against at each later time.  \n  Note that a student taking part a second time, with a fresh repo,\n  might require manual editing of that JSON file to remove that entry.\n- Better yet, there could be an option `sedrial instructor --allow-repo2` that \n  performs that editing automatically\n  and also checks that the new repo contains no instructor-signed commits.\n- Command `sedrila instructor --clean-up-repos-home`\n  to clean up instructor work directory trees-of-trees\n  by deleting all level-1 subtrees in which the `student.yaml`\n  has a `course_url` that is not mentioned in the \n  `SEDRILA_INSTRUCTOR_COURSE_URLS`environment variable.\n  This option should ask a safety question before starting to work.\n\n\n## Development process: TODO-handling during development\n\nWe use this convention for the development of `sedrila`.\nIt may also be helpful for course authors if the team is small enough.\n\nIf something is incomplete, add a TODO marker with a priorization digit:\n- `TODO 1`: to be completed soon (within a few days)\n- `TODO 2`: to be completed once the prio 1 things are done (within days or a few weeks)\n- `TODO 3`: to be completed at some later time (usually several weeks or more into the future,\n  because it is big) or never (because it is not-so-important: "nice-to-have features")\n\nAdd a short description of what needs to be done. Examples:\n- `TODO 1: find proper formulation`\n- `TODO 2: restructure to use ACME lib`\n- `TODO 3: add automatic grammar correction`\n\nIf you intend to do it yourself, add your name in parens:  \n`TODO 1: find proper formulation (Lutz)`\n\nThen use the IDE global search to work through these layer-by-layer.\nDemote items to a lower priority when they become stale or remove them.\nKick out prio 3 items when they become unlikely.\n\n\n## A currently needed refactoring: Target directory structure\n\nThe current layout of the source tree is wrong.\nCurrently, the `templates` and `baseresources` directories will end up \nas top-level directories when the package is installed,\nwhich means they will clash with any top-level modules of that name\nanywhere in our dependencies.\n\nWe need to perform the following refactorings to arrive at a proper structure:\n\n- `py` --> `sedrila`: This will be the top level directory that gets installed.\n- `sedrila/sdrl/*` --> `sedrila/*`: We remove the now-intermediate namespace.\n  This implies joining the current `sdrl/tests` into `sedrila/tests`.\n- `templates` --> `sedrila/templates`: The HTML templates simply become part of the\n  tree to be installed.\n- `baseresources` --> `sedrila/baseresources`: Ditto.\n\nThese changes require a lot of changes of import statements.\nFor instance, the current module `base` will become `sedrila.base`\nand `sdrl.course` will become `sedrila.course`.\nThe logic for computing `sedrila_libdir` in `courses.py` must be adapted.\nThe files lists in `pyproject.toml` must be corrected.\n',
     'author': 'Lutz Prechelt',
     'author_email': 'prechelt@inf.fu-berlin.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fubinf/sedrila',
```

### Comparing `sedrila-0.7.0/PKG-INFO` & `sedrila-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sedrila
-Version: 0.7.0
+Version: 1.0.0
 Summary: Tool infrastructure for building and running "self-driven lab" courses
 Home-page: https://github.com/fubinf/sedrila
 License: MIT
 Keywords: static site generator
 Author: Lutz Prechelt
 Author-email: prechelt@inf.fu-berlin.de
 Requires-Python: >=3.11,<4.0
```

