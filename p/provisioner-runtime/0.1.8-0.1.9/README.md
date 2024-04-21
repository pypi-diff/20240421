# Comparing `tmp/provisioner_runtime-0.1.8-py3-none-any.whl.zip` & `tmp/provisioner_runtime-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 131179 bytes, number of entries: 152
+Zip file size: 130703 bytes, number of entries: 152
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 external/ansible_playbooks/__init__.py
 -rwxr-xr-x  2.0 unx      368 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/apt_update_upgrade.yaml
 -rwxr-xr-x  2.0 unx     5549 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/common/shell_lib.sh
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/group_vars/all
 -rwxr-xr-x  2.0 unx      678 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/reboot.yaml
 -rwxr-xr-x  2.0 unx      353 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/roles/anchor/defaults/main.yaml
 -rwxr-xr-x  2.0 unx    10424 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/roles/anchor/files/anchor_run.sh
@@ -87,23 +87,23 @@
 -rwxr-xr-x  2.0 unx     1668 b- defN 80-Jan-01 00:00 provisioner/main.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/resources/__init__.py
 -rw-r--r--  2.0 unx       26 b- defN 80-Jan-01 00:00 provisioner/resources/config.yaml
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 provisioner/resources/version.txt
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/runner/__init__.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/__init__.py
 -rwxr-xr-x  2.0 unx     1228 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/ansible_fakes.py
--rw-r--r--  2.0 unx    16182 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/ansible_runner.py
+-rw-r--r--  2.0 unx    16236 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/ansible_runner.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/resources/__init__.py
 -rwxr-xr-x  2.0 unx     1957 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/resources/ansible.cfg
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/resources/callback_plugins/__init__.py
 -rwxr-xr-x  2.0 unx     5455 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/resources/callback_plugins/custom_yaml.py
 -rwxr-xr-x  2.0 unx     1081 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/resources/callback_plugins/fail_on_missing_hosts.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/shared/__init__.py
--rwxr-xr-x  2.0 unx     5942 b- defN 80-Jan-01 00:00 provisioner/shared/collaborators.py
--rwxr-xr-x  2.0 unx     7806 b- defN 80-Jan-01 00:00 provisioner/shared/collaborators_fakes.py
+-rwxr-xr-x  2.0 unx     5988 b- defN 80-Jan-01 00:00 provisioner/shared/collaborators.py
+-rwxr-xr-x  2.0 unx     7810 b- defN 80-Jan-01 00:00 provisioner/shared/collaborators_fakes.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/test_data/__init__.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/test_data/ansible/__init__.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/test_data/ansible/playbooks/__init__.py
 -rw-r--r--  2.0 unx     2668 b- defN 80-Jan-01 00:00 provisioner/test_data/domain.py
 -rwxr-xr-x  2.0 unx      256 b- defN 80-Jan-01 00:00 provisioner/test_data/internal_config.yaml
 -rwxr-xr-x  2.0 unx      180 b- defN 80-Jan-01 00:00 provisioner/test_data/user_config.yaml
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/test_lib/__init__.py
@@ -116,18 +116,18 @@
 -rwxr-xr-x  2.0 unx      184 b- defN 80-Jan-01 00:00 provisioner/utils/browser.py
 -rwxr-xr-x  2.0 unx     1057 b- defN 80-Jan-01 00:00 provisioner/utils/checks.py
 -rwxr-xr-x  2.0 unx      931 b- defN 80-Jan-01 00:00 provisioner/utils/checks_fakes.py
 -rwxr-xr-x  2.0 unx     2268 b- defN 80-Jan-01 00:00 provisioner/utils/github.py
 -rwxr-xr-x  2.0 unx     4589 b- defN 80-Jan-01 00:00 provisioner/utils/github_fakes.py
 -rwxr-xr-x  2.0 unx     1955 b- defN 80-Jan-01 00:00 provisioner/utils/hosts_file.py
 -rwxr-xr-x  2.0 unx      949 b- defN 80-Jan-01 00:00 provisioner/utils/hosts_file_fakes.py
--rwxr-xr-x  2.0 unx     6136 b- defN 80-Jan-01 00:00 provisioner/utils/httpclient.py
--rwxr-xr-x  2.0 unx     1807 b- defN 80-Jan-01 00:00 provisioner/utils/httpclient_fakes.py
+-rwxr-xr-x  2.0 unx     6551 b- defN 80-Jan-01 00:00 provisioner/utils/httpclient.py
+-rwxr-xr-x  2.0 unx     1832 b- defN 80-Jan-01 00:00 provisioner/utils/httpclient_fakes.py
 -rwxr-xr-x  2.0 unx     7052 b- defN 80-Jan-01 00:00 provisioner/utils/io_utils.py
