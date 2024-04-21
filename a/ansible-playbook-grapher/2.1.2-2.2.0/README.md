# Comparing `tmp/ansible_playbook_grapher-2.1.2-py2.py3-none-any.whl.zip` & `tmp/ansible_playbook_grapher-2.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 49560 bytes, number of entries: 17
--rw-r--r--  2.0 unx     2827 b- defN 24-Feb-24 22:58 ansibleplaybookgrapher/__init__.py
--rw-r--r--  2.0 unx    11280 b- defN 23-May-13 12:42 ansibleplaybookgrapher/cli.py
--rw-r--r--  2.0 unx    13757 b- defN 23-May-13 16:23 ansibleplaybookgrapher/graph_model.py
--rw-r--r--  2.0 unx    19929 b- defN 24-Feb-24 22:41 ansibleplaybookgrapher/parser.py
--rw-r--r--  2.0 unx     7014 b- defN 23-May-11 14:42 ansibleplaybookgrapher/utils.py
+Zip file size: 51198 bytes, number of entries: 18
+-rw-r--r--  2.0 unx       60 b- defN 24-Apr-21 18:32 ansibleplaybookgrapher/__init__.py
+-rw-r--r--  2.0 unx    12252 b- defN 24-Mar-25 22:27 ansibleplaybookgrapher/cli.py
+-rw-r--r--  2.0 unx    15624 b- defN 24-Mar-25 22:27 ansibleplaybookgrapher/graph_model.py
+-rw-r--r--  2.0 unx     2679 b- defN 24-Mar-23 05:55 ansibleplaybookgrapher/grapher.py
+-rw-r--r--  2.0 unx    20440 b- defN 24-Apr-21 17:53 ansibleplaybookgrapher/parser.py
+-rw-r--r--  2.0 unx     7031 b- defN 24-Mar-25 22:27 ansibleplaybookgrapher/utils.py
 -rw-r--r--  2.0 unx      358 b- defN 23-May-11 14:42 ansibleplaybookgrapher/data/graph.css
 -rw-r--r--  2.0 unx     5458 b- defN 23-May-11 14:42 ansibleplaybookgrapher/data/highlight-hover.js
--rw-r--r--  2.0 unx     8189 b- defN 23-May-13 12:42 ansibleplaybookgrapher/renderer/__init__.py
--rw-r--r--  2.0 unx    11304 b- defN 23-May-28 10:34 ansibleplaybookgrapher/renderer/mermaid.py
--rw-r--r--  2.0 unx    11050 b- defN 23-May-28 10:34 ansibleplaybookgrapher/renderer/graphviz/__init__.py
+-rw-r--r--  2.0 unx     8709 b- defN 24-Mar-25 22:27 ansibleplaybookgrapher/renderer/__init__.py
+-rw-r--r--  2.0 unx    13229 b- defN 24-Apr-18 20:30 ansibleplaybookgrapher/renderer/mermaid.py
+-rw-r--r--  2.0 unx    12104 b- defN 24-Mar-25 22:27 ansibleplaybookgrapher/renderer/graphviz/__init__.py
 -rw-r--r--  2.0 unx     7367 b- defN 23-May-13 12:42 ansibleplaybookgrapher/renderer/graphviz/postprocessor.py
--rw-r--r--  2.0 unx    35148 b- defN 24-Feb-24 23:00 ansible_playbook_grapher-2.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    22870 b- defN 24-Feb-24 23:00 ansible_playbook_grapher-2.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Feb-24 23:00 ansible_playbook_grapher-2.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       77 b- defN 24-Feb-24 23:00 ansible_playbook_grapher-2.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 24-Feb-24 23:00 ansible_playbook_grapher-2.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1657 b- defN 24-Feb-24 23:00 ansible_playbook_grapher-2.1.2.dist-info/RECORD
-17 files, 158418 bytes uncompressed, 46764 bytes compressed:  70.5%
+-rw-r--r--  2.0 unx    35148 b- defN 24-Apr-21 18:36 ansible_playbook_grapher-2.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    23247 b- defN 24-Apr-21 18:36 ansible_playbook_grapher-2.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-21 18:36 ansible_playbook_grapher-2.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       77 b- defN 24-Apr-21 18:36 ansible_playbook_grapher-2.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 24-Apr-21 18:36 ansible_playbook_grapher-2.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1745 b- defN 24-Apr-21 18:36 ansible_playbook_grapher-2.2.0.dist-info/RECORD
+18 files, 165661 bytes uncompressed, 48260 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: ansibleplaybookgrapher/cli.py
 Comment: 
 
 Filename: ansibleplaybookgrapher/graph_model.py
 Comment: 
 
+Filename: ansibleplaybookgrapher/grapher.py
+Comment: 
+
 Filename: ansibleplaybookgrapher/parser.py
 Comment: 
 
 Filename: ansibleplaybookgrapher/utils.py
 Comment: 
 
 Filename: ansibleplaybookgrapher/data/graph.css
@@ -27,26 +30,26 @@
 
 Filename: ansibleplaybookgrapher/renderer/graphviz/__init__.py
 Comment: 
 
 Filename: ansibleplaybookgrapher/renderer/graphviz/postprocessor.py
 Comment: 
 
-Filename: ansible_playbook_grapher-2.1.2.dist-info/LICENSE
+Filename: ansible_playbook_grapher-2.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: ansible_playbook_grapher-2.1.2.dist-info/METADATA
+Filename: ansible_playbook_grapher-2.2.0.dist-info/METADATA
 Comment: 
 
