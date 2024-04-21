# Comparing `tmp/ado_wrapper-1.2.3.tar.gz` & `tmp/ado_wrapper-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-1.2.3.tar", max compression
+gzip compressed data, was "ado_wrapper-1.2.5.tar", max compression
```

## Comparing `ado_wrapper-1.2.3.tar` & `ado_wrapper-1.2.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.2.3/LICENSE
--rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.2.3/README.md
--rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-1.2.3/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6504 2024-04-13 22:32:43.045229 ado_wrapper-1.2.3/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     2187 2024-04-15 19:13:07.849775 ado_wrapper-1.2.3/ado_wrapper/client.py
--rw-r--r--   0        0        0    25667 2024-04-11 13:43:04.075027 ado_wrapper-1.2.3/ado_wrapper/dumps.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.2.3/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.2.3/ado_wrapper/plan_resources/colours.py
--rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-1.2.3/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     1039 2024-04-09 15:28:42.529947 ado_wrapper-1.2.3/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1820 2024-04-12 10:52:50.915024 ado_wrapper-1.2.3/ado_wrapper/plan_resources/plan_resource.py
--rw-r--r--   0        0        0     1197 2024-04-14 14:26:49.075843 ado_wrapper-1.2.3/ado_wrapper/plan_resources/plan_state_manager.py
--rw-r--r--   0        0        0      959 2024-04-19 12:39:56.727239 ado_wrapper-1.2.3/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     3697 2024-04-15 19:19:32.967229 ado_wrapper-1.2.3/ado_wrapper/resources/annotated_tags.py
--rw-r--r--   0        0        0     3399 2024-04-15 19:15:02.852905 ado_wrapper-1.2.3/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    14176 2024-04-19 13:09:31.555935 ado_wrapper-1.2.3/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6583 2024-04-17 12:27:37.565922 ado_wrapper-1.2.3/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     7015 2024-04-19 13:08:56.187536 ado_wrapper-1.2.3/ado_wrapper/resources/environment.py
--rw-r--r--   0        0        0     3318 2024-04-15 19:13:07.863404 ado_wrapper-1.2.3/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0    14986 2024-04-19 10:09:09.141487 ado_wrapper-1.2.3/ado_wrapper/resources/merge_policies.py
--rw-r--r--   0        0        0     2145 2024-04-09 18:43:06.211713 ado_wrapper-1.2.3/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    13973 2024-04-17 12:29:03.443391 ado_wrapper-1.2.3/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12505 2024-04-15 09:20:30.240006 ado_wrapper-1.2.3/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0    10223 2024-04-19 08:59:23.116079 ado_wrapper-1.2.3/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0     5972 2024-04-17 09:03:01.080407 ado_wrapper-1.2.3/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4569 2024-04-14 10:59:03.753536 ado_wrapper-1.2.3/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8320 2024-04-14 15:16:24.207939 ado_wrapper-1.2.3/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     4905 2024-04-18 15:13:38.570059 ado_wrapper-1.2.3/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     8988 2024-04-19 12:11:56.341395 ado_wrapper-1.2.3/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     8158 2024-04-18 15:00:31.824976 ado_wrapper-1.2.3/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4412 2024-04-19 09:09:37.626208 ado_wrapper-1.2.3/ado_wrapper/utils.py
--rw-r--r--   0        0        0     2446 2024-04-19 13:10:08.802875 ado_wrapper-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.2.5/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.2.5/README.md
+-rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.2.5/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6516 2024-04-20 14:42:40.466955 ado_wrapper-1.2.5/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2187 2024-04-20 14:42:40.461532 ado_wrapper-1.2.5/ado_wrapper/client.py
+-rw-r--r--   0        0        0    25691 2024-04-21 11:28:27.535399 ado_wrapper-1.2.5/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.2.5/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.2.5/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      296 2024-04-20 14:42:40.463115 ado_wrapper-1.2.5/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1067 2024-04-20 14:52:39.222521 ado_wrapper-1.2.5/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1820 2024-04-20 14:42:40.459386 ado_wrapper-1.2.5/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0      810 2024-04-20 14:49:27.573050 ado_wrapper-1.2.5/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0      976 2024-04-20 14:42:40.468814 ado_wrapper-1.2.5/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     3686 2024-04-20 14:42:40.464925 ado_wrapper-1.2.5/ado_wrapper/resources/annotated_tags.py
+-rw-r--r--   0        0        0     3387 2024-04-20 14:42:40.459127 ado_wrapper-1.2.5/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    14412 2024-04-20 14:42:40.461841 ado_wrapper-1.2.5/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6583 2024-04-20 14:42:40.461166 ado_wrapper-1.2.5/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     7400 2024-04-21 11:21:05.077074 ado_wrapper-1.2.5/ado_wrapper/resources/environment.py
+-rw-r--r--   0        0        0     3308 2024-04-20 14:42:40.459124 ado_wrapper-1.2.5/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0    15041 2024-04-21 14:53:26.732423 ado_wrapper-1.2.5/ado_wrapper/resources/merge_policies.py
+-rw-r--r--   0        0        0     2135 2024-04-20 14:42:40.459308 ado_wrapper-1.2.5/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    13959 2024-04-20 14:42:40.461581 ado_wrapper-1.2.5/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12487 2024-04-20 14:42:40.465582 ado_wrapper-1.2.5/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0    10226 2024-04-21 11:31:44.945603 ado_wrapper-1.2.5/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0     5959 2024-04-21 11:45:20.048677 ado_wrapper-1.2.5/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4557 2024-04-20 14:42:40.463787 ado_wrapper-1.2.5/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8295 2024-04-21 11:27:53.911242 ado_wrapper-1.2.5/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4828 2024-04-21 14:52:13.248475 ado_wrapper-1.2.5/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     9221 2024-04-20 21:44:51.189171 ado_wrapper-1.2.5/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     7894 2024-04-20 14:58:04.398791 ado_wrapper-1.2.5/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4746 2024-04-21 11:34:45.103015 ado_wrapper-1.2.5/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2671 2024-04-21 14:54:40.879869 ado_wrapper-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.2.5/PKG-INFO
```

### Comparing `ado_wrapper-1.2.3/LICENSE` & `ado_wrapper-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.3/README.md` & `ado_wrapper-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.3/ado_wrapper/__main__.py` & `ado_wrapper-1.2.5/ado_wrapper/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import argparse
 
 from ado_wrapper.client import AdoClient
