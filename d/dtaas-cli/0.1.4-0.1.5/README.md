# Comparing `tmp/dtaas_cli-0.1.4.tar.gz` & `tmp/dtaas_cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtaas_cli-0.1.4.tar", max compression
+gzip compressed data, was "dtaas_cli-0.1.5.tar", max compression
```

## Comparing `dtaas_cli-0.1.4.tar` & `dtaas_cli-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1214 2024-04-14 05:22:19.653237 dtaas_cli-0.1.4/README.md
--rw-r--r--   0        0        0      423 2024-04-14 05:30:57.991423 dtaas_cli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-31 06:33:13.786621 dtaas_cli-0.1.4/src/__init__.py
--rw-r--r--   0        0        0     1231 2024-03-27 14:51:32.151684 dtaas_cli-0.1.4/src/cmd.py
--rw-r--r--   0        0        0     3150 2024-04-14 05:28:06.060701 dtaas_cli-0.1.4/src/pkg/config.py
--rw-r--r--   0        0        0     4127 2024-04-14 05:30:38.691639 dtaas_cli-0.1.4/src/pkg/users.py
--rw-r--r--   0        0        0     2319 2024-04-13 11:31:54.941367 dtaas_cli-0.1.4/src/pkg/utils.py
--rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 dtaas_cli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2106 2024-04-20 11:43:31.086953 dtaas_cli-0.1.5/README.md
+-rw-r--r--   0        0        0      423 2024-04-21 08:23:06.815067 dtaas_cli-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-21 08:22:23.250591 dtaas_cli-0.1.5/src/__init__.py
+-rw-r--r--   0        0        0     1155 2024-04-21 08:22:23.250591 dtaas_cli-0.1.5/src/cmd.py
+-rw-r--r--   0        0        0     3060 2024-04-21 08:22:23.250591 dtaas_cli-0.1.5/src/pkg/config.py
+-rw-r--r--   0        0        0     3992 2024-04-21 08:22:52.534911 dtaas_cli-0.1.5/src/pkg/users.py
+-rw-r--r--   0        0        0     2247 2024-04-21 08:22:23.250591 dtaas_cli-0.1.5/src/pkg/utils.py
+-rw-r--r--   0        0        0     2820 1970-01-01 00:00:00.000000 dtaas_cli-0.1.5/PKG-INFO
```

### Comparing `dtaas_cli-0.1.4/src/pkg/config.py` & `dtaas_cli-0.1.5/src/pkg/config.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-"""This file supports the DTaaS config class"""
-
-import click
-from src.pkg import utils
-
-class Config:
-    """The Config class for DTaaS"""
-
-    def __init__(self):
-        config, err = utils.importToml('dtaas.toml')
-        if err is not None:
-            raise click.ClickException("config initialisation failed: "+str(err))
-        self.data = config
-
-    def getConfig(self):
-        """Gets the config dictionary"""
-        if self.data is not None:
-            return self.data,None
-        return None, Exception("Config not initialised")
-
-    def getCommon(self):
-        """Gets the 'common' section of config """
-        conf, err = self.getConfig()
-        if err is not None:
-            return None, err
-
-        if 'common' not in conf:
-            return None, Exception("Config file error: Missing 'common' tag")
-        return conf['common'], None
-
-    def getUsers(self):
-        """Gets the 'users' section of config """
-        conf, err = self.getConfig()
-        if err is not None:
-            return None, err
-
-        if 'users' not in conf:
-            return None, Exception("Config file error: Missing 'users' tag")
-        return conf['users'], None
-
-
-    def getPath(self):
-        """Gets the 'path' from config.common """
-        confCommon, err = self.getCommon()
-        if err is not None:
-            return None, err
-
-        if 'path' not in confCommon or confCommon['path']=="":
-            return None, Exception("Config file error: DTaaS directory path not set in TOML")
-        return  str(confCommon['path']), None
-
-    def getServerDNS(self):
-        """Gets the 'server-dns' from config.common """
-        confCommon, err = self.getCommon()
-        if err is not None:
-            return None, err
-
-        if 'server-dns' not in confCommon and confCommon['server-dns']=="":
-            return None, Exception("Config file error: The server dns isn't set in TOML")
-        return str(confCommon['server-dns']), None
-
-    def getAddUsersList(self):
-        """Gets the 'add' list from config.users """
-        confUsers, err = self.getUsers()
-        if err is not None:
-            return None, err
-
-        if 'add' not in confUsers:
-            return None, Exception("Config file error: No 'add' list in 'users' tag")
-        addUsersList = [ str(username) for username in confUsers['add']]
-
-        if len(addUsersList)==0:
-            return None, Exception('Config file error: users.add list is empty')
-        
-        return addUsersList, None
-
-    def getDeleteUsersList(self):
-        """Gets the 'delete' list from config.users """
-        confUsers, err = self.getUsers()
-        if err is not None:
-            return None, err
-
-        if 'delete' not in confUsers:
-            return None, Exception("Config file error: No 'delete' list in 'users' tag")
-        deleteUsersList = [str(username) for username in confUsers['delete']]
-
-        if len(deleteUsersList)==0:
-            return None, Exception('Config file error: users.delete list is empty')
-        
-        return deleteUsersList, None
+"""This file supports the DTaaS config class"""
+
+import click
+from src.pkg import utils
+
+class Config:
+    """The Config class for DTaaS"""
+
+    def __init__(self):
+        config, err = utils.importToml('dtaas.toml')
+        if err is not None:
+            raise click.ClickException("config initialisation failed: "+str(err))
+        self.data = config
+
+    def getConfig(self):
+        """Gets the config dictionary"""
+        if self.data is not None:
+            return self.data,None
+        return None, Exception("Config not initialised")
+
+    def getCommon(self):
+        """Gets the 'common' section of config """
+        conf, err = self.getConfig()
+        if err is not None:
+            return None, err
+
+        if 'common' not in conf:
+            return None, Exception("Config file error: Missing 'common' tag")
+        return conf['common'], None
+
+    def getUsers(self):
+        """Gets the 'users' section of config """
+        conf, err = self.getConfig()
+        if err is not None:
+            return None, err
+
+        if 'users' not in conf:
+            return None, Exception("Config file error: Missing 'users' tag")
+        return conf['users'], None
+
+
+    def getPath(self):
+        """Gets the 'path' from config.common """
+        confCommon, err = self.getCommon()
+        if err is not None:
+            return None, err
+
+        if 'path' not in confCommon or confCommon['path']=="":
+            return None, Exception("Config file error: DTaaS directory path not set in TOML")
+        return  str(confCommon['path']), None
+
+    def getServerDNS(self):
+        """Gets the 'server-dns' from config.common """
+        confCommon, err = self.getCommon()
+        if err is not None:
+            return None, err
+
+        if 'server-dns' not in confCommon and confCommon['server-dns']=="":
+            return None, Exception("Config file error: The server dns isn't set in TOML")
+        return str(confCommon['server-dns']), None
+
+    def getAddUsersList(self):
+        """Gets the 'add' list from config.users """
+        confUsers, err = self.getUsers()
+        if err is not None:
+            return None, err
+
+        if 'add' not in confUsers:
+            return None, Exception("Config file error: No 'add' list in 'users' tag")
+        addUsersList = [ str(username) for username in confUsers['add']]
+
+        if len(addUsersList)==0:
+            return None, Exception('Config file error: users.add list is empty')
+        
+        return addUsersList, None
+
+    def getDeleteUsersList(self):
+        """Gets the 'delete' list from config.users """
+        confUsers, err = self.getUsers()
+        if err is not None:
+            return None, err
+
+        if 'delete' not in confUsers:
+            return None, Exception("Config file error: No 'delete' list in 'users' tag")
+        deleteUsersList = [str(username) for username in confUsers['delete']]
+
+        if len(deleteUsersList)==0:
+            return None, Exception('Config file error: users.delete list is empty')
+        
+        return deleteUsersList, None
```

### Comparing `dtaas_cli-0.1.4/src/pkg/users.py` & `dtaas_cli-0.1.5/src/pkg/users.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-"""This file has functions that handle the user cli commands"""
-
-import subprocess
-import shutil
-from src.pkg import utils
-
-def getComposeConfig(username, server, path):
-    """Makes and returns the config for the user"""
-
-    template = {}
-    mapping = {
-        "${DTAAS_DIR}": path,
-        "${username}" : username,
-    }
-    try:
-        if server==utils.LOCALHOST_SERVER:
-            template, err = utils.importYaml('users.local.yml')
-            utils.checkError(err)
-            
-        else:
-            template, err = utils.importYaml('users.server.yml')
-            utils.checkError(err)
-            mapping["${SERVER_DNS}"] = server
-
-        config, err = utils.replaceAll(template, mapping)
-        utils.checkError(err)
-    except Exception as e:
-        return e
-
-    return config, None
-
-def createUserFiles(users, filePath):
-    """Creates all the users' workspace directories"""
-    for username in users:
-        shutil.copytree(filePath+'/template', filePath+'/'+username, dirs_exist_ok=True)
-
-def addUsersToCompose(users, compose, server, path):
-    """Adds all the users config to the compose dictionary"""
-    for username in users:
-        config, err = getComposeConfig(username, server, path)
-        if err is not None:
-            return err
-        compose['services'][username] = config
-    return None
-
-def startUserContainers(users):
-    """Starts all the user containers in the 'users' list"""
-
-    cmd = ["docker compose -f compose.users.yml up -d"]
-    for username in users:
-        cmd.append(username)
-
-    cmdStr = " ".join(cmd)
-    result = subprocess.run(cmdStr, shell=True, check=False)
-    if result.returncode !=0:
-        return Exception("failed to start containers")
-    return None
-
-def stopUserContainers(users):
-    """Stops all the user containers in the 'users' list"""
-
-    cmd = ["docker compose -f 'compose.users.yml' down"]
-    for username in users:
-        cmd.append(username)
-
-    cmdStr = " ".join(cmd)
-    result = subprocess.run(cmdStr, shell=True, check=False)
-    if result.returncode != 0:
-        return Exception("failed to stop containers")
-    return None
-
-def addUsers(configObj):
-    """add cli command handler"""
-    try:
-        compose, err = utils.importYaml('compose.users.yml')
-        utils.checkError(err)
-        userList, err = configObj.getAddUsersList()
-        utils.checkError(err)
-        server, err= configObj.getServerDNS()
-        utils.checkError(err)
-        path, err = configObj.getPath()
-        utils.checkError(err)
-    except Exception as e:
-        return e
-
-    if 'version' not in compose:
-        compose['version'] = '3'
-    if 'services' not in compose:
-        compose['services'] = {}
-    if 'networks' not in compose:
-        compose['networks'] = {
-            'users': {
-                'name': 'dtaas-users',
-                'external': True
-            }
-        }
-
-    try:
-        err = createUserFiles(userList, path+'/files')
-        utils.checkError(err)
-        err = addUsersToCompose(userList, compose, server, path)
-        utils.checkError(err)
-        err = utils.exportYaml(compose, 'compose.users.yml')
-        utils.checkError(err)
-        err = startUserContainers(userList)
-        utils.checkError(err)
-    except Exception as e:
-        return e
-
-    return None
-
-def deleteUser(configObj):
-    """delete cli command handler"""
-    try:
-        compose,err = utils.importYaml('compose.users.yml')
-        utils.checkError(err)
-        userList, err = configObj.getDeleteUsersList()
-        utils.checkError(err)
-        err = stopUserContainers(userList)
-        utils.checkError(err)
-    except Exception as e:
-        return e
-
-    for username in userList:
-        if 'services' not in compose:
-            return None
-        if username not in compose['services']:
-            return None
-        del compose['services'][username]
-
-    err = utils.exportYaml(compose, 'compose.users.yml')
-    if err is not None:
-        return err
-    
-    return None
+"""This file has functions that handle the user cli commands"""
+
+import subprocess
+import shutil
+from src.pkg import utils
+
+def getComposeConfig(username, server, path):
+    """Makes and returns the config for the user"""
+
+    template = {}
+    mapping = {
+        "${DTAAS_DIR}": path,
+        "${username}" : username,
+    }
+    try:
+        if server==utils.LOCALHOST_SERVER:
+            template, err = utils.importYaml('users.local.yml')
+            utils.checkError(err)
+            
+        else:
+            template, err = utils.importYaml('users.server.yml')
+            utils.checkError(err)
+            mapping["${SERVER_DNS}"] = server
+
+        config, err = utils.replaceAll(template, mapping)
+        utils.checkError(err)
+    except Exception as e:
+        return e
+
+    return config, None
+
+def createUserFiles(users, filePath):
+    """Creates all the users' workspace directories"""
+    for username in users:
+        shutil.copytree(filePath+'/template', filePath+'/'+username, dirs_exist_ok=True)
+
+def addUsersToCompose(users, compose, server, path):
+    """Adds all the users config to the compose dictionary"""
+    for username in users:
+        config, err = getComposeConfig(username, server, path)
+        if err is not None:
+            return err
+        compose['services'][username] = config
+    return None
+
+def startUserContainers(users):
+    """Starts all the user containers in the 'users' list"""
+
+    cmd = ["docker compose -f compose.users.yml up -d"]
+    for username in users:
+        cmd.append(username)
+
+    cmdStr = " ".join(cmd)
+    result = subprocess.run(cmdStr, shell=True, check=False)
+    if result.returncode !=0:
+        return Exception("failed to start containers")
+    return None
+
+def stopUserContainers(users):
+    """Stops all the user containers in the 'users' list"""
+
+    cmd = ["docker compose -f 'compose.users.yml' down"]
+    for username in users:
+        cmd.append(username)
+
+    cmdStr = " ".join(cmd)
+    result = subprocess.run(cmdStr, shell=True, check=False)
+    if result.returncode != 0:
+        return Exception("failed to stop containers")
+    return None
+
+def addUsers(configObj):
+    """add cli command handler"""
+    try:
+        compose, err = utils.importYaml('compose.users.yml')
+        utils.checkError(err)
+        userList, err = configObj.getAddUsersList()
+        utils.checkError(err)
+        server, err= configObj.getServerDNS()
+        utils.checkError(err)
+        path, err = configObj.getPath()
+        utils.checkError(err)
+    except Exception as e:
+        return e
+
+    if 'version' not in compose:
+        compose['version'] = '3'
+    if 'services' not in compose:
+        compose['services'] = {}
+    if 'networks' not in compose:
+        compose['networks'] = {
+            'users': {
+                'name': 'dtaas-users',
+                'external': True
+            }
+        }
+
+    try:
+        err = createUserFiles(userList, path+'/files')
+        utils.checkError(err)
+        err = addUsersToCompose(userList, compose, server, path)
+        utils.checkError(err)
+        err = utils.exportYaml(compose, 'compose.users.yml')
+        utils.checkError(err)
+        err = startUserContainers(userList)
+        utils.checkError(err)
+    except Exception as e:
+        return e
+
+    return None
+
+def deleteUser(configObj):
+    """delete cli command handler"""
+    try:
+        compose,err = utils.importYaml('compose.users.yml')
+        utils.checkError(err)
+        userList, err = configObj.getDeleteUsersList()
+        utils.checkError(err)
+        err = stopUserContainers(userList)
+        utils.checkError(err)
+    except Exception as e:
+        return e
+
+    for username in userList:
+        if 'services' not in compose:
+            return None
+        if username not in compose['services']:
+            return None
+        del compose['services'][username]
+
+    err = utils.exportYaml(compose, 'compose.users.yml')
+    if err is not None:
+        return err
+    
+    return None
```

