# Comparing `tmp/ck_apstra_api-0.2.9.tar.gz` & `tmp/ck_apstra_api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ck_apstra_api-0.2.9.tar", max compression
+gzip compressed data, was "ck_apstra_api-0.3.0.tar", max compression
```

## Comparing `ck_apstra_api-0.2.9.tar` & `ck_apstra_api-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-09-28 00:59:26.688335 ck_apstra_api-0.2.9/LICENSE
--rw-r--r--   0        0        0     1226 2023-11-24 23:30:58.367886 ck_apstra_api-0.2.9/README.md
--rw-r--r--   0        0        0     1158 2023-12-09 00:15:06.151366 ck_apstra_api-0.2.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-28 01:27:34.624568 ck_apstra_api-0.2.9/src/ck_apstra_api/__init__.py
--rwxr-xr-x   0        0        0    29965 2023-11-29 15:31:31.415103 ck_apstra_api-0.2.9/src/ck_apstra_api/apstra_blueprint.py
--rwxr-xr-x   0        0        0     7944 2023-12-09 00:16:53.341642 ck_apstra_api-0.2.9/src/ck_apstra_api/apstra_session.py
--rw-r--r--   0        0        0     9265 2023-11-29 15:30:29.638239 ck_apstra_api-0.2.9/src/ck_apstra_api/cli.py
--rw-r--r--   0        0        0    24400 2023-10-08 05:14:40.501949 ck_apstra_api-0.2.9/src/ck_apstra_api/generic_system.py
--rw-r--r--   0        0        0    11866 2023-10-23 01:37:34.339126 ck_apstra_api-0.2.9/src/ck_apstra_api/ip_endpoint.py
--rw-r--r--   0        0        0     2346 2023-11-17 18:23:57.618869 ck_apstra_api-0.2.9/src/ck_apstra_api/pull_device_configuration.py
--rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 ck_apstra_api-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-09-28 00:59:26.688335 ck_apstra_api-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1226 2023-11-24 23:30:58.367886 ck_apstra_api-0.3.0/README.md
+-rw-r--r--   0        0        0     1159 2024-04-20 22:02:21.427173 ck_apstra_api-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-28 01:27:34.624568 ck_apstra_api-0.3.0/src/ck_apstra_api/__init__.py
+-rwxr-xr-x   0        0        0    31713 2024-04-20 21:12:09.368208 ck_apstra_api-0.3.0/src/ck_apstra_api/apstra_blueprint.py
+-rwxr-xr-x   0        0        0     8554 2024-03-11 19:18:58.683250 ck_apstra_api-0.3.0/src/ck_apstra_api/apstra_session.py
+-rw-r--r--   0        0        0     9265 2023-11-29 15:30:29.638239 ck_apstra_api-0.3.0/src/ck_apstra_api/cli.py
+-rw-r--r--   0        0        0    27801 2024-04-20 21:55:03.988787 ck_apstra_api-0.3.0/src/ck_apstra_api/generic_system.py
+-rw-r--r--   0        0        0    11866 2023-10-23 01:37:34.339126 ck_apstra_api-0.3.0/src/ck_apstra_api/ip_endpoint.py
+-rw-r--r--   0        0        0     2346 2023-11-17 18:23:57.618869 ck_apstra_api-0.3.0/src/ck_apstra_api/pull_device_configuration.py
+-rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 ck_apstra_api-0.3.0/PKG-INFO
```

### Comparing `ck_apstra_api-0.2.9/LICENSE` & `ck_apstra_api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.2.9/README.md` & `ck_apstra_api-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.2.9/pyproject.toml` & `ck_apstra_api-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "ck-apstra-api"
-version = "0.2.9"
+version = "0.3.0"
 description = "An implementation to use Apstra API"
 authors = [ "Charlie Kim <ckim@juniper.net>" ]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "<3.13,>=3.9"
+python = "<3.13,>=3.11"
 requests = "^2.31.0"
 pandas = "^2.1.1"
 pydantic = "^2.4.2"
 openpyxl = "^3.1.2"
 python-dotenv = "^1.0.0"
 click = "^8.1.7"
```

### Comparing `ck_apstra_api-0.2.9/src/ck_apstra_api/apstra_blueprint.py` & `ck_apstra_api-0.3.0/src/ck_apstra_api/apstra_blueprint.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 #!/usr/bin/env python3
 
 import logging
+from typing import Optional, Tuple
 import uuid
+from enum import StrEnum
+from functools import cache
 
 from ck_apstra_api.apstra_session import CkApstraSession
 from ck_apstra_api.apstra_session import prep_logging
 
-# def pretty_yaml(data: dict, label: str) -> None:
-#     print(f"==== {label}\n{yaml.dump(data)}\n====")
 
-
-class CkEnum:
-    MEMBER_SWITCH = 'member-switch'
-    MEMBER_INTERFACE = 'member-interface'
-    EVPN_INTERFACE = 'evpn-interface'
+class CkEnum(StrEnum):
+    MEMBER_SWITCH = 'member_switch'
+    MEMBER_INTERFACE = 'member_interface'
+    EVPN_INTERFACE = 'evpn_interface'
     LINK = 'link'
     TAG = 'tag'
-    GENERIC_SYSTEM = 'generic-system'
-    GENERIC_SYSTEM_INTERFACE = 'gs-intf'
-    TAGGED_VLANS = 'tagged-vlans'
-    UNTAGGED_VLAN = 'untagged-vlan'
-    REDUNDANCY_GROUP = 'redundancy-group'
+    GENERIC_SYSTEM = 'generic_system'
+    GENERIC_SYSTEM_INTERFACE = 'gs_intf'
+    TAGGED_VLANS = 'tagged_vlans'
+    UNTAGGED_VLAN = 'untagged_vlan'
+    REDUNDANCY_GROUP = 'redundancy_group'
+    AE_INTERFACE = 'ae'
 
 
 class CkApstraBlueprint:
+    # __slots__ = ['session', 'label', 'design', 'id', 'logger', 'url_prefix']
 
     def __init__(self,
                  session: CkApstraSession,
                  label: str,
                  id: str = None) -> None:
         """
         Initialize a CkApstraBlueprint object.
@@ -39,49 +41,47 @@
         self.session = session
         self.label = label
         self.id = id
         self.logger = logging.getLogger(f"CkApstraBlueprint({label})")
         if id:
             this_blueprint = self.session.get_items(f"blueprints/{id}")
             self.label = this_blueprint['label']
+            self.design = this_blueprint['design']
         else:
             self.get_id()
         self.url_prefix = f"{self.session.url_prefix}/blueprints/{self.id}"
 
-        self.system_label_2_id_cache = {}  # { system_label: { id: id, interface_map_id: id, device_profile_id: id }
-        self.system_id_2_label_cache = {}  # { system_label: { id: id, interface_map_id: id, device_profile_id: id }
+        # self.system_label_2_id_cache = {}  # { system_label: { id: id, interface_map_id: id, device_profile_id: id }
+        # self.system_id_2_label_cache = {}  # { system_label: { id: id, interface_map_id: id, device_profile_id: id }
         self.logger.debug(f"{self.id=}")
 
 
     def get_id(self) -> str:
         """
         Get the ID of the blueprint.
 
         Returns:
             The ID of the blueprint.
         """
+        if self.id:
+            return self.id
         # get summary lists of all the blueprints
-        blueprints = self.session.get_items('blueprints')['items']
-        labels = [x['label'] for x in blueprints ]
-        # self.logger.debug(f"{self.label=} {labels=} {blueprints=}")
-        self.id = [x['id'] for x in blueprints if x['label'] == self.label][0]
-        # for blueprint in blueprints:
-        #     if blueprint['label'] == self.label:
-        #         self.id = blueprint['id']
-        #         break
+        for blueprints in self.session.get_items('blueprints')['items']:
+            if blueprints['label'] == self.label:
+                self.id = blueprints['id']
+                self.design = blueprints['design']
+                return self.id
+        #     bp = [x for x in blueprints if x['label'] == self.label][0]
+        # self.id = bp['id']
+        # self.design = bp['design']
+        # self.id = [x['id'] for x in blueprints if x['label'] == self.label][0]
         if self.id is None:
             raise ValueError(f"Blueprint '{self.label}' not found.")
         return self.id
 
-    # def get_id(self) -> None:
-    #     """
-    #     Print the ID of the blueprint.
-    #     """
-    #     return self.id
-
     def dump(self) -> dict:
         """
         Dump the blueprint.
           {
             'relationships': {},
             'nodes': {},
             'last_modified_at': '2023-10-30T22:25:08.490380Z',            
@@ -101,24 +101,25 @@
         Args:
             query: The query string.
             strip: Strip the query string. Required in case of multi-line query.
 
         Returns:
             The content of the items, the results of the query.
         """
