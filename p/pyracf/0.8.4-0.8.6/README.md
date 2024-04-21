# Comparing `tmp/pyracf-0.8.4.tar.gz` & `tmp/pyracf-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracf-0.8.4.tar", last modified: Tue Apr 16 21:33:11 2024, max compression
+gzip compressed data, was "pyracf-0.8.6.tar", last modified: Sun Apr 21 10:13:56 2024, max compression
```

## Comparing `pyracf-0.8.4.tar` & `pyracf-0.8.6.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-16 21:33:11.184994 pyracf-0.8.4/
--rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.8.4/LICENSE
--rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.8.4/MANIFEST.in
--rw-r--r--   0 henri     (1000) henri     (1000)    15118 2024-04-16 21:33:11.184994 pyracf-0.8.4/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)    14510 2024-04-16 21:31:02.000000 pyracf-0.8.4/README.md
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-16 21:33:11.184994 pyracf-0.8.4/setup.cfg
--rw-rw-r--   0 henri     (1000) henri     (1000)      956 2024-04-16 21:32:36.000000 pyracf-0.8.4/setup.py
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-16 21:33:11.184994 pyracf-0.8.4/src/
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-16 21:33:11.184994 pyracf-0.8.4/src/pyracf/
--rw-rw-r--   0 henri     (1000) henri     (1000)    56953 2024-04-16 21:31:08.000000 pyracf-0.8.4/src/pyracf/__init__.py
--rw-rw-r--   0 henri     (1000) henri     (1000)     1829 2024-04-15 10:15:48.000000 pyracf-0.8.4/src/pyracf/getOffsets.py
--rw-rw-r--   0 henri     (1000) henri     (1000)   253950 2024-04-15 10:15:48.000000 pyracf-0.8.4/src/pyracf/offsets.json
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-16 21:33:11.184994 pyracf-0.8.4/src/pyracf.egg-info/
--rw-r--r--   0 henri     (1000) henri     (1000)    15118 2024-04-16 21:33:11.000000 pyracf-0.8.4/src/pyracf.egg-info/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)      279 2024-04-16 21:33:11.000000 pyracf-0.8.4/src/pyracf.egg-info/SOURCES.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        1 2024-04-16 21:33:11.000000 pyracf-0.8.4/src/pyracf.egg-info/dependency_links.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-16 21:33:11.000000 pyracf-0.8.4/src/pyracf.egg-info/requires.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        7 2024-04-16 21:33:11.000000 pyracf-0.8.4/src/pyracf.egg-info/top_level.txt
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-21 10:13:56.502463 pyracf-0.8.6/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2024-04-21 09:03:17.000000 pyracf-0.8.6/LICENSE
+-rw-rw-r--   0 henri     (1000) henri     (1000)      172 2024-04-21 09:03:17.000000 pyracf-0.8.6/MANIFEST.in
+-rw-r--r--   0 henri     (1000) henri     (1000)    16873 2024-04-21 10:13:56.502463 pyracf-0.8.6/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)    16265 2024-04-21 09:03:17.000000 pyracf-0.8.6/README.md
+-rw-rw-r--   0 henri     (1000) henri     (1000)      161 2024-04-21 09:03:17.000000 pyracf-0.8.6/pyproject.toml
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-21 10:13:56.502463 pyracf-0.8.6/setup.cfg
+-rw-rw-r--   0 henri     (1000) henri     (1000)      956 2024-04-21 10:13:30.000000 pyracf-0.8.6/setup.py
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-21 10:13:56.498463 pyracf-0.8.6/src/
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-21 10:13:56.502463 pyracf-0.8.6/src/pyracf/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    61872 2024-04-21 10:02:25.000000 pyracf-0.8.6/src/pyracf/__init__.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)     1829 2024-04-21 09:03:17.000000 pyracf-0.8.6/src/pyracf/getOffsets.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)   253950 2024-04-21 09:03:17.000000 pyracf-0.8.6/src/pyracf/offsets.json
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-21 10:13:56.502463 pyracf-0.8.6/src/pyracf.egg-info/
+-rw-r--r--   0 henri     (1000) henri     (1000)    16873 2024-04-21 10:13:56.000000 pyracf-0.8.6/src/pyracf.egg-info/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)      412 2024-04-21 10:13:56.000000 pyracf-0.8.6/src/pyracf.egg-info/SOURCES.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        1 2024-04-21 10:13:56.000000 pyracf-0.8.6/src/pyracf.egg-info/dependency_links.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-21 10:13:56.000000 pyracf-0.8.6/src/pyracf.egg-info/requires.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        7 2024-04-21 10:13:56.000000 pyracf-0.8.6/src/pyracf.egg-info/top_level.txt
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-21 10:13:56.502463 pyracf-0.8.6/test/
+-rw-rw-r--   0 henri     (1000) henri     (1000)      794 2024-04-21 09:03:17.000000 pyracf-0.8.6/test/test_connect_df.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)     1461 2024-04-21 09:03:17.000000 pyracf-0.8.6/test/test_frame_dataset.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)     1504 2024-04-21 09:03:17.000000 pyracf-0.8.6/test/test_frame_general.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)     6654 2024-04-21 09:03:17.000000 pyracf-0.8.6/test/test_frames.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)      466 2024-04-21 09:03:17.000000 pyracf-0.8.6/test/test_parsed.py
```

### Comparing `pyracf-0.8.4/LICENSE` & `pyracf-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.4/PKG-INFO` & `pyracf-0.8.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.8.4
+Version: 0.8.6
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -29,14 +29,30 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
+### 0.8.5 (fixes for pickles, pytest, wiki)
+- parse_fancycli now creates empty data frames for pickles it could not find
+- index added to data frames from old pickles, not for pickles that already have index fields
+- pytest framework for QA in development cycle, initial tests ensure attributes are the same with all 3 methods to obtain RACF profiles
+- wiki https://github.com/wizardofzos/pyracf/wiki
+
+### 0.8.3 (tree print format for grouptree and ownertree)
+- msys.grouptree and msys.ownertree are now properties instead of callables
+  print as unix tree or simple format, e.g. print(msys.ownertree)
+  default format looks like unix tree, change with msys.ownertree.setformat('simple')
+  dict structure accessible through .tree attribute
+- .connect('group') and .connect(None,'user') return a (single level) Index with user IDs, resp., groups, connected to the given entity
+  this helps with queries that test group membership
+- add IDSTAR\_ACCESS and ALL\_USER\_ACCESS to .datasets and .generals with, resp., permitted access on ID(*) and the higher value of UACC and IDSTAR_ACCESS.
+- fixed: correlate also builds internal tables from saved pickles
+
 ### 0.8.2 (property for most application segments)
 - application segments for dataset, group and user entities are avaible with entity prefix, e.g., msys.userTSO, msys.datasetDFP, msys.groupOMVS
 - system related application segments from general resources are published without prefix, e.g., msys.STDATA or msys.MFA
 - old properties msys.installdata and msys.userDistributedMappings are replaced by userUSRDATA and userDistributedIdMappings
 - most of these properties are automatically generated
 
 ### 0.8.0 (acl, gfilter, rfilter methods)
@@ -167,15 +183,14 @@
 | getdatasetrisk | Returns dict with users that have access or administrative authority on a profile | mysys.getdatasetrisk('SYS1.**') |
 | gfilter | Returns DataFrame with records matching the index fields specified, using RACF generic patterns | mysys.datasets.gfilter('SYS%.**')) or mysys.generals.gfilter('FACI*','BPX.**'))|
 | group | Returns DataFrame with group profiles matching selection | mysys.group('SYS1') |
 | groupConnect | Returns DataFrame with with user group connection records (0203 recordtype), use connect or connectData instead | mysys.groupConnect |
 | groups | Returns DataFrame with all group data | mysys.groups |
 | groupsWithoutUsers | Returns DataFrame with groups that have no connected users | mysys.groupsWithoutUsers |
 | grouptree | Returns dict with groups arranged by superior group | mysys.grouptree() |
-| installdata | Returns DataFrame with with user installation data (0204 recordtype) | mysys.installdata |
 | operations | Returns a DataFrame  with all operations users | mysys.operations |
 | orphans | Returns 2 DataFrames one with orphans in dataset profile access lists, and one for general resources | d, g = mysys.orphans |
 | ownertree | Returns dict with groups arranged by owner group or user ID | mysys.ownertree() |
 | parse | parses the unload. optional specify recordtypes | mysys.parse(recordtypes=['0200']) |
 | parse_fancycli | parses the unload with a fancy cli status update. optional recordtypes can be specified | mysys.parse_fancycli(recorddtypes=['0200']) |
 | revoked | Returns a DataFrame  with all revoked users | mysys.revoked |
 | rfilter | Returns DataFrame with records matching the index fields specified, using regex patterns | mysys.generals.rfilter('FAC.*','BPX\..*')) |