--rwxr-xr-x  2.0 unx     5893 b- defN 80-Jan-01 00:00 provisioner/utils/io_utils_fakes.py
+-rwxr-xr-x  2.0 unx     3888 b- defN 80-Jan-01 00:00 provisioner/utils/io_utils_fakes.py
 -rwxr-xr-x  2.0 unx     2130 b- defN 80-Jan-01 00:00 provisioner/utils/json_util.py
 -rwxr-xr-x  2.0 unx     4259 b- defN 80-Jan-01 00:00 provisioner/utils/network.py
 -rwxr-xr-x  2.0 unx      929 b- defN 80-Jan-01 00:00 provisioner/utils/network_fakes.py
 -rwxr-xr-x  2.0 unx     2043 b- defN 80-Jan-01 00:00 provisioner/utils/os.py
 -rwxr-xr-x  2.0 unx     4204 b- defN 80-Jan-01 00:00 provisioner/utils/package_loader.py
 -rwxr-xr-x  2.0 unx     5034 b- defN 80-Jan-01 00:00 provisioner/utils/paths.py
 -rwxr-xr-x  2.0 unx     2444 b- defN 80-Jan-01 00:00 provisioner/utils/paths_fakes.py
@@ -142,13 +142,13 @@
 -rwxr-xr-x  2.0 unx     8629 b- defN 80-Jan-01 00:00 provisioner/utils/prompter.py
 -rwxr-xr-x  2.0 unx     2400 b- defN 80-Jan-01 00:00 provisioner/utils/prompter_fakes.py
 -rwxr-xr-x  2.0 unx     2165 b- defN 80-Jan-01 00:00 provisioner/utils/properties.py
 -rwxr-xr-x  2.0 unx     1310 b- defN 80-Jan-01 00:00 provisioner/utils/properties_fakes.py
 -rwxr-xr-x  2.0 unx     2080 b- defN 80-Jan-01 00:00 provisioner/utils/summary.py
 -rwxr-xr-x  2.0 unx     1401 b- defN 80-Jan-01 00:00 provisioner/utils/summary_fakes.py
 -rwxr-xr-x  2.0 unx     2598 b- defN 80-Jan-01 00:00 provisioner/utils/yaml_util.py
--rw-r--r--  2.0 unx     1071 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      792 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.8.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    15772 b- defN 16-Jan-01 00:00 provisioner_runtime-0.1.8.dist-info/RECORD
-152 files, 339229 bytes uncompressed, 105037 bytes compressed:  69.0%
+-rw-r--r--  2.0 unx     1071 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      792 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.9.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    15772 b- defN 16-Jan-01 00:00 provisioner_runtime-0.1.9.dist-info/RECORD
+152 files, 337768 bytes uncompressed, 104561 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -435,23 +435,23 @@
 
 Filename: provisioner/utils/summary_fakes.py
 Comment: 
 
 Filename: provisioner/utils/yaml_util.py
 Comment: 
 
-Filename: provisioner_runtime-0.1.8.dist-info/LICENSE
+Filename: provisioner_runtime-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: provisioner_runtime-0.1.8.dist-info/METADATA
+Filename: provisioner_runtime-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: provisioner_runtime-0.1.8.dist-info/WHEEL
+Filename: provisioner_runtime-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: provisioner_runtime-0.1.8.dist-info/entry_points.txt
+Filename: provisioner_runtime-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: provisioner_runtime-0.1.8.dist-info/RECORD
+Filename: provisioner_runtime-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## provisioner/resources/version.txt

```diff
@@ -1 +1 @@
-0.1.8
+0.1.9
```

## provisioner/runner/ansible/ansible_runner.py

```diff
@@ -28,15 +28,15 @@
 ANSIBLE_CALLBACK_PLUGINS_DIR_NAME = "callback_plugins"
 
 ANSIBLE_PLAYBOOKS_PYTHON_PACKAGE = "external.ansible_playbooks.playbooks"
 ANSIBLE_PLAYBOOKS_DIR_NAME = "playbooks"
 
 ANSIBLE_STDOUT_PLUGIN_NAME = "custom_yaml"
 
-ANSIBLE_VALUES_SENSITIVE_KEYWORDS = ["token", "secret"]
+ANSIBLE_VALUES_SENSITIVE_KEYWORDS = ["token", "secret", "api_token", "api_secret", "password", "pass", "pwd"]
 
 INVENTORY_FORMAT = """
 [all:vars]
 ansible_connection=ssh
 
 # These are the user selected hosts from the prompted selection menu
 [selected_hosts]
```