-Filename: ansible_playbook_grapher-2.1.2.dist-info/WHEEL
+Filename: ansible_playbook_grapher-2.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: ansible_playbook_grapher-2.1.2.dist-info/entry_points.txt
+Filename: ansible_playbook_grapher-2.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: ansible_playbook_grapher-2.1.2.dist-info/top_level.txt
+Filename: ansible_playbook_grapher-2.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ansible_playbook_grapher-2.1.2.dist-info/RECORD
+Filename: ansible_playbook_grapher-2.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ansibleplaybookgrapher/__init__.py

```diff
@@ -1,76 +1,2 @@
-# Copyright (C) 2023 Mohamed El Mouctar HAIDARA
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-from typing import Dict, List, Set, Tuple
-
-from ansible.utils.display import Display
-
-from ansibleplaybookgrapher.graph_model import (
-    PlaybookNode,
-    RoleNode,
-    PlayNode,
-)
-from ansibleplaybookgrapher.parser import PlaybookParser
-from ansibleplaybookgrapher.utils import merge_dicts
-from .graph_model import PlaybookNode, PlayNode, TaskNode, RoleNode, BlockNode
-from .parser import PlaybookParser
-
-__version__ = "2.1.2"
+__version__ = "2.2.0"
 __prog__ = "ansible-playbook-grapher"
-
-display = Display()
-
-
-class Grapher:
-    def __init__(self, playbook_filenames: List[str]):
-        """
-        :param playbook_filenames: List of playbooks to graph
-        """
-        self.playbook_filenames = playbook_filenames
-
-    def parse(
-        self,
-        include_role_tasks: bool = False,
-        tags: List[str] = None,
-        skip_tags: List[str] = None,
-        group_roles_by_name: bool = False,
-    ) -> Tuple[List[PlaybookNode], Dict[RoleNode, Set[PlayNode]]]:
-        """
-        Parses all the provided playbooks
-        :param include_role_tasks: Should we include the role tasks
-        :param tags: Only add plays and tasks tagged with these values
-        :param skip_tags: Only add plays and tasks whose tags do not match these values
-        :param group_roles_by_name: Group roles by name instead of considering them as separate nodes with different IDs
-        :return:
-        """
-        playbook_nodes = []
-        roles_usage: Dict[RoleNode, Set[PlayNode]] = {}
-
-        for playbook_file in self.playbook_filenames:
-            display.display(f"Parsing playbook {playbook_file}")
-            playbook_parser = PlaybookParser(
-                playbook_filename=playbook_file,
-                tags=tags,
-                skip_tags=skip_tags,
-                include_role_tasks=include_role_tasks,
-                group_roles_by_name=group_roles_by_name,
-            )
-            playbook_node = playbook_parser.parse()
-            playbook_nodes.append(playbook_node)
-
-            # Update the usage of the roles
-            roles_usage = merge_dicts(roles_usage, playbook_node.roles_usage())
-
-        return playbook_nodes, roles_usage
```

## ansibleplaybookgrapher/cli.py

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Mohamed El Mouctar HAIDARA
+# Copyright (C) 2024 Mohamed El Mouctar HAIDARA
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -19,15 +19,16 @@
 
 from ansible.cli import CLI
 from ansible.cli.arguments import option_helpers
 from ansible.errors import AnsibleOptionsError
 from ansible.release import __version__ as ansible_version
 from ansible.utils.display import Display
 
-from ansibleplaybookgrapher import __prog__, __version__, Grapher
+from ansibleplaybookgrapher.grapher import Grapher
+from ansibleplaybookgrapher import __prog__, __version__
 from ansibleplaybookgrapher.renderer import OPEN_PROTOCOL_HANDLERS
 from ansibleplaybookgrapher.renderer.graphviz import GraphvizRenderer
 from ansibleplaybookgrapher.renderer.mermaid import (
     MermaidFlowChartRenderer,
     DEFAULT_DIRECTIVE as MERMAID_DEFAULT_DIRECTIVE,
     DEFAULT_ORIENTATION as MERMAID_DEFAULT_ORIENTATION,
 )
