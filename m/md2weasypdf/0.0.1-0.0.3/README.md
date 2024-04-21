# Comparing `tmp/md2weasypdf-0.0.1.tar.gz` & `tmp/md2weasypdf-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2weasypdf-0.0.1.tar", last modified: Sat Apr 20 00:24:16 2024, max compression
+gzip compressed data, was "md2weasypdf-0.0.3.tar", last modified: Sun Apr 21 18:46:10 2024, max compression
```

## Comparing `md2weasypdf-0.0.1.tar` & `md2weasypdf-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:24:16.876206 md2weasypdf-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    26501 2024-04-20 00:24:13.000000 md2weasypdf-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-20 00:24:16.876206 md2weasypdf-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-20 00:24:13.000000 md2weasypdf-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:24:16.876206 md2weasypdf-0.0.1/md2weasypdf/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-20 00:24:13.000000 md2weasypdf-0.0.1/md2weasypdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-20 00:24:13.000000 md2weasypdf-0.0.1/md2weasypdf/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:24:16.876206 md2weasypdf-0.0.1/md2weasypdf/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-20 00:24:13.000000 md2weasypdf-0.0.1/md2weasypdf/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-20 00:24:13.000000 md2weasypdf-0.0.1/md2weasypdf/extensions/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-20 00:24:13.000000 md2weasypdf-0.0.1/md2weasypdf/extensions/subscript.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-20 00:24:13.000000 md2weasypdf-0.0.1/md2weasypdf/extensions/textbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-20 00:24:13.000000 md2weasypdf-0.0.1/md2weasypdf/extensions/toc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-20 00:24:13.000000 md2weasypdf-0.0.1/md2weasypdf/printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:24:16.876206 md2weasypdf-0.0.1/md2weasypdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-20 00:24:16.000000 md2weasypdf-0.0.1/md2weasypdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-20 00:24:16.000000 md2weasypdf-0.0.1/md2weasypdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 00:24:16.000000 md2weasypdf-0.0.1/md2weasypdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 00:24:16.000000 md2weasypdf-0.0.1/md2weasypdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 00:24:16.000000 md2weasypdf-0.0.1/md2weasypdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 00:24:16.000000 md2weasypdf-0.0.1/md2weasypdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-20 00:24:13.000000 md2weasypdf-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-20 00:24:16.880206 md2weasypdf-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 00:24:13.000000 md2weasypdf-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:46:10.951985 md2weasypdf-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    26501 2024-04-21 18:46:06.000000 md2weasypdf-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-21 18:46:10.951985 md2weasypdf-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-21 18:46:06.000000 md2weasypdf-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:46:10.947985 md2weasypdf-0.0.3/md2weasypdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-21 18:46:06.000000 md2weasypdf-0.0.3/md2weasypdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-21 18:46:06.000000 md2weasypdf-0.0.3/md2weasypdf/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:46:10.951985 md2weasypdf-0.0.3/md2weasypdf/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-21 18:46:06.000000 md2weasypdf-0.0.3/md2weasypdf/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-21 18:46:06.000000 md2weasypdf-0.0.3/md2weasypdf/extensions/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-21 18:46:06.000000 md2weasypdf-0.0.3/md2weasypdf/extensions/footnotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-21 18:46:06.000000 md2weasypdf-0.0.3/md2weasypdf/extensions/subscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-21 18:46:06.000000 md2weasypdf-0.0.3/md2weasypdf/extensions/textbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-21 18:46:06.000000 md2weasypdf-0.0.3/md2weasypdf/extensions/toa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-21 18:46:06.000000 md2weasypdf-0.0.3/md2weasypdf/extensions/toc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-04-21 18:46:06.000000 md2weasypdf-0.0.3/md2weasypdf/printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:46:10.951985 md2weasypdf-0.0.3/md2weasypdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-21 18:46:10.000000 md2weasypdf-0.0.3/md2weasypdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-21 18:46:10.000000 md2weasypdf-0.0.3/md2weasypdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 18:46:10.000000 md2weasypdf-0.0.3/md2weasypdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 18:46:10.000000 md2weasypdf-0.0.3/md2weasypdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-21 18:46:10.000000 md2weasypdf-0.0.3/md2weasypdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 18:46:10.000000 md2weasypdf-0.0.3/md2weasypdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-21 18:46:06.000000 md2weasypdf-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-21 18:46:10.955985 md2weasypdf-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 18:46:06.000000 md2weasypdf-0.0.3/setup.py
```

### Comparing `md2weasypdf-0.0.1/LICENSE` & `md2weasypdf-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.1/md2weasypdf/__main__.py` & `md2weasypdf-0.0.3/md2weasypdf/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from functools import partial
 from pathlib import Path
 from threading import Timer
 from typing import Callable, Optional
 
 import typer
 from rich.console import Console