@@ -211,37 +226,53 @@
     mysys.parse()
     while mysys.status['status'] != 'Ready':
         time.sleep(5)
     mysys.xls('/path/to/my.xlsx')
 
 Print z/OS UNIX profiles
 
-    mysys.generals.gfilter('FAC*', 'BPX.**')
+    mysys.general('FACILITY', 'BPX.SUPERUSER')
+    mysys.general('FACILITY', 'BPX.**')  # show only the FACILITY BPX.** profile
+    mysys.general('FACILITY')  # show all FACILITY profiles
+
+    mysys.generals.gfilter('FAC*', 'BPX.**')  # show all BPX profiles
     mysys.generals.gfilter('UNIXPRIV') # print all in UNIXPRIV
 
 Show group information
 
     mysys.connect('SYS1')            # users connected to SYS1 groups
     mysys.connect('**','IBMUSER')    # groups IBMUSER is connected to
+
     mysys.connectData.gfilter('SYS*','IBM*') # connects using patterns
     mysys.connectData.rfilter('SYS[AB].*','PROD.*') # regex with alternatives
     mysys.connectData.query("USCON_GRP_SPECIAL=='YES' & USCON_REVOKE=='YES'")  # group special revoked
     mysys.connectData.query("GPMEM_AUTH==['CONNECT','JOIN']")  # users with connect authorities
 
+    mysys.users.query("index in @mysys.connect('SYS1').index")  # user details of users connected to SYS1
+
 Show access list information
 
     mysys.datasetPermit('SYS1.**')    # IDs permitted on SYS1.**
     mysys.datasetPermit(id='IBMUSER', access='ALTER')    # where is IBMUSER permitted
+    mysys.datasetPermit(id='*')       # where is ID(*) permitted
 
     mysys.datasets.gfilter('SYS1.**').acl(access='ALTER')    # IDs ALTER access on any SYS1 dataset profile
     mysys.datasets.gfilter('SYS%.**').acl(allows='UPDATE')    # IDs with access that allows UPDATE
     mysys.datasets.gfilter('SYS%.**').acl(allows='UPDATE', resolve=True)    # groups and user permits combined 
     mysys.datasets.gfilter('PROD.**').acl(permits=False, admin=True)    # who can change groups or profiles to change access on PROD data sets
     mysys.generals.gfilter('XFAC*', 'CKR.**').acl() # permits on zSecure Admin/Audit profile
 
+    mysys.datasets.query("ALL_USER_ACCESS=='UPDATE'")    # UACC or ID(*) set to UPDATE
+
+Show group tree information
+
+    print(msys.grouptree)  # group - superior group - subgroups in UNIX tree format
+    print(msys.ownertree.setformat('simple'))  # group - OWNER in simple format
+    msys.grouptree.tree  # get the dict
+
 
 # Updates 
 
 In this version we introduced IRRRDBU as an alternative to RACF. Examples have been updated. The RACF class from previous version is still available, but you're advised to change this to IRRDBU, as future version will have another user of the RACF class.
 
 # Contribute to PyRACF
```

### Comparing `pyracf-0.8.4/README.md` & `pyracf-0.8.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,30 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
+### 0.8.5 (fixes for pickles, pytest, wiki)
+- parse_fancycli now creates empty data frames for pickles it could not find
+- index added to data frames from old pickles, not for pickles that already have index fields
+- pytest framework for QA in development cycle, initial tests ensure attributes are the same with all 3 methods to obtain RACF profiles
+- wiki https://github.com/wizardofzos/pyracf/wiki
+
+### 0.8.3 (tree print format for grouptree and ownertree)
+- msys.grouptree and msys.ownertree are now properties instead of callables
+  print as unix tree or simple format, e.g. print(msys.ownertree)
+  default format looks like unix tree, change with msys.ownertree.setformat('simple')
+  dict structure accessible through .tree attribute
+- .connect('group') and .connect(None,'user') return a (single level) Index with user IDs, resp., groups, connected to the given entity
+  this helps with queries that test group membership
+- add IDSTAR\_ACCESS and ALL\_USER\_ACCESS to .datasets and .generals with, resp., permitted access on ID(*) and the higher value of UACC and IDSTAR_ACCESS.
+- fixed: correlate also builds internal tables from saved pickles
+
 ### 0.8.2 (property for most application segments)
 - application segments for dataset, group and user entities are avaible with entity prefix, e.g., msys.userTSO, msys.datasetDFP, msys.groupOMVS
 - system related application segments from general resources are published without prefix, e.g., msys.STDATA or msys.MFA
 - old properties msys.installdata and msys.userDistributedMappings are replaced by userUSRDATA and userDistributedIdMappings
 - most of these properties are automatically generated
 
 ### 0.8.0 (acl, gfilter, rfilter methods)
@@ -149,15 +165,14 @@
 | getdatasetrisk | Returns dict with users that have access or administrative authority on a profile | mysys.getdatasetrisk('SYS1.**') |
 | gfilter | Returns DataFrame with records matching the index fields specified, using RACF generic patterns | mysys.datasets.gfilter('SYS%.**')) or mysys.generals.gfilter('FACI*','BPX.**'))|
 | group | Returns DataFrame with group profiles matching selection | mysys.group('SYS1') |
 | groupConnect | Returns DataFrame with with user group connection records (0203 recordtype), use connect or connectData instead | mysys.groupConnect |
 | groups | Returns DataFrame with all group data | mysys.groups |
 | groupsWithoutUsers | Returns DataFrame with groups that have no connected users | mysys.groupsWithoutUsers |
 | grouptree | Returns dict with groups arranged by superior group | mysys.grouptree() |
-| installdata | Returns DataFrame with with user installation data (0204 recordtype) | mysys.installdata |
 | operations | Returns a DataFrame  with all operations users | mysys.operations |
 | orphans | Returns 2 DataFrames one with orphans in dataset profile access lists, and one for general resources | d, g = mysys.orphans |
 | ownertree | Returns dict with groups arranged by owner group or user ID | mysys.ownertree() |
 | parse | parses the unload. optional specify recordtypes | mysys.parse(recordtypes=['0200']) |
 | parse_fancycli | parses the unload with a fancy cli status update. optional recordtypes can be specified | mysys.parse_fancycli(recorddtypes=['0200']) |
 | revoked | Returns a DataFrame  with all revoked users | mysys.revoked |
 | rfilter | Returns DataFrame with records matching the index fields specified, using regex patterns | mysys.generals.rfilter('FAC.*','BPX\..*')) |
@@ -193,37 +208,53 @@
     mysys.parse()
     while mysys.status['status'] != 'Ready':
         time.sleep(5)
     mysys.xls('/path/to/my.xlsx')
 
 Print z/OS UNIX profiles
 
-    mysys.generals.gfilter('FAC*', 'BPX.**')
+    mysys.general('FACILITY', 'BPX.SUPERUSER')
+    mysys.general('FACILITY', 'BPX.**')  # show only the FACILITY BPX.** profile
+    mysys.general('FACILITY')  # show all FACILITY profiles
+
+    mysys.generals.gfilter('FAC*', 'BPX.**')  # show all BPX profiles
     mysys.generals.gfilter('UNIXPRIV') # print all in UNIXPRIV
 
 Show group information
 
     mysys.connect('SYS1')            # users connected to SYS1 groups
     mysys.connect('**','IBMUSER')    # groups IBMUSER is connected to
+
     mysys.connectData.gfilter('SYS*','IBM*') # connects using patterns
     mysys.connectData.rfilter('SYS[AB].*','PROD.*') # regex with alternatives
     mysys.connectData.query("USCON_GRP_SPECIAL=='YES' & USCON_REVOKE=='YES'")  # group special revoked
     mysys.connectData.query("GPMEM_AUTH==['CONNECT','JOIN']")  # users with connect authorities
 
+    mysys.users.query("index in @mysys.connect('SYS1').index")  # user details of users connected to SYS1
+
 Show access list information
 
     mysys.datasetPermit('SYS1.**')    # IDs permitted on SYS1.**
     mysys.datasetPermit(id='IBMUSER', access='ALTER')    # where is IBMUSER permitted
+    mysys.datasetPermit(id='*')       # where is ID(*) permitted
 
     mysys.datasets.gfilter('SYS1.**').acl(access='ALTER')    # IDs ALTER access on any SYS1 dataset profile
     mysys.datasets.gfilter('SYS%.**').acl(allows='UPDATE')    # IDs with access that allows UPDATE
     mysys.datasets.gfilter('SYS%.**').acl(allows='UPDATE', resolve=True)    # groups and user permits combined 
     mysys.datasets.gfilter('PROD.**').acl(permits=False, admin=True)    # who can change groups or profiles to change access on PROD data sets
     mysys.generals.gfilter('XFAC*', 'CKR.**').acl() # permits on zSecure Admin/Audit profile
 