@@ -71,14 +72,16 @@
             )
             output_path = renderer.render(
                 open_protocol_handler=self.options.open_protocol_handler,
                 open_protocol_custom_formats=self.options.open_protocol_custom_formats,
                 output_filename=self.options.output_filename,
                 view=self.options.view,
                 save_dot_file=self.options.save_dot_file,
+                hide_empty_plays=self.options.hide_empty_plays,
+                hide_plays_without_roles=self.options.hide_plays_without_roles,
             )
 
             return output_path
         else:
             renderer = MermaidFlowChartRenderer(
                 playbook_nodes=playbook_nodes,
                 roles_usage=roles_usage,
@@ -86,14 +89,16 @@
             output_path = renderer.render(
                 open_protocol_handler=self.options.open_protocol_handler,
                 open_protocol_custom_formats=self.options.open_protocol_custom_formats,
                 output_filename=self.options.output_filename,
                 view=self.options.view,
                 directive=self.options.renderer_mermaid_directive,
                 orientation=self.options.renderer_mermaid_orientation,
+                hide_empty_plays=self.options.hide_empty_plays,
+                hide_plays_without_roles=self.options.hide_plays_without_roles,
             )
             return output_path
 
     def _add_my_options(self):
         """
         Add some of my options to the parser
         :return:
@@ -109,15 +114,15 @@
         )
 
         self.parser.add_argument(
             "--include-role-tasks",
             dest="include_role_tasks",
             action="store_true",
             default=False,
-            help="Include the tasks of the role in the graph.",
+            help="Include the tasks of the roles in the graph. Applied when parsing the playbooks.",
         )
 
         self.parser.add_argument(
             "-s",
             "--save-dot-file",
             dest="save_dot_file",
             action="store_true",
@@ -201,14 +206,29 @@
         self.parser.add_argument(
             "--version",
             action="version",
             version=f"{__prog__} {__version__} (with ansible {ansible_version})",
         )
 
         self.parser.add_argument(
+            "--hide-plays-without-roles",
+            action="store_true",
+            default=False,
+            help="Hide the plays that end up with no roles in the graph (after applying the tags filter). "
+            "Only roles at the play level and include_role as tasks are considered (no import_role).",
+        )
+
+        self.parser.add_argument(
+            "--hide-empty-plays",
+            action="store_true",
+            default=False,
+            help="Hide the plays that end up with no tasks in the graph (after applying the tags filter).",
+        )
+
+        self.parser.add_argument(
             "playbook_filenames",
             help="Playbook(s) to graph",
             metavar="playbooks",
             nargs="+",
         )
 
         # Use ansible helper to add some default options also
```

## ansibleplaybookgrapher/graph_model.py

```diff
@@ -10,15 +10,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 import os
 from collections import defaultdict
-from typing import Dict, List, Set, Type, Tuple, Optional
+from typing import Dict, List, Set, Tuple, Optional
 
 from ansibleplaybookgrapher.utils import generate_id, get_play_colors
 
 
 class LoopMixin:
     """
     A mixin class for nodes that support looping
@@ -75,15 +75,15 @@
         """
         Set the path of this based on the raw object. Not all objects have path
         :return:
         """
         if self.raw_object and self.raw_object.get_ds():
             self.path, self.line, self.column = self.raw_object.get_ds().ansible_pos
 
-    def get_first_parent_matching_type(self, node_type: Type) -> Type:
+    def get_first_parent_matching_type(self, node_type: type) -> type:
         """
         Get the first parent of this node matching the given type
         :param node_type: The type of the parent to get
         :return:
         """
         current_parent = self.parent
 
@@ -160,14 +160,27 @@
                 f"The target composition '{target_composition}' is unknown. Supported are: {self._supported_compositions}"
             )
         self._compositions[target_composition].append(node)
         # The node index is position in the composition regardless of the type of the node
         node.index = self._node_counter + 1
         self._node_counter += 1
 
+    def get_nodes(self, target_composition: str) -> List:
+        """
+        Get a node from the compositions
+        :param target_composition:
+        :return: A list of the nodes
+        """
+        if target_composition not in self._supported_compositions:
+            raise Exception(
+                f"The target composition '{target_composition}' is unknown. Supported are: {self._supported_compositions}"
+            )
+
+        return self._compositions[target_composition]
+
     def get_all_tasks(self) -> List["TaskNode"]:
         """
         Return all the TaskNode inside this composite node
         :return:
         """
         tasks: List[TaskNode] = []
         self._get_all_tasks_nodes(tasks)
@@ -204,14 +217,41 @@
         """
         for _, nodes in self._compositions.items():
             for node in nodes:
                 if isinstance(node, CompositeNode):
                     node._get_all_links(links)
                 links[self].append(node)
 
+    def is_empty(self) -> bool:
+        """
+        Returns true if the composite node is empty, false otherwise
+        :return:
+        """
+        for _, nodes in self._compositions.items():
+            if len(nodes) > 0:
+                return False
+
+        return True
+
+    def has_node_type(self, node_type: type) -> bool:
+        """
+        Returns true if the composite node has at least one node of the given type, false otherwise
+        :param node_type: The type of the node
+        :return:
+        """
+        for _, nodes in self._compositions.items():
+            for node in nodes:
+                if isinstance(node, node_type):
+                    return True
+
+                if isinstance(node, CompositeNode):
+                    return node.has_node_type(node_type)
+
+        return False
+
 
 class CompositeTasksNode(CompositeNode):
     """
     A special composite node which only support adding "tasks". Useful for block and role
     """
 
     def __init__(
@@ -244,15 +284,15 @@
 
     @property
     def tasks(self) -> List[Node]:
         """
         The tasks attached to this block
         :return:
         """
-        return self._compositions["tasks"]
+        return self.get_nodes("tasks")
 
 
 class PlaybookNode(CompositeNode):
     """
     A playbook is a list of play
     """
 
@@ -279,21 +319,32 @@
         :return:
         """
         # Since the playbook is the whole file, the set the position as the beginning of the file
         self.path = os.path.join(os.getcwd(), self.name)
         self.line = 1
         self.column = 1
 
-    @property
-    def plays(self) -> List["PlayNode"]:
+    def plays(
+        self, exclude_empty: bool = False, exclude_without_roles: bool = False
+    ) -> List["PlayNode"]:
         """
         Return the list of plays
+        :param exclude_empty: Whether to exclude the empty plays from the result or not
+        :param exclude_without_roles: Whether to exclude the plays that do not have roles
         :return:
         """
-        return self._compositions["plays"]
+        plays = self.get_nodes("plays")
+
+        if exclude_empty:
+            plays = [play for play in plays if not play.is_empty()]
+
+        if exclude_without_roles:
+            plays = [play for play in plays if play.has_node_type(RoleNode)]
+
+        return plays
 
     def roles_usage(self) -> Dict["RoleNode", Set["PlayNode"]]:
         """
         For each role in the playbook, get the uniq plays that reference the role
         :return: A dict with key as role node and value the list of uniq plays that use it
         """
 
@@ -347,27 +398,31 @@
             supported_compositions=["pre_tasks", "roles", "tasks", "post_tasks"],
         )
         self.hosts = hosts or []
         self.colors: Tuple[str, str] = get_play_colors(self.id)
 
     @property
     def roles(self) -> List["RoleNode"]:
-        return self._compositions["roles"]
+        """
+        Return the roles of the plays. Tasks using "include_role" are NOT returned.
+        :return:
+        """
+        return self.get_nodes("roles")
 
     @property
     def pre_tasks(self) -> List["Node"]:
-        return self._compositions["pre_tasks"]
+        return self.get_nodes("pre_tasks")
 
     @property
     def post_tasks(self) -> List["Node"]:
-        return self._compositions["post_tasks"]
+        return self.get_nodes("post_tasks")
 
     @property
     def tasks(self) -> List["Node"]:
-        return self._compositions["tasks"]
+        return self.get_nodes("tasks")
 
 
 class BlockNode(CompositeTasksNode):
     """
     A block node: https://docs.ansible.com/ansible/latest/user_guide/playbooks_blocks.html
     """
```

## ansibleplaybookgrapher/parser.py

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Mohamed El Mouctar HAIDARA
+# Copyright (C) 2024 Mohamed El Mouctar HAIDARA
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -163,15 +163,15 @@
             add roles
                 if  include_role_tasks
                     add role_tasks
             add tasks
             add post_tasks
         :return:
         """
-
+        display.display(f"Parsing playbook {self.playbook_filename}")
         playbook = Playbook.load(
             self.playbook_filename,
             loader=self.data_loader,
             variable_manager=self.variable_manager,
         )
         # the root node
         playbook_root_node = PlaybookNode(self.playbook_filename, raw_object=playbook)
@@ -349,14 +349,24 @@
 
                 if isinstance(task_or_block, IncludeRole):
                     # Here we have an 'include_role'. The class IncludeRole is a subclass of TaskInclude.
                     # We do this because the management of an 'include_role' is different.
                     # See :func:`~ansible.playbook.included_file.IncludedFile.process_include_results` from line 155
                     display.v(f"An 'include_role' found: '{task_or_block.get_name()}'")
 
+                    if not task_or_block.evaluate_tags(
+                        only_tags=self.tags,
+                        skip_tags=self.skip_tags,
+                        all_vars=task_vars,
+                    ):
+                        display.vv(
+                            f"The include_role '{task_or_block.get_name()}' is skipped due to the tags."
+                        )
+                        continue  # Go to the next task
+
                     # Here we are using the role name instead of the task name to keep the same behavior  as a
                     #  traditional role
                     if self.group_roles_by_name:
                         # If we are grouping roles, we use the hash of role name as the node id
                         role_node_id = "role_" + hash_value(task_or_block._role_name)
                     else:
                         # Otherwise, a random id is used
```

## ansibleplaybookgrapher/utils.py

```diff
@@ -17,15 +17,15 @@
 import uuid
 from collections import defaultdict
 from itertools import chain
 from operator import methodcaller
 from typing import Tuple, List, Dict, Any, Set
 
 from ansible.errors import AnsibleError
-from ansible.module_utils._text import to_text
+from ansible.module_utils.common.text.converters import to_text
 from ansible.parsing.dataloader import DataLoader
 from ansible.playbook.role_include import IncludeRole
 from ansible.playbook.task import Task
 from ansible.playbook.task_include import TaskInclude
 from ansible.template import Templar
 from ansible.utils.display import Display
 from colour import Color
```

## ansibleplaybookgrapher/renderer/__init__.py

```diff
@@ -9,15 +9,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from abc import ABC, abstractmethod
-from typing import Dict, Optional, Set
+from typing import Dict, Optional, Set, List
 
 from ansible.utils.display import Display
 
 from ansibleplaybookgrapher.graph_model import (
     PlaybookNode,
     PlayNode,
     RoleNode,
@@ -40,44 +40,48 @@
     "custom": {},
 }
 
 
 class Renderer(ABC):
     def __init__(
         self,
-        playbook_nodes: PlaybookNode,
+        playbook_nodes: List[PlaybookNode],
         roles_usage: Dict[RoleNode, Set[PlayNode]],
     ):
         self.playbook_nodes = playbook_nodes
         self.roles_usage = roles_usage
 
     @abstractmethod
     def render(
         self,
         open_protocol_handler: str,
         open_protocol_custom_formats: Dict[str, str],
         output_filename: str,
         view: bool,
+        hide_empty_plays: bool = False,
+        hide_plays_without_roles: bool = False,
         **kwargs,
     ) -> str:
         """
         Render the playbooks to a file.
         :param open_protocol_handler: The protocol handler name to use
         :param open_protocol_custom_formats: The custom formats to use when the protocol handler is set to custom
-        :param output_filename: without any extension
+        :param output_filename: The output filename without any extension
         :param view: Whether to open the rendered file in the default viewer
+        :param hide_empty_plays: Whether to hide empty plays or not when rendering the graph
+        :param hide_plays_without_roles: Whether to hide plays without any roles or not
         :param kwargs:
-        :return: The filename of the rendered file
+        :return: The path of the rendered file
         """
         pass
 
 
 class PlaybookBuilder(ABC):
     """
-    This the base class to inherit from by the renderer to build a single Playbook in the target format.
+    This is the base class to inherit from by the renderer to build a single Playbook in the target format.
     It provides some methods that need to be implemented
     """
 
     def __init__(
         self,
         playbook_node: PlaybookNode,
         open_protocol_handler: str,
@@ -124,17 +128,24 @@
                 color=color,
                 fontcolor=fontcolor,
                 node_label_prefix=kwargs.pop("node_label_prefix", ""),
                 **kwargs,
             )
 
     @abstractmethod
-    def build_playbook(self, **kwargs) -> str:
+    def build_playbook(
+        self,
+        hide_empty_plays: bool = False,
+        hide_plays_without_roles: bool = False,
+        **kwargs,
+    ) -> str:
         """
         Build the whole playbook
+        :param hide_empty_plays: Whether to hide empty plays or not
+        :param hide_plays_without_roles:
         :param kwargs:
         :return: The rendered playbook as a string
         """
         pass
 
     @abstractmethod
     def build_play(self, play_node: PlayNode, **kwargs):
```