-        query_candidate = query_string.strip()        
-        if multiline:
-            query_candidate = query_candidate.replace("\n", '')
+        query_candidate = query_string.strip().replace("\n", '')        
+        # if multiline:
+        #     query_candidate = query_candidate.replace("\n", '')
         if print_prefix:
             self.logger.info(f"{print_prefix}: {query_string}")
         url = f"{self.url_prefix}/qe"
         payload = {
             "query": query_candidate
         }
         response = self.session.session.post(url, json=payload)
+        # self.logger.warning(f"query() {query_string=} {multiline=} {response=} {response.content=}")
         if print_prefix or response.status_code != 200:
             self.logger.warning(f"status_code {response.status_code} != 200: {payload=}, response.text={response.text}")
         # the content should have 'items'. otherwise, the query would be invalid
         elif 'items' not in response.json():
             self.logger.warning(f"items does not exist: {query_string=}, {response.text=}")
         return response.json()['items']
     
@@ -128,120 +129,123 @@
         system_query = f"node('system', system_type='switch', management_level='full_control', name='{SYSTEM_NODE_NAME}')"
         resp = self.query(system_query)
         self.managed_system_nodes = [x[SYSTEM_NODE_NAME] for x in resp]
         return self.managed_system_nodes
 
     
     # return the first entry for the system
+    @cache
     def get_system_with_im(self, system_label):
         system_im = self.query(f"node('system', label='{system_label}', name='system').out().node('interface_map', name='im')")[0]
-        if system_label not in self.system_label_2_id_cache:
-            self.system_label_2_id_cache[system_label] = system_im['system']['id']
-            self.system_id_2_label_cache[system_im['system']['id']] = system_label
-            if  'interface_map_id' not in self.system_label_2_id_cache[system_label]:
-                self.system_label_2_id_cache[system_label]['interface_map_id'] = system_im['im']['id']
-                self.system_label_2_id_cache[system_label]['device_profile_id'] = system_im['im']['device_profile_id']
+        # if system_label not in self.system_label_2_id_cache:
+        #     # self.system_label_2_id_cache[system_label] = { 'id': system_im['system']['id'] }
+        #     # self.system_id_2_label_cache[system_im['system']['id']] = system_label
+        #     if  'interface_map_id' not in self.system_label_2_id_cache[system_label]:
+        #         self.system_label_2_id_cache[system_label]['interface_map_id'] = system_im['im']['id']
+        #         self.system_label_2_id_cache[system_label]['device_profile_id'] = system_im['im']['device_profile_id']
         return system_im
 
-    def get_system_node_from_label(self, system_label) -> dict:
+    # can be checked before the system creation - should not be cached in such case
+    # @cache
+    def get_system_node_from_label(self, system_label) -> Tuple[Optional[dict], Optional[str]]:
         """
         Return the system dict from the system label
         called from move_access_switch
         """
-        # cache the id of the system_label if not already cached
-        if system_label not in self.system_label_2_id_cache:
-            system_query_result = self.query(f"node('system', label='{system_label}', name='system')")
-            # skip if the system does not exist
-            if len(system_query_result) == 0:
-                return None            
-            id = system_query_result[0]['system']['id']
-            # sn = system_query_result[0]['system']['system_id']
-            # deploy_mode = system_query_result[0]['system']['deploy_mode']
-            # self.system_label_2_id_cache[system_label] = { 
-            #     'id': id,
-            #     'sn': sn,
-            #     'deploy_mode': deploy_mode
-            #     }
-            self.system_label_2_id_cache[system_label] = system_query_result[0]['system']
-            self.system_id_2_label_cache[id] = system_label
-        return self.system_label_2_id_cache[system_label]
+        query = f"node('system', label='{system_label}', name='system')"
+        system_query_result = self.query(query)
+        if len(system_query_result) == 0:
+            return None, f"{system_label} not found for {query} from {self.label}:{self.id}"
+        return system_query_result[0]['system'], None
+
 
     def get_system_label(self, system_id):
         '''
         Get the system label from the system id
         '''
         if system_id not in self.system_id_2_label_cache:
             return None
         return self.system_id_2_label_cache[system_id]
 
-    def get_server_interface_nodes(self, system_label, intf_name=None) -> str:
+    def get_server_interface_nodes(self, generic_system_label, intf_name=None) -> str:
         """
         Return interface nodes of a system label
             return CkEnum.MEMBER_INTERFACE and CkEnum.MEMBER_SWITCH
                 optionally CkEnum.EVPN_INTERFACE if it is a LAG
             It can be used for VLAN CT association
             TODO: implement intf_name in case of multiple link generic system
         TODO: cache generic system interface id
         called by move_access_switch
         """