-from ado_wrapper.utils import get_internal_field_names, get_resource_variables, ResourceType
+from ado_wrapper.utils import (
+    ResourceType,
+    get_internal_field_names,
+    get_resource_variables,
+)
 
 
 def main() -> None:  # pylint: disable=too-many-branches, too-many-statements
     ALL_RESOURCES = get_resource_variables()
 
     parser = argparse.ArgumentParser(
         prog="AdoWrapper", description="A tool to manage Azure DevOps resources and interface with the ADO API", usage=""
@@ -44,15 +48,15 @@
 
     if args.email is None and args.token is None and args.ado_org is None and args.ado_project is None and args.creds_file is None:
         raise ValueError("You must provide either --email and --token or --creds_file")
 
     if args.email is not None and args.token is not None and args.ado_org is not None and args.ado_project is not None:
         ado_client = AdoClient(args.email, args.token, args.ado_org, args.ado_project, state_file_name=args.state_file)
     elif args.creds_file:
-        with open(args.creds_file, "r", encoding="utf-8") as f:
+        with open(args.creds_file, encoding="utf-8") as f:
             creds = f.read().split("\n")
             ado_client = AdoClient(creds[0], creds[1], creds[2], creds[3], state_file_name=args.state_file)
 
     if args.purge_state:
         # Deletes everything in the state file
         print("[ADO_WRAPPER] Purging state")
         ado_client.state_manager.wipe_state()
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/client.py` & `ado_wrapper-1.2.5/ado_wrapper/client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Literal
 
 import requests
 from requests.auth import HTTPBasicAuth
 
-from ado_wrapper.state_manager import StateManager
 from ado_wrapper.plan_resources.plan_state_manager import PlanStateManager
+from ado_wrapper.state_manager import StateManager
 from ado_wrapper.utils import AuthenticationError
 
 
 class AdoClient:
     def __init__(  # pylint: disable=too-many-arguments
         self, ado_email: str, ado_pat: str, ado_org: str, ado_project: str,
         state_file_name: str | None = "main.state", bypass_initialisation: bool = False,
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/dumps.py` & `ado_wrapper-1.2.5/ado_wrapper/dumps.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     ],
     "triggerInfo": {},
     "id": "{build_id}",
     "buildNumber": "20240101.1",
     "status": "notStarted",
     "queueTime": "2024-03-17T11:03:29.2982876Z",
     "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/Builds/{build_id}",
-    "definition": {"drafts": [], "id": "{build_def_id}", "name": "ado_wrapper-test-build", "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/Definitions/{build_id}?revision=1", "uri": "vstfs:///Build/Definition/{build_id}", "path": "\\", "type": "build", "queueStatus": "enabled", "revision": 1, "project": {"id": "{ado_client.project_id}", "name": "Platform", "url": "https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}", "state": "wellFormed", "revision": "{revision}", "visibility": "private", "lastUpdateTime": "2024-01-01T12:14:30.36Z"}},
+    "definition": {"drafts": [], "id": "{build_def_id}", "name": "ado_wrapper-test-build", "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/Definitions/{build_id}?revision=1", "uri": "vstfs:///Build/Definition/{build_id}", "path": "\\", "type": "build", "queueStatus": "enabled", "revision": 1, "project": {"id": "{ado_client.project_id}", "name": "{ado_client.project}", "url": "https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}", "state": "wellFormed", "revision": "{revision}", "visibility": "private", "lastUpdateTime": "2024-01-01T12:14:30.36Z"}},
     "buildNumberRevision": 1,
-    "project": {"id": "{ado_client.project_id}", "name": "Platform", "url": "https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}", "state": "wellFormed", "revision": 399, "visibility": "private", "lastUpdateTime": "2024-02-06T14:14:30.36Z"},
+    "project": {"id": "{ado_client.project_id}", "name": "{ado_client.project}", "url": "https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}", "state": "wellFormed", "revision": 399, "visibility": "private", "lastUpdateTime": "2024-02-06T14:14:30.36Z"},
     "uri": "vstfs:///Build/Build/93458",
     "sourceBranch": "refs/heads/my-branch",
     "sourceVersion": "<commit_id>",
     "queue": {"id": "{queue_id}", "name": "<pool_name>", "pool": {"id": "{pool_id}", "name": "<pool_name"}},
     "priority": "normal",
     "reason": "manual",
     "requestedFor": {"displayName": "<First Last>", "url": "https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<user_id>", "_links": {"avatar": {"href": "https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>"}}, "id": "<user_id>", "uniqueName": "<first.last@company.com>", "imageUrl": "https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>", "descriptor": "<user_descriptor>"},
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-1.2.5/ado_wrapper/plan_resources/plan_repo.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
-from ado_wrapper.client import AdoClient
 from ado_wrapper.resources.repo import Repo
 
+if TYPE_CHECKING:
+    from ado_wrapper.client import AdoClient
+
 UNKNOWN_UNTIL_APPLY = "Unknown until apply"
 BYPASS_CHECK = True
 
 
 class PlanRepo:
-    def get_by_id(self, ado_client: AdoClient, repo_id: str) -> Repo:
+    def get_by_id(self, ado_client: "AdoClient", repo_id: str) -> Repo:
         state_copy = ado_client.state_manager.load_state()["resources"][self.__class__.__name__].get(repo_id)  # type: ignore
         if state_copy:
             return Repo.from_json(state_copy)  # type: ignore[return-value]
         return Repo.get_by_id(ado_client, repo_id)
 
     @staticmethod
-    def create(ado_client: AdoClient, _: str, payload: dict[str, Any]) -> Repo:
+    def create(ado_client: "AdoClient", _: str, payload: dict[str, Any]) -> Repo:
         name = payload["name"]
-        if not BYPASS_CHECK:
-            if Repo.get_by_name(ado_client, name):
-                raise ValueError(f"Repo {name} already exists")
+        if not BYPASS_CHECK and Repo.get_by_name(ado_client, name):
+            raise ValueError(f"Repo {name} already exists")
         return Repo(UNKNOWN_UNTIL_APPLY, name)
 
-    def update(self, ado_client: AdoClient, url: str, attribute_name: str, attribute_value: Any, payload: dict[str, Any]) -> Repo:
+    def update(self, ado_client: "AdoClient", url: str, attribute_name: str, attribute_value: Any, payload: dict[str, Any]) -> Repo:
         return ""  # type: ignore[return-value]
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/plan_resources/plan_resource.py` & `ado_wrapper-1.2.5/ado_wrapper/plan_resources/plan_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from ado_wrapper.utils import extract_id
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
     from ado_wrapper.state_managed_abc import StateManagedResource
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/resources/__init__.py` & `ado_wrapper-1.2.5/ado_wrapper/resources/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from ado_wrapper.resources.annotated_tags import AnnotatedTag
 from ado_wrapper.resources.branches import Branch
 from ado_wrapper.resources.builds import Build, BuildDefinition
 from ado_wrapper.resources.commits import Commit
 from ado_wrapper.resources.environment import Environment, PipelineAuthorisation
 from ado_wrapper.resources.groups import Group
-from ado_wrapper.resources.merge_policies import MergePolicies, MergeBranchPolicy, MergePolicyDefaultReviewer
+from ado_wrapper.resources.merge_policies import (
+    MergeBranchPolicy,
+    MergePolicies,
+    MergePolicyDefaultReviewer,
+)
 from ado_wrapper.resources.projects import Project
 from ado_wrapper.resources.pull_requests import PullRequest
 from ado_wrapper.resources.releases import Release, ReleaseDefinition
-from ado_wrapper.resources.repo import Repo, BuildRepository
+from ado_wrapper.resources.repo import BuildRepository, Repo
 from ado_wrapper.resources.service_endpoint import ServiceEndpoint
 from ado_wrapper.resources.teams import Team
-from ado_wrapper.resources.users import AdoUser, TeamMember, Member, Reviewer
+from ado_wrapper.resources.users import AdoUser, Member, Reviewer, TeamMember
 from ado_wrapper.resources.variable_groups import VariableGroup
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/resources/annotated_tags.py` & `ado_wrapper-1.2.5/ado_wrapper/resources/annotated_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
+import json
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import TYPE_CHECKING, Any
 
-import json
-
-from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import Member
+from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.utils import from_ado_date_string
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 
 @dataclass
@@ -21,28 +20,28 @@
     object_id: str = field(metadata={"is_id_field": True})
     name: str
     message: str
     tagged_by: Member
     created_at: datetime
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, Any]) -> "AnnotatedTag":
+    def from_request_payload(cls, data: dict[str, Any]) -> AnnotatedTag:
         member = Member(data["taggedBy"]["name"], data["taggedBy"]["email"], "UNKNOWN")
         created_at = datetime.fromisoformat(data["taggedBy"]["date"])
         return cls(data["objectId"], data["name"], data["message"], member, created_at)
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, repo_id: str, branch_id: str) -> "AnnotatedTag":  # type: ignore[override]
+    def get_by_id(cls, ado_client: AdoClient, repo_id: str, branch_id: str) -> AnnotatedTag:  # type: ignore[override]
         return super().get_by_url(
             ado_client,
             f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/annotatedtags/{branch_id}?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
 
     @classmethod
-    def create(cls, ado_client: AdoClient, repo_id: str, name: str, message: str, object_id: str) -> "AnnotatedTag":  # type: ignore[override]
+    def create(cls, ado_client: AdoClient, repo_id: str, name: str, message: str, object_id: str) -> AnnotatedTag:  # type: ignore[override]
         return super().create(
             ado_client,
             f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/annotatedTags?api-version=7.1-preview.1",
             payload={"name": name, "message": message, "taggedObject": {"objectId": object_id}},
         )  # type: ignore[return-value]
 
     @classmethod
@@ -51,15 +50,15 @@
         raise NotImplementedError("You can't delete a tag!")
 
     # # ============ End of requirement set by all state managed resources ================== #
     # # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # # =============== Start of additional methods included with class ===================== #
 
     @classmethod
-    def get_all_by_repo(cls, ado_client: AdoClient, repo_name: str) -> list["AnnotatedTag"]:
+    def get_all_by_repo(cls, ado_client: AdoClient, repo_name: str) -> list[AnnotatedTag]:
         """Unofficial API."""
         request = ado_client.session.post(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_git/{repo_name}/tags/?api-version=7.1-preview.1"
         )
         assert request.status_code == 200
         second_half = request.text.split("ms.vss-code-web.git-tags-data-provider")[1].removeprefix('":')
         trimmed_second_half = second_half.split("ms.vss-code-web.navigation-data-provider")[0].removesuffix(',"')
@@ -70,12 +69,12 @@
                 Member(x["tagger"]["name"], x["tagger"]["email"], "UNKNOWN"),
                 from_ado_date_string(x["tagger"]["date"]),
             )
             for x in json_data if "comment" in x  # fmt: skip
         ]
 
     @classmethod
-    def get_by_name(cls, ado_client: AdoClient, repo_id: str, tag_name: str) -> "AnnotatedTag | None":
+    def get_by_name(cls, ado_client: AdoClient, repo_id: str, tag_name: str) -> AnnotatedTag | None:
         for tag in cls.get_all_by_repo(ado_client, repo_id):
             if tag.name == tag_name:
                 return tag
         raise ValueError(f"Tag {tag_name} not found")
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/resources/branches.py` & `ado_wrapper-1.2.5/ado_wrapper/resources/branches.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Literal, TYPE_CHECKING
+from typing import TYPE_CHECKING, Literal
 
 from ado_wrapper.state_managed_abc import StateManagedResource
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 BranchEditableAttribute = Literal["name"]
@@ -19,30 +19,30 @@
     """
 
     branch_id: str = field(metadata={"is_id_field": True})
     name: str = field(metadata={"editable": True})  # Maybe more?
     repo_id: str = field(repr=False)
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, str | dict[str, str]]) -> "Branch":
+    def from_request_payload(cls, data: dict[str, str | dict[str, str]]) -> Branch:
         return cls(
             data["objectId"],  # type: ignore[arg-type]
             data["name"].removeprefix("refs/heads/"),  # type: ignore[union-attr]
             data["url"].split("/")[-2],  # type: ignore[union-attr]
         )
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, repo_id: str, branch_id: str) -> "Branch":  # type: ignore[override]
+    def get_by_id(cls, ado_client: AdoClient, repo_id: str, branch_id: str) -> Branch:  # type: ignore[override]
         for branch in cls.get_all_by_repo(ado_client, repo_id):
             if branch.branch_id == branch_id:
                 return branch
         raise ValueError(f"Branch {branch_id} not found")
 
     @classmethod
-    def create(cls, ado_client: AdoClient, repo_id: str, branch_name: str, source_branch: str = "main") -> "Branch":  # type: ignore[override]
+    def create(cls, ado_client: AdoClient, repo_id: str, branch_name: str, source_branch: str = "main") -> Branch:  # type: ignore[override]
         raise NotImplementedError("You can't create a branch without a commit, use Commit.create instead")
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, repo_id: str, branch_id: str) -> None:
         raise NotImplementedError("You can't delete a branch without a commit, use Commit.delete instead")
         # return super().delete_by_id(
         #     ado_client,
@@ -51,26 +51,26 @@
         # )
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
-    def get_all_by_repo(cls, ado_client: AdoClient, repo_id: str) -> list["Branch"]:
+    def get_all_by_repo(cls, ado_client: AdoClient, repo_id: str) -> list[Branch]:
         return super().get_all(
             ado_client,
             f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/refs?filter=heads&api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
-    def get_by_name(cls, ado_client: AdoClient, repo_id: str, branch_name: str) -> "Branch | None":
+    def get_by_name(cls, ado_client: AdoClient, repo_id: str, branch_name: str) -> Branch | None:
         for branch in cls.get_all_by_repo(ado_client, repo_id):
             if branch.name == branch_name:
                 return branch
         raise ValueError(f"Branch {branch_name} not found")
 
     @classmethod
-    def get_main_branch(cls, ado_client: AdoClient, repo_id: str) -> "Branch":
+    def get_main_branch(cls, ado_client: AdoClient, repo_id: str) -> Branch:
         return [x for x in cls.get_all_by_repo(ado_client, repo_id) if x.name in ("main", "master")][0]
 
     def delete(self, ado_client: AdoClient) -> None:  # Has to exist for multi-ids
         self.delete_by_id(ado_client, self.repo_id, self.branch_id)
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/resources/builds.py` & `ado_wrapper-1.2.5/ado_wrapper/resources/builds.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from datetime import datetime
-from dataclasses import dataclass, field
-from typing import Any, Literal, TYPE_CHECKING
 import time
+from dataclasses import dataclass, field
+from datetime import datetime
+from typing import TYPE_CHECKING, Any, Literal
 
-from ado_wrapper.utils import from_ado_date_string
-from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.environment import Environment, PipelineAuthorisation
 from ado_wrapper.resources.repo import BuildRepository
 from ado_wrapper.resources.users import Member
+from ado_wrapper.state_managed_abc import StateManagedResource
+from ado_wrapper.utils import from_ado_date_string
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 BuildDefinitionEditableAttribute = Literal["name", "description"]
 BuildStatus = Literal["notStarted", "inProgress", "completed", "cancelling", "postponed", "notSet", "none"]
 QueuePriority = Literal["low", "belowNormal", "normal", "aboveNormal", "high"]
@@ -160,14 +160,15 @@
         )  # type: ignore[return-value]
 
     @classmethod
     def allow_on_environment(cls, ado_client: "AdoClient", definition_id: str, environment_id: str) -> PipelineAuthorisation:
         environment = Environment.get_by_id(ado_client, environment_id)
         return environment.add_pipeline_permission(ado_client, definition_id)
 
+
 # ========================================================================================================
 
 
 @dataclass
 class BuildDefinition(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/build/definitions?view=azure-devops-rest-7.1"""
 