+from typing_extensions import Annotated
 from watchdog.events import FileSystemEvent, FileSystemEventHandler
 from watchdog.observers import Observer
 
 from .printer import Printer
 
 console = Console()
 
@@ -55,24 +56,27 @@
             console.print_exception()
 
     def on_modified(self, event: FileSystemEvent):
         self.on_created(event)
 
 
 def main(
-    input: Path = typer.Argument(help="Folder or file used as input"),
-    output_dir: Path = typer.Argument(),
+    input: Annotated[Path, typer.Argument(help="Folder or file used as input")],
+    output_dir: Annotated[Path, typer.Argument(help="Folder where resulting files are written to")] = Path("."),
     *,
-    bundle: bool = typer.Option(False, help="Bundle all input documents into a single output file"),
-    title: Optional[str] = typer.Option(None, help="Title of the resulting document. Can only be used in conjunction with bundle."),
-    layouts_dir: Path = typer.Option("layouts", help="Base folder containing the available layouts"),
-    layout: Optional[str] = typer.Option(None, help="Default layout to use"),
-    output_html: bool = typer.Option(False, help="Additionally output the raw HTML file which is used to create the pdf"),
-    filename_filter: Optional[str] = typer.Option(None, help="Regular expression to filter files in input directory by subpath and/or filename"),
-    watch: bool = False,
+    bundle: Annotated[bool, typer.Option(help="Bundle all input documents into a single output file")] = False,
+    title: Annotated[Optional[str], typer.Option(help="Title of the resulting document. Can only be used in conjunction with bundle.")] = None,
+    layouts_dir: Annotated[Path, typer.Option(help="Base folder containing the available layouts")] = "layouts",
+    layout: Annotated[Optional[str], typer.Option(help="Default layout to use")] = None,
+    output_html: Annotated[bool, typer.Option(help="Additionally output the raw HTML file which is used to create the pdf")] = False,
+    filename_filter: Annotated[
+        Optional[str],
+        typer.Option(help="Regular expression to filter files in input directory by subpath and/or filename"),
+    ] = None,
+    watch: Annotated[bool, typer.Option(help="Watch input directory for changes and re-run the conversion")] = False,
 ):
     try:
         printer = Printer(
             input=input,
             output_dir=output_dir,
             layouts_dir=layouts_dir,
             bundle=bundle,
@@ -80,29 +84,45 @@
             layout=layout,
             output_html=output_html,
             filename_filter=filename_filter,
         )
 
     except ValueError as error:
         console.print("Error:", error, style="bold red")
-        return
+        raise typer.Exit(1)
 
     if watch:
+
+        def execute():
+            try:
+                for document, output_path in printer.execute():
+                    console.log(
+                        f"Created PDF",
+                        f'"{document.title}"',
+                        f"(out of {len(document.articles)})" if len(document.articles) > 1 else f"(from {document.articles[0].source})",
+                        "->",
+                        output_path,
+                    )
+
+                console.log("Completed document creation")
+
+            except ValueError as error:
+                console.log("Error:", error, style="bold red")
+
+            except Exception:
+                console.print_exception()
+
         observer = Observer()
-        add_watch_directory = partial(observer.schedule, FileChangeHandler(printer.execute), recursive=True)
+        add_watch_directory = partial(observer.schedule, FileChangeHandler(execute), recursive=True)
         add_watch_directory(input)
         add_watch_directory(layouts_dir)
 
         observer.start()
 
-        try:
-            printer.execute()
-
-        except Exception:
-            console.print_exception()
+        execute()
 
         try:
             while True:
                 time.sleep(1)
 
         finally:
             observer.stop()
```

### Comparing `md2weasypdf-0.0.1/md2weasypdf/extensions/checkbox.py` & `md2weasypdf-0.0.3/md2weasypdf/extensions/checkbox.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.1/md2weasypdf/extensions/textbox.py` & `md2weasypdf-0.0.3/md2weasypdf/extensions/textbox.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.1/md2weasypdf/extensions/toc.py` & `md2weasypdf-0.0.3/md2weasypdf/extensions/toc.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from markdown.extensions import toc
 from markdown.extensions.toc import get_name, nest_toc_tokens, slugify, stashedHTML2text, unescape, unique
 from markdown.util import code_escape
 
 
 class TocTreeprocessor(toc.TocTreeprocessor):
     def __init__(self, md: Markdown, config: dict[str, Any]) -> None:
-        self.id_prefix = config.pop('id_prefix')
+        self.id_prefix = config.pop('id_prefix', '')
         super().__init__(md, config)
 
     def build_toc_div(self, toc_list: list) -> etree.Element:
         """Return a string div given a toc list."""
         div = etree.Element("div")
         div.attrib["class"] = self.toc_class