+    mysys.datasets.query("ALL_USER_ACCESS=='UPDATE'")    # UACC or ID(*) set to UPDATE
+
+Show group tree information
+
+    print(msys.grouptree)  # group - superior group - subgroups in UNIX tree format
+    print(msys.ownertree.setformat('simple'))  # group - OWNER in simple format
+    msys.grouptree.tree  # get the dict
+
 
 # Updates 
 
 In this version we introduced IRRRDBU as an alternative to RACF. Examples have been updated. The RACF class from previous version is still available, but you're advised to change this to IRRDBU, as future version will have another user of the RACF class.
 
 # Contribute to PyRACF
```

### Comparing `pyracf-0.8.4/setup.py` & `pyracf-0.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyracf",
-    version="0.8.4",
+    version="0.8.6",
     author="Wizard of z/OS",
     author_email="wizard@zdevops.com",
     description="Parsing IRRDBU00 unloads in panda dataframes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wizardofzos/pyracf",
     project_urls={
```

### Comparing `pyracf-0.8.4/src/pyracf/__init__.py` & `pyracf-0.8.6/src/pyracf/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,91 +34,184 @@
         else:  # property object
             newroutine = func.fget
         warnings.warn(f"{oldname} is deprecated and will be removed, use {newroutine.__name__} instead.")
         return newroutine(*arg,**keywords)
     deprecated_func.func = func
     return deprecated_func
 
+class GroupStructureTree(dict):
+    ''' Dict with group names starting from SYS1 (group tree) or from (multiple) user IDs (owner tree).
+    Printing these objects, the tree will be formatted as Unix tree (default, or after .setformat('unix') or with mainframe characters (after .setformat('simple').
+    The dict may be accessed with .tree '''
+    def __init__(self,df,linkup_field="GPBD_SUPGRP_ID"):
+        # get all owners... (group or user) or all superior groups
+        tree = {}
+        where_is = {}
+        higher_ups = df.groupby(linkup_field)
+        for higher_up in higher_ups.groups.keys():
+            if higher_up not in tree:
+                tree[higher_up] = []
+                for group in higher_ups.get_group(higher_up)['GPBD_NAME'].values:
+                    tree[higher_up].append(group)
+                    where_is[group] = tree[higher_up]
+        # initially, for an owner tree, anchor can be a user (like IBMUSER) or a group
+        # now we gotta condense it, so only IBMUSER and other group owning users are at top level
+        # for group tree, we should end up with SYS1, and a list of groups
+        deletes = []
+        for anchor in tree:
+            if anchor in where_is:
+                supgrpMembers = where_is[anchor]
+                ix = supgrpMembers.index(anchor)
+                supgrpMembers[ix] = {anchor: tree[anchor]}
+                deletes.append(anchor)
+        for anchor in deletes:
+            tree.pop(anchor)
+        if '' in tree:  # bring SYS1 to the top, supgroup of SYS1 is ''
+            tree = tree[''][0]
+        self.tree = tree
+        self._format = 'unix'
+        
+    def __get__(self):
+        ''' class objects have a value too '''
+        return self.tree
+
+    def __str__(self):
+        ''' what happens when print(object) is issued '''
+        return self.simple_format(self.tree) if self._format=='simple' else self.unix_format(self.tree)
+        
+    def setformat(self,format='unix'):
+        ''' set default format for next print '''
+        if format in ['unix','simple']:
+            self._format = format
+            return self
+        else:
+            warnings.warn(f'Unsupported format value {format}, select unix or simple.')
+
+    def unix_format(self,branch=None,prefix=''):
+        ''' print groups, prefixed with vertical bars to show depth '''
+        BOX_START = u'\u250C'
+        BOX_ENTRY = u'\u251C'
+        BOX_CONT = u'\u2502'
+        BOX_END = u'\u2514'
+        if not branch:
+            branch = self.tree
+        info = ''
+        if type(branch)==str:
+            info += prefix + ' ' +  str(branch) + '\n'
+        elif type(branch)==list:
+            # indent 1 level, prev level continues with just a bar
+            if prefix and prefix[-1]==BOX_ENTRY:
+                prefix = prefix[0:-1]+BOX_CONT
+            for node in branch:
+                # last node in a branch gets an END indicator, others get a T
+                mark = ' '+BOX_END if (node==branch[-1]) else ' '+BOX_ENTRY
+                info += self.unix_format(node,prefix=prefix+mark)
+        else:
+            for (node,values) in branch.items():
+                info += prefix + ' ' + str(node) + '\n'
+                # only 1 END indicator (which we just printed)
+                if prefix and prefix[-1]==BOX_END:
+                    prefix = prefix[0:-1]+' '
+                info += self.unix_format(values,prefix=prefix)
+        return info
+
+    def simple_format(self,branch=None,depth=0):
+        ''' print groups, prefixed with vertical bars to show depth '''
+        if not branch:
+            branch = self.tree
+        info = ''
+        if type(branch)==str:
+            info += ' |'*depth + ' ' +  str(branch) + '\n'
+        elif type(branch)==list:
+            depth += 1
+            for node in branch:            
+                info += self.simple_format(node,depth)
+        else:
+            for (node,values) in branch.items():
+                info += ' |'*depth + ' '  + str(node) + '\n'
+                info += self.simple_format(values,depth)
+        return info
+
 class RACF:
     
     # Our states
     STATE_BAD         = -1
     STATE_INIT        =  0
     STATE_PARSING     =  1
     STATE_READY       =  2
     STATE_CORRELATING =  3
 
-    # keep track of names used for a record type, "index" must be a list of field names
-    # A dict with `key` -> RecordType
-    #                   'name' -> Internal name (and prefix for pickle-files, and should match prefix in offsets.json for variables in the table (GPMEM_NAME etc...))
+    # keep track of names used for a record type, record type + name must match those in offsets.json
+    # A dict with 'key' -> RecordType
+    #                   'name' -> Internal name (and prefix for pickle-files, variables in the dfs (GPMEM_NAME etc... from offsets.json))
     #                   'df'   -> name of internal df
-    #                   'index' -> index if different than <name>_NAME
-    #                   'publisher' -> property in class to get the df
-    #                                *         -> as df without the _
+    #                   'index' -> index if different from <name>_NAME (and <name>_CLASS_NAME for GRxxx)
+    #                   'publisher' -> adds property in class to get the df (default: no publisher)
+    #                                *         -> same as df without the _
     #                                all but * -> this name as property
     _recordtype_info = {
-    '0100': {'name':'GPBD', 'df':'_groups'},
-    '0101': {'name':'GPSGRP', 'df':'_subgroups'},
-    '0102': {'name':'GPMEM', 'df':'_connects', "index":["GPMEM_NAME","GPMEM_MEMBER_ID"]},
+    '0100': {'name':'GPBD', 'df':'_groups', 'publisher':'*'},
+    '0101': {'name':'GPSGRP', 'df':'_subgroups', 'publisher':'*'},
+    '0102': {'name':'GPMEM', 'df':'_connects', "index":["GPMEM_NAME","GPMEM_MEMBER_ID"], 'publisher':'*'},
     '0103': {'name':'GPINSTD', 'df':'_groupUSRDATA', 'publisher':'*'},
     '0110': {'name':'GPDFP', 'df':'_groupDFP', 'publisher':'*'},
     '0120': {'name':'GPOMVS', 'df':'_groupOMVS', 'publisher':'*'},
     '0130': {'name':'GPOVM', 'df':'_groupOVM'},
     '0141': {'name':'GPTME', 'df':'_groupTME', 'publisher':'*'},
     '0151': {'name':'GPCSD', 'df':'_groupCSDATA', 'publisher':'*'},
-    '0200': {'name':'USBD', 'df':'_users'},
-    '0201': {'name':'USCAT', 'df':'_userCategories'},
-    '0202': {'name':'USCLA', 'df':'_userClasses'},
-    '0203': {'name':'USGCON', 'df':'_groupConnect', "index":["USGCON_GRP_ID","USGCON_NAME"]},
+    '0200': {'name':'USBD', 'df':'_users', 'publisher':'*'},
+    '0201': {'name':'USCAT', 'df':'_userCategories', 'publisher':'*'},
+    '0202': {'name':'USCLA', 'df':'_userClasses', 'publisher':'*'},
+    '0203': {'name':'USGCON', 'df':'_groupConnect', "index":["USGCON_GRP_ID","USGCON_NAME"], 'publisher':'*'},
     '0204': {'name':'USINSTD', 'df':'_userUSRDATA'},  # , 'publisher':'*'
-    '0205': {'name':'USCON', 'df':'_connectData', "index":["USCON_GRP_ID","USCON_NAME"]},
+    '0205': {'name':'USCON', 'df':'_connectData', "index":["USCON_GRP_ID","USCON_NAME"], 'publisher':'*'},
     '0206': {'name':'USRSF', 'df':'_userRRSFdata', 'publisher':'userRRSFDATA'},
     '0207': {'name':'USCERT', 'df':'_userCERTname', 'publisher':'*'},
     '0208': {'name':'USNMAP', 'df':'_userAssociationMapping', 'publisher':'*'},
     '0209': {'name':'USDMAP', 'df':'_userDistributedIdMapping'},  # , 'publisher':'*'
     '020A': {'name':'USMFA', 'df':'_userMFAfactor', 'publisher':'*'},
     '020B': {'name':'USMPOL', 'df':'_userMFApolicies', 'publisher':'*'},
     '0210': {'name':'USDFP', 'df':'_userDFP', 'publisher':'*'},
     '0220': {'name':'USTSO', 'df':'_userTSO', 'publisher':'*'},
-    '0230': {'name':'USCICS', 'df':'_userCICS'},
-    '0231': {'name':'USCOPC', 'df':'_userCICSoperatorClasses'},
-    '0232': {'name':'USCRSL', 'df':'_userCICSrslKeys'},
-    '0233': {'name':'USCTSL', 'df':'_userCICStslKeys'},
-    '0240': {'name':'USLAN', 'df':'_userLANGUAGE'},
-    '0250': {'name':'USOPR', 'df':'_userOPERPARM'},
-    '0251': {'name':'USOPRP', 'df':'_userOPERPARMscope'},
+    '0230': {'name':'USCICS', 'df':'_userCICS', 'publisher':'*'},
+    '0231': {'name':'USCOPC', 'df':'_userCICSoperatorClasses', 'publisher':'*'},
+    '0232': {'name':'USCRSL', 'df':'_userCICSrslKeys', 'publisher':'*'},
+    '0233': {'name':'USCTSL', 'df':'_userCICStslKeys', 'publisher':'*'},
+    '0240': {'name':'USLAN', 'df':'_userLANGUAGE', 'publisher':'*'},
+    '0250': {'name':'USOPR', 'df':'_userOPERPARM', 'publisher':'*'},
+    '0251': {'name':'USOPRP', 'df':'_userOPERPARMscope', 'publisher':'*'},
     '0260': {'name':'USWRK', 'df':'_userWORKATTR', 'publisher':'*'},
     '0270': {'name':'USOMVS', 'df':'_userOMVS', 'publisher':'*'},
-    '0280': {'name':'USNETV', 'df':'_userNETVIEW'},
-    '0281': {'name':'USNOPC', 'df':'_userNETVIEWopclass'},
-    '0282': {'name':'USNDOM', 'df':'_userNETVIEWdomains'},
+    '0280': {'name':'USNETV', 'df':'_userNETVIEW', 'publisher':'*'},
+    '0281': {'name':'USNOPC', 'df':'_userNETVIEWopclass', 'publisher':'*'},
+    '0282': {'name':'USNDOM', 'df':'_userNETVIEWdomains', 'publisher':'*'},
     '0290': {'name':'USDCE', 'df':'_userDCE'},
     '02A0': {'name':'USOVM', 'df':'_userOVM'},
     '02B0': {'name':'USLNOT', 'df':'_userLNOTES'},
     '02C0': {'name':'USNDS', 'df':'_userNDS'},
     '02D0': {'name':'USKERB', 'df':'_userKERB'},
     '02E0': {'name':'USPROXY', 'df':'_userPROXY'},
     '02F0': {'name':'USEIM', 'df':'_userEIM'},
     '02G1': {'name':'USCSD', 'df':'_userCSDATA', 'publisher':'*'},
     '1210': {'name':'USMFAC', 'df':'_userMFAfactorTags', 'publisher':'*'},
-    '0400': {'name':'DSBD', 'df':'_datasets'},
-    '0401': {'name':'DSCAT', 'df':'_datasetCategories'},
-    '0402': {'name':'DSCACC', 'df':'_datasetConditionalAccess', "index":["DSCACC_NAME","DSCACC_AUTH_ID","DSCACC_ACCESS"]},
+    '0400': {'name':'DSBD', 'df':'_datasets', 'publisher':'*'},
+    '0401': {'name':'DSCAT', 'df':'_datasetCategories', 'publisher':'*'},
+    '0402': {'name':'DSCACC', 'df':'_datasetConditionalAccess', "index":["DSCACC_NAME","DSCACC_AUTH_ID","DSCACC_ACCESS"], 'publisher':'*'},
     '0403': {'name':'DSVOL', 'df':'_datasetVolumes'},
-    '0404': {'name':'DSACC', 'df':'_datasetAccess', "index":["DSACC_NAME","DSACC_AUTH_ID","DSACC_ACCESS"]},
+    '0404': {'name':'DSACC', 'df':'_datasetAccess', "index":["DSACC_NAME","DSACC_AUTH_ID","DSACC_ACCESS"], 'publisher':'*'},
     '0405': {'name':'DSINSTD', 'df':'_datasetUSRDATA', 'publisher':'*'},
     '0406': {'name':'DSMEM', 'df':'_datasetMember'},
     '0410': {'name':'DSDFP', 'df':'_datasetDFP', 'publisher':'*'},
     '0421': {'name':'DSTME', 'df':'_datasetTME', 'publisher':'*'},
     '0431': {'name':'DSCSD', 'df':'_datasetCSDATA', 'publisher':'*'},
     '0500': {'name':'GRBD', 'df':'_generals'},
-    '0501': {'name':'GRTVOL', 'df':'_generalTAPEvolume'},
-    '0502': {'name':'GRCAT', 'df':'_generalCategories'},
+    '0501': {'name':'GRTVOL', 'df':'_generalTAPEvolume', 'publisher':'*'},
+    '0502': {'name':'GRCAT', 'df':'_generalCategories', 'publisher':'*'},
     '0503': {'name':'GRMEM', 'df':'_generalMembers'},
-    '0504': {'name':'GRVOL', 'df':'_generalTAPEvolumes'},
+    '0504': {'name':'GRVOL', 'df':'_generalTAPEvolumes', 'publisher':'*'},
     '0505': {'name':'GRACC', 'df':'_generalAccess', "index":["GRACC_CLASS_NAME","GRACC_NAME","GRACC_AUTH_ID","GRACC_ACCESS"]},
     '0506': {'name':'GRINSTD', 'df':'_generalUSRDATA', 'publisher':'*'},
     '0507': {'name':'GRCACC', 'df':'_generalConditionalAccess', "index":["GRCACC_CLASS_NAME","GRCACC_NAME","GRCACC_AUTH_ID","GRCACC_ACCESS"]},
     '0508': {'name':'GRFLTR', 'df':'_generalDistributedIdFilter', 'publisher':'DistributedIdFilter'},
     '0509': {'name':'GRDMAP', 'df':'_generalDistributedIdMapping', 'publisher':'DistributedIdMapping'},
     '0510': {'name':'GRSES', 'df':'_generalSESSION', 'publisher':'SESSION'}, # APPCLU profiles
     '0511': {'name':'GRSESE', 'df':'_generalSESSIONentities', 'publisher':'SESSIONentities'},
@@ -165,43 +258,45 @@
     # strictly speaking only needed for parse() function, but also not limited to one instance.
     with importlib.resources.open_text("pyracf", "offsets.json") as file:
         _offsets = json.load(file)
     for offset in _offsets:
         rtype = _offsets[offset]['record-type']
         if rtype in _recordtype_info.keys():
           _recordtype_info[rtype].update({"offsets": _offsets[offset]["offsets"]})
+    try:
+        del file, rtype, rinfo, offset, _offsets  # don't need these as class attributes
+    except NameError:
+        pass
 
     _grouptree          = None  # dict with lists
     _ownertree          = None  # dict with lists
     _grouptreeLines     = None  # df with all supgroups up to SYS1
     _ownertreeLines     = None  # df with owners up to SYS1 or user ID
     
-    accessKeywords = ['NONE','EXECUTE','READ','UPDATE','CONTROL','ALTER','-owner-']
+    accessKeywords = [' ','NONE','EXECUTE','READ','UPDATE','CONTROL','ALTER','-owner-']
     
     def accessAllows(level=None):
         ''' return list of access levels that allow the given access, e.g.
         RACF.accessAllows('UPDATE') returns [,'UPDATE','CONTROL','ALTER','-owner-']
         for use in pandas .query("ACCESS in @RACF.accessAllows('UPDATE')")
         '''
         return RACF.accessKeywords[RACF.accessKeywords.index(level):]
 
     def __init__(self, irrdbu00=None, pickles=None, prefix=''):
 
-        self._state = self.STATE_INIT
-
-                
         # activate acl() method on our dataframes, so it get called with our instance's variables, the frame, and all optional parms
         # e.g. msys._datasetAccess.loc[['SYS1.**']].acl(permits=True, explode=False, resolve=False, admin=False, sort="user")
         pd.core.base.PandasObject.acl = lambda *x,**y: RACF.acl(self,*x,**y)
 
         # generic and regex filter on the index levels of a frame
         # e.g. msys._datasets.gfilter('SYS1.**').acl(resolve=True, allows='UPDATE', sort="user")
         pd.core.base.PandasObject.gfilter = RACF.gfilter
         pd.core.base.PandasObject.rfilter = RACF.rfilter
 
+        self._state = self.STATE_INIT
 
         if not irrdbu00 and not pickles:
             self._state = self.STATE_BAD
         else:
             if not pickles:
                 self._irrdbu00 = irrdbu00
                 self._state    = self.STATE_INIT
@@ -223,21 +318,24 @@
                     setattr(self, dfname, pd.read_pickle(pickle))
                     recordsRetrieved = len(getattr(self, dfname))
                     self._records[recordtype] = {
                       "seen": recordsRetrieved,
                       "parsed": recordsRetrieved
                     }
                     self._unloadlines += recordsRetrieved
+
+            # create remaining public DFs as empty
             for (rtype,rinfo) in RACF._recordtype_info.items():
-                if 'publisher' in rinfo:
-                    publisher = rinfo['publisher'] if rinfo['publisher']!='*' else rinfo['df'].lstrip('_')
-                    if hasattr(self, rinfo['df']):
-                        setattr(self, publisher, getattr(self, rinfo['df']))
-                    else:
-                        setattr(self, publisher, lambda x: warnings.warn(f"{publisher} has not been collected."))
+                if not hasattr(self, rinfo['df']):
+                    setattr(self, rinfo['df'], pd.DataFrame())
+                    self._records[rtype] = {
+                      "seen": 0,
+                      "parsed": 0
+                    }
+
             self._state = self.STATE_CORRELATING
             self._correlate()
             self._state = self.STATE_READY
             self._stoptime = datetime.now()
 
         else:
             # Running threads
@@ -339,20 +437,14 @@
                         self._parsed[r].append(irrmodel)
                         self._records[r]['parsed'] += 1
         # all models parsed :)
 
         for (rtype,rinfo) in RACF._recordtype_info.items():
             if rtype in thingswewant:
                 setattr(self, rinfo['df'], pd.DataFrame.from_dict(self._parsed[rtype]))
-            if 'publisher' in rinfo:
-                publisher = rinfo['publisher'] if rinfo['publisher']!='*' else rinfo['df'].lstrip('_')
-                if hasattr(self, rinfo['df']):
-                    setattr(self, publisher, getattr(self, rinfo['df']))
-                else:
-                    setattr(self, publisher, lambda x: warnings.warn(f"{publisher} has not been collected."))
 
         # TODO: Reduce memory use, delete self._parsed after dataframes are made
 
         # We need the correlate anyways all the times so let's run it
         self.THREAD_COUNT -= 1
         if self.THREAD_COUNT == 0:
             self._state = self.STATE_CORRELATING
@@ -364,42 +456,79 @@
     def parsed(self, rname):
         """ how many records with this name (type) were parsed """
         rtype = RACF._recordname_type[rname]
         return self._records[rtype]['parsed'] if rtype in self._records else 0
         
     def _correlate(self, thingswewant=_recordtype_info.keys()):
         """ construct tables that combine the raw dataframes for improved processing """
-
+        
+        # use the table definitions in _recordtype_info finalize the dfs:
         # set consistent index columns for existing dfs: profile key, connect group+user, of profile class+key (for G.R.)
+        # define properties to access the dfs, in addition to the properties defined as functions below
         for (rtype,rinfo) in RACF._recordtype_info.items():
             if rtype in thingswewant and rtype in self._records and self._records[rtype]['parsed']>0:
                 if "index" in rinfo:
                     keys = rinfo["index"]
-                    names = [keys[i].replace(rinfo["name"]+"_","_") for i in range(len(keys))]
+                    names = [k.replace(rinfo["name"]+"_","_") for k in keys]
                 elif rtype[1]=="5":  # general resources
                     keys = [rinfo["name"]+"_CLASS_NAME",rinfo["name"]+"_NAME"]
                     names = ["_CLASS_NAME","_NAME"]
                 else:
                     keys = rinfo["name"]+"_NAME"
                     names = "_NAME"
-                getattr(self,rinfo['df']).set_index(keys,drop=False,inplace=True)
-                getattr(self,rinfo['df']).rename_axis(names,inplace=True)  # prevent ambiguous index / column names 
-        
+                if getattr(self,rinfo['df']).index.names!=names:  # reuse existing index for pickles
+                    getattr(self,rinfo['df']).set_index(keys,drop=False,inplace=True)
+                    getattr(self,rinfo['df']).rename_axis(names,inplace=True)  # prevent ambiguous index / column names 
+            if 'publisher' in rinfo:
+                publisher = rinfo['publisher'] if rinfo['publisher']!='*' else rinfo['df'].lstrip('_')
+                if hasattr(self, rinfo['df']):
+                    setattr(self, publisher, getattr(self, rinfo['df']))
+                else:
+                    setattr(self, publisher, lambda x: warnings.warn(f"{publisher} has not been collected."))
+
+
         # copy group auth (USE,CREATE,CONNECT,JOIN) to complete the connectData list, using index alignment
-        if self.parsed("GPMEM") == 0 or self.parsed("USCON") == 0:
-            raise StoopidException("Need to parse GPMEM and USCON first...")
-        else: 
+        if self.parsed("GPBD") > 0 and self.parsed("GPMEM") > 0 and self.parsed("USCON") > 0:
             self._connectData["GPMEM_AUTH"] = self._connects["GPMEM_AUTH"]
+
+        # copy ID(*) access into resource frames, similar to UACC: IDSTAR_ACCESS and ALL_USER_ACCESS
+        if self.parsed("DSBD") > 0 and self.parsed("DSACC") > 0 and 'IDSTAR_ACCESS' not in self._datasets.columns:
+            uaccs = pd.DataFrame()
+            uaccs["UACC_NUM"] = self._datasets["DSBD_UACC"].map(RACF.accessKeywords.index)
+            uaccs["IDSTAR_ACCESS"] = self._datasetAccess.gfilter(None, '*').droplevel([1,2])['DSACC_ACCESS'].drop_duplicates()
+            uaccs["IDSTAR_ACCESS"] = uaccs["IDSTAR_ACCESS"].fillna(' ')
+            uaccs["IDSTAR_NUM"] = uaccs["IDSTAR_ACCESS"].map(RACF.accessKeywords.index)
+            uaccs["ALL_USER_NUM"] = uaccs[["IDSTAR_NUM","UACC_NUM"]].max(axis=1)
+            uaccs["ALL_USER_ACCESS"] = uaccs['ALL_USER_NUM'].map(RACF.accessKeywords.__getitem__)
+            column = self._datasets.columns.to_list().index('DSBD_UACC')
+            self._datasets.insert(column+1,"IDSTAR_ACCESS",uaccs["IDSTAR_ACCESS"])
+            self._datasets.insert(column+2,"ALL_USER_ACCESS",uaccs["ALL_USER_ACCESS"])
+            del uaccs
+        
+        if self.parsed("GRBD") > 0 and self.parsed("GRACC") > 0 and 'IDSTAR_ACCESS' not in self._generals.columns:
+            uaccs = pd.DataFrame()
+            uaccs["UACC"] = self._generals["GRBD_UACC"]
+            uaccs["UACC"] = uaccs["UACC"].where(uaccs["UACC"].isin(RACF.accessKeywords),other=' ')  # DIGTCERT fields may be distorted
+            uaccs["UACC_NUM"] = uaccs["UACC"].map(RACF.accessKeywords.index)
+            uaccs["IDSTAR_ACCESS"] = self._generalAccess.gfilter(None, '*').droplevel([1,2])['GRACC_ACCESS'].drop_duplicates()
+            uaccs["IDSTAR_ACCESS"] = uaccs["IDSTAR_ACCESS"].fillna(' ')
+            uaccs["IDSTAR_NUM"] = uaccs["IDSTAR_ACCESS"].map(RACF.accessKeywords.index)
+            uaccs["ALL_USER_NUM"] = uaccs[["IDSTAR_NUM","UACC_NUM"]].max(axis=1)
+            uaccs["ALL_USER_ACCESS"] = uaccs['ALL_USER_NUM'].map(RACF.accessKeywords.__getitem__)
+            column = self._generals.columns.to_list().index('GRBD_UACC')
+            self._generals.insert(column+1,"IDSTAR_ACCESS",uaccs["IDSTAR_ACCESS"])
+            self._generals.insert(column+2,"ALL_USER_ACCESS",uaccs["ALL_USER_ACCESS"])
+            del uaccs
         
-        self._connectByUser = self._connectData.set_index("USCON_NAME",drop=False).rename_axis('NAME')
-        self._connectByGroup = self._connectData.set_index("USCON_GRP_ID",drop=False).rename_axis('GRP_ID')
+        # self._connectByUser = self._connectData.set_index("USCON_NAME",drop=False).rename_axis('NAME')
+        # self._connectByGroup = self._connectData.set_index("USCON_GRP_ID",drop=False).rename_axis('GRP_ID')
             
         # dicts containing lists of groups for printing group structure
-        self._ownertree = self.ownertree()
-        self._grouptree = self.grouptree()
+        self._ownertree = self.ownertree
+        self._grouptree = self.grouptree
 
         # self._grouptreeLines: frame of group + name of all superior groups until SYS1
         gtl = self._groups[['GPBD_NAME','GPBD_SUPGRP_ID']]
         gtlLen = 0
         while len(gtl)>gtlLen:
             nextup = gtl[gtlLen:]\
                      .query("GPBD_NAME!='SYS1' & GPBD_SUPGRP_ID!='SYS1'")\
@@ -455,18 +584,18 @@
 
     def generic2regex(selection, lenient='%&*'):
         ''' Change a RACF generic pattern into regex to match with text strings in pandas cells.  use lenient="" to match with dsnames/resources '''
         if selection in ('**',''):
             return '.*$'
         else:
             return selection.replace('*.**','`dot``ast`')\
-                    .replace('.**','\`dot``dot``ast`')\
-                    .replace('*','[\w@#$`lenient`]`ast`')\
-                    .replace('%','[\w@#$]')\
-                    .replace('.','\.')\
+                    .replace('.**',r'\`dot``dot``ast`')\
+                    .replace('*',r'[\w@#$`lenient`]`ast`')\
+                    .replace('%',r'[\w@#$]')\
+                    .replace('.',r'\.')\
                     .replace('`dot`','.')\
                     .replace('`ast`','*')\
                     .replace('`lenient`',lenient)\
                     +'$'
 
 
     def giveMeProfiles(self, df, selection=None, option=None):
@@ -474,91 +603,89 @@
         option controls how selection is interpreted, and how data must be returned:
         None is for (expensive) backward compatibility, returns a df with 1 profile.
         LIST returns a series for 1 profile, much faster and easier to process.
         '''
         if not selection:
             raise StoopidException('profile criteria not specified...')
         if option in (None,'LIST','L'):  # return 1 profile
-            # 1 string, several strings in a tuple, or a mix of strings and None, but the latter must be tested with get_level_values
-            if type(selection)==str: pass
+            # 1 string, several strings in a tuple, or a mix of strings and None
+            if type(selection)==str and not option:
+                selection = [selection]  # [] forces return of a df, not a Series
             elif type(selection)==tuple:
-                selections = len(selection)
-                strings = [type(selection[i])==str and selection[i]!='**' for i in range(selections)]
-                if all(strings): pass
+                if any([s in (None,'**') for s in selection]):  # any qualifiers are a mask
+                    selection = tuple(slice(None) if s in (None,'**') else s for s in selection),
                 else:
-                    locs = pd.array([True]*df.shape[0], dtype="boolean")
-                    for s in range(selections):
-                        if selection[s] not in (None,'**'):
-                            locs &= (df.index.get_level_values(s)==selection[s])
-                    selection = locs
+                    selection = [selection]
             else:
-                raise StoopidException(f'specify patterns for profile, (group,userid) or (class,profile), not {selection}')
-            if option == None and type(selection) in (str,tuple):  # return DataFrame for 1 profile
-                try:
-                    return df.loc[[selection]]
-                except KeyError:
+                pass
+            try:
+                return df.loc[selection]
+            except KeyError:
+                if not option:  # return DataFrame with profiles
                     return pd.DataFrame()
-            else:  # return Series for 1 profile, or use loc[array]
-                try:
-                    return df.loc[selection]
-                except KeyError:
+                else:  # return Series 
                     return []
         else:
             raise StoopidException(f'unexpected last parameter {option}')
 
 
     def gfilter(df, *selection):
         ''' Search profiles using GENERIC pattern on the index fields.  selection can be one or more values, corresponding to index levels of the df '''
-        locs = pd.array([True]*df.shape[0], dtype="boolean")
+        locs = pd.array([True]*df.shape[0])
         for s in range(len(selection)):
             if selection[s] not in (None,'**'):
-                locs &= (df.index.get_level_values(s).str.match(RACF.generic2regex(selection[s])))
+                if selection[s]=='*':
+                    locs &= (df.index.get_level_values(s)=='*')
+                else: 
+                    locs &= (df.index.get_level_values(s).str.match(RACF.generic2regex(selection[s])))
         return df.loc[locs]
 
     def rfilter(df, *selection):
         ''' Search profiles using refex on the index fields.  selection can be one or more values, corresponding to index levels of the df '''
-        locs = pd.array([True]*df.shape[0], dtype="boolean")
+        locs = pd.array([True]*df.shape[0])
         for s in range(len(selection)):
             if selection[s] not in (None,'**','.*'):
                 locs &= (df.index.get_level_values(s).str.match(selection[s]))
         return df.loc[locs]
 
     # user frames
 
-    @property
-    def users(self):
-        if self._state != self.STATE_READY:
-            raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
-        try:
-            return self._users
-        except:
-            raise StoopidException('No USBD records parsed!')
-    
     def user(self, userid=None, pattern=None):
         return self.giveMeProfiles(self._users, userid, pattern)
 
-
-    @property
-    def connectData(self):
-        if self._state != self.STATE_READY:
-            raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
-        return self._connectData
-        
     def connect(self, group=None, userid=None, pattern=None):
-        return self.giveMeProfiles(self._connectData, (group,userid), pattern)
+        ''' connect('SYS1') returns 1 index level with user IDs, connect(None,'IBMUSER') returns 1 index level with group names '''
+        if pattern=='L' or pattern=='LIST':
+            return self.giveMeProfiles(self._connectData, (group,userid), pattern)
+        else:
+            if group and (not userid or userid=='**'):
+                # with group given, return connected user IDs via index (.loc['group'] strips level(0))
+                selection = group
+            elif userid and (not group or group=='**'):
+                # with user ID given, return connected groups via index (only level(0))
+                return self._connectData.loc[(slice(None),userid),].droplevel(1)
+            else:
+                # with group + user ID given, return 1 entry with all index levels (because only the data columns will be of interest)
+                selection = [(group,userid)]
+            try:
+                return self._connectData.loc[selection]
+            except KeyError:
+                return pd.DataFrame()
 
 
     @property
     def userUSRDATA(self):
+        # retained here due to deprecated property definition
         return self._userUSRDATA
 
     installdata = property(deprecated(userUSRDATA,"installdata"))
 
     @property
     def userDistributedIdMapping(self):
+        # retained here due to deprecated property definition
         return self._userDistributedIdMapping
 
     userDistributedMapping = property(deprecated(userDistributedIdMapping,"userDistributedMapping"))
 
 
     @property
     def specials(self):
@@ -575,74 +702,32 @@
     @property
     def revoked(self):
         return self._users.loc[self._users['USBD_REVOKE'] == 'YES']
 
 
     # group frames
 
-    @property
-    def groups(self, query=None):
-        if self._state != self.STATE_READY:
-            raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
-        return self._groups
-    
     def group(self, group=None, pattern=None):
         return self.giveMeProfiles(self._groups, group, pattern)
 
     @property
     def groupsWithoutUsers(self):
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._groups.loc[~self.groups.GPBD_NAME.isin(self._connectData.USCON_GRP_ID)]
     
-    @property
-    def groupConnect(self):
-        if self._state != self.STATE_READY:
-            raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
-        return self._groupConnect
-
-    @property
-    def connects(self):
-        if self._state != self.STATE_READY:
-            raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
-        return self._connects
-
-    @property
-    def subgroups(self):
-        if self._state != self.STATE_READY:
-            raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
-        return self._subgroups
-
 
     # dataset frames
         
-    @property
-    def datasets(self):
-        if self._state != self.STATE_READY:
-            raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
-        return self._datasets
-
     def dataset(self, profile=None, pattern=None):
         return self.giveMeProfiles(self._datasets, profile, pattern)
 
-    @property
-    def datasetConditionalAccess(self):
-        if self._state != self.STATE_READY:
-            raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
-        return self._datasetConditionalAccess
-
     def datasetConditionalPermit(self, profile=None, id=None, access=None, pattern=None):
         return self.giveMeProfiles(self._datasetConditionalAccess, (profile,id,access), pattern)
 
-    @property
-    def datasetAccess(self):
-        if self._state != self.STATE_READY:
-            raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
-        return self._datasetAccess
-
     def datasetPermit(self, profile=None, id=None, access=None, pattern=None):
         return self.giveMeProfiles(self._datasetAccess, (profile,id,access), pattern)
 
     @property
     def uacc_read_datasets(self):
         return self._datasets.loc[self._datasets.DSBD_UACC=="READ"]
     @property
@@ -656,45 +741,49 @@
         return self._datasets.loc[self._datasets.DSBD_UACC=="ALTER"]
 
 
     # general resource frames
 
     @property
     def generals(self, query=None):
+        # retained here due to deprecated property definition
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._generals
 
     generics = property(deprecated(generals,"generics"))
 
     def general(self, resclass=None, profile=None, pattern=None):
         return self.giveMeProfiles(self._generals, (resclass,profile), pattern)
 
     @property
     def generalMembers(self, query=None):
+        # retained here due to deprecated property definition
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._generalMembers    
 
     genericMembers = property(deprecated(generalMembers,"genericMembers"))
 
     @property
     def generalAccess(self, query=None):
+        # retained here due to deprecated property definition
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._generalAccess
 
     genericAccess = property(deprecated(generalAccess,"genericAccess"))
     
     def generalPermit(self, resclass=None, profile=None, id=None, access=None, pattern=None):
         return self.giveMeProfiles(self._generalAccess, (resclass,profile,id,access), pattern)
     
     
     @property
     def generalConditionalAccess(self):
+        # retained here due to deprecated property definition
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._generalConditionalAccess
 
     genericConditionalAccess = property(deprecated(generalConditionalAccess,"genericConditionalAccess"))
     
     def generalConditionalPermit(self, resclass=None, profile=None, id=None, access=None, pattern=None):
@@ -732,32 +821,32 @@
             tbProfileKeys = ["CLASS_NAME","NAME"]
         else:
             raise StoopidException(f'Table {tbName} not supported for acl( ), except DSBD, DSACC, DSCACC, GRBD, GRACC or GRCACC.')
 
         if tbName in ["DSBD","GRBD"]:
             # profiles selected, add corresp. access + cond.access frames
             tbProfiles = df[[tbName+"_"+k for k in tbProfileKeys+["OWNER_ID","UACC"]]].copy()
-            tbProfiles.columns = [tbProfiles.columns[i].replace(tbName+"_","") for i in range(len(tbProfiles.columns))]
+            tbProfiles.columns = [c.replace(tbName+"_","") for c in tbProfiles.columns]
             tbPermits = []
             for tb in [tbEntity+"ACC",tbEntity+"CACC"]:
                 if self.parsed(tb)>0:
                     tbPermits.append(getattr(self,self._recordname_df[tb])\
                                      .merge(tbProfiles["UACC"], left_index=True, right_index=True))
-                    tbPermits[-1].columns = [tbPermits[-1].columns[i].replace(tb+"_","") for i in range(len(tbPermits[-1].columns))]
+                    tbPermits[-1].columns = [c.replace(tb+"_","") for c in tbPermits[-1].columns]
             tbPermits = pd.concat(tbPermits,sort=False)\
                           .drop(["RECORD_TYPE","ACCESS_CNT","UACC"],axis=1)\
                           .fillna(' ') 
         elif tbName in ["DSACC","DSCACC","GRACC","GRCACC"]:
             # access frame selected, add profiles from frame tbEntity+BD
             tbPermits = df.copy()
-            tbPermits.columns = [tbPermits.columns[i].replace(tbName+"_","") for i in range(len(tbPermits.columns))]
+            tbPermits.columns = [c.replace(tbName+"_","") for c in tbPermits.columns]
             tbPermits.drop(["RECORD_TYPE","ACCESS_CNT"],axis=1,inplace=True)
             tbProfiles = getattr(self,self._recordname_df[tbEntity+"BD"])\
                          .loc[tbPermits.droplevel([-2,-1]).index.drop_duplicates()].copy()
-            tbProfiles.columns = [tbProfiles.columns[i].replace(tbEntity+"BD_","") for i in range(len(tbProfiles.columns))]
+            tbProfiles.columns = [c.replace(tbEntity+"BD_","") for c in tbProfiles.columns]
             tbProfiles = tbProfiles[tbProfileKeys+["OWNER_ID","UACC"]]
         else:
             raise StoopidException(f'Table {tbName} not supported for acl( ), except DSBD, DSACC, DSCACC, GRBD, GRACC or GRCACC.')
           
         # tbProfiles and tbPermits have column names without the tbName prefix
         
         returnFields = ["USER_ID","AUTH_ID","ACCESS"]
@@ -768,16 +857,19 @@
                   "access":["RANKED_ACCESS","USER_ID"],
                   "id":["AUTH_ID"]+tbProfileKeys, 
                   "admin":"ADMIN_ID", 
                   "profile":tbProfileKeys+["USER_ID"]}
         if sort not in sortBy:
             raise StoopidException(f'Sort value {sort} not supported for acl( ), use one of {",".join(sortBy.keys())}.')
         
+        if explode or resolve or admin:  # get view of connectData with only one index level (the group name)
+            groupMembers = self._connectData.droplevel(1)
+
         if explode or resolve:  # get user IDs connected to groups into field USER_ID
-            acl = pd.merge(tbPermits, self._connectByGroup[["USCON_NAME"]], how="left", left_on="AUTH_ID", right_index=True)
+            acl = pd.merge(tbPermits, groupMembers[["USCON_NAME"]], how="left", left_on="AUTH_ID", right_index=True)
             acl.insert(3,"USER_ID",acl["USCON_NAME"].where(acl["USCON_NAME"].notna(),acl["AUTH_ID"]))
         elif permits:  # just the userid+access from RACF, add USER_ID column for consistency
             acl = tbPermits
             acl.insert(3,"USER_ID",acl["AUTH_ID"].where(~ acl["AUTH_ID"].isin(self._groups.index.values),"-group-"))
         else:
             acl = pd.DataFrame(columns=tbProfileKeys+returnFields)
         if permits or explode or resolve:  # add -uacc- pseudo access
@@ -838,23 +930,23 @@
                                          .drop(["GPBD_OWNER_ID","GPBD_SUPGRP_ID"],axis=1)
             admin_grpspec2 = pd.merge(admin_grpspec1, self._ownertreeLines, how="inner", left_on="AUTH_ID", right_index=True)\
                                .drop(["GPBD_NAME","GROUP"],axis=1)
             admin_grpspec1.rename({"GPBD_NAME":"OWNER_IDS"},axis=1,inplace=True)
             
             # identify group special on ACL group and on any owning group
             admin_grpspec = pd.merge(pd.concat([admin_grpspec1,admin_grpspec2,profile_groupowner1,profile_groupowner2], sort=False),\
-                                     self._connectByGroup[["USCON_NAME","USCON_GRP_ID","USCON_GRP_SPECIAL"]]\
+                                     groupMembers[["USCON_NAME","USCON_GRP_ID","USCON_GRP_SPECIAL"]]\
                                              .query('USCON_GRP_SPECIAL == "YES"'),
                                      how="inner", left_on="OWNER_IDS", right_index=True)\
                                .rename({"USCON_NAME":"ADMIN_ID","OWNER_IDS":"VIA"},axis=1)\
                                .drop(["USCON_GRP_ID","USCON_GRP_SPECIAL"],axis=1)
             admin_grpspec["AUTHORITY"] = "GRPSPECIAL"
 
             # CONNECT or JOIN authority on an ACL group
-            admin_grpauth = pd.merge(tbPermits, self._connectByGroup[["USCON_NAME","USCON_GRP_ID","GPMEM_AUTH"]]
+            admin_grpauth = pd.merge(tbPermits, groupMembers[["USCON_NAME","USCON_GRP_ID","GPMEM_AUTH"]]
                                                  .query('GPMEM_AUTH==["CONNECT","JOIN"]'),
                                      how="inner", left_on="AUTH_ID", right_index=True)\
                               .rename({"USCON_NAME":"ADMIN_ID","USCON_GRP_ID":"VIA","GPMEM_AUTH":"AUTHORITY"},axis=1)
             admin_grpauth["USER_ID"] = "-group-"
             
             acl = pd.concat([acl,profile_userowners,admin_gowners,admin_grpspec,admin_grpauth],
                             ignore_index=True, sort=False).fillna(' ')
@@ -1005,53 +1097,32 @@
                         centry = rdict.get(i,None)
                         if centry:
                             value = shared_strings[centry.string]
                             worksheet.write(j, i, value, accessLevelFormats[value])
 
         writer.close()   
 
-    def tree(self,linkup_field="GPBD_SUPGRP_ID"):
-        # get all owners... (group or user) or all superior groups
-        tree = {}
-        where_is = {}
-        higher_ups = self._groups.groupby(linkup_field)
-        for higher_up in higher_ups.groups.keys():
-            if higher_up not in tree:
-                tree[higher_up] = []
-                for group in higher_ups.get_group(higher_up)['GPBD_NAME'].values:
-                    tree[higher_up].append(group)
-                    where_is[group] = tree[higher_up]
-        # initially, for an owner tree, anchor can be a user (like IBMUSER) or a group
-        # now we gotta condense it, so only IBMUSER and other group owning users are at top level
-        # for group tree, we should end up with SYS1, and a list of groups
-        deletes = []
-        for anchor in tree:
-            if anchor in where_is:
-                supgrpMembers = where_is[anchor]
-                ix = supgrpMembers.index(anchor)
-                supgrpMembers[ix] = {anchor: tree[anchor]}
-                deletes.append(anchor)
-        for anchor in deletes:
-            tree.pop(anchor)
-        return tree
 
+    @property
     def ownertree(self):
         ''' 
         create dict with the user IDs that own groups as key, and a list of their owned groups as values.
         if a group in this list owns group, the list is replaced by a dict.
         '''
-        return self._ownertree if self._ownertree else self.tree("GPBD_OWNER_ID")
+        return self._ownertree if self._ownertree else GroupStructureTree(self._groups,"GPBD_OWNER_ID")
 
+    @property
     def grouptree(self):
         ''' 
         create dict starting with SYS1, and a list of groups owned by SYS1 as values.
         if a group in this list owns group, the list is replaced by a dict.
         because SYS1s superior group is blank/missing, we return the first group that is owned by "".
         '''
-        return self._grouptree if self._grouptree else self.tree("GPBD_SUPGRP_ID")[""][0]
+        return self._grouptree if self._grouptree else GroupStructureTree(self._groups,"GPBD_SUPGRP_ID")
+
 
     def getdatasetrisk(self, profile=''):
         '''This will produce a dict as follows:
       
         '''
         try:
             if self.parsed("GPBD") == 0 or self.parsed("USCON") == 0 or self.parsed("USBD") == 0 or self.parsed("DSACC") == 0 or self.parsed("DSBD") == 0:
```

### Comparing `pyracf-0.8.4/src/pyracf/getOffsets.py` & `pyracf-0.8.6/src/pyracf/getOffsets.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.4/src/pyracf/offsets.json` & `pyracf-0.8.6/src/pyracf/offsets.json`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.4/src/pyracf.egg-info/PKG-INFO` & `pyracf-0.8.6/src/pyracf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.8.4
+Version: 0.8.6
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -29,14 +29,30 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/3.1.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
+### 0.8.5 (fixes for pickles, pytest, wiki)
+- parse_fancycli now creates empty data frames for pickles it could not find
+- index added to data frames from old pickles, not for pickles that already have index fields
+- pytest framework for QA in development cycle, initial tests ensure attributes are the same with all 3 methods to obtain RACF profiles
+- wiki https://github.com/wizardofzos/pyracf/wiki
+
+### 0.8.3 (tree print format for grouptree and ownertree)
+- msys.grouptree and msys.ownertree are now properties instead of callables
+  print as unix tree or simple format, e.g. print(msys.ownertree)
+  default format looks like unix tree, change with msys.ownertree.setformat('simple')
+  dict structure accessible through .tree attribute
+- .connect('group') and .connect(None,'user') return a (single level) Index with user IDs, resp., groups, connected to the given entity
+  this helps with queries that test group membership
+- add IDSTAR\_ACCESS and ALL\_USER\_ACCESS to .datasets and .generals with, resp., permitted access on ID(*) and the higher value of UACC and IDSTAR_ACCESS.
+- fixed: correlate also builds internal tables from saved pickles
+
 ### 0.8.2 (property for most application segments)
 - application segments for dataset, group and user entities are avaible with entity prefix, e.g., msys.userTSO, msys.datasetDFP, msys.groupOMVS
 - system related application segments from general resources are published without prefix, e.g., msys.STDATA or msys.MFA
 - old properties msys.installdata and msys.userDistributedMappings are replaced by userUSRDATA and userDistributedIdMappings
 - most of these properties are automatically generated
 
 ### 0.8.0 (acl, gfilter, rfilter methods)
@@ -167,15 +183,14 @@
 | getdatasetrisk | Returns dict with users that have access or administrative authority on a profile | mysys.getdatasetrisk('SYS1.**') |
 | gfilter | Returns DataFrame with records matching the index fields specified, using RACF generic patterns | mysys.datasets.gfilter('SYS%.**')) or mysys.generals.gfilter('FACI*','BPX.**'))|
 | group | Returns DataFrame with group profiles matching selection | mysys.group('SYS1') |
 | groupConnect | Returns DataFrame with with user group connection records (0203 recordtype), use connect or connectData instead | mysys.groupConnect |
 | groups | Returns DataFrame with all group data | mysys.groups |
 | groupsWithoutUsers | Returns DataFrame with groups that have no connected users | mysys.groupsWithoutUsers |
 | grouptree | Returns dict with groups arranged by superior group | mysys.grouptree() |
-| installdata | Returns DataFrame with with user installation data (0204 recordtype) | mysys.installdata |
 | operations | Returns a DataFrame  with all operations users | mysys.operations |
 | orphans | Returns 2 DataFrames one with orphans in dataset profile access lists, and one for general resources | d, g = mysys.orphans |
 | ownertree | Returns dict with groups arranged by owner group or user ID | mysys.ownertree() |
 | parse | parses the unload. optional specify recordtypes | mysys.parse(recordtypes=['0200']) |
 | parse_fancycli | parses the unload with a fancy cli status update. optional recordtypes can be specified | mysys.parse_fancycli(recorddtypes=['0200']) |
 | revoked | Returns a DataFrame  with all revoked users | mysys.revoked |
 | rfilter | Returns DataFrame with records matching the index fields specified, using regex patterns | mysys.generals.rfilter('FAC.*','BPX\..*')) |
@@ -211,37 +226,53 @@
     mysys.parse()
     while mysys.status['status'] != 'Ready':
         time.sleep(5)
     mysys.xls('/path/to/my.xlsx')
 
 Print z/OS UNIX profiles
 
-    mysys.generals.gfilter('FAC*', 'BPX.**')
+    mysys.general('FACILITY', 'BPX.SUPERUSER')
+    mysys.general('FACILITY', 'BPX.**')  # show only the FACILITY BPX.** profile
+    mysys.general('FACILITY')  # show all FACILITY profiles
+
+    mysys.generals.gfilter('FAC*', 'BPX.**')  # show all BPX profiles
     mysys.generals.gfilter('UNIXPRIV') # print all in UNIXPRIV
 
 Show group information
 
     mysys.connect('SYS1')            # users connected to SYS1 groups
     mysys.connect('**','IBMUSER')    # groups IBMUSER is connected to
+
     mysys.connectData.gfilter('SYS*','IBM*') # connects using patterns
     mysys.connectData.rfilter('SYS[AB].*','PROD.*') # regex with alternatives
     mysys.connectData.query("USCON_GRP_SPECIAL=='YES' & USCON_REVOKE=='YES'")  # group special revoked
     mysys.connectData.query("GPMEM_AUTH==['CONNECT','JOIN']")  # users with connect authorities
 
+    mysys.users.query("index in @mysys.connect('SYS1').index")  # user details of users connected to SYS1
+
 Show access list information
 
     mysys.datasetPermit('SYS1.**')    # IDs permitted on SYS1.**
     mysys.datasetPermit(id='IBMUSER', access='ALTER')    # where is IBMUSER permitted
+    mysys.datasetPermit(id='*')       # where is ID(*) permitted
 
     mysys.datasets.gfilter('SYS1.**').acl(access='ALTER')    # IDs ALTER access on any SYS1 dataset profile
     mysys.datasets.gfilter('SYS%.**').acl(allows='UPDATE')    # IDs with access that allows UPDATE
     mysys.datasets.gfilter('SYS%.**').acl(allows='UPDATE', resolve=True)    # groups and user permits combined 
     mysys.datasets.gfilter('PROD.**').acl(permits=False, admin=True)    # who can change groups or profiles to change access on PROD data sets
     mysys.generals.gfilter('XFAC*', 'CKR.**').acl() # permits on zSecure Admin/Audit profile
 
+    mysys.datasets.query("ALL_USER_ACCESS=='UPDATE'")    # UACC or ID(*) set to UPDATE
+
+Show group tree information
+
+    print(msys.grouptree)  # group - superior group - subgroups in UNIX tree format
+    print(msys.ownertree.setformat('simple'))  # group - OWNER in simple format
+    msys.grouptree.tree  # get the dict
+
 
 # Updates 
 
 In this version we introduced IRRRDBU as an alternative to RACF. Examples have been updated. The RACF class from previous version is still available, but you're advised to change this to IRRDBU, as future version will have another user of the RACF class.
 
 # Contribute to PyRACF
```