## provisioner/shared/collaborators.py

```diff
@@ -153,11 +153,11 @@
             return self.__hosts_file
 
         return self._lock_and_get(callback=create_hosts_file)
 
     def http_client(self) -> HttpClient:
         def create_http_client():
             if not self.__http_client:
-                self.__http_client = HttpClient.create(self.__ctx, io_utils=self.io_utils(), printer=self.printer())
+                self.__http_client = HttpClient.create(self.__ctx, io_utils=self.io_utils(), progress_indicator=self.progress_indicator(), printer=self.printer())
             return self.__http_client
 
         return self._lock_and_get(callback=create_http_client)
```

## provisioner/shared/collaborators_fakes.py

```diff
@@ -118,15 +118,15 @@
         def create_printer():
             if not self.__printer:
                 self.__printer = FakePrinter.create(self.__ctx)
             return self.__printer
 
         return self._lock_and_get(callback=create_printer)
 
-    def progress_indicator(self) -> ProgressIndicator:
+    def progress_indicator(self) -> FakeProgressIndicator:
         def create_progress_indicator():
             if not self.__progress_indicator:
                 self.__progress_indicator = FakeProgressIndicator.create(self.__ctx)
             return self.__progress_indicator
 
         return self._lock_and_get(callback=create_progress_indicator)
```

## provisioner/utils/httpclient.py

```diff
@@ -1,22 +1,23 @@
 #!/usr/bin/env python3
 
 import os
 import shutil
 import tempfile
 from typing import Optional
 
+from provisioner.utils.printer import Printer
+from provisioner.utils.progress_indicator import ProgressIndicator
 import requests
 from loguru import logger
 from requests import RequestException
 
 from provisioner.errors.cli_errors import DownloadFileException
 from provisioner.infra.context import Context
 from provisioner.utils.io_utils import IOUtils
-from provisioner.utils.printer import Printer
 
 
 class ErrorResponse:
     message: str = ""
     is_timeout: bool = False
 
     def __init__(self, request_exception: Optional[RequestException] = None, exception: Optional[Exception] = None):
@@ -57,28 +58,42 @@
 
 
 class HttpClient:
 
     _dry_run: bool = None
     _verbose: bool = None
     io: IOUtils = None
+    progress_indicator: ProgressIndicator = None
     printer: Printer = None
 
     @staticmethod
-    def create(ctx: Context, io_utils: IOUtils, printer: Printer) -> "HttpClient":
+    def create(
+        ctx: Context, 
+        io_utils: IOUtils, 
+        progress_indicator: ProgressIndicator,
+        printer: Printer) -> "HttpClient":
+
         dry_run = ctx.is_dry_run()
         verbose = ctx.is_verbose()
         logger.debug(f"Creating http client (dry_run: {dry_run}, verbose: {verbose})...")
-        client = HttpClient(io_utils, printer, dry_run, verbose)
+        client = HttpClient(io_utils, progress_indicator, printer, dry_run, verbose)
         return client
 
-    def __init__(self, io_utils: IOUtils, printer: Printer, dry_run: bool, verbose: bool) -> None:
+    def __init__(
+            self, 
+            io_utils: IOUtils, 
+            progress_indicator: ProgressIndicator, 
+            printer: Printer, 
+            dry_run: bool, 
+            verbose: bool) -> None:
+        
         self._dry_run = dry_run
         self._verbose = verbose
         self.io = io_utils
+        self.progress_indicator = progress_indicator
         self.printer = printer
 
     def raw_client(self):
         return requests
 
     def _base_request(
         self,
@@ -155,20 +170,20 @@
         file_path = os.path.join(download_folder_resolved, filename)
 
         if verify_already_downloaded and self.io.file_exists_fn(file_path):
             logger.debug("Found previously downloaded file. path: {}", file_path)
             return file_path
 
         resp = requests.get(url, stream=True, allow_redirects=True)
-        if resp.status_code != 200:
-            resp.raise_for_status()
+        if resp.status_code < 200 or resp.status_code > 299:
+            # resp.raise_for_status()
             raise DownloadFileException(f"Request to {url} returned status code {resp.status_code}")
 
         if progress_bar:
-            self.printer.progress_indicator.progress_bar.download_file_fn(
+            self.progress_indicator.get_progress_bar().download_file_fn(
                 response=resp, download_folder=download_folder_resolved
             )
         else:
             self.printer.print_fn(f"Downloading file {filename}...")
             with open(file_path, "wb") as f:
                 shutil.copyfileobj(resp.raw, f)
```

