# Comparing `tmp/screenapi_cli-0.1.5a3.tar.gz` & `tmp/screenapi_cli-0.1.5a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenapi_cli-0.1.5a3.tar", max compression
+gzip compressed data, was "screenapi_cli-0.1.5a4.tar", max compression
```

## Comparing `screenapi_cli-0.1.5a3.tar` & `screenapi_cli-0.1.5a4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1092 2024-03-23 16:06:49.120124 screenapi_cli-0.1.5a3/LICENSE
--rw-r--r--   0        0        0     1381 2024-03-25 19:41:34.179648 screenapi_cli-0.1.5a3/README.md
--rw-r--r--   0        0        0        0 2024-03-26 06:15:38.237432 screenapi_cli-0.1.5a3/app/__init__.py
--rw-r--r--   0        0        0     9241 2024-04-11 16:34:55.215188 screenapi_cli-0.1.5a3/app/__main__.py
--rw-r--r--   0        0        0     1360 2024-04-01 07:33:03.304661 screenapi_cli-0.1.5a3/app/common.py
--rw-r--r--   0        0        0        0 2024-03-24 18:09:29.678307 screenapi_cli-0.1.5a3/app/export/__init__.py
--rw-r--r--   0        0        0     1689 2024-04-15 17:50:49.954658 screenapi_cli-0.1.5a3/app/export/cli.py
--rw-r--r--   0        0        0        0 2024-03-24 14:33:45.903715 screenapi_cli-0.1.5a3/app/setup/__init__.py
--rw-r--r--   0        0        0     1083 2024-03-25 19:15:41.722738 screenapi_cli-0.1.5a3/app/setup/utils.py
--rw-r--r--   0        0        0       97 2024-03-24 17:32:30.550768 screenapi_cli-0.1.5a3/app/txt/__init__.py
--rw-r--r--   0        0        0     5737 2024-03-29 09:45:40.583647 screenapi_cli-0.1.5a3/app/txt/cli.py
--rw-r--r--   0        0        0     6056 2024-03-25 18:55:58.756247 screenapi_cli-0.1.5a3/app/txt/deprecated_cli.py
--rw-r--r--   0        0        0        0 2024-03-27 04:52:19.596215 screenapi_cli-0.1.5a3/app/xlsx/__init__.py
--rw-r--r--   0        0        0    11219 2024-04-16 15:41:00.869229 screenapi_cli-0.1.5a3/app/xlsx/main.py
--rw-r--r--   0        0        0      795 2024-04-16 16:11:49.480663 screenapi_cli-0.1.5a3/pyproject.toml
--rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 screenapi_cli-0.1.5a3/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-03-23 16:06:49.120124 screenapi_cli-0.1.5a4/LICENSE
+-rw-r--r--   0        0        0     1381 2024-03-25 19:41:34.179648 screenapi_cli-0.1.5a4/README.md
+-rw-r--r--   0        0        0        0 2024-03-26 06:15:38.237432 screenapi_cli-0.1.5a4/app/__init__.py
+-rw-r--r--   0        0        0     9369 2024-04-17 05:58:50.361946 screenapi_cli-0.1.5a4/app/__main__.py
+-rw-r--r--   0        0        0     1360 2024-04-01 07:33:03.304661 screenapi_cli-0.1.5a4/app/common.py
+-rw-r--r--   0        0        0        0 2024-03-24 18:09:29.678307 screenapi_cli-0.1.5a4/app/export/__init__.py
+-rw-r--r--   0        0        0     1689 2024-04-15 17:50:49.954658 screenapi_cli-0.1.5a4/app/export/cli.py
+-rw-r--r--   0        0        0        0 2024-03-24 14:33:45.903715 screenapi_cli-0.1.5a4/app/setup/__init__.py
+-rw-r--r--   0        0        0     1083 2024-03-25 19:15:41.722738 screenapi_cli-0.1.5a4/app/setup/utils.py
+-rw-r--r--   0        0        0       97 2024-03-24 17:32:30.550768 screenapi_cli-0.1.5a4/app/txt/__init__.py
+-rw-r--r--   0        0        0     5737 2024-03-29 09:45:40.583647 screenapi_cli-0.1.5a4/app/txt/cli.py
+-rw-r--r--   0        0        0     6056 2024-03-25 18:55:58.756247 screenapi_cli-0.1.5a4/app/txt/deprecated_cli.py
+-rw-r--r--   0        0        0        0 2024-03-27 04:52:19.596215 screenapi_cli-0.1.5a4/app/xlsx/__init__.py
+-rw-r--r--   0        0        0    11650 2024-04-20 11:04:14.938423 screenapi_cli-0.1.5a4/app/xlsx/main.py
+-rw-r--r--   0        0        0      795 2024-04-21 17:34:41.710687 screenapi_cli-0.1.5a4/pyproject.toml
+-rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 screenapi_cli-0.1.5a4/PKG-INFO
```

### Comparing `screenapi_cli-0.1.5a3/LICENSE` & `screenapi_cli-0.1.5a4/LICENSE`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a3/README.md` & `screenapi_cli-0.1.5a4/README.md`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a3/app/__main__.py` & `screenapi_cli-0.1.5a4/app/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,15 @@
         typer.Option("--output-dir", "--output", "-o", help="output directory path"),
     ] = None,
     max_workers: Annotated[
         int, typer.Option("--max-workers", "-w", help="number of workers")
     ] = configGet("default", "max_workers"),
     overwrite: Annotated[bool, typer.Option(help="overwrite existing data")] = False,
     skip_images: Annotated[bool, typer.Option(help="skip saving images")] = False,