```

### Comparing `md2weasypdf-0.0.1/md2weasypdf/printer.py` & `md2weasypdf-0.0.3/md2weasypdf/printer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,76 @@
 import os
 import re
 import warnings
+from dataclasses import dataclass
 from datetime import date
 from functools import cache
 from glob import iglob
 from pathlib import Path
 from subprocess import check_output
-from typing import NamedTuple, Optional
+from typing import List, NamedTuple, Optional
 
 import frontmatter
-from jinja2 import Environment, FileSystemLoader, select_autoescape
+from jinja2 import Environment, FileSystemLoader, Template, select_autoescape
 from markdown import Markdown
 from markdown_grid_tables import GridTableExtension
 from weasyprint import HTML
 
 from . import extensions
 
 
-class Document(NamedTuple):
-    filename: str
+class Article(NamedTuple):
+    source: Path
     title: str
     content: str
     meta: dict[str, object]
     has_custom_headline: bool
     hash: str
 
 
+@dataclass
+class Document:
+    title: str
+    template: Template
+    layout_dir: Path
+    articles: List[Article]
+
+    def write_pdf(self, output_dir: Path, output_html: bool = False):
+        html = self.template.render(
+            date=date.today().isoformat(),
+            commit=os.getenv("CI_COMMIT_SHORT_SHA", "00000000"),
+            articles=self.articles,
+            title=self.title,
+        )
+
+        output_filename = self.title.replace(" ", "_")
+        if output_html:
+            with open(output_dir / f"{output_filename}.html", "w", encoding="utf-8") as html_file:
+                html_file.write(html)
+
+        pdf_output_target = output_dir / f"{output_filename}.pdf"
+        HTML(string=html, base_url=str(self.layout_dir)).write_pdf(target=pdf_output_target)
+        return pdf_output_target
+
+
 class Printer:
     @staticmethod
-    def _ensure_path(path: Path):
+    def _ensure_path(path: Path, dir: Optional[bool] = None, create: Optional[bool] = None):
         if not path.is_absolute():
             path = Path(os.path.join(os.getcwd(), path))
 
         if not path.exists():
-            raise FileNotFoundError("Path does not exist")
+            if create and dir:
+                path.mkdir(parents=True)
+
+            else:
+                raise FileNotFoundError("Path does not exist")
+
+        if dir is True and not path.is_dir():
+            raise ValueError(f"{path} is not a directory")
 
         return path
 
     def __init__(
         self,
         input: Path,
         output_dir: Path,
@@ -45,16 +78,16 @@
         bundle: bool = False,
         title: Optional[str] = None,
         layout: Optional[str] = None,
         output_html: bool = False,
         filename_filter: Optional[str] = None,
     ):
         self.input = self._ensure_path(input)