## provisioner/utils/httpclient_fakes.py

```diff
@@ -7,15 +7,15 @@
 from provisioner.test_lib.faker import TestFakes
 from provisioner.utils.httpclient import HttpClient
 
 
 class FakeHttpClient(TestFakes, HttpClient):
     def __init__(self, dry_run: bool, verbose: bool):
         TestFakes.__init__(self)
-        HttpClient.__init__(self, io_utils=None, printer=None, dry_run=dry_run, verbose=verbose)
+        HttpClient.__init__(self, io_utils=None, progress_indicator=None, printer=None, dry_run=dry_run, verbose=verbose)
 
     @staticmethod
     def create(ctx: Context) -> "FakeHttpClient":
         fake = FakeHttpClient(dry_run=ctx.is_dry_run(), verbose=ctx.is_verbose())
         fake.get_fn = MagicMock(side_effect=fake.get_fn)
         fake.head_fn = MagicMock(side_effect=fake.head_fn)
         fake.post_fn = MagicMock(side_effect=fake.post_fn)
```

## provisioner/utils/io_utils_fakes.py

```diff
@@ -1,122 +1,80 @@
 #!/usr/bin/env python3
 
-import pathlib
-from typing import List
+from unittest.mock import MagicMock
 
 from provisioner.infra.context import Context
-from provisioner.test_lib.test_errors import FakeEnvironmentAssertionError
+from provisioner.test_lib.faker import TestFakes
 from provisioner.utils.io_utils import IOUtils
 
 
-class FakeIOUtils(IOUtils):
-
-    __registered_read_file_safe_paths: dict[str, str] = None
-    __registered_is_archive: dict[str, bool] = None
-    __registered_unpack_archive: dict[str, str] = None
-    __registered_set_file_permissions: List[str] = None
-    __registered_write_symlink: List[str] = None
-
-    __mocked_is_archive: dict[str, bool] = None
-    __mocked_unpack_archive: dict[str, str] = None  # return value: archive parent folder path
+class FakeIOUtils(TestFakes, IOUtils):
 
     def __init__(self, ctx: Context):
-        super().__init__(ctx)
-        self.__registered_read_file_safe_paths = {}
-        self.__registered_is_archive = {}
-        self.__registered_unpack_archive = {}
-        self.__registered_set_file_permissions = []
-        self.__registered_write_symlink = []
-        self.__mocked_is_archive = {}
-        self.__mocked_unpack_archive = {}
-
-    @staticmethod
-    def _create_fake(ctx: Context) -> "FakeIOUtils":
-        io = FakeIOUtils(ctx)
-        io.read_file_safe_fn = lambda file_path: io._read_file_safe_selector(file_path)
-        io.write_file_fn = lambda content, file_name, dir_path=None, executable=False: "/test/script/file/{}".format(
-            file_name
-        )
-        io.create_directory_fn = lambda folder_path: folder_path
-        io.delete_file_fn = lambda file_path: True
-        io.file_exists_fn = lambda file_path: True
-        io.is_archive_fn = lambda file_path: io._register_is_archive(file_path)
-        io.unpack_archive_fn = lambda file_path: io._register_unpack_archive(file_path)
-        io.set_file_permissions_fn = lambda file_path, permissions_octal=0o111: io._register_set_file_permissions(
-            file_path, permissions_octal
-        )
-        io.write_symlink_fn = lambda file_path, symlink_path: io._register_write_symlink(file_path, symlink_path)
-        io.copy_file_fn = lambda from_path, to_path: None
-        io.copy_directory_fn = lambda from_path, to_path: None
-        return io
+        TestFakes.__init__(self)
+        IOUtils.__init__(self, ctx)
 
     @staticmethod
     def create(ctx: Context) -> "FakeIOUtils":
-        return FakeIOUtils._create_fake(ctx)
-
-    def register_file_read(self, file_path: str, expected_output: str):
-        # When opting to use the FakeIOUtils instead of mocking via @mock.patch, we'll override the read function
-        self.__registered_read_file_safe_paths[file_path] = expected_output
-
-    def _read_file_safe_selector(self, file_path: str) -> str:
-        if file_path not in self.__registered_read_file_safe_paths:
-            raise LookupError(f"Fake IO read file path is not defined. name: {file_path}")
-        return self.__registered_read_file_safe_paths.get(file_path)
-
-    def _register_is_archive(self, file_path: str) -> bool:
-        is_archive = self.__mocked_is_archive.get(file_path, False)
-        self.__registered_is_archive[file_path] = is_archive
-        return is_archive
-
-    def assert_is_archive(self, file_path: str, is_archive: bool) -> None:
-        if file_path not in self.__registered_is_archive:
-            raise FakeEnvironmentAssertionError(
-                f"IOUtils expected to check if a filepath is of type archive but it never triggered. file_path: {file_path}"
-            )
-        elif is_archive != self.__registered_is_archive[file_path]:
-            raise FakeEnvironmentAssertionError(
-                "IOUtils expected a file to have a specific archive state but it never matched.\n"
-                + f"Actual:\n{self.__registered_is_archive[file_path]}\n"
-                + f"Expected:\n{is_archive}"
-            )
-
-    def mock_is_archive(self, file_path: str, is_archive: bool) -> None:
-        self.__mocked_is_archive[file_path] = is_archive
-
-    def _register_unpack_archive(self, file_path: str) -> str:
-        parent_folder_path = self.__mocked_unpack_archive.get(file_path, None)
-        self.__registered_unpack_archive[file_path] = (
-            parent_folder_path if parent_folder_path else str(pathlib.Path(file_path).parent)
-        )
-        return self.__registered_unpack_archive[file_path]
-
-    def assert_unpack_archive(self, file_path: str) -> None:
-        if file_path not in self.__registered_unpack_archive:
-            raise FakeEnvironmentAssertionError(
-                "IOUtils expected to unpack an archive but it never triggered.\n"
-                + f"Actual:\n{self.__registered_unpack_archive.keys()}\n"
-                + f"Expected:\n{file_path}"
-            )
-
-    def _register_set_file_permissions(self, file_path: str, permissions_octal: int) -> str:
-        self.__registered_set_file_permissions.append(f"{file_path}__{permissions_octal}")
-        return file_path
-
-    def assert_set_file_permissions(self, file_path: str, permissions_octal: int) -> None:
-        if f"{file_path}__{permissions_octal}" not in self.__registered_set_file_permissions:
-            raise FakeEnvironmentAssertionError(
-                "IOUtils expected to set file permissions but it never triggered.\n"
-                + f"Actual:\n{self.__registered_set_file_permissions}\n"
-                + f"Expected:\n{file_path}__{permissions_octal}"
-            )
-
-    def _register_write_symlink(self, file_path: str, symlink_path: str) -> str:
-        self.__registered_write_symlink.append(f"{file_path}__{symlink_path}")
-        return symlink_path
-
-    def assert_write_symlink(self, file_path: str, symlink_path: str) -> None:
-        if f"{file_path}__{symlink_path}" not in self.__registered_write_symlink:
-            raise FakeEnvironmentAssertionError(
-                "IOUtils expected to write symlink but it never triggered.\n"
-                + f"Actual:\n{self.__registered_write_symlink}\n"
-                + f"Expected:\n{file_path}__{symlink_path}"
-            )
+        fake = FakeIOUtils(ctx=ctx)
+        fake.create_directory_fn = MagicMock(side_effect=fake.create_directory_fn)
+        fake.copy_file_fn = MagicMock(side_effect=fake.copy_file_fn)
+        fake.copy_directory_fn = MagicMock(side_effect=fake.copy_directory_fn)
+        fake.write_file_fn = MagicMock(side_effect=fake.write_file_fn)
+        fake.delete_file_fn = MagicMock(side_effect=fake.delete_file_fn)
+        fake.read_file_safe_fn = MagicMock(side_effect=fake.read_file_safe_fn)
+        fake.write_symlink_fn = MagicMock(side_effect=fake.write_symlink_fn)
+        fake.read_symlink_fn = MagicMock(side_effect=fake.read_symlink_fn)
+        fake.get_symlink_real_path_fn = MagicMock(side_effect=fake.get_symlink_real_path_fn)
+        fake.remove_symlink_fn = MagicMock(side_effect=fake.remove_symlink_fn)
+        fake.symlink_exists_fn = MagicMock(side_effect=fake.symlink_exists_fn)
+        fake.file_exists_fn = MagicMock(side_effect=fake.file_exists_fn)
+        fake.is_archive_fn = MagicMock(side_effect=fake.is_archive_fn)
+        fake.unpack_archive_fn = MagicMock(side_effect=fake.unpack_archive_fn)
+        fake.set_file_permissions_fn = MagicMock(side_effect=fake.set_file_permissions_fn)
+        return fake
+
+    def create_directory_fn(self, folder_path: str) -> bool:
+        return self.trigger_side_effect("create_directory_fn", folder_path)
+    
+    def copy_file_fn(self, from_path: str, to_path: str) -> bool:
+        return self.trigger_side_effect("copy_file_fn", from_path, to_path)
+    
+    def copy_directory_fn(self, from_path: str, to_path: str) -> bool:
+        return self.trigger_side_effect("copy_directory_fn", from_path, to_path)
+    
+    def write_file_fn(self, content: str, file_name: str, dir_path: str = None, executable: bool = False) -> str:
+        return self.trigger_side_effect("write_file_fn", content, file_name, dir_path, executable)
+    
+    def delete_file_fn(self, file_path: str) -> bool:
+        return self.trigger_side_effect("delete_file_fn", file_path)
+    
+    def read_file_safe_fn(self, file_path: str) -> str:
+        return self.trigger_side_effect("read_file_safe_fn", file_path)
+    
+    def write_symlink_fn(self, file_path: str, symlink_path: str) -> bool:
+        return self.trigger_side_effect("write_symlink_fn", file_path, symlink_path)
+    
+    def read_symlink_fn(self, symlink_path: str) -> str:
+        return self.trigger_side_effect("read_symlink_fn", symlink_path)
+    
+    def get_symlink_real_path_fn(self, symlink_path: str) -> str:
+        return self.trigger_side_effect("get_symlink_real_path_fn", symlink_path)
+    
+    def remove_symlink_fn(self, symlink_path: str) -> bool:
+        return self.trigger_side_effect("remove_symlink_fn", symlink_path)
+    
+    def symlink_exists_fn(self, symlink_path: str) -> bool:
+        return self.trigger_side_effect("symlink_exists_fn", symlink_path)
+    
+    def file_exists_fn(self, file_path: str) -> bool:
+        return self.trigger_side_effect("file_exists_fn", file_path)
+    
+    def is_archive_fn(self, file_path: str) -> bool:
+        return self.trigger_side_effect("is_archive_fn", file_path)
+    
+    def unpack_archive_fn(self, file_path: str) -> str:
+        return self.trigger_side_effect("unpack_archive_fn", file_path)
+    
+    def set_file_permissions_fn(self, file_path: str, permissions_octal: int = 0o111) -> bool:
+        return self.trigger_side_effect("set_file_permissions_fn", file_path, permissions_octal)
+
```