+    check: Annotated[str, typer.Option(help="Check for `x` key while checking already parsed data")] = None
 ):
     from app.xlsx.main import main
 
     print(f"[bold]Updating sheet from {input_path}[/]")
     print(f"Number of workers: {max_workers}")
     print(f"Overwrite existing data: {overwrite}")
     print(f"Skip saving images: {skip_images}")
@@ -209,14 +210,15 @@
     main(
         input_path=input_path,
         site=site,
         max_workers=max_workers,
         output_dir=output_dir,
         overwrite=overwrite,
         skip_images=skip_images,
+        check=check
     )
 
 
 @app.command(help="List config", name="config")
 def list_configs():
     for section in config.sections():
         print(f"[bold]\[{section}]")
```

### Comparing `screenapi_cli-0.1.5a3/app/common.py` & `screenapi_cli-0.1.5a4/app/common.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a3/app/export/cli.py` & `screenapi_cli-0.1.5a4/app/export/cli.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a3/app/setup/utils.py` & `screenapi_cli-0.1.5a4/app/setup/utils.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a3/app/txt/cli.py` & `screenapi_cli-0.1.5a4/app/txt/cli.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a3/app/txt/deprecated_cli.py` & `screenapi_cli-0.1.5a4/app/txt/deprecated_cli.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a3/app/xlsx/main.py` & `screenapi_cli-0.1.5a4/app/xlsx/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -163,33 +163,39 @@
     df.sort_values(by=sort_by, inplace=True)
 
     df.rename(columns=read_mapping(site.value, swap=True), inplace=True)
 
     df.to_excel(output_file, index=False)
 
 
-def doneIds(output_dir: str):
+def doneIds(output_dir: str, check: Optional[str] = None):
     ids = []
     for root, dirs, files in os.walk(output_dir):
         if root.startswith(("images")):
             continue
         for file in files:
             if file.startswith("converted"):
                 continue
             if file.endswith(".json"):
                 with open(os.path.join(root, file)) as _f:
                     d = json.loads(_f.read())
                     try:
+                        if check:
+                            if d.get(check) in ["", "0", None]:
+                                os.remove(os.path.join(root, file))
+
                         if d.get("title") in ["", "0"] or d.get("description") in [
                             "",
                             "0",
                         ]:
                             os.remove(os.path.join(root, file))
                         else:
                             ids.append(int(os.path.basename(file).split(".")[0]))