## ansibleplaybookgrapher/renderer/mermaid.py

```diff
@@ -8,67 +8,81 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
 from pathlib import Path
+import json
+import zlib
+from base64 import urlsafe_b64encode
+import webbrowser
 from typing import Dict, Set, List
 
 from ansible.utils.display import Display
 
-from ansibleplaybookgrapher import BlockNode, RoleNode, TaskNode, PlayNode, PlaybookNode
+from ansibleplaybookgrapher.graph_model import (
+    BlockNode,
+    RoleNode,
+    TaskNode,
+    PlayNode,
+    PlaybookNode,
+)
 from ansibleplaybookgrapher.renderer import PlaybookBuilder, Renderer
 
 display = Display()
 
 # Default directive when rendering the graph.
-# More info at
-#   https://mermaid.js.org/config/directives.html
-#
+# More info at https://mermaid.js.org/config/directives.html
 DEFAULT_DIRECTIVE = '%%{ init: { "flowchart": { "curve": "bumpX" } } }%%'
 DEFAULT_ORIENTATION = "LR"  # Left to right
 
 
 class MermaidFlowChartRenderer(Renderer):
     def __init__(
         self,
         playbook_nodes: List[PlaybookNode],
         roles_usage: Dict["RoleNode", Set[PlayNode]],
     ):
-        self.playbook_nodes = playbook_nodes
-        self.roles_usage = roles_usage
+        super().__init__(playbook_nodes, roles_usage)
 
     def render(
         self,
         open_protocol_handler: str,
         open_protocol_custom_formats: Dict[str, str],
         output_filename: str,
         view: bool,
+        hide_empty_plays: bool = False,
+        hide_plays_without_roles: bool = False,
+        directive: str = DEFAULT_DIRECTIVE,
+        orientation: str = DEFAULT_ORIENTATION,
         **kwargs,
     ) -> str:
         """
 
-        :param open_protocol_handler:
-        :param open_protocol_custom_formats:
-        :param output_filename: without any extension
-        :param view:
+        :param open_protocol_handler: Not supported for the moment
+        :param open_protocol_custom_formats: Not supported for the moment
+        :param output_filename: The output filename without any extension
+        :param view: Not supported for the moment
+        :param hide_empty_plays: Whether to hide empty plays or not when rendering the graph
+        :param hide_plays_without_roles: Whether to hide plays without any roles or not
+        :param directive: Mermaid directive
+        :param orientation: Mermaid graph orientation
         :param kwargs:
         :return:
         """
         # TODO: Add support for protocol handler
         # TODO: Add support for hover
+
         mermaid_code = "---\n"
         mermaid_code += "title: Ansible Playbook Grapher\n"
         mermaid_code += "---\n"
 
-        directive = kwargs.get("directive", DEFAULT_DIRECTIVE)
-        orientation = kwargs.get("orientation", DEFAULT_ORIENTATION)
-
         display.vvv(f"Using '{directive}' as directive for the mermaid chart")
         mermaid_code += f"{directive}\n"
 
         mermaid_code += f"flowchart {orientation}\n"
 
         # Mermaid only supports adding style to links by using the order of the link when it is created
         # https://mermaid.js.org/syntax/flowchart.html#styling-links
@@ -82,35 +96,63 @@
                 open_protocol_handler=open_protocol_handler,
                 open_protocol_custom_formats=open_protocol_custom_formats,
                 roles_usage=self.roles_usage,
                 roles_built=roles_built,
                 link_order=link_order,
             )
 
-            mermaid_code += playbook_builder.build_playbook()
+            mermaid_code += playbook_builder.build_playbook(
+                hide_empty_plays=hide_empty_plays,
+                hide_plays_without_roles=hide_plays_without_roles,
+            )
             link_order = playbook_builder.link_order
             roles_built.update(playbook_builder.roles_built)
 
         final_output_path_file = Path(f"{output_filename}.mmd")
         # Make the sure the parents directories exist
         final_output_path_file.parent.mkdir(exist_ok=True, parents=True)
         final_output_path_file.write_text(mermaid_code)
 
         display.display(
             f"Mermaid code written to {final_output_path_file}", color="green"
         )
 
         if view:
-            # TODO: implement the view option
-            #  https://github.com/mermaidjs/mermaid-live-editor/issues/41 and https://mermaid.ink/
-            display.warning(
-                "The --view option is not supported yet by the mermaid renderer"
-            )
+            MermaidFlowChartRenderer.view(mermaid_code)
+
+        return str(final_output_path_file)
+
+    @staticmethod
+    def view(mermaid_code: str):
+        """
+        View the mermaid code in the browser using https://mermaid.live/
 
-        return final_output_path_file
+        This is based on:
+          - https://github.com/mermaid-js/mermaid-live-editor/blob/b5978e6faf7635e39452855fb4d062d1452ab71b/src/lib/util/serde.ts#L19-L29
+          - https://github.com/mermaidjs/mermaid-live-editor/issues/41#issuecomment-1820242778
+
+        :param mermaid_code:
+        :return:
+        """
+        graph_state = {
+            "code": mermaid_code,
+            "mermaid": {"theme": "default"},
+            "autoSync": True,
+            "updateDiagram": True,
+        }
+
+        compressed = zlib.compress(json.dumps(graph_state).encode("utf-8"), level=9)
+
+        url_path = f'pako:{urlsafe_b64encode(compressed).decode("utf-8")}'
+        url = f"https://mermaid.live/edit#{url_path}"
+
+        display.display(f"Mermaid live editor URL: {url}")
+
+        # Display url using the default browser in a new tag
+        webbrowser.open(url, new=2)
 
 
 class MermaidFlowChartPlaybookBuilder(PlaybookBuilder):
     def __init__(
         self,
         playbook_node: PlaybookNode,
         open_protocol_handler: str,
@@ -122,38 +164,50 @@
         super().__init__(
             playbook_node,
             open_protocol_handler,
             open_protocol_custom_formats,
             roles_usage,
             roles_built,
         )
+
         self.mermaid_code = ""
         # Used as an identifier for the links
         self.link_order = link_order
         # The current depth level of the nodes. Used for indentation
-        self._identation_level = 1
+        self._indentation_level = 1
 
-    def build_playbook(self, **kwargs) -> str:
+    def build_playbook(
+        self,
+        hide_empty_plays: bool = False,
+        hide_plays_without_roles=False,
+        **kwargs: bool,
+    ) -> str:
         """
         Build the playbook
+        :param hide_plays_without_roles: Whether to hide plays without any roles or not
+        :param hide_empty_plays: Whether to hide empty plays or not
+        :param hide_plays_without_roles: Whether to hide plays without any roles or not
         :param kwargs:
         :return:
         """
         display.vvv(
             f"Converting the playbook '{self.playbook_node.name}' to mermaid format"
         )
 
         # Playbook node
         self.add_comment(f"Start of the playbook '{self.playbook_node.name}'")
         self.add_text(f'{self.playbook_node.id}("{self.playbook_node.name}")')
 
-        self._identation_level += 1
-        for play_node in self.playbook_node.plays:
+        self._indentation_level += 1
+        for play_node in self.playbook_node.plays(
+            exclude_empty=hide_empty_plays,
+            exclude_without_roles=hide_plays_without_roles,
+        ):
             self.build_play(play_node)
-        self._identation_level -= 1
+        self._indentation_level -= 1
 
         self.add_comment(f"End of the playbook '{self.playbook_node.name}'\n")
 
         return self.mermaid_code
 
     def build_play(self, play_node: PlayNode, **kwargs):
         """
@@ -174,17 +228,17 @@
             source_id=play_node.parent.id,
             text=f"{play_node.index}",
             dest_id=play_node.id,
             style=f"stroke:{color},color:{color}",
         )
 
         # traverse the play
-        self._identation_level += 1
+        self._indentation_level += 1
         self.traverse_play(play_node)
-        self._identation_level -= 1
+        self._indentation_level -= 1
 
         self.add_comment(f"End of the play '{play_node.name}'")
 
     def build_task(self, task_node: TaskNode, color: str, fontcolor: str, **kwargs):
         """
 
         :param task_node:
@@ -241,22 +295,22 @@
         # Role node
         self.add_text(f'{role_node.id}("[role] {role_node.name}")')
         self.add_text(
             f"style {role_node.id} fill:{node_color},color:{fontcolor},stroke:{node_color}"
         )
 
         # Role tasks
-        self._identation_level += 1
+        self._indentation_level += 1
         for role_task in role_node.tasks:
             self.build_node(
                 node=role_task,
                 color=node_color,
                 fontcolor=fontcolor,
             )
-        self._identation_level -= 1
+        self._indentation_level -= 1
 
         self.add_comment(f"End of the role '{role_node.name}'")
 
     def build_block(self, block_node: BlockNode, color: str, fontcolor: str, **kwargs):
         """
 
         :param block_node:
@@ -279,22 +333,22 @@
             text=f"{block_node.index} {block_node.when}",
             dest_id=block_node.id,
             style=f"stroke:{color},color:{color}",
         )
 
         self.add_text(f'subgraph subgraph_{block_node.id}["{block_node.name} "]')
 
-        self._identation_level += 1
+        self._indentation_level += 1
         for task in block_node.tasks:
             self.build_node(
                 node=task,
                 color=color,
                 fontcolor=fontcolor,
             )
-        self._identation_level -= 1
+        self._indentation_level -= 1
 
         self.add_text("end")  # End of the subgraph
         self.add_comment(f"End of the block '{block_node.name}'")
 
     def add_link(
         self,
         source_id: str,
@@ -339,8 +393,8 @@
 
     @property
     def indentation(self) -> str:
         """
         Return the current indentation level as tabulations
         :return:
         """
-        return "\t" * self._identation_level
+        return "\t" * self._indentation_level
```