@@ -248,14 +249,18 @@
             f"/{ado_client.ado_project}/_apis/build/definitions?api-version=7.1",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
+    @classmethod
+    def get_all_by_name(cls, ado_client: "AdoClient", name: str) -> "list[BuildDefinition]":
+        return cls.get_by_abstract_filter(ado_client, lambda x: x.name == name)  # type: ignore[return-value, attr-defined]
+
     def get_all_builds_by_definition(self, ado_client: "AdoClient") -> "list[Build]":
         return Build.get_all_by_definition(ado_client, self.build_definition_id)
 
     @classmethod
     def get_all_by_repo_id(cls, ado_client: "AdoClient", repo_id: str) -> "list[BuildDefinition]":
         return super().get_all(
             ado_client,
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/resources/commits.py` & `ado_wrapper-1.2.5/ado_wrapper/resources/commits.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from datetime import datetime
 from dataclasses import dataclass, field
-from typing import Literal, Any, TYPE_CHECKING
+from datetime import datetime
+from typing import TYPE_CHECKING, Any, Literal
 
-from ado_wrapper.utils import from_ado_date_string, InvalidPermissionsError
-from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import Member
+from ado_wrapper.state_managed_abc import StateManagedResource
+from ado_wrapper.utils import InvalidPermissionsError, from_ado_date_string
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 ChangeType = Literal["edit", "add", "delete"]
 FIRST_COMMIT_ID = "0000000000000000000000000000000000000000"  # I don't know why this works, but it does, please leave it.
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/resources/environment.py` & `ado_wrapper-1.2.5/ado_wrapper/resources/environment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from datetime import datetime
-from typing import Any, Literal, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Literal
 
-from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import Member
+from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.utils import from_ado_date_string
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 EnvironmentEditableAttribute = Literal["name", "description"]
 
@@ -84,20 +84,25 @@
     # # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # # =============== Start of additional methods included with class ===================== #
 
     @classmethod
     def get_by_name(cls, ado_client: AdoClient, name: str) -> Environment:
         return cls.get_by_abstract_filter(ado_client, lambda x: x.name == name)  # type: ignore[return-value, attr-defined]
 
+    # # =============== Pipeline Permissions ===================== #
+
     def get_pipeline_permissions(self, ado_client: AdoClient) -> dict[str, Any]:
         return PipelineAuthorisation.get_all_for_environment(ado_client, self.environment_id)  # type: ignore[return-value]
 
     def add_pipeline_permission(self, ado_client: AdoClient, pipeline_id: str) -> PipelineAuthorisation:
         return PipelineAuthorisation.create(ado_client, self.environment_id, pipeline_id)
 
+    def remove_pipeline_permissions(self, ado_client: AdoClient, pipeline_id: str) -> None:
+        PipelineAuthorisation.delete_by_id(ado_client, self.environment_id, pipeline_id)
+
 @dataclass
 class PipelineAuthorisation:
     pipeline_authorisation_id: str
     environment_id: str
     authorized: bool
     authorized_by: Member
     authorized_on: datetime
@@ -109,38 +114,43 @@
             environment_id,
             data["authorized"],
             Member.from_request_payload(data["authorizedBy"]),
             from_ado_date_string(data["authorizedOn"]),
         )
 
     @classmethod
-    def get_all_for_environment(cls, ado_client: AdoClient, environment_id: str) -> list[PipelineAuthorisation]:  # type: ignore[override]
+    def get_all_for_environment(cls, ado_client: AdoClient, environment_id: str) -> list[PipelineAuthorisation]:
         request = ado_client.session.get(
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project_id}/_apis/pipelines/pipelinePermissions/environment/{environment_id}",
+            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/pipelines/pipelinePermissions/environment/{environment_id}",
         ).json()
         return [cls.from_request_payload(x, request["resource"]["id"]) for x in request["pipelines"]]
 
     @classmethod
-    def create(cls, ado_client: AdoClient, environment_id: str, pipeline_id: str, authorized: bool=True) -> PipelineAuthorisation:
+    def create(cls, ado_client: AdoClient, environment_id: str, pipeline_id: str, authorized: bool = True) -> PipelineAuthorisation:
         all_existing = cls.get_all_for_environment(ado_client, environment_id)
-        payload = {"pipelines": [{"id": x.pipeline_authorisation_id, "authorized": True} for x in all_existing]}
+        payload: dict[str, Any] = {"pipelines": [{"id": x.pipeline_authorisation_id, "authorized": True} for x in all_existing]}
         payload["pipelines"] = [x for x in payload["pipelines"] if x["id"] != pipeline_id]  # Remove existing entry if it exists
         payload["pipelines"].append({"id": pipeline_id, "authorized": authorized})
         payload |= {"resource": {"type": "environment", "id": environment_id}}
 
         request = ado_client.session.patch(
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project_id}/_apis/pipelines/pipelinePermissions/environment/{environment_id}?api-version=7.1-preview.1",
+            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/pipelines/pipelinePermissions/environment/{environment_id}?api-version=7.1-preview.1",
             json=payload,
         )
         if request.status_code == 404:
             raise ValueError(f"Pipeline {pipeline_id} not found.")
+        if not request.json()["pipelines"]:
+            raise ValueError(f"Pipeline {pipeline_id} not found.")
         created_pipeline_dict = max(request.json()["pipelines"], key=lambda x: x["authorizedOn"])
         return cls.from_request_payload(created_pipeline_dict, environment_id)
 
-    def update(self, ado_client: AdoClient, authorized: bool) -> None:  # type: ignore[override]
+    def update(self, ado_client: AdoClient, authorized: bool) -> None:
         self.delete_by_id(ado_client, self.environment_id, self.pipeline_authorisation_id)
         new = self.create(ado_client, self.environment_id, self.pipeline_authorisation_id, authorized)
         self.__dict__.update(new.__dict__)
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, environment_id: str, pipeline_authorisation_id: str) -> None:
-        cls.create(ado_client, environment_id, pipeline_authorisation_id, False)
+        try:
+            cls.create(ado_client, environment_id, pipeline_authorisation_id, False)
+        except ValueError:
+            pass
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/resources/groups.py` & `ado_wrapper-1.2.5/ado_wrapper/resources/groups.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
 from dataclasses import dataclass, field
+from typing import TYPE_CHECKING
 
 from ado_wrapper.state_managed_abc import StateManagedResource
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 
@@ -17,46 +17,46 @@
     name: str = field(metadata={"internal_name": "displayName"})  # Not editable
     description: str
     group_id: str  # Not editable, don't use
     origin_id: str = field(metadata={"internal_name": "originId"})  # Not editable, don't use
     # group_members: list[GroupMember] = field(default_factory=list)
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, str]) -> "Group":
+    def from_request_payload(cls, data: dict[str, str]) -> Group:
         return cls(data["url"].split("/_apis/Graph/Groups/", maxsplit=1)[1], data["displayName"], data.get("description", ""),
                    data["domain"].removeprefix("vstfs:///Classification/TeamProject/"), data["originId"])  # fmt: skip
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, group_descriptor: str) -> "Group":
+    def get_by_id(cls, ado_client: AdoClient, group_descriptor: str) -> Group:
         return super().get_by_url(
             ado_client,  # Preview required
             f"https://vssps.dev.azure.com/{ado_client.ado_org}/_apis/graph/groups/{group_descriptor}?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
 
     @classmethod
-    def create(cls, ado_client: AdoClient, name: str) -> "Group":  # type: ignore[override]
+    def create(cls, ado_client: AdoClient, name: str) -> Group:  # type: ignore[override]
         raise NotImplementedError
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, group_id: str) -> None:  # type: ignore[override]
         raise NotImplementedError
 
     @classmethod
