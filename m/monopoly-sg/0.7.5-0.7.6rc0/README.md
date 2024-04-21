# Comparing `tmp/monopoly_sg-0.7.5.tar.gz` & `tmp/monopoly_sg-0.7.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monopoly_sg-0.7.5.tar", max compression
+gzip compressed data, was "monopoly_sg-0.7.6rc0.tar", max compression
```

## Comparing `monopoly_sg-0.7.5.tar` & `monopoly_sg-0.7.6rc0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1072 2023-11-25 08:00:21.000000 monopoly_sg-0.7.5/LICENSE.md
--rw-r--r--   0        0        0     2624 2023-12-27 07:15:14.515773 monopoly_sg-0.7.5/README.md
--rw-r--r--   0        0        0     2053 2024-04-20 05:11:27.654820 monopoly_sg-0.7.5/pyproject.toml
--rw-r--r--   0        0        0       59 2023-11-25 08:00:21.000000 monopoly_sg-0.7.5/src/monopoly/__init__.py
--rw-r--r--   0        0        0     8005 2024-02-11 14:35:16.392192 monopoly_sg-0.7.5/src/monopoly/cli.py
--rw-r--r--   0        0        0     3389 2024-01-14 10:44:28.918012 monopoly_sg-0.7.5/src/monopoly/config.py
--rw-r--r--   0        0        0     4005 2024-01-14 09:33:42.855330 monopoly_sg-0.7.5/src/monopoly/constants.py
--rw-r--r--   0        0        0   299608 2023-12-28 09:49:25.899409 monopoly_sg-0.7.5/src/monopoly/examples/example_statement.pdf
--rw-r--r--   0        0        0      620 2023-12-01 13:26:34.000000 monopoly_sg-0.7.5/src/monopoly/examples/multiple_statements.py
--rw-r--r--   0        0        0      742 2023-12-02 13:07:54.000000 monopoly_sg-0.7.5/src/monopoly/examples/single_statement.py
--rw-r--r--   0        0        0      491 2024-01-01 12:59:34.183692 monopoly_sg-0.7.5/src/monopoly/log.py
--rw-r--r--   0        0        0     5467 2024-04-20 05:11:27.654820 monopoly_sg-0.7.5/src/monopoly/pdf.py
--rw-r--r--   0        0        0     3804 2024-04-05 13:52:17.787640 monopoly_sg-0.7.5/src/monopoly/processor.py
--rw-r--r--   0        0        0     2853 2024-04-20 05:11:27.654820 monopoly_sg-0.7.5/src/monopoly/processors/__init__.py
--rw-r--r--   0        0        0     3964 2024-01-14 09:33:55.555328 monopoly_sg-0.7.5/src/monopoly/processors/base.py
--rw-r--r--   0        0        0       55 2023-12-01 13:26:34.000000 monopoly_sg-0.7.5/src/monopoly/processors/citibank/__init__.py
--rw-r--r--   0        0        0     1020 2024-01-14 07:44:48.150290 monopoly_sg-0.7.5/src/monopoly/processors/citibank/citibank.py
--rw-r--r--   0        0        0       40 2023-12-01 13:26:34.000000 monopoly_sg-0.7.5/src/monopoly/processors/dbs/__init__.py
--rw-r--r--   0        0        0     1365 2024-04-19 14:20:45.535418 monopoly_sg-0.7.5/src/monopoly/processors/dbs/dbs.py
--rw-r--r--   0        0        0      964 2024-04-19 14:21:07.835415 monopoly_sg-0.7.5/src/monopoly/processors/example_bank.py
--rw-r--r--   0        0        0       43 2023-12-01 13:26:34.000000 monopoly_sg-0.7.5/src/monopoly/processors/hsbc/__init__.py
--rw-r--r--   0        0        0     1158 2024-01-11 15:47:10.530736 monopoly_sg-0.7.5/src/monopoly/processors/hsbc/hsbc.py
--rw-r--r--   0        0        0       43 2023-12-01 13:26:34.000000 monopoly_sg-0.7.5/src/monopoly/processors/ocbc/__init__.py
--rw-r--r--   0        0        0     1506 2024-04-19 14:18:09.005435 monopoly_sg-0.7.5/src/monopoly/processors/ocbc/ocbc.py
--rw-r--r--   0        0        0       83 2023-12-01 13:26:34.000000 monopoly_sg-0.7.5/src/monopoly/processors/standard_chartered/__init__.py
--rw-r--r--   0        0        0     1007 2024-01-12 14:33:27.070256 monopoly_sg-0.7.5/src/monopoly/processors/standard_chartered/standard_chartered.py
--rw-r--r--   0        0        0      216 2023-12-28 15:35:17.896832 monopoly_sg-0.7.5/src/monopoly/statements/__init__.py
--rw-r--r--   0        0        0     7669 2024-04-19 14:24:09.875401 monopoly_sg-0.7.5/src/monopoly/statements/base.py
--rw-r--r--   0        0        0     3105 2024-02-11 14:35:16.392192 monopoly_sg-0.7.5/src/monopoly/statements/credit_statement.py
--rw-r--r--   0        0        0     4278 2024-02-11 14:35:16.392192 monopoly_sg-0.7.5/src/monopoly/statements/debit_statement.py
--rw-r--r--   0        0        0     1521 2024-04-19 14:24:09.875401 monopoly_sg-0.7.5/src/monopoly/write.py
--rw-r--r--   0        0        0       69 2023-11-25 10:08:54.000000 monopoly_sg-0.7.5/tests/test_utils/__init__.py
--rw-r--r--   0        0        0      790 2023-11-25 10:08:54.000000 monopoly_sg-0.7.5/tests/test_utils/skip.py
--rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 monopoly_sg-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-11-25 08:00:21.000000 monopoly_sg-0.7.6rc0/LICENSE.md
+-rw-r--r--   0        0        0     2624 2024-04-21 03:16:26.522623 monopoly_sg-0.7.6rc0/README.md
+-rw-r--r--   0        0        0     2055 2024-04-21 09:08:13.435099 monopoly_sg-0.7.6rc0/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-11-25 08:00:21.000000 monopoly_sg-0.7.6rc0/src/monopoly/__init__.py
+-rw-r--r--   0        0        0     8005 2024-02-11 14:35:16.392192 monopoly_sg-0.7.6rc0/src/monopoly/cli.py
+-rw-r--r--   0        0        0     3389 2024-01-14 10:44:28.918012 monopoly_sg-0.7.6rc0/src/monopoly/config.py
+-rw-r--r--   0        0        0     4005 2024-01-14 09:33:42.855330 monopoly_sg-0.7.6rc0/src/monopoly/constants.py
+-rw-r--r--   0        0        0   299608 2023-12-28 09:49:25.899409 monopoly_sg-0.7.6rc0/src/monopoly/examples/example_statement.pdf
+-rw-r--r--   0        0        0      620 2023-12-01 13:26:34.000000 monopoly_sg-0.7.6rc0/src/monopoly/examples/multiple_statements.py
+-rw-r--r--   0        0        0      742 2023-12-02 13:07:54.000000 monopoly_sg-0.7.6rc0/src/monopoly/examples/single_statement.py
+-rw-r--r--   0        0        0      491 2024-01-01 12:59:34.183692 monopoly_sg-0.7.6rc0/src/monopoly/log.py
+-rw-r--r--   0        0        0     5935 2024-04-21 09:07:06.175123 monopoly_sg-0.7.6rc0/src/monopoly/pdf.py
+-rw-r--r--   0        0        0     3808 2024-04-21 08:04:57.716452 monopoly_sg-0.7.6rc0/src/monopoly/processor.py
+-rw-r--r--   0        0        0     3032 2024-04-21 08:00:23.086550 monopoly_sg-0.7.6rc0/src/monopoly/processors/__init__.py
+-rw-r--r--   0        0        0     4100 2024-04-21 08:04:53.386453 monopoly_sg-0.7.6rc0/src/monopoly/processors/base.py
+-rw-r--r--   0        0        0       55 2023-12-01 13:26:34.000000 monopoly_sg-0.7.6rc0/src/monopoly/processors/citibank/__init__.py
+-rw-r--r--   0        0        0     1020 2024-01-14 07:44:48.150290 monopoly_sg-0.7.6rc0/src/monopoly/processors/citibank/citibank.py
+-rw-r--r--   0        0        0       40 2023-12-01 13:26:34.000000 monopoly_sg-0.7.6rc0/src/monopoly/processors/dbs/__init__.py
+-rw-r--r--   0        0        0     1365 2024-04-19 14:20:45.535418 monopoly_sg-0.7.6rc0/src/monopoly/processors/dbs/dbs.py
+-rw-r--r--   0        0        0      964 2024-04-21 07:51:47.386734 monopoly_sg-0.7.6rc0/src/monopoly/processors/example_bank.py
+-rw-r--r--   0        0        0       43 2023-12-01 13:26:34.000000 monopoly_sg-0.7.6rc0/src/monopoly/processors/hsbc/__init__.py
+-rw-r--r--   0        0        0     1158 2024-01-11 15:47:10.530736 monopoly_sg-0.7.6rc0/src/monopoly/processors/hsbc/hsbc.py
+-rw-r--r--   0        0        0       43 2023-12-01 13:26:34.000000 monopoly_sg-0.7.6rc0/src/monopoly/processors/ocbc/__init__.py
+-rw-r--r--   0        0        0     1506 2024-04-19 14:18:09.005435 monopoly_sg-0.7.6rc0/src/monopoly/processors/ocbc/ocbc.py
+-rw-r--r--   0        0        0       83 2023-12-01 13:26:34.000000 monopoly_sg-0.7.6rc0/src/monopoly/processors/standard_chartered/__init__.py
+-rw-r--r--   0        0        0     1007 2024-01-12 14:33:27.070256 monopoly_sg-0.7.6rc0/src/monopoly/processors/standard_chartered/standard_chartered.py
+-rw-r--r--   0        0        0      216 2023-12-28 15:35:17.896832 monopoly_sg-0.7.6rc0/src/monopoly/statements/__init__.py
+-rw-r--r--   0        0        0     7669 2024-04-19 14:24:09.875401 monopoly_sg-0.7.6rc0/src/monopoly/statements/base.py
+-rw-r--r--   0        0        0     3105 2024-02-11 14:35:16.392192 monopoly_sg-0.7.6rc0/src/monopoly/statements/credit_statement.py
+-rw-r--r--   0        0        0     4278 2024-02-11 14:35:16.392192 monopoly_sg-0.7.6rc0/src/monopoly/statements/debit_statement.py
+-rw-r--r--   0        0        0     1465 2024-04-21 08:04:57.716452 monopoly_sg-0.7.6rc0/src/monopoly/write.py
+-rw-r--r--   0        0        0       69 2023-11-25 10:08:54.000000 monopoly_sg-0.7.6rc0/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0      790 2023-11-25 10:08:54.000000 monopoly_sg-0.7.6rc0/tests/test_utils/skip.py
+-rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 monopoly_sg-0.7.6rc0/PKG-INFO
```

### Comparing `monopoly_sg-0.7.5/LICENSE.md` & `monopoly_sg-0.7.6rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/README.md` & `monopoly_sg-0.7.6rc0/README.md`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/pyproject.toml` & `monopoly_sg-0.7.6rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monopoly-sg"
-version = "0.7.5"
+version = "0.7.6rc0"
 description = "PDF parsing for Singaporean banks"
 repository = "https://github.com/benjamin-awd/monopoly"
 authors = ["benjamin-awd <benjamindornel@gmail.com>"]
 packages = [
     { include = "monopoly", from = "src" },
     { include = "test_utils", from = "tests" }
 ]
@@ -19,15 +19,15 @@
 python = "^3.11, <3.12"
 pandas = "^2.1.3"
 pydantic-settings = "^2.0.3"
 pymupdf = "^1.23.7"
 pdftotext = "^2.2.2"
 click = "^8.1.7"
 tqdm = "^4.66.1"
-pdf2john = "^0.1.10"
+pdf2john = "^0.2.0"
 tabulate = "^0.9.0"
 mypy = "^1.7.1"
 pydantic = "^2.5.2"
 
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.7,<25.0"
```