-        self.output_dir = self._ensure_path(output_dir)
-        self.layouts_dir = self._ensure_path(layouts_dir)
+        self.output_dir = self._ensure_path(output_dir, dir=True, create=True)
+        self.layouts_dir = self._ensure_path(layouts_dir, dir=True)
         self.bundle = bundle
         self.title = title
         self.layout = layout
         self.output_html = output_html
         self.filename_filter = re.compile(filename_filter) if filename_filter else None
         self.jinja_env = Environment(
             autoescape=select_autoescape(),
@@ -68,96 +101,102 @@
             if not os.path.isdir(self.input):
                 warnings.warn("Option bundle has no effect when using a single file as input")
 
         elif not self.bundle:
             if self.title:
                 raise ValueError("A title cannot be specified when not using bundle.")
 
-    def _load_document(self, document_path):
-        with open(document_path, mode="r", encoding="utf-8") as file:
-            filename = os.path.basename(document_path)
-            if filename.startswith("_"):
-                return
-
-            if self.filename_filter and not re.search(self.filename_filter, document_path):
-                return
-
-            md = Markdown(
-                extensions=[
-                    extensions.TocExtension(id_prefix=filename, toc_depth="2-6"),
-                    extensions.SubscriptExtension(),
-                    extensions.TextboxExtension(),
-                    extensions.CheckboxExtension(),
-                    GridTableExtension(),
-                ],
-            )
+    def _load_article(self, source: Path | str):
+        if isinstance(source, str):
+            source = Path(source)
+
+        with open(source, mode="r", encoding="utf-8") as file:
+            article = frontmatter.load(file)
+
+        md = Markdown(
+            extensions=[
+                extensions.FootnoteExtension(),
+                extensions.TableExtension(),
+                extensions.ToaExtension(),
+                extensions.AbbrExtension(),
+                extensions.TocExtension(id_prefix=source.name, toc_depth="2-6"),
+                extensions.SubscriptExtension(),
+                extensions.TextboxExtension(),
+                extensions.CheckboxExtension(),
+                GridTableExtension(),
+            ],
+        )
 
-            document = frontmatter.load(file)
-            content = (
-                Environment(
-                    autoescape=select_autoescape(),
-                    loader=FileSystemLoader(searchpath=[os.path.dirname(document_path), self.input, os.getcwd()]),
-                )
-                .from_string(document.content)
-                .render()
+        content = (
+            Environment(
+                autoescape=select_autoescape(),
+                loader=FileSystemLoader(searchpath=[os.path.dirname(source), self.input, os.getcwd()]),
             )
+            .from_string(article.content)
+            .render()
+        )
 
-            return Document(
-                filename=filename,
-                title=filename.removesuffix(".md").replace("_", " "),
-                content=md.convert(content),
-                meta=document.metadata,
-                has_custom_headline=content.startswith("# "),
-                hash=str(check_output(["git", "hash-object", document_path]), "utf-8"),
-            )
+        return Article(
+            source=source,
+            title=source.name.removesuffix(".md").replace("_", " "),
+            content=md.convert(content),
+            meta=article.metadata,
+            has_custom_headline=content.startswith("# "),
+            hash=str(check_output(["git", "hash-object", source]), "utf-8"),
+        )
 
     def execute(self):
-        documents = []
-        if os.path.isdir(self.input):
-            for document_path in sorted(iglob(os.path.join(self.input, "**/*.md"), recursive=True)):
-                if document := self._load_document(document_path):
-                    documents.append(document)
+        self._load_template.cache_clear()
+        articles: List[Article] = []
+        if self.input.is_dir():
+            for article_path in sorted(iglob(os.path.join(self.input, "**/*.md"), recursive=True)):
+                if os.path.basename(article_path).startswith("_"):
+                    continue
+
+                if self.filename_filter and not re.search(self.filename_filter, article_path):
+                    continue
+
+                articles.append(self._load_article(article_path))
 
         else:
-            documents.append(self._load_document(self.input))
+            articles.append(self._load_article(self.input))
+
+        write_options = {"output_dir": self.output_dir, "output_html": self.output_html}
 
         if self.bundle:
-            self._render_and_output(documents)
+            doc = Document(
+                self.title,
+                *self._load_template(self.layout),
+                articles,
+            )
+            yield doc, doc.write_pdf(**write_options)
 
         else:
-            os.makedirs(self.output_dir, exist_ok=True)
-            for doc in documents:
-                self._render_and_output(doc)
-
-    def _render_and_output(self, content: list[Document] | Document):
-        template, layout_dir = self._load_template(self.layout if self.bundle else content.meta.get('layout', self.layout))
-        html = template.render(
-            date=date.today().isoformat(),
-            commit=os.getenv("CI_COMMIT_SHORT_SHA", "00000000"),
-            content_documents=content if self.bundle else [content],
-            title=self.title if self.bundle else content.title or "",
-        )
+            for article in articles:
+                try:
+                    doc = Document(
+                        article.title,
+                        *self._load_template(article.meta.get('layout', self.layout)),
+                        [article],
+                    )
 
-        target = os.path.join(
-            self.output_dir,
-            self.title.replace(" ", "_") if self.bundle else content.filename.removesuffix(".md"),
-        )
+                except ValueError as error:
+                    raise ValueError(f"Could not create document for {article.source}: {error}") from error
 
-        if self.output_html:
-            with open(target + ".html", "w", encoding="utf-8") as html_file:
-                html_file.write(html)
-
-        HTML(string=html, base_url=layout_dir).write_pdf(target=target + ".pdf")
+                yield doc, doc.write_pdf(**write_options)
 
     def _get_layout_dir(self, layout: str):
-        if os.path.isdir(layout_dir := os.path.join(self.layouts_dir, layout)):
+        if not layout:
+            raise ValueError("No layout defined")
+
+        if os.path.isdir(layout_dir := self.layouts_dir / layout):
             return layout_dir
 
-        raise ValueError("Layout could not be found")
+        raise ValueError("Layout \"{layout}\" could not be found")
 
     @cache
     def _load_template(self, layout):
         layout_dir = self._get_layout_dir(layout)
-        with open(os.path.join(layout_dir, "index.html"), mode="rb") as file:
+        with open(layout_dir / "index.html", mode="rb") as file:
             template = self.jinja_env.from_string(str(file.read(), "utf-8"))
 
         return template, layout_dir
```

### Comparing `md2weasypdf-0.0.1/setup.cfg` & `md2weasypdf-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = md2weasypdf
-version = 0.0.1
+version = 0.0.3
 author = Manuel Stingl
 author_email = contact@stingl.st
 description = Print PDFs from Markdown Files using Weasyprint
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GNU LGPLv2.1
 classifiers =
```