-    def get_all(cls, ado_client: AdoClient) -> list["Group"]:  # type: ignore[override]
+    def get_all(cls, ado_client: AdoClient) -> list[Group]:  # type: ignore[override]
         return super().get_all(
             ado_client,  # Preview required
             f"https://vssps.dev.azure.com/{ado_client.ado_org}/_apis/graph/groups?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
-    def get_by_name(cls, ado_client: AdoClient, group_name: str) -> "Group | None":
+    def get_by_name(cls, ado_client: AdoClient, group_name: str) -> Group | None:
         return cls.get_by_abstract_filter(ado_client, lambda group: group.name == group_name)  # type: ignore[return-value, attr-defined]
 
     # @classmethod
     # def get_all_by_member(cls, ado_client: AdoClient, member_descriptor_id: str) -> list["Group"]:
     #     raise NotImplementedError
     # Will finish this later
     # return [group for group in cls.get_all(ado_client) if group.group_descriptor == member_descriptor_id]
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/resources/merge_policies.py` & `ado_wrapper-1.2.5/ado_wrapper/resources/merge_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from datetime import datetime
-from typing import Any, Literal, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Literal
 
-from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import Reviewer
-from ado_wrapper.utils import from_ado_date_string
+from ado_wrapper.state_managed_abc import StateManagedResource
+from ado_wrapper.utils import from_ado_date_string, requires_initialisation
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 WhenChangesArePushed = Literal["require_revote_on_each_iteration", "require_revote_on_last_iteration",
                                "reset_votes_on_source_push", "reset_rejections_on_source_push", "do_nothing"]  # fmt: skip
 merge_complete_name_mapping = {
@@ -45,18 +45,19 @@
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> StateManagedResource:
         return cls(data["id"], data["settings"]["requiredReviewerIds"][0], data["isBlocking"])
 
     @staticmethod
     def get_default_reviewers(ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> list[Reviewer]:
+        requires_initialisation(ado_client)
         payload = {"contributionIds": ["ms.vss-code-web.branch-policies-data-provider"],
                    "dataProviderContext": {"properties": {"projectId": ado_client.ado_project_id, "repositoryId": repo_id, "refName": f"refs/heads/{branch_name}"}}}  # fmt: skip
         request = ado_client.session.post(
-            "https://dev.azure.com/VFCloudEngineering/_apis/Contribution/HierarchyQuery?api-version=7.1-preview.1",
+            f"https://dev.azure.com/{ado_client.ado_org}/_apis/Contribution/HierarchyQuery?api-version=7.1-preview.1",
             json=payload,
         ).json()
         if request is None:
             return []
         all_reviewers = [Reviewer(x["displayName"], x["uniqueName"], x["id"], 0, False) for x in request["dataProviders"]["ms.vss-code-web.branch-policies-data-provider"]["identities"]]  # fmt: skip
         for policy_group in request["dataProviders"]["ms.vss-code-web.branch-policies-data-provider"]["policyGroups"].values():
             if policy_group["currentScopePolicies"] is None:
@@ -78,27 +79,27 @@
             "isEnabled": True,
             "settings": {
                 "requiredReviewerIds": [reviewer_id],
                 "scope": [{"repositoryId": repo_id, "refName": f"refs/heads/{branch_name}", "matchKind": "Exact"}],
             },
         }
         request = ado_client.session.post(
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project_id}/_apis/policy/configurations?api-version=7.1",
+            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/policy/configurations?api-version=7.1",
             json=payload,
         )
         assert request.status_code == 200, f"Error setting branch policy: {request.text}"
 
     @staticmethod
     def remove_default_reviewer(ado_client: AdoClient, repo_id: str, reviewer_id: str, branch_name: str = "main") -> None:
         policies = MergePolicies.get_default_reviewers_by_repo_id(ado_client, repo_id, branch_name)
         policy_id = [x for x in policies if x.required_reviewer_id == reviewer_id][0].policy_id if policies is not None else None  # type: ignore[comparison-overlap]  # fmt: skip
         if not policy_id:
             return
         request = ado_client.session.delete(
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project_id}/_apis/policy/configurations/{policy_id}?api-version=7.1",
+            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/policy/configurations/{policy_id}?api-version=7.1",
         )
         assert request.status_code == 204, "Error removing required reviewer"
 
 
 @dataclass
 class MergeBranchPolicy(StateManagedResource):
     policy_id: str = field(metadata={"is_id_field": True})
@@ -109,29 +110,29 @@
     prohibit_last_pushers_vote: bool
     allow_completion_with_rejects: bool
     when_new_changes_are_pushed: WhenChangesArePushed
     created_date: datetime = field(repr=False)
     is_inherited: bool = field(default=False, repr=False)
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, Any], is_inherited: bool) -> "MergeBranchPolicy":  # type: ignore[override]
+    def from_request_payload(cls, data: dict[str, Any], is_inherited: bool) -> MergeBranchPolicy:  # type: ignore[override]
         settings = data["settings"]
         when_new_changes_are_pushed = merge_complete_name_mapping[
             ([x for x in merge_complete_name_mapping if settings.get(x, False)] or ["do_nothing"])[0]
         ]  # Any or "do_nothing"  # fmt: skip
         branch_name: str | None = settings["scope"][0]["refName"]
         return cls(
             data["id"], settings["scope"][0]["repositoryId"], (branch_name.removeprefix("refs/heads/") if branch_name else None),
             settings["minimumApproverCount"], settings["creatorVoteCounts"], settings["blockLastPusherVote"], settings["allowDownvotes"],
             when_new_changes_are_pushed, from_ado_date_string(data["createdDate"]),  # type: ignore[arg-type]
             is_inherited  # fmt: skip
         )
 
     @classmethod
-    def get_branch_policy(cls, ado_client: AdoClient, repo_id: str, branch_name: str) -> "MergeBranchPolicy | None":
+    def get_branch_policy(cls, ado_client: AdoClient, repo_id: str, branch_name: str) -> MergeBranchPolicy | None:
         """Gets the latest merge requirements for a pull request."""
         policy = MergePolicies.get_all_branch_policies_by_repo_id(ado_client, repo_id, branch_name)
         return policy[0] if policy else None
 
     @staticmethod
     def set_branch_policy(ado_client: AdoClient, repo_id: str, minimum_approver_count: int,
                           creator_vote_counts: bool, prohibit_last_pushers_vote: bool, allow_completion_with_rejects: bool,
@@ -154,27 +155,27 @@
             "type": {"id": _get_type_id(ado_client, "Minimum number of reviewers")},
             "isEnabled": True,
             "isBlocking": True,
         }
         request_method = "POST" if latest_policy_id is None else "PUT"
         request = ado_client.session.request(
             request_method,
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project_id}/_apis/policy/Configurations/{latest_policy_id or ''}".rstrip(
+            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/policy/Configurations/{latest_policy_id or ''}".rstrip(
                 "/"
             ),  # fmt: skip
             json=payload,
             headers={"Accept": "application/json;api-version=7.1"},
         )
         assert request.status_code == 200, f"Error setting branch policy: {request.text}"
 
 
 @dataclass
 class MergePolicies(StateManagedResource):
     @classmethod
-    def from_request_payload(cls, data: dict[str, Any]) -> list["MergePolicyDefaultReviewer | MergeBranchPolicy"] | None:  # type: ignore[override]
+    def from_request_payload(cls, data: dict[str, Any]) -> list[MergePolicyDefaultReviewer | MergeBranchPolicy] | None:  # type: ignore[override]
         """Used internally to get a list of all policies."""
         policy_groups: dict[str, Any] = data["dataProviders"]["ms.vss-code-web.branch-policies-data-provider"]["policyGroups"] or {}  # fmt: skip
         all_policies = []
         for policy_group in policy_groups.values():
             for policy in policy_group["currentScopePolicies"] or []:  # If it's None, don't loop
                 settings = policy["settings"]
                 # Limit merge types
@@ -199,15 +200,15 @@
 
             # for inherited_policy in policy_group["inheritedPolicies"] or []:
             #     all_policies.append(MergeBranchPolicy.from_request_payload(inherited_policy, True))
 
         return all_policies or None  # type: ignore[return-value]
 
     @classmethod