+                    except FileNotFoundError:
+                        continue
                     except Exception as e:
                         print(e)
 
     print("Already done: ", len(ids))
     return ids
 
 
@@ -210,14 +216,15 @@
     except Exception as error:
         print(f"Current URL: {data.get('url')}")
         print(f"Error: {error}")
         print("Exiting...")
         # exit(1)
 
     jsonResponse: dict[str, str] = response.json()
+    # print(jsonResponse)
 
     if "image" in jsonResponse and not skipImages:
         with open(
             os.path.join(OUTPUT_DIR, "images", str(data["sl"]) + ".png"),
             "wb",
         ) as f:
             image_url = jsonResponse["image"]
@@ -233,22 +240,22 @@
         str(data.get("sl")) + ".json",
     )
 
     os.makedirs(Path(output_filename).parent, exist_ok=True)
 
     try:
         for key, value in jsonResponse.items():
-            if key == "username" or key == "description" or key == "title":
-                if jsonResponse[key] not in ["", "0"]:
-                    data["description"] = jsonResponse[key]
+            if key in data and key != "description":
+                data[key] = value
 
-            if key in data:
-                if key == "description":
+            if key in ["title", "username", "description"]:
+                if "description" in data and data["description"] not in ["", "0"]:
                     continue
-                data[key] = value
+                if key in jsonResponse and jsonResponse[key] not in ["", "0"]:
+                    data["description"] = jsonResponse[key]
 
         with open(output_filename, "w") as file:
             json.dump(data, file, indent=2)
         # print(f"Saved to {output_filename}")
         progress.update(taskId, advance=1)
     except Exception as error:
         print(f"Error saving to {output_filename}: {error}")
@@ -258,14 +265,15 @@
     input_path: Path,
     site: sheetType,
     output_dir: Optional[Path] = None,
     save: Optional[bool] = True,
     max_workers: Optional[int] = config.get("default", "max_workers"),
     overwrite: Optional[bool] = False,
     skip_images: Optional[bool] = False,
+    check: Optional[str] = None,
 ):
     global OUTPUT_DIR
     if output_dir is None:
         # global output_dir
         output_dir = os.path.join(
             os.path.dirname(input_path), getId(Path(input_path).stem)
         )
@@ -278,15 +286,15 @@
     os.makedirs(output_dir, exist_ok=True)
     os.makedirs(os.path.join(output_dir, "images"), exist_ok=True)
     # try:
     data = convert_to_json(input_path=input_path, site=site)
     original_length = len(data)
 
     if not overwrite:
-        done_already = doneIds(output_dir)
+        done_already = doneIds(output_dir, check)
     else:
         done_already = []
     data = [i for i in data if i["sl"] not in done_already]
 
     client = Client(
         http2=True,
         timeout=None,
@@ -351,14 +359,14 @@
     )
 
     print("Done!")
 
 
 if __name__ == "__main__":
     main(
-        input_path=Path("dumps/goibibo.xlsx"),
+        input_path=Path("dumps/Redbus_SM_4thApril (1).xlsx"),
         site=sheetType.social,
         save=True,
         overwrite=True,
         skip_images=True,
         max_workers=5,
     )
```

### Comparing `screenapi_cli-0.1.5a3/pyproject.toml` & `screenapi_cli-0.1.5a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "screenapi-cli"
-version = "0.1.5a3"
+version = "0.1.5a4"
 description = "A cli interface to interact with screenapi"
 authors = ["RONY <iamrony777@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "app" },
 ]
```

### Comparing `screenapi_cli-0.1.5a3/PKG-INFO` & `screenapi_cli-0.1.5a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screenapi-cli
-Version: 0.1.5a3
+Version: 0.1.5a4
 Summary: A cli interface to interact with screenapi
 License: MIT
 Author: RONY
 Author-email: iamrony777@pm.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