## ansibleplaybookgrapher/renderer/graphviz/__init__.py

```diff
@@ -41,27 +41,34 @@
 
 class GraphvizRenderer(Renderer):
     def __init__(
         self,
         playbook_nodes: List[PlaybookNode],
         roles_usage: Dict["RoleNode", Set[PlayNode]],
     ):
-        self.playbook_nodes = playbook_nodes
-        self.roles_usage = roles_usage
+        super().__init__(playbook_nodes, roles_usage)
 
     def render(
         self,
         open_protocol_handler: str,
         open_protocol_custom_formats: Dict[str, str],
         output_filename: str,
         view: bool,
+        hide_empty_plays: bool = False,
+        hide_plays_without_roles=False,
         **kwargs,
     ) -> str:
         """
-        :return: The filename where the playbooks where rendered
+        :param open_protocol_handler: The protocol handler name to use
+        :param open_protocol_custom_formats: The custom formats to use when the protocol handler is set to custom
+        :param output_filename: The output filename without any extension
+        :param view: Whether to open the rendered file in the default viewer
+        :param hide_empty_plays: Whether to hide empty plays or not when rendering the graph
+        :param hide_plays_without_roles: Whether to hide plays without any roles or not
+        :return: The path of the rendered file
         """
         save_dot_file = kwargs.get("save_dot_file", False)
 
         # Set of the roles that have been built so far for all the playbooks
         roles_built = set()
         digraph = Digraph(
             format="svg",
@@ -73,15 +80,18 @@
                 playbook_node,
                 open_protocol_handler=open_protocol_handler,
                 open_protocol_custom_formats=open_protocol_custom_formats,
                 roles_usage=self.roles_usage,
                 roles_built=roles_built,
                 digraph=digraph,
             )
-            builder.build_playbook()
+            builder.build_playbook(
+                hide_empty_plays=hide_empty_plays,
+                hide_plays_without_roles=hide_plays_without_roles,
+            )
             roles_built.update(builder.roles_built)
 
         display.display("Rendering the graph...")
         svg_path = digraph.render(
             cleanup=not save_dot_file,
             format="svg",
             filename=output_filename,
@@ -271,30 +281,37 @@
                 self.build_node(
                     node=role_task,
                     color=role_color,
                     fontcolor=fontcolor,
                     digraph=role_subgraph,
                 )
 
-    def build_playbook(self, **kwargs) -> str:
+    def build_playbook(
+        self, hide_empty_plays: bool = False, hide_plays_without_roles=False, **kwargs
+    ) -> str:
         """
         Convert the PlaybookNode to the graphviz dot format
+        :param hide_empty_plays: Whether to hide empty plays or not when rendering the graph
+        :param hide_plays_without_roles: Whether to hide plays without any roles or not
         :return: The text representation of the graphviz dot format for the playbook
         """
         display.vvv(f"Converting the graph to the dot format for graphviz")
         # root node
         self.digraph.node(
             self.playbook_node.id,
             label=self.playbook_node.name,
             style="dotted",
             id=self.playbook_node.id,
             URL=self.get_node_url(self.playbook_node, "file"),
         )
 
-        for play in self.playbook_node.plays:
+        for play in self.playbook_node.plays(
+            exclude_empty=hide_empty_plays,
+            exclude_without_roles=hide_plays_without_roles,
+        ):
             with self.digraph.subgraph(name=play.name) as play_subgraph:
                 self.build_play(play, digraph=play_subgraph, **kwargs)
 
         return self.digraph.source
 
     def build_play(self, play_node: PlayNode, **kwargs):
         """
```