-    def get_all_by_repo_id(cls, ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> list["MergePolicyDefaultReviewer | MergeBranchPolicy"] | None:  # fmt: skip
+    def get_all_by_repo_id(cls, ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> list[MergePolicyDefaultReviewer | MergeBranchPolicy] | None:  # fmt: skip
         payload = {"contributionIds": ["ms.vss-code-web.branch-policies-data-provider"], "dataProviderContext": {"properties": {
             "repositoryId": repo_id, "refName": f"refs/heads/{branch_name}", "sourcePage": {"routeValues": {"project": ado_client.ado_project}}}}}  # fmt: skip
         request = ado_client.session.post(
             f"https://dev.azure.com/{ado_client.ado_org}/_apis/Contribution/HierarchyQuery?api-version=7.0-preview.1",
             json=payload,
         ).json()
         return cls.from_request_payload(request)
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/resources/projects.py` & `ado_wrapper-1.2.5/ado_wrapper/resources/projects.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
-from typing import Any, TYPE_CHECKING
-from datetime import datetime
 from dataclasses import dataclass, field
+from datetime import datetime
+from typing import TYPE_CHECKING, Any
 
 from ado_wrapper.state_managed_abc import StateManagedResource
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 
@@ -15,39 +15,39 @@
     "https://learn.microsoft.com/en-us/rest/api/azure/devops/core/projects?view=azure-devops-rest-7.1"
     project_id: str = field(metadata={"is_id_field": True})  # None are editable
     name: str
     description: str
     last_update_time: datetime | None = None
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, Any]) -> "Project":
+    def from_request_payload(cls, data: dict[str, Any]) -> Project:
         return cls(data["id"], data["name"], data.get("description", ""), data.get("lastUpdateTime"))
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, project_id: str) -> "Project":
+    def get_by_id(cls, ado_client: AdoClient, project_id: str) -> Project:
         return super().get_by_url(
             ado_client,
             f"/_apis/projects/{project_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
-    def create(cls, ado_client: AdoClient, project_name: str, project_description: str) -> "Project":  # type: ignore[override]
+    def create(cls, ado_client: AdoClient, project_name: str, project_description: str) -> Project:  # type: ignore[override]
         raise NotImplementedError
 
     @staticmethod
     def delete_by_id(ado_client: AdoClient, project_id: str) -> None:  # type: ignore[override]
         raise NotImplementedError
 
     @classmethod
-    def get_all(cls, ado_client: AdoClient) -> list["Project"]:  # type: ignore[override]
+    def get_all(cls, ado_client: AdoClient) -> list[Project]:  # type: ignore[override]
         return super().get_all(
             ado_client,
             "/_apis/projects?api-version=7.1",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
-    def get_by_name(cls, ado_client: AdoClient, project_name: str) -> "Project | None":
+    def get_by_name(cls, ado_client: AdoClient, project_name: str) -> Project | None:
         return cls.get_by_abstract_filter(ado_client, lambda project: project.name == project_name)  # type: ignore[return-value, attr-defined]
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-1.2.5/ado_wrapper/resources/pull_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
-from datetime import datetime
-from typing import Any, Literal, TYPE_CHECKING
 from dataclasses import dataclass, field
+from datetime import datetime
+from typing import TYPE_CHECKING, Any, Literal
 
-from ado_wrapper.utils import from_ado_date_string
-from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import Member, Reviewer
+from ado_wrapper.state_managed_abc import StateManagedResource
+from ado_wrapper.utils import from_ado_date_string
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
     from ado_wrapper.resources.repo import Repo
 
 PullRequestEditableAttribute = Literal["title", "description", "merge_status", "is_draft"]
 PullRequestStatus = Literal["active", "completed", "abandoned", "all", "notSet"]
@@ -36,36 +36,36 @@
     merge_status: MergeStatus = field(default="notSet", metadata={"editable": True, "internal_name": "status"})
     reviewers: list[Reviewer] = field(default_factory=list, repr=False)  # Static(ish)
 
     def __str__(self) -> str:
         return f"PullRequest(id={self.pull_request_id}, title={self.title}, repo_name={self.repo.name}, author={self.author!s}, status={self.merge_status})"
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, Any]) -> "PullRequest":
+    def from_request_payload(cls, data: dict[str, Any]) -> PullRequest:
         from ado_wrapper.resources.repo import Repo  # Circular import
 
         author = Member.from_request_payload(data["createdBy"])
         reviewers = [Reviewer.from_request_payload(reviewer) for reviewer in data["reviewers"]]
         repository = Repo(data["repository"]["id"], data["repository"]["name"])
         return cls(str(data["pullRequestId"]), data["title"], data.get("description", ""), data["sourceRefName"],
                    data["targetRefName"], author, from_ado_date_string(data["creationDate"]), repository,
                    from_ado_date_string(data.get("closedDate")), data["isDraft"], data.get("mergeStatus", "notSet"), reviewers)  # fmt: skip
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, pull_request_id: str) -> "PullRequest":
+    def get_by_id(cls, ado_client: AdoClient, pull_request_id: str) -> PullRequest:
         return super().get_by_url(
             ado_client,
             f"/{ado_client.ado_project}/_apis/git/pullrequests/{pull_request_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def create(  # type: ignore[override]
         cls, ado_client: AdoClient, repo_id: str, from_branch_name: str, pull_request_title: str,
         pull_request_description: str, is_draft: bool = False
-    ) -> "PullRequest":  # fmt: skip
+    ) -> PullRequest:  # fmt: skip
         """Takes a list of reviewer ids, a branch to pull into main, and an option to start as draft"""
         # https://stackoverflow.com/questions/64655138/add-reviewers-to-azure-devops-pull-request-in-api-call   <- Why we can't allow reviewers from the get go
         # , "reviewers": [{"id": reviewer_id for reviewer_id in reviewer_ids}]
         payload = {"sourceRefName": f"refs/heads/{from_branch_name}", "targetRefName": "refs/heads/main", "title": pull_request_title,
                    "description": pull_request_description, "isDraft": is_draft}  # fmt: skip
         request = ado_client.session.post(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullrequests?api-version=7.1",
@@ -175,30 +175,30 @@
 @dataclass
 class PullRequestCommentThread(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/pull-request-thread-comments/list?view=azure-devops-rest-7.1
     Represents a chain of comments on a pull request, with the status e.g. Resolved, Active, etc."""
 
     thread_id: str
     status: str | None
-    comments: list["PullRequestComment"]
+    comments: list[PullRequestComment]
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, Any]) -> "PullRequestCommentThread":
+    def from_request_payload(cls, data: dict[str, Any]) -> PullRequestCommentThread:
         comments = [PullRequestComment.from_request_payload(comment) for comment in data["comments"]]
         return cls(data["id"], data.get("status"), comments)
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, repo_id: str, pull_request_id: str, thread_id: str) -> PullRequestCommentThread:  # type: ignore[override]
         return super().get_by_url(
             ado_client,
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullRequests/{pull_request_id}/threads/{thread_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
-    def create(cls, ado_client: AdoClient, repo_id: str, pull_request_id: str, content: str) -> "PullRequest":  # type: ignore[override]
+    def create(cls, ado_client: AdoClient, repo_id: str, pull_request_id: str, content: str) -> PullRequest:  # type: ignore[override]
         return super().create(
             ado_client,
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullRequests/{pull_request_id}/threads?api-version=7.1",
             {"comments": [{"commentType": 1, "content": content}]},
         )  # type: ignore[return-value]
 
     def update(self, ado_client: AdoClient, attribute_name: PrCommentStatus, attribute_value: Any) -> None:  # type: ignore[override]
@@ -236,12 +236,12 @@
     def __str__(self) -> str:
         return (
             f"PullRequestComment(comment_id={self.comment_id}, author_email=`{self.author.email}`, content=`{self.content}`, "
             f"creation_date={self.creation_date}, comment_type={self.comment_type}{', is_deleted=True' if self.is_deleted else ''})"
         )
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, Any]) -> "PullRequestComment":
+    def from_request_payload(cls, data: dict[str, Any]) -> PullRequestComment:
         author = Member.from_request_payload(data["author"])
         liked_users = [Member.from_request_payload(user) for user in data.get("usersLiked", [])]
         return cls(str(data["id"]), str(data["parentCommentId"]), data.get("content"), author, from_ado_date_string(data["publishedDate"]),
                    data.get("commentType", "regular"), data.get("isDeleted", False), liked_users)  # fmt: skip
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/resources/releases.py` & `ado_wrapper-1.2.5/ado_wrapper/resources/releases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from datetime import datetime
 from dataclasses import dataclass, field
-from typing import Any, Literal, TYPE_CHECKING
+from datetime import datetime
+from typing import TYPE_CHECKING, Any, Literal
 
+from ado_wrapper.resources.users import Member
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.utils import from_ado_date_string
-from ado_wrapper.resources.users import Member
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 ReleaseDefinitionEditableAttribute = Literal["name", "description", "release_name_format", "variable_groups"]
 ReleaseStatus = Literal["active", "abandoned", "draft", "undefined"]
 
@@ -98,15 +98,15 @@
     variable_groups: list[int] | None = field(default_factory=list, repr=False)  # type: ignore[assignment]
     keep_forever: bool = field(default=False, repr=False)
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "Release":
         created_by = Member.from_request_payload(data["createdBy"])
         return cls(str(data["id"]), data["name"], data["status"], from_ado_date_string(data["createdOn"]), created_by, data["description"],
-                   data.get("variables", None), data.get("variableGroups", None), data["keepForever"])  # fmt: skip
+                   data.get("variables"), data.get("variableGroups"), data["keepForever"])  # fmt: skip
 
     @classmethod  # TO-DO: Test
     def get_by_id(cls, ado_client: "AdoClient", release_id: str) -> "Release":
         return super().get_by_url(
             ado_client,
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/releases/{release_id}?api-version=7.1",
         )  # type: ignore[return-value]
@@ -173,15 +173,15 @@
             raise ValueError("No agent pool id has been found! Cannot do this operation!")
         return self._agent_pool_id
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "ReleaseDefinition":
         created_by = Member.from_request_payload(data["createdBy"])
         return cls(str(data["id"]), data["name"], data.get("description") or "", created_by, from_ado_date_string(data["createdOn"]),
-                   data["releaseNameFormat"], data["variableGroups"], data.get("isDeleted", False), data.get("variables", None),
+                   data["releaseNameFormat"], data["variableGroups"], data.get("isDeleted", False), data.get("variables"),
                    data.get("environments", []), data.get("environments", [{"deployPhases": [{"deploymentInput": {"queueId": "1"}}]}]
                             )[0]["deployPhases"][0]["deploymentInput"]["queueId"], data.get("revision", "1"), data)  # fmt: skip
 
     @classmethod
     def get_by_id(cls, ado_client: "AdoClient", release_definition_id: str) -> "ReleaseDefinition":
         return super().get_by_url(
             ado_client,
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/resources/repo.py` & `ado_wrapper-1.2.5/ado_wrapper/resources/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from __future__ import annotations
 
 import io
 import zipfile
 from dataclasses import dataclass, field
-from typing import Any, Literal, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Literal
 
 import requests
 
-from ado_wrapper.state_managed_abc import StateManagedResource
-from ado_wrapper.resources.pull_requests import PullRequest, PullRequestStatus
 from ado_wrapper.resources.commits import Commit
 from ado_wrapper.resources.merge_policies import MergePolicies
+from ado_wrapper.resources.pull_requests import PullRequest, PullRequestStatus
+from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.utils import ResourceNotFound, UnknownError
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
-    from ado_wrapper.resources.merge_policies import MergeBranchPolicy, WhenChangesArePushed
+    from ado_wrapper.resources.merge_policies import (
+        MergeBranchPolicy,
+        WhenChangesArePushed,
+    )
 
 RepoEditableAttribute = Literal["name", "default_branch", "is_disabled"]
 
 # ====================================================================
 
 
 @dataclass
@@ -29,28 +32,28 @@
     repo_id: str = field(metadata={"is_id_field": True})
     name: str = field(metadata={"editable": True})
     default_branch: str = field(default="main", repr=False, metadata={"editable": True, "internal_name": "defaultBranch"})
     is_disabled: bool = field(default=False, repr=False, metadata={"editable": True, "internal_name": "isDisabled"})
     # WARNING, disabling a repo means it's not able to be deleted, proceed with caution.
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, str]) -> "Repo":
+    def from_request_payload(cls, data: dict[str, str]) -> Repo:
         return cls(
             data["id"], data["name"], data.get("defaultBranch", "main").removeprefix("refs/heads/"), bool(data.get("isDisabled", False))
         )
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, repo_id: str) -> "Repo":
+    def get_by_id(cls, ado_client: AdoClient, repo_id: str) -> Repo:
         return super().get_by_url(
             ado_client,
             f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
-    def create(cls, ado_client: AdoClient, name: str, include_readme: bool = True) -> "Repo":  # type: ignore[override]
+    def create(cls, ado_client: AdoClient, name: str, include_readme: bool = True) -> Repo:  # type: ignore[override]
         repo: Repo = super().create(
             ado_client,
             f"/{ado_client.ado_project}/_apis/git/repositories?api-version=7.1",
             {"name": name},
         )  # type: ignore[assignment]
         if include_readme:
             Commit.add_initial_readme(ado_client, repo.repo_id)
@@ -71,26 +74,26 @@
         return super().delete_by_id(
             ado_client,
             f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}?api-version=7.1",
             repo_id,
         )
 
     @classmethod
-    def get_all(cls, ado_client: AdoClient) -> list["Repo"]:  # type: ignore[override]
+    def get_all(cls, ado_client: AdoClient) -> list[Repo]:  # type: ignore[override]
         return super().get_all(
             ado_client,
             f"/{ado_client.ado_project}/_apis/git/repositories?api-version=7.1",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
-    def get_by_name(cls, ado_client: AdoClient, repo_name: str) -> "Repo | None":  # type: ignore[return]
+    def get_by_name(cls, ado_client: AdoClient, repo_name: str) -> Repo | None:  # type: ignore[return]
         """Warning, this function must fetch `all` repos to work, be cautious when calling it in a loop."""
         for repo in cls.get_all(ado_client):
             if repo.name == repo_name:
                 return repo
 
     def get_file(self, ado_client: AdoClient, file_path: str, branch_name: str = "main") -> str:
         request = ado_client.session.get(
@@ -135,20 +138,20 @@
         except zipfile.BadZipFile as e:
             print(f"{self.name} ({self.repo_id}) couldn't be unzipped:", e)
 
         bytes_io.close()
         # =========== That's all I have to say ==================
         return files
 
-    def create_pull_request(self, ado_client: AdoClient, branch_name: str, pull_request_title: str, pull_request_description: str) -> "PullRequest":  # fmt: skip
+    def create_pull_request(self, ado_client: AdoClient, branch_name: str, pull_request_title: str, pull_request_description: str) -> PullRequest:  # fmt: skip
         """Helper function which redirects to the PullRequest class to make a PR"""
         return PullRequest.create(ado_client, self.repo_id, branch_name, pull_request_title, pull_request_description)
 
     @staticmethod
-    def get_all_pull_requests(ado_client: AdoClient, repo_id: str, status: PullRequestStatus = "all") -> list["PullRequest"]:
+    def get_all_pull_requests(ado_client: AdoClient, repo_id: str, status: PullRequestStatus = "all") -> list[PullRequest]:
         return PullRequest.get_all_by_repo_id(ado_client, repo_id, status)
 
     def delete(self, ado_client: AdoClient) -> None:
         if self.is_disabled:
             self.update(ado_client, "is_disabled", False)
         self.delete_by_id(ado_client, self.repo_id)
 
@@ -156,21 +159,21 @@
     def get_content_static(
         ado_client: AdoClient, repo_id: str, file_types: list[str] | None = None, branch_name: str = "main"
     ) -> dict[str, str]:
         repo = Repo.get_by_id(ado_client, repo_id)
         return repo.get_contents(ado_client, file_types, branch_name)
 
     @staticmethod
-    def get_branch_merge_policy(ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> "MergeBranchPolicy | None":
+    def get_branch_merge_policy(ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> MergeBranchPolicy | None:
         return MergePolicies.get_branch_policy(ado_client, repo_id, branch_name)
 
     @staticmethod
     def set_branch_merge_policy(ado_client: AdoClient, repo_id: str, minimum_approver_count: int,
                           creator_vote_counts: bool, prohibit_last_pushers_vote: bool, allow_completion_with_rejects: bool,
-                          when_new_changes_are_pushed: WhenChangesArePushed, branch_name: str = "main") -> "MergePolicies | None":  # fmt: skip
+                          when_new_changes_are_pushed: WhenChangesArePushed, branch_name: str = "main") -> MergePolicies | None:  # fmt: skip
         return MergePolicies.set_branch_policy(ado_client, repo_id, minimum_approver_count, creator_vote_counts,
                                                prohibit_last_pushers_vote, allow_completion_with_rejects, when_new_changes_are_pushed,
                                                branch_name)  # fmt: skip
 
 
 # ====================================================================
 
@@ -180,19 +183,19 @@
     build_repository_id: str = field(metadata={"is_id_field": True})
     name: str | None = None
     type: str = "TfsGit"
     clean: bool | None = None
     checkout_submodules: bool = field(default=False, metadata={"internal_name": "checkoutSubmodules"})
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, str | bool]) -> "BuildRepository":
+    def from_request_payload(cls, data: dict[str, str | bool]) -> BuildRepository:
         return cls(data["id"], data.get("name"), data.get("type", "TfsGit"), data.get("clean"), data.get("checkoutSubmodules", False))  # type: ignore[arg-type]
 
     @classmethod
-    def from_json(cls, data: dict[str, str | bool]) -> "BuildRepository":
+    def from_json(cls, data: dict[str, str | bool]) -> BuildRepository:
         return cls(data["id"], data.get("name"), data.get("type", "TfsGit"), data.get("clean"), data.get("checkoutSubmodules", False))  # type: ignore[arg-type]
 
     def to_json(self) -> dict[str, str | bool | None]:
         return {
             "id": self.build_repository_id, "name": self.name, "type": self.type,
             "clean": self.clean, "checkoutSubmodules": self.checkout_submodules,  # fmt: skip
         }
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/resources/service_endpoint.py` & `ado_wrapper-1.2.5/ado_wrapper/resources/service_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Any, Literal, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Literal
 
-from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import Member
+from ado_wrapper.state_managed_abc import StateManagedResource
+from ado_wrapper.utils import requires_initialisation
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 ServiceEndpointEditableAttribute = Literal["name"]
 
 
@@ -40,37 +41,29 @@
             Member.from_request_payload(data["createdBy"]),
             data.get("description", ""), data["authorization"], data["isShared"],
             data["isOutdated"], data["isReady"], data["owner"],
             data["serviceEndpointProjectReferences"],  # fmt: skip
         )
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, repo_id: str) -> "ServiceEndpoint":
+    def get_by_id(cls, ado_client: AdoClient, repo_id: str) -> ServiceEndpoint:
         return super().get_by_url(
             ado_client,
             f"/{ado_client.ado_project}/_apis/serviceendpoint/endpoints/{repo_id}",
         )  # type: ignore[return-value]
 
     @classmethod
     def create(cls, ado_client: AdoClient, name: str, service_endpoint_type: str, url: str,  # type: ignore[override]
                username: str = "", password: str = "",  access_token: str = "") -> ServiceEndpoint:  # fmt: skip
         """Creates a service endpoint, pass in either username and password or access_token."""
         assert ((username and password) and not access_token) or (access_token and not (username and password)), "Either username and password or access_token must be passed in."  # fmt: skip
+        requires_initialisation(ado_client)
         payload = {
-            "name": name,
-            "type": service_endpoint_type,
-            "url": url,
-            "isShared": True,
-            "isReady": True,
-            "serviceEndpointProjectReferences": [
-                {
-                    "projectReference": {"id": ado_client.ado_project_id},  # fmt: skip
-                    "name": name,
-                }
-            ],
+            "name": name, "type": service_endpoint_type, "url": url, "isShared": True, "isReady": True,
+            "serviceEndpointProjectReferences": [{"projectReference": {"id": ado_client.ado_project_id}}],  # fmt: skip
         }
         if username and password:
             payload["authorization"] = {"scheme": "UsernamePassword", "parameters": {"Username": username, "Password": password}}
         elif access_token:
             payload["authorization"] = {"parameters": {"AccessToken": access_token}, "scheme": "Token"}
         return super().create(
             ado_client, "/_apis/serviceendpoint/endpoints?api-version=7.1", payload,  # fmt: skip
@@ -83,22 +76,23 @@
         #     ado_client, "put",
         #     f"_apis/serviceendpoint/endpoints/{self.service_endpoint_id}?api-version=7.1",
         #     attribute_name, attribute_value, self._raw_data,  # fmt: skip
         # )
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, service_endpoint_id: str) -> None:  # type: ignore[override]
+        requires_initialisation(ado_client)
         return super().delete_by_id(
             ado_client,
             f"/_apis/serviceendpoint/endpoints/{service_endpoint_id}?projectIds={ado_client.ado_project_id}&api-version=7.1",
             service_endpoint_id,
         )
 
     @classmethod
-    def get_all(cls, ado_client: AdoClient) -> list["ServiceEndpoint"]:  # type: ignore[override]
+    def get_all(cls, ado_client: AdoClient) -> list[ServiceEndpoint]:  # type: ignore[override]
         return super().get_all(
             ado_client,
             f"/{ado_client.ado_project}/_apis/serviceendpoint/endpoints?api-version=7.1",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/resources/teams.py` & `ado_wrapper-1.2.5/ado_wrapper/resources/teams.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
 from dataclasses import dataclass, field
+from typing import TYPE_CHECKING
 
-from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import TeamMember
+from ado_wrapper.state_managed_abc import StateManagedResource
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 
 @dataclass
 class Team(StateManagedResource):
@@ -20,55 +20,55 @@
     description: str
     team_members: list[TeamMember] = field(default_factory=list)
 
     def __str__(self) -> str:
         return f"{self.name} ({self.team_id}" + (", ".join([str(member) for member in self.team_members])) + ")"
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, str]) -> "Team":
+    def from_request_payload(cls, data: dict[str, str]) -> Team:
         return cls(data["id"], data["name"], data.get("description", ""), [])
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, team_id: str) -> "Team":
+    def get_by_id(cls, ado_client: AdoClient, team_id: str) -> Team:
         resource: Team = super().get_by_url(
             ado_client,
             f"/_apis/projects/{ado_client.ado_project}/teams/{team_id}?$expandIdentity={True}&api-version=7.1-preview.1",
         )  # type: ignore[assignment]
         resource.team_members = resource.get_members(ado_client)
         return resource
 
     @classmethod
-    def create(cls, ado_client: AdoClient, name: str, description: str) -> "Team":  # type: ignore[override]
+    def create(cls, ado_client: AdoClient, name: str, description: str) -> Team:  # type: ignore[override]
         raise NotImplementedError
         # request = ado_client.session.post(f"/_apis/teams?api-version=7.1", json={"name": name, "description": description}).json()
         # return cls.from_request_payload(request)
 
     def update(self, ado_client: AdoClient, attribute_name: str, attribute_value: str) -> None:  # type: ignore[override]
         raise NotImplementedError
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, team_id: str) -> None:  # type: ignore[override]
         raise NotImplementedError
 
     @classmethod
-    def get_all(cls, ado_client: AdoClient) -> list["Team"]:  # type: ignore[override]
+    def get_all(cls, ado_client: AdoClient) -> list[Team]:  # type: ignore[override]
         return super().get_all(
             ado_client,
             "/_apis/teams?api-version=7.1-preview.2",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
-    def get_by_name(cls, ado_client: AdoClient, team_name: str) -> "Team | None":
+    def get_by_name(cls, ado_client: AdoClient, team_name: str) -> Team | None:
         return cls.get_by_abstract_filter(ado_client, lambda team: team.name == team_name)  # type: ignore[return-value, attr-defined]
 
-    def get_members(self, ado_client: AdoClient) -> list["TeamMember"]:
+    def get_members(self, ado_client: AdoClient) -> list[TeamMember]:
         request = ado_client.session.get(
             f"https://dev.azure.com/{ado_client.ado_org}/_apis/projects/{ado_client.ado_project}/teams/{self.team_id}/members?api-version=7.1-preview.2",
         ).json()
         if "value" not in request and request.get("message", "").startswith("The team with id "):  # If the team doesn't exist anymore.
             return []
         team_members = [TeamMember.from_request_payload(member) for member in request["value"]]
         self.team_members = team_members
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/resources/users.py` & `ado_wrapper-1.2.5/ado_wrapper/resources/users.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
-from typing import Literal, Any, TYPE_CHECKING
 from dataclasses import dataclass, field
+from typing import TYPE_CHECKING, Any, Literal
 
 from ado_wrapper.state_managed_abc import StateManagedResource
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 VOTE_ID_TO_TYPE = {
@@ -29,59 +29,59 @@
     email: str
     origin: str
     origin_id: str  # DON'T USE THIS, USE `descriptor_id` INSTEAD
     # "subjectKind": "user",
     # "metaType": "member",
     # "directoryAlias": "MiryabblliS",
     # "domain": "68283f3b-8487-4c86-adb3-a5228f18b893",
-    # "url": "https://vssps.dev.azure.com/vfuk-digital/_apis/Graph/Users/aad.M2Q5NDlkZTgtZDI2Yi03MGQ3LWEyYjItMDAwYTQzYTdlNzFi",
+    # "url": "https://vssps.dev.azure.com/{ado_client.}/_apis/Graph/Users/aad.M2Q5NDlkZTgtZDI2Yi03MGQ3LWEyYjItMDAwYTQzYTdlNzFi",
 
     def __str__(self) -> str:
         return f"{self.display_name} ({self.email})"
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, str]) -> "AdoUser":
+    def from_request_payload(cls, data: dict[str, str]) -> AdoUser:
         return cls(data["descriptor"], data["displayName"], data["mailAddress"].removeprefix("vstfs:///Classification/TeamProject/"),
                    data["origin"], data["originId"])  # fmt: skip
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, descriptor_id: str) -> "AdoUser":
+    def get_by_id(cls, ado_client: AdoClient, descriptor_id: str) -> AdoUser:
         return super().get_by_url(
             ado_client,  # Preview required
             f"https://vssps.dev.azure.com/{ado_client.ado_org}/_apis/graph/users/{descriptor_id}?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
 
     @classmethod
-    def create(cls, ado_client: AdoClient, member_name: str, member_email: str) -> "AdoUser":  # type: ignore[override]
+    def create(cls, ado_client: AdoClient, member_name: str, member_email: str) -> AdoUser:  # type: ignore[override]
         raise NotImplementedError("Creating a new user is not supported")
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, member_id: str) -> None:  # type: ignore[override]
         raise NotImplementedError("Deleting a user is not supported")
 
     @classmethod
-    def get_all(cls, ado_client: AdoClient) -> list["AdoUser"]:  # type: ignore[override]
+    def get_all(cls, ado_client: AdoClient) -> list[AdoUser]:  # type: ignore[override]
         return super().get_all(
             ado_client,  # Preview required
             f"https://vssps.dev.azure.com/{ado_client.ado_org}/_apis/graph/users?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
-    def get_by_email(cls, ado_client: AdoClient, member_email: str) -> "AdoUser":
+    def get_by_email(cls, ado_client: AdoClient, member_email: str) -> AdoUser:
         user: AdoUser = cls.get_by_abstract_filter(ado_client, lambda user: user.email == member_email)  # type: ignore[attr-defined, assignment]
         if user is None:
             raise ValueError(f"Member with email {member_email} not found")
         return user
 
     @classmethod
-    def get_by_name(cls, ado_client: AdoClient, member_name: str) -> "AdoUser | None":
+    def get_by_name(cls, ado_client: AdoClient, member_name: str) -> AdoUser | None:
         return cls.get_by_abstract_filter(ado_client, lambda user: user.display_name == member_name)  # type: ignore[return-value, attr-defined]
 
 
 # ======================================================================================================= #
 # ------------------------------------------------------------------------------------------------------- #
 # ======================================================================================================= #
 
@@ -91,26 +91,26 @@
     """A stripped down member class which is often returned by the API, for example in build requests or PRs."""
 
     name: str
     email: str
     member_id: str = field(metadata={"is_id_field": True}, repr=False)
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, Any]) -> "Member":
+    def from_request_payload(cls, data: dict[str, Any]) -> Member:
         # displayName, uniqueName/mailAddress, id/originId
         # This gets returned slightly differently from different APIs
         return cls(data["displayName"], data.get("uniqueName") or data.get("mailAddress", "UNKNOWN"),  # type: ignore[arg-type]
                    data.get("id") or data["originId"])  # fmt: skip
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, member_id: str) -> "Member":
+    def get_by_id(cls, ado_client: AdoClient, member_id: str) -> Member:
         raise NotImplementedError("Getting a member by ID is not supported")
 
     @classmethod
-    def create(cls, ado_client: AdoClient, member_name: str, member_email: str) -> "Member":  # type: ignore[override]
+    def create(cls, ado_client: AdoClient, member_name: str, member_email: str) -> Member:  # type: ignore[override]
         raise NotImplementedError("Creating a new member is not supported")
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, member_id: str) -> None:  # type: ignore[override]
         raise NotImplementedError("Deleting a member is not supported")
 
 
@@ -129,27 +129,27 @@
     def __str__(self) -> str:
         return f"{super().__str__()}" + (" (Team Admin)" if self.is_team_admin else "")
 
     def __repr__(self) -> str:
         return f"{super().__str__().removesuffix(')')}, team_admin={self.is_team_admin})"
 
     @classmethod
-    def from_json(cls, data: dict[str, Any]) -> "TeamMember":
+    def from_json(cls, data: dict[str, Any]) -> TeamMember:
         return cls(data["name"], data["email"], data["id"], data["is_team_admin"])
 
     def to_json(self) -> dict[str, Any]:
         return {
             "name": self.name,
             "email": self.email,
             "id": self.member_id,
             "is_team_admin": self.is_team_admin,
         }
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, Any]) -> "TeamMember":
+    def from_request_payload(cls, data: dict[str, Any]) -> TeamMember:
         return cls(data["identity"]["displayName"], data["identity"]["uniqueName"], data["identity"]["id"], data.get("isTeamAdmin", False))
 
 
 # ======================================================================================================= #
 # ------------------------------------------------------------------------------------------------------- #
 # ======================================================================================================= #
 
@@ -174,16 +174,16 @@
             "email": self.email,
             "id": self.member_id,
             "vote": self.vote,
             "is_required": self.is_required,
         }
 
     @classmethod
-    def from_json(cls, data: dict[str, Any]) -> "Reviewer":
+    def from_json(cls, data: dict[str, Any]) -> Reviewer:
         return cls(data["name"], data["email"], data["id"], data["vote"], data["isRequired"])
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, Any]) -> "Reviewer":
+    def from_request_payload(cls, data: dict[str, Any]) -> Reviewer:
         return cls(data["displayName"], data["uniqueName"], data["id"], data["vote"], data.get("isRequired", False))
 
 
 # ======================================================================================================= #
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-1.2.5/ado_wrapper/resources/variable_groups.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
-from datetime import datetime
-from typing import Any, TYPE_CHECKING, Literal
 from dataclasses import dataclass, field
+from datetime import datetime
+from typing import TYPE_CHECKING, Any, Literal
 
-from ado_wrapper.utils import from_ado_date_string
-from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import Member
+from ado_wrapper.state_managed_abc import StateManagedResource
+from ado_wrapper.utils import from_ado_date_string, requires_initialisation
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 VariableGroupEditableAttribute = Literal["variables"]
 
 
@@ -24,79 +24,79 @@
     variables: dict[str, str] = field(metadata={"editable": True})
     created_on: datetime
     created_by: Member
     modified_by: Member
     modified_on: datetime | None = None
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, Any]) -> "VariableGroup":
+    def from_request_payload(cls, data: dict[str, Any]) -> VariableGroup:
         # print("\n", data)
         created_by = Member.from_request_payload(data["createdBy"])
         modified_by = Member.from_request_payload(data["modifiedBy"])
         return cls(str(data["id"]), data["name"], data.get("description", ""),
                    {key: value["value"] if isinstance(value, dict) else value for key, value in data["variables"].items()},
                    from_ado_date_string(data["createdOn"]), created_by, modified_by, from_ado_date_string(data.get("modifiedOn")))  # fmt: skip
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, variable_group_id: str) -> "VariableGroup":
+    def get_by_id(cls, ado_client: AdoClient, variable_group_id: str) -> VariableGroup:
         return super().get_by_url(
             ado_client,
             f"/{ado_client.ado_project}/_apis/distributedtask/variablegroups/{variable_group_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def create(  # type: ignore[override]
         cls, ado_client: AdoClient, variable_group_name: str, variable_group_description: str, variables: dict[str, str]  # fmt: skip
-    ) -> "VariableGroup":
+    ) -> VariableGroup:
         payload = {
             "name": variable_group_name,
-            "description": variable_group_description,
             "variables": variables,
             "type": "Vsts",
             "variableGroupProjectReferences": [
                 {
                     "description": variable_group_description,
                     "name": variable_group_name,
-                    "projectReference": {"id": ado_client.ado_project_id, "name": ado_client.ado_project},
+                    "projectReference": {"name": ado_client.ado_project},
                 }
             ],
         }
         return super().create(
             ado_client,
             f"/{ado_client.ado_project}/_apis/distributedtask/variablegroups?api-version=7.1",
             payload,
         )  # type: ignore[return-value]
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, variable_group_id: str) -> None:  # type: ignore[override]
+        requires_initialisation(ado_client)
         return super().delete_by_id(
             ado_client,
             f"/_apis/distributedtask/variablegroups/{variable_group_id}?projectIds={ado_client.ado_project_id}&api-version=7.1",
             variable_group_id,
         )
 
     def update(self, ado_client: AdoClient, attribute_name: VariableGroupEditableAttribute, attribute_value: Any) -> None:  # type: ignore[override]
         # WARNING: This method works 80-90% of the time, for some reason, it fails randomly, ADO API is at fault.
         params = {
-            "variableGroupProjectReferences": [{"name": self.name, "projectReference": {"id": ado_client.ado_project_id}}],
-             "id": self.variable_group_id, "name": self.name, "type": "Vsts", "variables": self.variables  # fmt: skip
+            "variableGroupProjectReferences": [{"name": self.name, "projectReference": {"name": ado_client.ado_project}}],
+            "name": self.name, "variables": self.variables  # fmt: skip
         }
         super().update(
             ado_client, "put",
             f"/_apis/distributedtask/variablegroups/{self.variable_group_id}?api-version=7.1",
             attribute_name, attribute_value, params  # fmt: skip
         )
 
     @classmethod
-    def get_all(cls, ado_client: AdoClient) -> list["VariableGroup"]:  # type: ignore[override]
+    def get_all(cls, ado_client: AdoClient) -> list[VariableGroup]:  # type: ignore[override]
         return super().get_all(
             ado_client,
             f"/{ado_client.ado_project}/_apis/distributedtask/variablegroups?api-version=7.1",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
-    def get_by_name(cls, ado_client: AdoClient, name: str) -> "VariableGroup | None":
+    def get_by_name(cls, ado_client: AdoClient, name: str) -> VariableGroup | None:
         return cls.get_by_abstract_filter(ado_client, lambda variable_group: variable_group.name == name)  # type: ignore[return-value, attr-defined]
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/state_managed_abc.py` & `ado_wrapper-1.2.5/ado_wrapper/state_managed_abc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Any, TYPE_CHECKING, Literal, Callable
 from dataclasses import dataclass, fields
 from datetime import datetime
+from typing import TYPE_CHECKING, Any, Callable, Literal
 
+from ado_wrapper.plan_resources.plan_resource import PlannedStateManagedResource
 from ado_wrapper.utils import (
-    get_resource_variables, extract_id, get_internal_field_names,
-    ResourceAlreadyExists, DeletionFailed, ResourceNotFound, UpdateFailed,  # fmt: skip
+    DeletionFailed, ResourceAlreadyExists, ResourceNotFound, UpdateFailed,
+    extract_id, get_internal_field_names, get_resource_variables,  # fmt: skip
 )
-from ado_wrapper.plan_resources.plan_resource import PlannedStateManagedResource
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 
 def recursively_convert_to_json(attribute_name: str, attribute_value: Any) -> tuple[str, Any]:
     if isinstance(attribute_value, dict):
@@ -52,15 +52,15 @@
     def from_json(cls, data: dict[str, Any]) -> "StateManagedResource":
         return cls(**recursively_convert_from_json(data))
 
     def to_json(self) -> dict[str, Any]:
         attribute_names = [field_obj.name for field_obj in fields(self)]
         attribute_values = [getattr(self, field_obj.name) for field_obj in fields(self)]
         combined = zip(attribute_names, attribute_values)
-        return dict(recursively_convert_to_json(attribute_name, attribute_value) for attribute_name, attribute_value in combined)  ####
+        return dict(recursively_convert_to_json(attribute_name, attribute_value) for attribute_name, attribute_value in combined)
 
     @classmethod
     def get_by_id(cls, ado_client: "AdoClient", resource_id: str) -> "StateManagedResource":
         raise NotImplementedError
 
     @classmethod
     def get_by_url(cls, ado_client: "AdoClient", url: str) -> "StateManagedResource":
@@ -76,14 +76,18 @@
         return cls.from_request_payload(request.json())
 
     @classmethod
     def create(
         cls, ado_client: "AdoClient", url: str, payload: dict[str, Any] | None = None, refetch: bool = False
     ) -> "StateManagedResource | PlannedStateManagedResource":
         """When creating, often the response doesn't contain all the data, refetching does a .get_by_id() after creation."""
+        # If it already exists:
+        # if cls.get_by_id(ado_client, extract_unique_name(payload)):
+        #     raise ResourceAlreadyExists(f"The {cls.__name__} with that identifier already exist!")
+        #     <update the resource>
         if ado_client.plan_mode:
             return PlannedStateManagedResource.create(cls, ado_client, url, payload)
         if not url.startswith("https://"):
             url = f"https://dev.azure.com/{ado_client.ado_org}" + url
         request = ado_client.session.post(url, json=payload or {})  # Create a brand new dict
         if request.status_code >= 300:
             if request.status_code == 401:
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/state_manager.py` & `ado_wrapper-1.2.5/ado_wrapper/state_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import json
-from pathlib import Path
 from datetime import datetime
+from pathlib import Path
+from typing import TYPE_CHECKING, Any, Literal, TypedDict
 from uuid import uuid4
-from typing import Any, TypedDict, TYPE_CHECKING, Literal
 
-from ado_wrapper.utils import DeletionFailed, get_resource_variables, ResourceType
+from ado_wrapper.utils import DeletionFailed, ResourceType, get_resource_variables
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 STATE_FILE_VERSION = "1.6"
 
 
 class StateFileType(TypedDict):
     state_file_version: str
     resources: dict[ResourceType, dict[str, Any]]
 
 
 EMPTY_STATE: StateFileType = {
     "state_file_version": STATE_FILE_VERSION,
-    "resources": {resource: {} for resource in get_resource_variables().keys()},  # type: ignore[misc]
+    "resources": {resource: {} for resource in get_resource_variables()},  # type: ignore[misc]
 }
 
 
 class StateManager:
     def __init__(self, ado_client: "AdoClient", state_file_name: str | None = "main.state") -> None:
         self.ado_client = ado_client
         self.state_file_name = state_file_name
@@ -34,15 +34,15 @@
             self.wipe_state()  # Will automatically create the file
 
         self.state: StateFileType = self.load_state() if self.state_file_name is not None else EMPTY_STATE
 
     def load_state(self) -> StateFileType:
         if self.state_file_name is None:
             return self.state
-        with open(self.state_file_name, "r", encoding="utf-8") as state_file:
+        with open(self.state_file_name, encoding="utf-8") as state_file:
             try:
                 return json.load(state_file)  # type: ignore[no-any-return]
             except json.JSONDecodeError as exc:
                 raise json.JSONDecodeError("State file is not valid JSON, it might have been corrupted?", exc.doc, exc.pos)
 
     def write_state_file(self, state_data: StateFileType) -> None:
         if self.state_file_name is None:
@@ -124,15 +124,17 @@
             for resource_id in all_states["resources"][resource_type]:
                 instance = ALL_RESOURCES[resource_type].get_by_id(self.ado_client, resource_id)
                 if instance.to_json() != all_states["resources"][resource_type][resource_id]["data"]:
                     all_states["resources"][resource_type][resource_id]["data"] = instance.to_json()
         return all_states
 
     def load_all_resources_with_prefix_into_state(self, prefix: str) -> None:
-        from ado_wrapper.resources import VariableGroup, Repo, ReleaseDefinition, BuildDefinition, ServiceEndpoint  # type: ignore[attr-defined]
+        from ado_wrapper.resources import (  # type: ignore[attr-defined]
+            BuildDefinition, ReleaseDefinition, Repo, ServiceEndpoint, VariableGroup,  # fmt: skip
+        )
 
         for repo in Repo.get_all(self.ado_client):
             if repo.name.startswith(prefix):
                 self.ado_client.state_manager.import_into_state("Repo", repo.repo_id)
 
         for variable_group in VariableGroup.get_all(self.ado_client):
             if variable_group.name.startswith(prefix):
@@ -145,13 +147,7 @@
         for build_definition in BuildDefinition.get_all(self.ado_client):
             if build_definition.name.startswith(prefix):
                 self.ado_client.state_manager.import_into_state("BuildDefinition", build_definition.build_definition_id)
 
         for service_endpoint in ServiceEndpoint.get_all(self.ado_client):
             if service_endpoint.name.startswith(prefix):
                 self.ado_client.state_manager.import_into_state("ServiceEndpoint", service_endpoint.service_endpoint_id)
-
-    # Unused
-    # def all_resources(self) -> Generator[tuple[ResourceType, str], None, None]:
-    #     for resource_type in self.load_state()["resources"]:
-    #         for resource_id in self.load_state()["resources"][resource_type]:
-    #             yield resource_type, resource_id
```

### Comparing `ado_wrapper-1.2.3/ado_wrapper/utils.py` & `ado_wrapper-1.2.5/ado_wrapper/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from datetime import datetime, timezone
-from typing import overload, TYPE_CHECKING, Literal
 from dataclasses import fields
+from datetime import datetime, timezone
+from typing import TYPE_CHECKING, Literal, overload
 
 if TYPE_CHECKING:
     from ado_wrapper.state_managed_abc import StateManagedResource
+    from ado_wrapper.client import AdoClient
 
 
 @overload
 def from_ado_date_string(date_string: str) -> datetime:
     ...
 
 
@@ -116,14 +117,23 @@
     pass
 
 
 class AuthenticationError(Exception):
     pass
 
 
+class ConfigurationError(Exception):
+    pass
+
+
+def requires_initialisation(ado_client: "AdoClient"):
+    if not ado_client.ado_project_id:
+        raise ConfigurationError("The client has not been initialised. Please disable `bypass_initialisation` method before using this function.")
+
+
 def get_resource_variables() -> dict[str, type["StateManagedResource"]]:  # We do this to avoid circular imports
     """This returns a mapping of resource name (str) to the class type of the resource. This is used to dynamically create instances of resources."""
     from ado_wrapper.resources import (  # type: ignore[attr-defined]  # pylint: disable=possibly-unused-variable
         AnnotatedTag, Branch, Build, BuildDefinition, Commit, Environment, Group, MergePolicies, MergeBranchPolicy,
         MergePolicyDefaultReviewer, Project, PullRequest, Release, ReleaseDefinition, Repo, BuildRepository, Team,
         AdoUser, Member, ServiceEndpoint, Reviewer, VariableGroup,  # fmt: skip
     )
```

### Comparing `ado_wrapper-1.2.3/PKG-INFO` & `ado_wrapper-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 1.2.3
+Version: 1.2.5
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