## Comparing `provisioner_runtime-0.1.8.dist-info/LICENSE` & `provisioner_runtime-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `provisioner_runtime-0.1.8.dist-info/METADATA` & `provisioner_runtime-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: provisioner-runtime
-Version: 0.1.8
+Version: 0.1.9
 Summary: Provision Everything Anywhere
 Author: Zachi Nachshon
 Author-email: zachi.nachshon@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `provisioner_runtime-0.1.8.dist-info/RECORD` & `provisioner_runtime-0.1.9.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -82,27 +82,27 @@
 provisioner/infra/context.py,sha256=XKhLaNFaBxCCJrPKCH__cGDK2lzMRSl7OSjvfMT2b40,2452
 provisioner/infra/evaluator.py,sha256=kEukOBHkFgqD9_ntkXRuodfiU9sLgZ4d5mWsyeD02Is,2682
 provisioner/infra/log.py,sha256=61ST3qmrIf-CZUZtJVnKRgZp49vGeViQpUMp0nkVaqI,4102
 provisioner/infra/remote_context.py,sha256=U-7juzMelcFbuWzUfmgylMxrj88CczOo7vZ6fRyGlTQ,962
 provisioner/main.py,sha256=xLg-poqJ_0yRT_1TuABTGTDBgi9q6xwyKRpUIYZZ9PU,1668
 provisioner/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/resources/config.yaml,sha256=loN-e5Ptp7nKPssrjJ867g5RHppCYzwvVLfm5NoaVRE,26
-provisioner/resources/version.txt,sha256=QK4wsf7vC_oxaRRpzBC0UZrzPE8DzdBEbPyyxMgV3xo,5
+provisioner/resources/version.txt,sha256=USNvs6-s4bnon1SU7HP3GZApiKaobI8r3L0xh1eqggA,5
 provisioner/runner/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/runner/ansible/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/runner/ansible/ansible_fakes.py,sha256=1fIDJ4v8X2B7BBfmo_Ge6_If6mTaNEPOE-Mrz7066rQ,1228
-provisioner/runner/ansible/ansible_runner.py,sha256=eMOczcQPhp9flK481wyq0eMBAfGLdKhPkOew9CXgPgw,16182
+provisioner/runner/ansible/ansible_runner.py,sha256=Kc3xsi-15qvTSDcalVzrRVmNFe6JpekWwvUpYfipKKY,16236
 provisioner/runner/ansible/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/runner/ansible/resources/ansible.cfg,sha256=SXL8xHPL8xT-g-DbOzqUlQzYRKEyHU6UfVGVE4ApCjo,1957
 provisioner/runner/ansible/resources/callback_plugins/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/runner/ansible/resources/callback_plugins/custom_yaml.py,sha256=zkuML167l04C6ddi15fQ64v-UZ-oICLiYlFCDcocfxI,5455
 provisioner/runner/ansible/resources/callback_plugins/fail_on_missing_hosts.py,sha256=VBPELMNY380V7UDAYUfyo4oEyuzypfLEgHSe-HazZ_k,1081
 provisioner/shared/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-provisioner/shared/collaborators.py,sha256=eAHJ5y7xMJluYLyMsjyYAK2nvOixpGtu_SVhRHMHwkQ,5942
-provisioner/shared/collaborators_fakes.py,sha256=NtnFb9-jWS_PtOxKllrk9k6KTGWdGygKvXd0iDiiVIk,7806
+provisioner/shared/collaborators.py,sha256=-lyoZgFPFe1X_taM9zYcMG5MMjg1mWxxUg7Pkp7G5ng,5988
+provisioner/shared/collaborators_fakes.py,sha256=G7hXY1uF2sRsCsnW3dJmybw2Dz8zUbT_xzZ1oQI-OXM,7810
 provisioner/test_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/test_data/ansible/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/test_data/ansible/playbooks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/test_data/domain.py,sha256=LlO_PiSDVgD7bNv2fwxpXF6Twqtdq_NvSzfppqNUIiY,2668
 provisioner/test_data/internal_config.yaml,sha256=sVjXtaLCA0xsMTJwM_BFlr-eaI1yWsqoi8HzCW8g7aM,256
 provisioner/test_data/user_config.yaml,sha256=j0EVnae8sD71qtLubasS-pKRwlpS2p88nkjd6f-hRfk,180
 provisioner/test_lib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -115,18 +115,18 @@
 provisioner/utils/browser.py,sha256=hcobhmcK1qnesTHwj-u5hgXJsVWUjVRGP2yHdmjejnE,184
 provisioner/utils/checks.py,sha256=9KIAPscTyT-i2-4bfZ2tUsxysFdctfiN58mxxJ31uyQ,1057
 provisioner/utils/checks_fakes.py,sha256=W48dnyWJSnC_DU0hsyP0LDk1oolCj1sBOOMqgZLT_UE,931
 provisioner/utils/github.py,sha256=wMFi3jJR82rEywiJZrdg85ngdEtxZG8qf-kSVjazw-M,2268
 provisioner/utils/github_fakes.py,sha256=W9_LyeuHSpmv7sgBHd0DKJ7SZtRilUNRsn08hloq79M,4589
 provisioner/utils/hosts_file.py,sha256=JLMUUywOGaCxkb3_2Yc9UhewQc5WZBtrwE_QnvQsRag,1955
 provisioner/utils/hosts_file_fakes.py,sha256=Cck6tHSYoqPg5Qt7sRYXxJalxSanJVrdmEvxu7Pm150,949
-provisioner/utils/httpclient.py,sha256=-zhvG0fLUuzP5YRCMIY_aUDBUuGAMK2qUhBCg_-b2yM,6136
-provisioner/utils/httpclient_fakes.py,sha256=i3wYxUYeVd_4KTJ0J5rdNED8nmKuH-MytbfaClDQRhs,1807
+provisioner/utils/httpclient.py,sha256=DcsS2jbJLNfEdh7CguaaKifV9HPBQBXGU41D47hSbCo,6551
+provisioner/utils/httpclient_fakes.py,sha256=eTKpoYiAdaN9PCO_2HYGMF9iTyVepCZVKSTzIbE8cR8,1832
 provisioner/utils/io_utils.py,sha256=k_5NEWHCfZfFiFoZfyWblVt6_rZ2YcypcI5NiMndIDc,7052
-provisioner/utils/io_utils_fakes.py,sha256=3Xq2LBVS1K1d6HH4TSqaKHwjp36uaoaURbsqyTXPrQo,5893
+provisioner/utils/io_utils_fakes.py,sha256=citc1gQnBfSBZT0i6LncYX-pyMJdpJ1zYN3dyvuT5dQ,3888
 provisioner/utils/json_util.py,sha256=ktri9CwcYL1BQS1g6oEIj3zLx4ichqkTRQopS9IoXuA,2130
 provisioner/utils/network.py,sha256=DrRPNVmD7LB7_fePjh4UJdZL6bTf_UOiG7uB6pkpIho,4259
 provisioner/utils/network_fakes.py,sha256=p5ji7K8dKBBdTvTjcpjJWtXVZ01hKkT3IoHfO-sJJ-4,929
 provisioner/utils/os.py,sha256=TKexh743-Ho9bmcQ1Arax17SZJ43bjL_f1lxC5o7A9s,2043
 provisioner/utils/package_loader.py,sha256=aIMe5hvmLfEPzMjGrjEZDXSy7xi27Uw6U_7R7dpvdOk,4204
 provisioner/utils/paths.py,sha256=ifqRgTjdDV7AbMB9myEGS3VwLzwYhVDHWIX9o5Z4oXY,5034
 provisioner/utils/paths_fakes.py,sha256=WXLUCMxoSRsNR0LXzJousT0Kks8k_QhppJAyMr3kcQY,2444
@@ -141,12 +141,12 @@
 provisioner/utils/prompter.py,sha256=RWhDat_577wsM1die636ctuuhNB1-dZWJqlA9bobLJw,8629
 provisioner/utils/prompter_fakes.py,sha256=qqB7pikYvh8RIoArDFq1JYC1PaBdLleQFwC_Gp_ZbSY,2400
 provisioner/utils/properties.py,sha256=pPAV_NFRCfNvy6G87p_a2JpC7P5VRlviEFgORIiucBg,2165
 provisioner/utils/properties_fakes.py,sha256=1fsOQu9FTA12H2XH4I4Wn_H9Bg8hZqYVco-wn-pOHuk,1310
 provisioner/utils/summary.py,sha256=U9dYFFJe_Nodw-1y52K650HOO2d35IVQoCZNU8qPUD4,2080
 provisioner/utils/summary_fakes.py,sha256=YMm6sBiNw5MGCO-ILwnPx0u715_-vJOnyno1czLkeNM,1401
 provisioner/utils/yaml_util.py,sha256=-i1hIyh05hhJYa8bJBjreMfEaZdNkheU6zSvnhgVe-Y,2598
-provisioner_runtime-0.1.8.dist-info/LICENSE,sha256=rcr78KAutoVDcl3EaX33JjBsvfatzmlKWJ0-Ji3I7tk,1071
-provisioner_runtime-0.1.8.dist-info/METADATA,sha256=9sUVoYIjyCmv0NTaTKAkCivrjdbYRRY9buKUfdQNVKA,792
-provisioner_runtime-0.1.8.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-provisioner_runtime-0.1.8.dist-info/entry_points.txt,sha256=YyXkOvQA01nCNiVumyuvhjPWhndn3ZwrvVGFQQ6O74k,53
-provisioner_runtime-0.1.8.dist-info/RECORD,,
+provisioner_runtime-0.1.9.dist-info/LICENSE,sha256=rcr78KAutoVDcl3EaX33JjBsvfatzmlKWJ0-Ji3I7tk,1071
+provisioner_runtime-0.1.9.dist-info/METADATA,sha256=i9dweza09QJNlUZ1O7w5NdfMTjHD4jLR4BAaHHx5j7A,792
+provisioner_runtime-0.1.9.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+provisioner_runtime-0.1.9.dist-info/entry_points.txt,sha256=YyXkOvQA01nCNiVumyuvhjPWhndn3ZwrvVGFQQ6O74k,53
+provisioner_runtime-0.1.9.dist-info/RECORD,,
```