-        interface_query = f"""
-            match(
-                node('system', system_type='server', label='{system_label}')
-                    .out('hosted_interfaces').node('interface', name='{CkEnum.GENERIC_SYSTEM_INTERFACE}')
-                    .out('link').node('link', name='{CkEnum.LINK}')
-                    .in_('link').node('interface', name='{CkEnum.MEMBER_INTERFACE}')
-                    .in_('hosted_interfaces').node('system', system_type='switch', name='{CkEnum.MEMBER_SWITCH}'),
-                optional(
-                    node('interface', po_control_protocol='evpn', name='{CkEnum.EVPN_INTERFACE}')
-                        .out('composed_of').node('interface')
-                        .out('composed_of').node(name='{CkEnum.MEMBER_INTERFACE}')
-                )
+        interface_query = f"""match(
+            node('system', system_type='server', label='{generic_system_label}', name='{CkEnum.GENERIC_SYSTEM}')
+                .out('hosted_interfaces').node('interface', name='{CkEnum.GENERIC_SYSTEM_INTERFACE}')
+                .out('link').node('link', name='{CkEnum.LINK}')
+                .in_('link').node('interface', if_type='ethernet', name='{CkEnum.MEMBER_INTERFACE}')
+                .in_('hosted_interfaces').node('system', system_type='switch', name='{CkEnum.MEMBER_SWITCH}'),
+            optional(
+                node(name='{CkEnum.REDUNDANCY_GROUP}')
+                    .out('hosted_interfaces').node('interface', po_control_protocol='evpn', name='{CkEnum.EVPN_INTERFACE}')
+                    .out('composed_of').node('interface')
+                    .out('composed_of').node(name='{CkEnum.MEMBER_INTERFACE}')
+            ),
+            optional(
+                node(name='{CkEnum.MEMBER_INTERFACE}')
+                    .in_('composed_of').node('interface', name='{CkEnum.AE_INTERFACE}')
+            ),
+            optional(
+                node('tag', name='{CkEnum.TAG}').out().node(name='{CkEnum.LINK}')
             )
-        """
+        )"""
+        # self.logger.warning(f"get_server_interface_nodes() {system_label=} {interface_query=}")
         return self.query(interface_query, multiline=True)
 
-    def get_switch_interface_nodes(self, system_labels, intf_name=None) -> str:
+    def get_switch_interface_nodes(self, switch_labels=None, intf_name=None) -> str:
         """
         Return interface nodes of the switches
-            system_labels: list of system labels or a str for the single system label
+            switch_labels: list of system labels, a str for the single system label, or None for all switches
             return CkEnum.MEMBER_INTERFACE and CkEnum.MEMBER_SWITCH
                 optionally CkEnum.EVPN_INTERFACE if it is a LAG
             It can be used for VLAN CT association
             TODO: implement intf_name in case of multiple link generic system
         TODO: cache generic system interface id
         """
-        the_system_labels = system_labels if isinstance(system_labels, list) else [system_labels] if isinstance(system_labels, str) else []
-        if len(the_system_labels) == 0:
-            self.logger.warning(f"{system_labels=} is not a list or string")
+        if switch_labels is None:
+            label_selection = ''
+        elif isinstance(switch_labels, list):
+            label_selection = f" label=is_in({switch_labels}),"
+        elif isinstance(switch_labels, str):
+            label_selection = f" label='{switch_labels}',"
+        else:
+            self.logger.warning(f"{switch_labels=} is not a list or string")
             return []
         intf_name_filter = f", if_name='{intf_name}'" if intf_name else ""
-        interface_query = f"""
-            match(
-                node('system', system_type='server', name='{CkEnum.GENERIC_SYSTEM}')
-                    .out('hosted_interfaces').node('interface', name='{CkEnum.GENERIC_SYSTEM_INTERFACE}')
-                    .out('link').node('link', name='{CkEnum.LINK}')
-                    .in_('link').node('interface', if_type='ethernet', name='{CkEnum.MEMBER_INTERFACE}'{intf_name_filter})
-                    .in_('hosted_interfaces').node('system', system_type='switch', label=is_in({the_system_labels}), name='{CkEnum.MEMBER_SWITCH}'),
-                optional(
-                    node('redundancy_group')
-                        .out('hosted_interfaces').node('interface', po_control_protocol='evpn', name='{CkEnum.EVPN_INTERFACE}')
-                        .out('composed_of').node('interface')
-                        .out('composed_of').node(name='{CkEnum.MEMBER_INTERFACE}')
-                ),
-                optional(
-                    node('tag', name='tag').out().node(name='{CkEnum.LINK}')
-                    )
+        interface_query = f"""match(
+            node('system', system_type='server', name='{CkEnum.GENERIC_SYSTEM}')
+                .out('hosted_interfaces').node('interface', name='{CkEnum.GENERIC_SYSTEM_INTERFACE}')
+                .out('link').node('link', name='{CkEnum.LINK}')
+                .in_('link').node('interface', if_type='ethernet', name='{CkEnum.MEMBER_INTERFACE}'{intf_name_filter})
+                .in_('hosted_interfaces').node('system', system_type='switch',{label_selection} name='{CkEnum.MEMBER_SWITCH}'),
+            optional(
+                node(name='{CkEnum.REDUNDANCY_GROUP}')
+                    .out('hosted_interfaces').node('interface', po_control_protocol='evpn', name='{CkEnum.EVPN_INTERFACE}')
+                    .out('composed_of').node('interface')
+                    .out('composed_of').node(name='{CkEnum.MEMBER_INTERFACE}')
+            ),
+            optional(
+                node(name='{CkEnum.MEMBER_INTERFACE}')
+                    .in_('composed_of').node('interface', name='{CkEnum.AE_INTERFACE}')
+            ),
+            optional(
+                node('tag', name='{CkEnum.TAG}').out().node(name='{CkEnum.LINK}')
             )
-        """
-        # self.logger.debug(f"{interface_query=}")
-        interface_nodes = self.query(interface_query, multiline=True)
-        # self.logger.debug(f"{interface_nodes=}")
+        )"""
+        interface_nodes = self.query(interface_query)
         return interface_nodes
 
-
     def get_single_vlan_ct_id(self, vn_id: int):
         '''
         Get the single VLAN CT ID
 
         Return tuple of (tagged CT id, untagged CT id)
         '''
         ct_list_spec = f"""
@@ -259,14 +263,16 @@
         # untagged_ct = [x['id'] for x in ct_list if x and 'untagged' in x['ep_endpoint_policy']['attributes']][0] or None
         return (tagged_ct, untagged_ct)
 
     def get_ct_ids(self, ct_labels: list) -> list:
         '''
         Get the CT IDs from the CT labels
         '''
+        if isinstance(ct_labels, str):
+            ct_labels = [ct_labels]
         ct_list_query = f"""
             node('ep_endpoint_policy', policy_type_name='batch', label=is_in({ct_labels}), name='ep')
         """
         ct_list = self.query(ct_list_query, multiline=True)
         if len(ct_list) == 0:
             self.logger.debug(f"No CTs found for {ct_labels=}")
             return []
@@ -395,33 +401,36 @@
             "tags": [],
             "nodes": [ "atl1tor-r5r14a<->_atl_rack_1_001_sys010(link-000000002)[1]" ],
             "remove": [],
             "assigned_to_all": []        
         '''
         tagging_spec = {
             'add': [],
-            'tags': [],
+            # 'tags': [],
             'nodes': [],
             'remove': [],
             'assigned_to_all': [],
         }
         # take string or list 
         the_nodes_list = nodes if isinstance(nodes, list) else [nodes] if isinstance(nodes, str) else []
         if len(the_nodes_list) == 0:
             self.logger.warning(f"{nodes=} is not a list or string")
             return
+        # in case of single tags_to_add
+        if isinstance(tags_to_add, str):
+            tags_to_add = [tags_to_add]
         # no need to check the present of tags in tags_to_add 
         tag_nodes = self.query(f"node(id=is_in({the_nodes_list})).in_().node('tag', label=is_in({tags_to_add}), name='tag')")
         are_tags_the_same = len(tag_nodes) == (len(tags_to_add) * len(nodes))
         self.logger.debug(f"{nodes=} {the_nodes_list=} {tags_to_add=}, {tags_to_remove=}, {are_tags_the_same=} {tag_nodes}")
 
         # self.logger.debug(f"{nodes=} {tags_to_add=}, {tags_to_remove=} {are_tags_the_same=}")
         # The tags are the same as the existing tags
-        if are_tags_the_same or (not tags_to_add and not tags_to_remove):
-            return
+        # if are_tags_the_same or (not tags_to_add and not tags_to_remove):
+        #     return
         tagging_spec['nodes'] = the_nodes_list
         tagging_spec['add'] = tags_to_add
         tagging_spec['remove'] = tags_to_remove
         return self.session.session.post(f"{self.url_prefix}/tagging", json=tagging_spec, params={'aync': 'full'})
 
     def post_item(self, item_url: str, post_spec: dict, params={'type': 'staging'}):
         '''
@@ -431,20 +440,21 @@
 
     def put_item(self, item_url: str, put_spec: dict, params={'type': 'staging'}):
         '''
         Put an item
         '''
         return self.session.session.put(f"{self.url_prefix}/{item_url}", json=put_spec, params=params)
 
-    def batch(self, batch_spec: dict, params=None) -> None:
+    def batch(self, batch_spec: dict, params=None) -> dict:
         '''
         Run API commands in batch
         '''
         url = f"{self.url_prefix}/batch"
-        self.session.session.post(url, json=batch_spec, params=params)
+        result = self.session.session.post(url, json=batch_spec, params=params)
+        return result
 
     # def get_cts_on_generic_system_with_only_ae(self, generic_system_label) -> list:
     #     '''
     #     Get the CTS of generic system with single AE
     #     '''
     #     ct_list_spec = f"""
     #         match(
@@ -693,15 +703,36 @@
     from dotenv import load_dotenv
     import os
 
     load_dotenv()
     log_level = os.getenv('logging_level', 'DEBUG')
     prep_logging(log_level)
 
-    apstra_server_host = os.getenv('apstra_server_host')
-    apstra_server_port = os.getenv('apstra_server_port')
-    apstra_server_username = os.getenv('apstra_server_username')
-    apstra_server_password = os.getenv('apstra_server_password')
+    # apstra_server_host = os.getenv('apstra_server_host')
+    # apstra_server_port = os.getenv('apstra_server_port')
+    # apstra_server_username = os.getenv('apstra_server_username')
+    # apstra_server_password = os.getenv('apstra_server_password')
+    apstra_server_host = '10.85.192.50'
+    apstra_server_port = '443'
+    apstra_server_username = 'admin'
+    apstra_server_password = 'zaq1@WSXcde3$RFV'
 
     apstra = CkApstraSession(apstra_server_host, apstra_server_port, apstra_server_username, apstra_server_password)
-    bp = CkApstraBlueprint(apstra, os.getenv('main_blueprint'))
+    # bp = CkApstraBlueprint(apstra, os.getenv('main_blueprint'))
+    bp = CkApstraBlueprint(apstra, 'infor-pristine')
+    # breakpoint()
+    # bp = CkApstraBlueprint(apstra, 'ATLANTA-Master')
+    # links = bp.get_switch_interface_nodes(['atl1tor-r5r15a', 'atl1tor-r5r15b'])
+    links = bp.get_switch_interface_nodes('atl1tor-r5r15a')
+    # links = bp.get_switch_interface_nodes()
+    # links = bp.get_server_interface_nodes('r5r15-sys018')
+    # # links = bp.get_server_interface_nodes('atl1tor-r1r16')
+    print(f"{links=} {len(links)=}")
+    # # query_str1 = f"""match(
+    # #     node('virtual_network', vn_id='101353', name='vn').in_('member_vns').node('security_zone', name='rz'),
+    # #     node(name='vn').out('instantiated_by').node('vn_instance', name='vn_instance')
+    # #         .in_('hosted_vn_instances').node(name='switch')
+    # #         .in_('composed_of_systems').node('redundancy_group', name='redundancy_group'),
+    # # )"""
+    # result = bp.query(query_str1)
+    # print(f"{query_str1=} {len(result)=} {result=}")
     print(bp.get_id())
```

### Comparing `ck_apstra_api-0.2.9/src/ck_apstra_api/apstra_session.py` & `ck_apstra_api-0.3.0/src/ck_apstra_api/apstra_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,18 +61,32 @@
         self.session = requests.Session()
         urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
         self.session.verify = False
         self.session.headers.update({'Content-Type': "application/json"})
         self.url_prefix = f"https://{self.host}:{self.port}/api"
         self.last_error = None
 
+        self.get_version()
         self.login()
 
         self.device_profile_cache = {}  # { device_profile_id: data }
 
+    def get_version(self) -> str:
+        """
+        Get the version of the Apstra controller.
+
+        Returns:
+            The version of the Apstra controller.
+        """
+        url = f"{self.url_prefix}/versions/server"
+        response = self.session.get(url)
+        version = response.json()["version"]
+        self.version = version
+        return self.version
+
     def login(self) -> None:
         """
         Log in to the Apstra controller.
         """
         url = f"{self.url_prefix}/user/login"
         payload = {
             "username": self.username,
@@ -231,21 +245,26 @@
     from dotenv import load_dotenv
     import os
 
     load_dotenv()
     log_level = os.getenv('logging_level', 'DEBUG')
     prep_logging(log_level)
 
-    apstra_server_host = os.getenv('apstra_server_host')
-    apstra_server_port = os.getenv('apstra_server_port')
-    apstra_server_username = os.getenv('apstra_server_username')
-    apstra_server_password = os.getenv('apstra_server_password')
+    # apstra_server_host = os.getenv('apstra_server_host')
+    # apstra_server_port = os.getenv('apstra_server_port')
+    # apstra_server_username = os.getenv('apstra_server_username')
+    # apstra_server_password = os.getenv('apstra_server_password')
+    apstra_server_host = '10.85.192.50'
+    apstra_server_port = '443'
+    apstra_server_username = 'admin'
+    apstra_server_password = 'zaq1@WSXcde3$RFV'
 
     apstra = CkApstraSession(apstra_server_host, apstra_server_port, apstra_server_username, apstra_server_password)
     apstra.print_token()
 
+    logging.info(f"version {apstra.version}")
     logging.info(f"Done {apstra.is_online()=}")
 
     logouted = apstra.logout()
     logging.info(f"Done {logouted=}")
 
     logging.info(f"Done {apstra.is_online()=}")
```

### Comparing `ck_apstra_api-0.2.9/src/ck_apstra_api/cli.py` & `ck_apstra_api-0.3.0/src/ck_apstra_api/cli.py`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.2.9/src/ck_apstra_api/generic_system.py` & `ck_apstra_api-0.3.0/src/ck_apstra_api/generic_system.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 
 import logging
-import pandas as pd
 from math import isnan
 from pathlib import Path
 from pydantic import BaseModel, validator, StrictStr, field_validator, Field
-from typing import List, Optional, Any, TypeVar, Annotated
-import numpy as np
+from typing import List, Optional, Any, Tuple, TypeVar, Annotated
 import os
 import uuid
 
-import click
-
-from ck_apstra_api.apstra_session import prep_logging
-from ck_apstra_api.cli import CkJobEnv
+from ck_apstra_api.apstra_session import CkApstraSession
 from ck_apstra_api.apstra_blueprint import CkApstraBlueprint, CkEnum
 
 class GenericSystemModel(BaseModel):
     """
     The variables from the excel sheet generic_systems
     """
     blueprint: str
@@ -104,27 +99,29 @@
     input_file_path = Path(excel_file_sting) 
     df = pd.read_excel(input_file_path, sheet_name=sheet_name, header=[1])
     df = df.replace({np.nan: None})
 
     df.apply(process_row, axis=1)
     return generic_system_data
 
-@click.command(name='read-generic-systems')
-def click_read_generic_systems():
-    job_env = CkJobEnv()
-    generic_systems = read_generic_systems(job_env.excel_input_file, 'generic_systems')
-    for bp_label, bp_data in generic_systems.items():
-        logging.debug(f"{bp_label=}")
-        for gs_label, gs_links_list in bp_data.items():
-            logging.debug(f"{gs_label=}")
-            for link in gs_links_list:
-                logging.debug(f"{link=}")
-
-def form_lacp(job_env: CkJobEnv, generic_system_label: str, generic_system_links_list: list):
-    bp = job_env.main_bp
+# @click.command(name='read-generic-systems')
+# def click_read_generic_systems():
+#     job_env = CkJobEnv()
+#     generic_systems = read_generic_systems(job_env.excel_input_file, 'generic_systems')
+#     for bp_label, bp_data in generic_systems.items():
+#         logging.debug(f"{bp_label=}")
+#         for gs_label, gs_links_list in bp_data.items():
+#             logging.debug(f"{gs_label=}")
+#             for link in gs_links_list:
+#                 logging.debug(f"{link=}")
+
+# def form_lacp(job_env: CkJobEnv, generic_system_label: str, generic_system_links_list: list):
+def form_lacp(apstra_bp, generic_system_label: str, generic_system_links_list: list):
+    # bp = job_env.main_bp
+    bp = apstra_bp
     bp_label = bp.label
     lag_spec = {
         'links': {
             # <link_node_id>: {
             #     'group_label': group_label,
             #     'lag_mode': lag_mode,
             # }
@@ -140,17 +137,17 @@
             logging.warning(f"Skipping: Generic system {generic_system_label} has invalid lag_mode {lag_mode}")
             continue
         link_id_num += 1
         group_label = f"link{link_id_num}"
         # iterate over the 4 member interfaces
         for member_number in range(4):
             member_number += 1
-            sw_label = link[f"label{member_number}"]
-            sw_ifname = link[f"ifname{member_number}"]
-            gs_ifname = link[f"gs_ifname{member_number}"]
+            sw_label = link[f"label{member_number}"] if f"label{member_number}" in link else link[f"switch{member_number}"]
+            sw_ifname = link[f"ifname{member_number}"] if f"ifname{member_number}" in link else link[f"switch_intf{member_number}"]
+            gs_ifname = link[f"gs_ifname{member_number}"] if f"gs_ifname{member_number}" in link else link[f"server_intf{member_number}"]
             # skip if now switch is defined
             if not sw_label or not sw_ifname:
                 continue
             if sw_ifname[:2] not in ['et', 'xe', 'ge']:
                 logging.warning(f"Skipping: Generic system {generic_system_label} has invalid interface name {sw_ifname}")
                 continue
             switch_link_nodes = bp.get_switch_interface_nodes([sw_label], sw_ifname)
@@ -172,36 +169,38 @@
         logging.debug(f"{lag_spec=}")
         lag_updated = bp.patch_leaf_server_link_labels(lag_spec)
         if lag_updated:
             logging.warning(f"Unexpected return: LACP updated for generic system {generic_system_label} in blueprint {bp_label}: {lag_updated}")
         # logging.debug(f"lag_updated: {lag_updated}")
     
 
-def add_tags(job_env: CkJobEnv, generic_system_label: str, generic_system_links_list: list):
-    bp = job_env.main_bp
-    bp_label = bp.label
+# def add_tags(job_env: CkJobEnv, generic_system_label: str, generic_system_links_list: list):
+#     bp = job_env.main_bp
+def add_tags(apstra_bp, generic_system_label: str, generic_system_links_list: list) -> Tuple[Optional[str], Optional[str]]:
+    bp = apstra_bp
     link_id_num = 0
-    generic_system_node = bp.get_system_node_from_label(generic_system_label)
-    if generic_system_node is None:
-        logging.warning(f"Skipping: Generic system {generic_system_label} does not exist in blueprint {bp_label}")
-        return
+    generic_system_node, error = bp.get_system_node_from_label(generic_system_label)
+    if error:
+        logging.warning(f"add_tags skipping: {error}")
+        return None, f"add_tags {generic_system_label} not found in blueprint {bp.label}"
     generic_system_id = generic_system_node['id']
     for link in generic_system_links_list:
         link_id_num += 1
         group_label = f"link{link_id_num}"
         gs_tags = link['gs_tags']
         if len(gs_tags) > 0:
             bp.post_tagging(generic_system_id, tags_to_add=gs_tags)            
         # iterate over the 4 member interfaces        
         for member_number in range(4):
             member_number += 1
-            sw_label = link[f"label{member_number}"]
-            sw_ifname = link[f"ifname{member_number}"]
-            gs_ifname = link[f"gs_ifname{member_number}"]
-            member_tags = link[f"tags{member_number}"]  # list of string(tag)
+            # take care of old one like label1, label2, label3, label4
+            sw_label = link[f"label{member_number}"] if f"label{member_number}" in link else link[f"switch{member_number}"]
+            sw_ifname = link[f"ifname{member_number}"] if f"ifname{member_number}" in link else link[f"switch_intf{member_number}"]
+            gs_ifname = link[f"gs_ifname{member_number}"] if f"gs_ifname{member_number}" in link else link[f"server_intf{member_number}"]
+            member_tags = link[f"tags{member_number}"]  if f"tags{member_number}" in link else [] # list of string(tag)
             # the switch label and the interface should be defined. If not, skip
             if not sw_label or not sw_ifname:
                 continue
             # the switch interface name should be legit
             if sw_ifname[:2] not in ['et', 'xe', 'ge']:
                 logging.warning(f"Skipping: Generic system {generic_system_label} has invalid interface name {sw_ifname}")
                 continue
@@ -213,16 +212,18 @@
             # logging.debug(f"{member_tags=}")
             if len(member_tags) > 0:
                 logging.debug(f"{member_tags=}")
                 bp.post_tagging(link_node_id, tags_to_add=member_tags)
                 
 
 
-def rename_generic_system_intf(job_env: CkJobEnv, generic_system_label: str, generic_system_links_list: list):
-    bp = job_env.main_bp
+# def rename_generic_system_intf(job_env: CkJobEnv, generic_system_label: str, generic_system_links_list: list):
+#     bp = job_env.main_bp
+def rename_generic_system_intf(apstra_bp, generic_system_label: str, generic_system_links_list: list):
+    bp = apstra_bp
     bp_label = bp.label
     patch_cable_map_spec = {
         'links': [
             # {
             #     'endpoints': [
             #         {
             #             'interface': {
@@ -242,17 +243,17 @@
     }
     link_id_num = 0
     for link in generic_system_links_list:
         link_id_num += 1
         group_label = f"link{link_id_num}"
         for member_number in range(4):
             member_number += 1
-            sw_label = link[f"label{member_number}"]
-            sw_ifname = link[f"ifname{member_number}"]
-            gs_ifname = link[f"gs_ifname{member_number}"]
+            sw_label = link[f"label{member_number}"] if f"label{member_number}" in link else link[f"switch{member_number}"]
+            sw_ifname = link[f"ifname{member_number}"] if f"ifname{member_number}" in link else link[f"switch_intf{member_number}"]
+            gs_ifname = link[f"gs_ifname{member_number}"] if f"gs_ifname{member_number}" in link else link[f"server_intf{member_number}"]
             # skip if data is missing
             if not sw_label or not sw_ifname:
                 continue
             if sw_ifname[:2] not in ['et', 'xe', 'ge']:
                 logging.warning(f"Skipping: Generic system {generic_system_label} has invalid interface name {sw_ifname}")
                 continue
             switch_link_nodes = bp.get_switch_interface_nodes([sw_label], sw_ifname)
@@ -291,17 +292,20 @@
         logging.debug(f"{patch_cable_map_spec=}")
         patch_cable_map_spec_updated = bp.patch_cable_map(patch_cable_map_spec)
         if patch_cable_map_spec_updated:
             logging.warning(f"Unexpected return: cable map updated for generic system {generic_system_label} in blueprint {bp_label}: {patch_cable_map_spec_updated}")
         # logging.debug(f"patch_cable_map_spec_updated: {patch_cable_map_spec_updated}"
 
 
-def assign_connectivity_templates(job_env: CkJobEnv, generic_system_label: str, gs_links_list: list):
+# def assign_connectivity_templates(job_env: CkJobEnv, generic_system_label: str, gs_links_list: list):
+#     # update connectivity templates - this should be run after lag update
+#     bp = job_env.main_bp
+def assign_connectivity_templates(apstra_bp, generic_system_label: str, gs_links_list: list):
     # update connectivity templates - this should be run after lag update
-    bp = job_env.main_bp
+    bp = apstra_bp
     bp_label = bp.label
     ct_assign_spec = {
         'application_points': [
             # {
             #     'id': <interface_id>,
             #     'policies': [
             #         {
@@ -312,52 +316,56 @@
             # }
         ]
 
     }
     for link in gs_links_list:
         # ct_names takes precedence
         ct_names = link['ct_names']
-        untagged_vlan = link['untagged_vlan']
-        tagged_vlans = link['tagged_vlans']
+        # untagged_vlan = link['untagged_vlan']
+        # tagged_vlans = link['tagged_vlans']
         ct_ids = []
-        if (ct_names and len(ct_names) == 0) and untagged_vlan is None and len(tagged_vlans) == 0:
+        # if (ct_names and len(ct_names) == 0) and untagged_vlan is None and len(tagged_vlans) == 0:
+        if ct_names and len(ct_names) == 0:
             logging.debug(f"Skipping: Generic system {generic_system_label} has no CTs {link=}")
             continue
         if ct_names:
-            ct_ids = bp.get_ct_ids(ct_names)
-            if len(ct_ids) != len(ct_names):
-                logging.error(f"Skipping: Generic system {generic_system_label} has wrong data {ct_names=} {ct_ids=}")
-                continue
-        else:
-            # can have untagged too
-            # TODO: check if the CTs exist and create if not
-            # TODO: naming rule
-            if link['tagged_vlans']:
-                for tagged_vlan_id in link['tagged_vlans']:
-                    ct_ids.append(bp.get_single_vlan_ct_or_create(tagged_vlan_id, is_tagged=True))
-                # logging.debug(f"{untagged_vlan=}, {ct_ids=}")
-            if untagged_vlan:
-                # conentional name: vn123-untagged
-                # untagged_vlan_name = f"vn{untagged_vlan_id}-untagged"
-                # ct_ids = bp.get_ct_ids([untagged_vlan_name])
-                # if len(ct_ids) != 1:
-                #     added = bp.add_single_vlan_ct(200000 + untagged_vlan_id, untagged_vlan_id, is_tagged=False)
-                #     logging.debug(f"Added CT {untagged_vlan_name}: {added}")
-                # ct_ids = bp.get_ct_ids([untagged_vlan_name])
-                # logging.debug(f"{untagged_vlan_name=}, {ct_ids=}")
-                ct_ids.append(bp.get_single_vlan_ct_or_create(untagged_vlan, is_tagged=False))
-                logging.debug(f"{untagged_vlan=}, {ct_ids=}")
+            ct_name_list = ct_names.split(',')
+            ct_ids = bp.get_ct_ids(ct_name_list)
+            if len(ct_ids) != len(ct_name_list):
+                logging.error(f"Skipping: Generic system {generic_system_label} has wrong data {ct_name_list=} {ct_ids=}")
+                continue
+        # else:
+        #     # can have untagged too
+        #     # TODO: check if the CTs exist and create if not
+        #     # TODO: naming rule
+        #     if link['tagged_vlans']:
+        #         for tagged_vlan_id in link['tagged_vlans']:
+        #             ct_ids.append(bp.get_single_vlan_ct_or_create(tagged_vlan_id, is_tagged=True))
+        #         # logging.debug(f"{untagged_vlan=}, {ct_ids=}")
+        #     if untagged_vlan:
+        #         # conentional name: vn123-untagged
+        #         # untagged_vlan_name = f"vn{untagged_vlan_id}-untagged"
+        #         # ct_ids = bp.get_ct_ids([untagged_vlan_name])
+        #         # if len(ct_ids) != 1:
+        #         #     added = bp.add_single_vlan_ct(200000 + untagged_vlan_id, untagged_vlan_id, is_tagged=False)
+        #         #     logging.debug(f"Added CT {untagged_vlan_name}: {added}")
+        #         # ct_ids = bp.get_ct_ids([untagged_vlan_name])
+        #         # logging.debug(f"{untagged_vlan_name=}, {ct_ids=}")
+        #         ct_ids.append(bp.get_single_vlan_ct_or_create(untagged_vlan, is_tagged=False))
+        #         logging.debug(f"{untagged_vlan=}, {ct_ids=}")
         if 'ct_ids' not in locals():
             logging.debug(f"Skipping: Generic system {generic_system_label} has no CTs")
             continue
         logging.debug(f"{link=} {ct_ids=}")
-        intf_nodes = bp.get_switch_interface_nodes([link['label1']], link['ifname1'])
+        # intf_nodes = bp.get_switch_interface_nodes([link['label1']], link['ifname1'])
+        intf_nodes = bp.get_switch_interface_nodes([link['switch1']], link['switch_intf1'])
         if len(intf_nodes) == 0:
             logging.warning(f"{len(intf_nodes)=}, {intf_nodes=}")
-            logging.warning(f"Skipping: Generic system {generic_system_label} has invalid interface {link['label1']}:{link['ifname1']}")
+            # logging.warning(f"Skipping: Generic system {generic_system_label} has invalid interface {link['label1']}:{link['ifname1']}")
+            logging.warning(f"Skipping: Generic system {generic_system_label} has invalid interface {link['switch1']}:{link['switch_intf1']}")
             continue
         ap_id = None
         if intf_nodes[0][CkEnum.EVPN_INTERFACE]:
             ap_id = intf_nodes[0][CkEnum.EVPN_INTERFACE]['id']
         else:
             ap_id = intf_nodes[0][CkEnum.MEMBER_INTERFACE]['id']
         ct_assign_spec['application_points'].append({
@@ -369,207 +377,267 @@
         # logging.debug(f"{ct_assign_spec=}")
         ct_assign_updated = bp.patch_obj_policy_batch_apply(ct_assign_spec, params={'async': 'full'})
         logging.debug(f"CT assign updated for generic system {generic_system_label} in blueprint {bp_label}: {ct_assign_updated} {ct_assign_spec=}")
         # logging.debug(f"ct_assign_updated: {ct_assign_updated}"
 
 
 
-def add_generic_systems(job_env: CkJobEnv, generic_systems: dict):
+def add_single_generic_system(bp, gs_label, gs_links_list) -> Tuple[Optional[str], Optional[str]]:
+    # gs_count += 1
+    gs_link_total = len(gs_links_list)
+    # logging.info(f"add_generic_system Adding generic system {gs_count}/{gs_total}: {gs_label} with {gs_link_total} links")
+    existing_gs, _ = bp.get_system_node_from_label(gs_label)
+    if existing_gs:
+        logging.warning(f"add_single_generic_system Skipping: Generic system {gs_label} already exists in blueprint {bp.label}")
+        # TODO: verify the content
+        return None, None
+    # if gs_link_total > 1:
+    #     logging.warning(f"Adding generic system {gs_label} with {gs_link_total} links\n{gs_links_list}")
+    #     return
+    generic_system_spec = {
+        'links': [],
+        'new_systems': [],
+    }
+    # to form logical device
+    speed_count = {}
+    system_type = 'server'
+
+    for link in gs_links_list:
+    #     logging.debug(f"{link=}")
+        link_speed = link['speed']
+        system_type = 'external' if link['is_external'] else 'server'
+        for link_id_num in range(1, 5):
+            # link_id_num = link_number + 1
+            switch_label = link[f"switch{link_id_num}"]
+            this_ifname = link[f"switch_intf{link_id_num}"]
+            # skip if data is missing
+            if not switch_label:
+                continue
+            if this_ifname[:2] not in ['et', 'xe', 'ge']:
+                error_message = f"Error: wrong interface for {gs_label} - {switch_label}:{this_ifname}"
+                # logging.warning(f"add_single_generic_system Error : {error_message}")
+                return None, error_message
+            logging.debug(f"{switch_label=}")
+            switch_node, error = bp.get_system_node_from_label(switch_label)
+            if error:
+                error_message = f"Error: generic system {gs_label} has absent switch {switch_label}\n\tFrom get_system_node_from_label {error}"
+                # logging.warning(f"add_single_generic_system {error_message}")
+                return None, error_message
+            switch_id = switch_node['id']
+            link_spec = {
+                'switch': {
+                    'system_id': switch_id,
+                    'transformation_id': bp.get_transformation_id(link[f"switch{link_id_num}"], this_ifname , link_speed),
+                    'if_name': link[f"switch_intf{link_id_num}"],
+                },
+                'system': {
+                    'system_id': None,
+                },
+                # 'lag_mode':link['lag_mode'],
+                'lag_mode': None,
+            }
+            generic_system_spec['links'].append(link_spec)
+            # speed_count[link_speed] = getattr(speed_count, link_speed, 0) + 1
+            logging.debug(f"{link_speed=}, {speed_count=}")
+            if link_speed not in speed_count:
+                speed_count[link_speed] = 1
+            else:
+                speed_count[link_speed] += 1
+
+    new_system = {
+        'system_type': system_type,
+        'label': gs_label,
+        'port_channel_id_min': 0,
+        'port_channel_id_max': 0,
+        'logical_device': {
+            'display_name': None,
+            'id': None,
+            'panels': [
+                {
+                    'panel_layout': {
+                        'row_count': 1,
+                        'column_count': sum(speed_count.values()),
+                    },
+                    'port_indexing': {
+                        'order': 'T-B, L-R',
+                        'start_index': 1,
+                        'schema': 'absolute'
+                    },
+                    "port_groups": [
+                        # {
+                        #     "count": 4,
+                        #     "speed": {
+                        #         "unit": "G",
+                        #         "value": 10
+                        #     },
+                        #     "roles": [
+                        #         "leaf",
+                        #         "access"
+                        #     ]
+                        # }
+                    ]
+                }
+            ]
+        },
+    }
+    display_name = 'auto'
+    for speed, count in speed_count.items():
+        port_group = {
+            'count': count,
+            'speed': {
+                'unit': speed[-1],
+                'value': int(speed[:-1]),
+            },
+            'roles': ['leaf', 'access'],
+        }
+        new_system['logical_device']['panels'][0]['port_groups'].append(port_group)
+        display_name = f"{display_name}-{count}x{speed}"
+    new_system['logical_device']['display_name'] = display_name
+    new_system['logical_device']['id'] = display_name
+    generic_system_spec['new_systems'].append(new_system)
+    logging.debug(f"add_single_generic_system {generic_system_spec=}, {speed_count=}")
+
+    generic_system_created = bp.add_generic_system(generic_system_spec)
+    logging.info(f"add_single_generic_system {gs_label} created in blueprint {bp.label}")
+
+    return None, None
+                                                                             
+
+def add_generic_system(apstra_session, generic_systems: dict) -> Tuple[Optional[str], Optional[str]]:
     """
-    Add the generic systems to the Apstra server from the given generic systems data.
+    Add a single generic system to the Apstra server from the given generic systems data.
+    Revised from add_generic_systems.
 
     Generic systems data:
     {
         <blueprint_label>: {
             <generic_system_label>: [
                 {
                     "blueprint": "blueprint1",
                     "system_label": "generic_system1",
                     "is_external": false,
                     "speed": "10G",
                     "lag_mode": null,
+                    "ct_names": null,
  
-                    "label1": "eth1",
-                    "ifname1": "eth1",
-                    "gs_ifname1": null,
-
-                    "label2": null,
-                    "ifname2": null,
-                    "gs_ifname2": null,
-
-                    "label3": null,
-                    "ifname3": null,
-                    "gs_ifname3": null,
-
-                    "label4": null,
-                    "ifname4": null,
-                    "gs_ifname4": null,
+                    "switch1": "server-leaf-1",
+                    "switch_intf1": "xe-0/0/0",
+                    "server_intf1": eth0,
+
+                    "switch2": null,
+                    "switch_intf2": null,
+                    "server_intf2": null,
+
+                    "switch3": null,
+                    "switch_intf3": null,
+                    "server_intf3": null,
+
+                    "switch4": null,
+                    "switch_intf4": null,
+                    "server_intf4": null,
 
-                    "ct_names": null,
                     "comment": null
                 }
             ]
         }
     }
     """
 
     ## create the generic systems
     bp_total = len(generic_systems)  # total number of blueprints
     bp_count = 0
-    logging.info(f"Adding generic systems to {bp_total} blueprints")
+    logging.info(f"add_generic_system Adding generic systems to {bp_total} blueprints")
     for bp_label, bp_data in generic_systems.items():
         bp_count += 1
-        logging.info(f"Adding generic systems to blueprint {bp_count}/{bp_total}: {bp_label}")
-        bp = CkApstraBlueprint(job_env.session, bp_label)
+        logging.info(f"add_generic_system Adding generic systems to blueprint {bp_count}/{bp_total}: {bp_label}")
+        bp = CkApstraBlueprint(apstra_session, bp_label)
         # logging.debug(f"{bp=}, {bp.id=}")
         gs_total = len(bp_data)
         gs_count = 0
-        logging.info(f"Adding {gs_total} generic systems to blueprint {bp_label}")
+        logging.info(f"add_generic_system Adding {gs_total} generic systems to blueprint {bp_label}")
         for gs_label, gs_links_list in bp_data.items():
             gs_count += 1
             gs_link_total = len(gs_links_list)
-            logging.info(f"Adding generic system {gs_count}/{gs_total}: {gs_label} with {gs_link_total} links")
-            if bp.get_system_node_from_label(gs_label):
-                logging.info(f"Skipping: Generic system {gs_label} already exists in blueprint {bp_label}")
-                continue
-            # if gs_link_total > 1:
-            #     logging.warning(f"Adding generic system {gs_label} with {gs_link_total} links\n{gs_links_list}")
-            #     return
-            generic_system_spec = {
-                'links': [],
-                'new_systems': [],
-            }
-            # to form logical device
-            speed_count = {}
-            system_type = 'server'
-
-            for link in gs_links_list:
-            #     logging.debug(f"{link=}")
-                link_speed = link['speed']
-                system_type = 'external' if link['is_external'] else 'server'
-                for link_number in range(4):
-                    link_id_num = link_number + 1
-                    label_label = f"label{link_id_num}"
-                    this_ifname = link[f"ifname{link_id_num}"]
-                    # skip if data is missing
-                    if not link[label_label]:
-                        continue
-                    if this_ifname[:2] not in ['et', 'xe', 'ge']:
-                        logging.warning(f"Skipping: Generic system {gs_label} has invalid interface name {this_ifname}")
-                        continue
-                    logging.debug(f"{label_label=}, {link[label_label]=}")
-                    switch_id = bp.get_system_node_from_label(link[label_label])['id']
-                    link_spec = {
-                        'switch': {
-                            'system_id': switch_id,
-                            'transformation_id': bp.get_transformation_id(link[f"label{link_id_num}"], this_ifname , link_speed),
-                            'if_name': link[f"ifname{link_id_num}"],
-                        },
-                        'system': {
-                            'system_id': None,
-                        },
-                        # 'lag_mode':link['lag_mode'],
-                        'lag_mode': None,
-                    }
-                    generic_system_spec['links'].append(link_spec)
-                    # speed_count[link_speed] = getattr(speed_count, link_speed, 0) + 1
-                    logging.debug(f"{link_speed=}, {speed_count=}")
-                    if link_speed not in speed_count:
-                        speed_count[link_speed] = 1
-                    else:
-                        speed_count[link_speed] += 1
-
-            new_system = {
-                'system_type': system_type,
-                'label': gs_label,
-                'port_channel_id_min': 0,
-                'port_channel_id_max': 0,
-                'logical_device': {
-                    'display_name': None,
-                    'id': None,
-                    'panels': [
-                        {
-                            'panel_layout': {
-                                'row_count': 1,
-                                'column_count': sum(speed_count.values()),
-                            },
-                            'port_indexing': {
-                                'order': 'T-B, L-R',
-                                'start_index': 1,
-                                'schema': 'absolute'
-                            },
-                            "port_groups": [
-                                # {
-                                #     "count": 4,
-                                #     "speed": {
-                                #         "unit": "G",
-                                #         "value": 10
-                                #     },
-                                #     "roles": [
-                                #         "leaf",
-                                #         "access"
-                                #     ]
-                                # }
-                            ]
-                        }
-                    ]
-                },
-            }
-            display_name = 'auto'
-            for speed, count in speed_count.items():
-                port_group = {
-                    'count': count,
-                    'speed': {
-                        'unit': speed[-1],
-                        'value': int(speed[:-1]),
-                    },
-                    'roles': ['leaf', 'access'],
-                }
-                new_system['logical_device']['panels'][0]['port_groups'].append(port_group)
-                display_name = f"{display_name}-{count}x{speed}"
-            new_system['logical_device']['display_name'] = display_name
-            new_system['logical_device']['id'] = display_name
-            generic_system_spec['new_systems'].append(new_system)
-            logging.debug(f"{generic_system_spec=}, {speed_count=}")
-
-            generic_system_created = bp.add_generic_system(generic_system_spec)
-            logging.info(f"Generic system {gs_label} created in blueprint {bp_label}")
+            logging.info(f"add_generic_system Adding generic system {gs_count}/{gs_total}: {gs_label} with {gs_link_total} links")
+            _, error = add_single_generic_system(bp, gs_label, gs_links_list)
+            if error:
+                logging.warning(f"add_generic_system Error for {gs_label=}:\n\tFrom add_single_generic_system: {error}")
+                # return None, f"add_generic_system {error}"
 
         ## form LACP in the BP iterating over the generic systems
         for gs_label, gs_links_list in bp_data.items():
-            form_lacp(job_env, gs_label, gs_links_list)
-            add_tags(job_env, gs_label, gs_links_list)
-            rename_generic_system_intf(job_env, gs_label, gs_links_list)
+            form_lacp(bp, gs_label, gs_links_list)
+            add_tags(bp, gs_label, gs_links_list)
+            rename_generic_system_intf(bp, gs_label, gs_links_list)
 
             # # update connectivity templates - this should be run after lag update
             # assign_connectivity_templates(job_env, gs_label, gs_links_list)
+            assign_connectivity_templates(bp, gs_label, gs_links_list)
 
+        return None, None    
 
-@click.command(name='add-generic-systems')
-def click_add_generic_systems():
-    job_env = CkJobEnv()
-    generic_systems = read_generic_systems(job_env.excel_input_file, 'generic_systems')
-    add_generic_systems(job_env, generic_systems)
 
 
-@click.command(name='assign-connectivity-templates')
-def click_assign_connecitivity_templates():
-    job_env = CkJobEnv()
-    generic_systems = read_generic_systems(job_env.excel_input_file, 'generic_systems')
-    bp_total = len(generic_systems)  # total number of blueprints
-    bp_count = 0
-    logging.info(f"Adding connecitivity templates to {bp_total} blueprints")
-    for bp_label, bp_data in generic_systems.items():
-        bp_count += 1
-        logging.info(f"Adding connecitivity templates to blueprint {bp_count}/{bp_total}: {bp_label}")
-        bp = CkApstraBlueprint(job_env.session, bp_label)
-        # logging.debug(f"{bp=}, {bp.id=}")
-        gs_total = len(bp_data)
-        gs_count = 0
-        logging.info(f"Adding {gs_total} generic systems to blueprint {bp_label}")
-        for gs_label, gs_links_list in bp_data.items():
-            form_lacp(job_env, gs_label, gs_links_list)
-            assign_connectivity_templates(job_env, gs_label, gs_links_list)
-
 if __name__ == "__main__":
-    click_add_generic_systems()
+    # click_add_generic_systems()
+    apstra_server_host = '10.85.192.45'
+    apstra_server_port = '443'
+    apstra_server_username = 'admin'
+    apstra_server_password = 'admin'
+
+    apstra = CkApstraSession(apstra_server_host, apstra_server_port, apstra_server_username, apstra_server_password)
+    apstra.print_token()
+    
+    generic_systems = {
+        'terra': {
+            'single-home-1': [
+                {
+                    "blueprint": "terra",
+                    "system_label": "single-home-1",
+                    "is_external": False,
+                    "speed": "10G",
+                    "lag_mode": None,
+                    "ct_names": "vn20",
+                    "gs_tags": "single",
+                    "server_intf1": "eth0",
+                    "switch1": "server_1",
+                    "switch_intf1": "xe-0/0/11",
+                    "server_intf2": None,
+                    "switch2": None,
+                    "switch_intf2": None,
+                    "server_intf3": None,
+                    "switch3": None,
+                    "switch_intf3": None,
+                    "server_intf4": None,
+                    "switch4": None,
+                    "switch_intf4": None,
+                    "comment": None
+                }
+            ],
+            'dual-home-1': [
+                {
+                    "blueprint": "terra",
+                    "system_label": "dual-home-1",
+                    "is_external": False,
+                    "speed": "10G",
+                    "lag_mode": "lacp_active",
+                    "ct_names": "vn20,vn101",
+                    "gs_tags": "dual",
+                    "server_intf1": "eth0",
+                    "switch1": "server_1",
+                    "switch_intf1": "xe-0/0/12",
+                    "server_intf2": "eth1",
+                    "switch2": "server_2",
+                    "switch_intf2": "xe-0/0/12",
+                    "server_intf3": None,
+                    "switch3": None,
+                    "switch_intf3": None,
+                    "server_intf4": None,
+                    "switch4": None,
+                    "switch_intf4": None,
+                    "comment": None
+                }
+            ]
+        }
+    }
+    add_generic_system(apstra, generic_systems)
```

### Comparing `ck_apstra_api-0.2.9/src/ck_apstra_api/ip_endpoint.py` & `ck_apstra_api-0.3.0/src/ck_apstra_api/ip_endpoint.py`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.2.9/src/ck_apstra_api/pull_device_configuration.py` & `ck_apstra_api-0.3.0/src/ck_apstra_api/pull_device_configuration.py`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.2.9/PKG-INFO` & `ck_apstra_api-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: ck-apstra-api
-Version: 0.2.9
+Version: 0.3.0
 Summary: An implementation to use Apstra API
 License: MIT
 Author: Charlie Kim
 Author-email: ckim@juniper.net
-Requires-Python: >=3.9,<3.13
+Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.1.1,<3.0.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