## Comparing `ansible_playbook_grapher-2.1.2.dist-info/LICENSE` & `ansible_playbook_grapher-2.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ansible_playbook_grapher-2.1.2.dist-info/METADATA` & `ansible_playbook_grapher-2.2.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: ansible-playbook-grapher
-Version: 2.1.2
+Version: 2.2.0
 Summary: A command line tool to create a graph representing your Ansible playbook tasks and roles
 Home-page: https://github.com/haidaraM/ansible-playbook-grapher
-Download-URL: https://github.com/haidaraM/ansible-playbook-grapher/archive/v2.1.2.tar.gz
+Download-URL: https://github.com/haidaraM/ansible-playbook-grapher/archive/v2.2.0.tar.gz
 Author: HAIDARA Mohamed El Mouctar
 Author-email: elmhaidara@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ansible-core (<2.16.4,>=2.15)
-Requires-Dist: graphviz (<1,>=0.18)
-Requires-Dist: colour (<1)
-Requires-Dist: lxml (<6)
-Requires-Dist: svg.path (<7)
+Requires-Dist: ansible-core <2.16.5,>=2.15
+Requires-Dist: graphviz <1,>=0.18
+Requires-Dist: colour <1
+Requires-Dist: lxml <6
+Requires-Dist: svg.path <7
 
 # Ansible Playbook Grapher
 
 ![Testing](https://github.com/haidaraM/ansible-playbook-grapher/workflows/Testing/badge.svg)
 [![PyPI version](https://badge.fury.io/py/ansible-playbook-grapher.svg)](https://badge.fury.io/py/ansible-playbook-grapher)
 [![Coverage Status](https://coveralls.io/repos/github/haidaraM/ansible-playbook-grapher/badge.svg?branch=main)](https://coveralls.io/github/haidaraM/ansible-playbook-grapher?branch=main)
 
@@ -47,15 +47,15 @@
   file.  
   Optionally, you can
   set [the open protocol to use VSCode](https://code.visualstudio.com/docs/editor/command-line#_opening-vs-code-with-urls)
   with `--open-protocol-handler vscode`: it will open the folders when double-clicking on roles (not `include_role`) and
   the files for the others nodes. The cursor will be at the task exact position in the file.  
   Lastly, you can provide your own protocol formats
   with `--open-protocol-handler custom --open-protocol-custom-formats '{}'`. See the help
-  and [an example.](https://github.com/haidaraM/ansible-playbook-grapher/blob/12cee0fbd59ffbb706731460e301f0b886515357/ansibleplaybookgrapher/graphbuilder.py#L33-L42).
+  and [an example.](https://github.com/haidaraM/ansible-playbook-grapher/blob/12cee0fbd59ffbb706731460e301f0b886515357/ansibleplaybookgrapher/graphbuilder.py#L33-L42)
 - Filer tasks based on tags
 - Export the dot file used to generate the graph with Graphviz.
 
 ## Prerequisites
 
 - Python 3.10 at least. Might work with some previous versions but the code is NOT tested against them.
   See [support matrix](https://docs.ansible.com/ansible/latest/reference_appendices/release_and_maintenance.html#ansible-core-support-matrix).
@@ -69,18 +69,28 @@
   ```
 
 I try to respect [Red Hat Ansible Engine Life Cycle](https://access.redhat.com/support/policy/updates/ansible-engine)
 for the supported Ansible version.
 
 ## Installation
 
-```shell script
+```shell
 pip install ansible-playbook-grapher
 ```
 
+You can also install the unpublished version from GitHub direction. Examples: 
+
+```shell
+# Install the version from the main branch
+pip install "ansible-playbook-grapher @ git+https://github.com/haidaraM/ansible-playbook-grapher"
+
+# Install the version from a specific branch
+pip install "ansible-playbook-grapher @ git+https://github.com/haidaraM/ansible-playbook-grapher@specific-branch"
+```
+
 ### Renderers
 
 At the time of writing, two renderers are supported:
 
 1. `graphviz` (default): Generate the graph in SVG. It has more features and is more tested: open protocol,
    highlight linked nodes...
 2. `mermaid-flowchart`: Generate the graph in [Mermaid](https://mermaid.js.org/syntax/flowchart.html) format. You can
```

## Comparing `ansible_playbook_grapher-2.1.2.dist-info/RECORD` & `ansible_playbook_grapher-2.2.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-ansibleplaybookgrapher/__init__.py,sha256=a5wzvZyzXX9VLHZF30iWucvSZ3RsB7W0UKMBQdTzEwI,2827
-ansibleplaybookgrapher/cli.py,sha256=2Hr_9IilWO0tBU5bheXPukslamzwwxRKAMSl8fIaRm0,11280
-ansibleplaybookgrapher/graph_model.py,sha256=mlWmoJJCVDWLWqUSxVfqzzyqlQGR552Fa4i5ygVQX2s,13757
-ansibleplaybookgrapher/parser.py,sha256=Bg80ax-FGtPh4aMFWQdRnx7o_Tjb0B8qVhNru4WmWSk,19929
-ansibleplaybookgrapher/utils.py,sha256=zA-cqsZXQeDHtGKSQvE1VojufC-XUc3O6g9Z2stePsA,7014
+ansibleplaybookgrapher/__init__.py,sha256=Nw104BUi9_jwAPmryDsmHGI1BFLYkA4YA8CuSyq_hmc,60
+ansibleplaybookgrapher/cli.py,sha256=zwa8-m8kDN2wdAJAOlpLf8BQFj8lbwk7KDhZrW5uE-8,12252
+ansibleplaybookgrapher/graph_model.py,sha256=vgFYIt8OIe7a5frfxcbkGxGSjaJcEIxKpQNsMwVVkfU,15624
+ansibleplaybookgrapher/grapher.py,sha256=sv9wkGXCcncwfasABCWiqdts9f6M5nDA6aAmg8m1Jiw,2679
+ansibleplaybookgrapher/parser.py,sha256=sTKYk8udQH3TyACZOpjGYtUjvFT7BWSh7YOrl00BmWo,20440
+ansibleplaybookgrapher/utils.py,sha256=806W3t89d13CojWCBhZsSx_cKwWyEqYyin_C0PHxg90,7031
 ansibleplaybookgrapher/data/graph.css,sha256=qavGSKdZrqaZYnRt9BfUQXLN65pK1iMA5KjsGm_nLDQ,358
 ansibleplaybookgrapher/data/highlight-hover.js,sha256=9uzi0vi4O2nq3OcJS-rKiqrEcGbXRZp0LkDmgKr4yls,5458
-ansibleplaybookgrapher/renderer/__init__.py,sha256=fhHpnesA4t8ERxGs67CupLBPw4a-9dnV5UtXk0TDPsY,8189
-ansibleplaybookgrapher/renderer/mermaid.py,sha256=gkKBLRyh8PAW1C3fvlSLiDs1IKx5g-OFERlLVnJtTuw,11304
-ansibleplaybookgrapher/renderer/graphviz/__init__.py,sha256=DMn7VisId1mF3gvMpzQspuHtUTX6BSCB_osK_eKmJLE,11050
+ansibleplaybookgrapher/renderer/__init__.py,sha256=EAe43j5a0RERQRBpDfGf8mx62g_JGPSeCNOe9tPKEhI,8709
+ansibleplaybookgrapher/renderer/mermaid.py,sha256=TWqoV8ZPn2_s49sLSZwsIGhgtiKZ2S8OumvFhVzeIok,13229
+ansibleplaybookgrapher/renderer/graphviz/__init__.py,sha256=KYbZq-KGhSlIZPpdOwNXT-TDoEhRFSEYEFIKyaT7Mms,12104
 ansibleplaybookgrapher/renderer/graphviz/postprocessor.py,sha256=pR_CFeXdaaKLFO0Y0GRMXqzmEvzh6ZZdAtvBbOFOgbo,7367
-ansible_playbook_grapher-2.1.2.dist-info/LICENSE,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
-ansible_playbook_grapher-2.1.2.dist-info/METADATA,sha256=kP_cADoP-YJOCY0bDSKz5VYeFpmJ9RioFORzQa4ScRQ,22870
-ansible_playbook_grapher-2.1.2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-ansible_playbook_grapher-2.1.2.dist-info/entry_points.txt,sha256=wUiLaLPGWO72NzS8DzTseCcpF7ZC0IglJvrHwT5KXaI,77
-ansible_playbook_grapher-2.1.2.dist-info/top_level.txt,sha256=28v1PSNEaxaneuj2r3oh30LSAfAl_hlhNELiesTP6Ns,23
-ansible_playbook_grapher-2.1.2.dist-info/RECORD,,
+ansible_playbook_grapher-2.2.0.dist-info/LICENSE,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
+ansible_playbook_grapher-2.2.0.dist-info/METADATA,sha256=zhWdHqpkX3IaFrCLt4sEsk2Up4hCCvSPE3y5i1oNpZw,23247
+ansible_playbook_grapher-2.2.0.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
+ansible_playbook_grapher-2.2.0.dist-info/entry_points.txt,sha256=wUiLaLPGWO72NzS8DzTseCcpF7ZC0IglJvrHwT5KXaI,77
+ansible_playbook_grapher-2.2.0.dist-info/top_level.txt,sha256=28v1PSNEaxaneuj2r3oh30LSAfAl_hlhNELiesTP6Ns,23
+ansible_playbook_grapher-2.2.0.dist-info/RECORD,,
```