### Comparing `monopoly_sg-0.7.5/src/monopoly/cli.py` & `monopoly_sg-0.7.6rc0/src/monopoly/cli.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/src/monopoly/config.py` & `monopoly_sg-0.7.6rc0/src/monopoly/config.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/src/monopoly/constants.py` & `monopoly_sg-0.7.6rc0/src/monopoly/constants.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/src/monopoly/examples/example_statement.pdf` & `monopoly_sg-0.7.6rc0/src/monopoly/examples/example_statement.pdf`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/src/monopoly/examples/multiple_statements.py` & `monopoly_sg-0.7.6rc0/src/monopoly/examples/multiple_statements.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/src/monopoly/examples/single_statement.py` & `monopoly_sg-0.7.6rc0/src/monopoly/examples/single_statement.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/src/monopoly/pdf.py` & `monopoly_sg-0.7.6rc0/src/monopoly/pdf.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,37 +41,38 @@
 class BadPasswordFormatError(Exception):
     """Exception raised passwords are not provided in a proper format"""
 
 
 class PdfParser:
     def __init__(
         self,
-        file_path: Path,
+        file_path: Optional[Path] = None,
+        file_bytes: Optional[bytes] = None,
         pdf_config: Optional[PdfConfig] = None,
     ):
         """
         Class responsible for parsing PDFs and returning raw text
 
         The page_range variable determines which pages are extracted.
         All pages are extracted by default.
         """
         self.file_path = file_path
+        self.file_bytes = file_bytes
 
         if pdf_config is None:
             pdf_config = PdfConfig()
 
         self.passwords = pdf_config.passwords
         self.page_range = slice(*pdf_config.page_range)
         self.page_bbox = pdf_config.page_bbox
 
     def open(self):
         """
         Opens and decrypts a PDF document
         """
-        logger.debug("Opening pdf from path %s", self.file_path)
         document = self.document
 
         if not document.is_encrypted:
             return document
 
         if not self.passwords:
             raise MissingPasswordError("No password found in PDF configuration")
@@ -124,23 +125,35 @@
         raise RuntimeError("Unable to retrieve pages")
 
     @cached_property
     def document(self) -> fitz.Document:
         """
         Returns a Python representation of a PDF document.
         """
-        return fitz.Document(self.file_path)
+        if self.file_path:
+            return fitz.Document(filename=self.file_path)
+
+        if self.file_bytes:
+            return fitz.Document(stream=self.file_bytes)
+
+        raise RuntimeError("Either file path or file bytestream must be passed")
 
     @cached_property
     def extractor(self) -> EncryptionMetadataExtractor:
         """
         Returns an instance of pdf2john, used to retrieve and return
         the encryption metadata from a PDF's encryption dictionary
         """
-        return EncryptionMetadataExtractor(self.file_path)
+        if self.file_path:
+            return EncryptionMetadataExtractor(file_name=self.file_path)
+
+        if self.file_bytes:
+            return EncryptionMetadataExtractor(file_bytes=self.file_bytes)
+
+        raise RuntimeError("Either file path or file bytestream must be passed")
 
     @staticmethod
     def _remove_vertical_text(page: fitz.Page):
         """Helper function to remove vertical text, based on writing direction (wdir).
 
         This helps avoid situations where the PDF is oddly parsed, due to vertical text
         inside the PDF.
```

### Comparing `monopoly_sg-0.7.5/src/monopoly/processor.py` & `monopoly_sg-0.7.6rc0/src/monopoly/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 
     credit_config: CreditStatementConfig
     debit_config: DebitStatementConfig
     statement: CreditStatement | DebitStatement
 
     def __init__(
         self,
-        file_path: Path,
+        file_name: str,
         parser: PdfParser,
         statement: CreditStatement | DebitStatement,
     ):
-        self.file_path = file_path
+        self.file_name = file_name
         self.parser = parser
         self.statement = statement
 
     def extract(self) -> CreditStatement | DebitStatement:
         """Extracts transactions from the statement, and performs
         a safety check to make sure that total transactions add up"""
         statement = self.statement
@@ -92,15 +92,15 @@
         statement: CreditStatement | DebitStatement,
         output_directory: Path,
     ):
         if isinstance(output_directory, str):
             output_directory = Path(output_directory)
 
         filename = generate_name(
-            file_path=self.file_path,
+            document=self.parser.document,
             format_type="file",
             statement_config=statement.statement_config,
             statement_type=statement.statement_type,
             statement_date=statement.statement_date,
         )
 
         output_path = output_directory / filename
```

### Comparing `monopoly_sg-0.7.5/src/monopoly/processors/__init__.py` & `monopoly_sg-0.7.6rc0/src/monopoly/processors/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,25 +32,33 @@
 
 
 class UnsupportedBankError(Exception):
     """Raised when a processor cannot be found for a specific bank"""
 
 
 def detect_processor(
-    file_path: Path, passwords: Optional[list[SecretStr]] = None
+    file_path: Optional[Path] = None,
+    file_bytes: Optional[bytes] = None,
+    passwords: Optional[list[SecretStr]] = None,
 ) -> ProcessorBase:
     """
     Reads the encryption metadata or actual metadata (if the PDF is not encrypted),
     and checks for a bank based on unique identifiers.
     """
-    parser = PdfParser(file_path, pdf_config=PdfConfig(passwords=passwords))
+    parser = PdfParser(
+        file_path=file_path,
+        file_bytes=file_bytes,
+        pdf_config=PdfConfig(passwords=passwords),
+    )
     for processor in processors:
         metadata_items = processor.get_identifiers(parser)
         if is_bank_identified(metadata_items, processor):
-            return processor(file_path=file_path, passwords=passwords)
+            return processor(
+                file_path=file_path, file_bytes=file_bytes, passwords=passwords
+            )
 
     raise UnsupportedBankError("This bank is currently unsupported")
 
 
 def is_bank_identified(
     metadata_items: list[EncryptionIdentifier | MetadataIdentifier],
     processor: Type[ProcessorBase],
```

### Comparing `monopoly_sg-0.7.5/src/monopoly/processors/base.py` & `monopoly_sg-0.7.6rc0/src/monopoly/processors/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,32 +23,35 @@
 
     # overwritten if pdf_config exists in bank class
     pdf_config: PdfConfig = PdfConfig()
     identifiers: list[EncryptionIdentifier | MetadataIdentifier]
 
     def __init__(
         self,
-        file_path: Path,
+        file_path: Optional[Path] = None,
+        file_bytes: Optional[bytes] = None,
         passwords: Optional[list[SecretStr]] = None,
     ):
         # this allows the user to override the default pydantic password
         # and supply their own password via the bank subclasses
         if passwords:
             self.pdf_config.passwords = passwords
 
-        parser = PdfParser(file_path, self.pdf_config)
+        parser = PdfParser(
+            file_path=file_path, file_bytes=file_bytes, pdf_config=self.pdf_config
+        )
 
         self.pages = parser.get_pages()
         self.document = parser.document
 
         if isinstance(file_path, str):
             file_path = Path(file_path)
 
         super().__init__(
-            parser=parser, file_path=file_path, statement=self.get_statement()
+            parser=parser, file_name=self.document.name, statement=self.get_statement()
         )
 
     @cached_property
     def statement_config(self) -> CreditStatementConfig | DebitStatementConfig:
         if self.debit_header and self.debit_config:
             return self.debit_config
         return self.credit_config
```

### Comparing `monopoly_sg-0.7.5/src/monopoly/processors/citibank/citibank.py` & `monopoly_sg-0.7.6rc0/src/monopoly/processors/citibank/citibank.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/src/monopoly/processors/dbs/dbs.py` & `monopoly_sg-0.7.6rc0/src/monopoly/processors/dbs/dbs.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/src/monopoly/processors/example_bank.py` & `monopoly_sg-0.7.6rc0/src/monopoly/processors/example_bank.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/src/monopoly/processors/hsbc/hsbc.py` & `monopoly_sg-0.7.6rc0/src/monopoly/processors/hsbc/hsbc.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/src/monopoly/processors/ocbc/ocbc.py` & `monopoly_sg-0.7.6rc0/src/monopoly/processors/ocbc/ocbc.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/src/monopoly/processors/standard_chartered/standard_chartered.py` & `monopoly_sg-0.7.6rc0/src/monopoly/processors/standard_chartered/standard_chartered.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/src/monopoly/statements/base.py` & `monopoly_sg-0.7.6rc0/src/monopoly/statements/base.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/src/monopoly/statements/credit_statement.py` & `monopoly_sg-0.7.6rc0/src/monopoly/statements/credit_statement.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/src/monopoly/statements/debit_statement.py` & `monopoly_sg-0.7.6rc0/src/monopoly/statements/debit_statement.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/tests/test_utils/skip.py` & `monopoly_sg-0.7.6rc0/tests/test_utils/skip.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.5/PKG-INFO` & `monopoly_sg-0.7.6rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: monopoly-sg
-Version: 0.7.5
+Version: 0.7.6rc0
 Summary: PDF parsing for Singaporean banks
 Home-page: https://github.com/benjamin-awd/monopoly
 License: MIT
 Author: benjamin-awd
 Author-email: benjamindornel@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: mypy (>=1.7.1,<2.0.0)
 Requires-Dist: pandas (>=2.1.3,<3.0.0)
-Requires-Dist: pdf2john (>=0.1.10,<0.2.0)
+Requires-Dist: pdf2john (>=0.2.0,<0.3.0)
 Requires-Dist: pdftotext (>=2.2.2,<3.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
 Requires-Dist: pymupdf (>=1.23.7,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Project-URL: Repository, https://github.com/benjamin-awd/monopoly
```

