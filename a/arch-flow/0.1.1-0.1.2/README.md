# Comparing `tmp/arch_flow-0.1.1.tar.gz` & `tmp/arch_flow-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arch_flow-0.1.1.tar", last modified: Thu Apr 18 04:04:02 2024, max compression
+gzip compressed data, was "arch_flow-0.1.2.tar", last modified: Sun Apr 21 05:44:11 2024, max compression
```

## Comparing `arch_flow-0.1.1.tar` & `arch_flow-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 04:04:02.249727 arch_flow-0.1.1/
--rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.1.1/LICENCE
--rw-rw-rw-   0        0        0      981 2024-04-18 04:04:02.248222 arch_flow-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     6634 2024-04-18 01:45:54.000000 arch_flow-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 04:04:02.159965 arch_flow-0.1.1/arch_flow/
--rw-rw-rw-   0        0        0     4506 2024-04-16 07:34:12.000000 arch_flow-0.1.1/arch_flow/ArchFlow.py
--rw-rw-rw-   0        0        0      877 2024-04-16 07:34:12.000000 arch_flow-0.1.1/arch_flow/DirectoryCreator.py
--rw-rw-rw-   0        0        0     3198 2024-04-17 08:26:17.000000 arch_flow-0.1.1/arch_flow/DirectoryExplorer.py
--rw-rw-rw-   0        0        0     3130 2024-04-16 07:34:12.000000 arch_flow-0.1.1/arch_flow/StringManipulator.py
--rw-rw-rw-   0        0        0       32 2024-04-16 07:33:26.000000 arch_flow-0.1.1/arch_flow/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 04:04:02.198059 arch_flow-0.1.1/arch_flow/exceptions/
--rw-rw-rw-   0        0        0      594 2024-04-16 07:34:12.000000 arch_flow-0.1.1/arch_flow/exceptions/ExceptionHandler.py
--rw-rw-rw-   0        0        0     1132 2024-04-16 07:34:12.000000 arch_flow-0.1.1/arch_flow/exceptions/FileOrDirectoryExistsError.py
--rw-rw-rw-   0        0        0      631 2024-04-16 07:34:12.000000 arch_flow-0.1.1/arch_flow/exceptions/NotFoundException.py
-drwxrwxrwx   0        0        0        0 2024-04-18 04:04:02.223658 arch_flow-0.1.1/arch_flow/implementations/
--rw-rw-rw-   0        0        0     2191 2024-04-16 07:34:12.000000 arch_flow-0.1.1/arch_flow/implementations/DirectoryCreatorImplementation.py
--rw-rw-rw-   0        0        0     7367 2024-04-16 07:34:12.000000 arch_flow-0.1.1/arch_flow/implementations/DirectoryExplorerImplementation.py
--rw-rw-rw-   0        0        0     7653 2024-03-15 22:56:29.000000 arch_flow-0.1.1/arch_flow/implementations/StringManipulatorImplementation.py
-drwxrwxrwx   0        0        0        0 2024-04-18 04:04:02.232739 arch_flow-0.1.1/arch_flow/output/
--rw-rw-rw-   0        0        0     2372 2024-03-15 22:56:29.000000 arch_flow-0.1.1/arch_flow/output/OutputHandler.py
-drwxrwxrwx   0        0        0        0 2024-04-18 04:04:02.246221 arch_flow-0.1.1/arch_flow/utils/
--rw-rw-rw-   0        0        0      470 2024-03-15 22:56:29.000000 arch_flow-0.1.1/arch_flow/utils/DirectoryExplorerUtil.py
--rw-rw-rw-   0        0        0     1801 2024-04-16 07:34:12.000000 arch_flow-0.1.1/arch_flow/utils/Filter.py
-drwxrwxrwx   0        0        0        0 2024-04-18 04:04:02.247223 arch_flow-0.1.1/arch_flow.egg-info/
--rw-rw-rw-   0        0        0      981 2024-04-18 04:04:02.000000 arch_flow-0.1.1/arch_flow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      743 2024-04-18 04:04:02.000000 arch_flow-0.1.1/arch_flow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 04:04:02.000000 arch_flow-0.1.1/arch_flow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-18 04:04:02.000000 arch_flow-0.1.1/arch_flow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-18 04:04:02.000000 arch_flow-0.1.1/arch_flow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 04:04:02.249727 arch_flow-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1182 2024-04-18 04:03:53.000000 arch_flow-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 05:44:11.393680 arch_flow-0.1.2/
+-rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.1.2/LICENCE
+-rw-rw-rw-   0        0        0      981 2024-04-21 05:44:11.392680 arch_flow-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6634 2024-04-18 01:45:54.000000 arch_flow-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 05:44:11.338681 arch_flow-0.1.2/arch_flow/
+-rw-rw-rw-   0        0        0     4393 2024-04-21 05:43:57.000000 arch_flow-0.1.2/arch_flow/ArchFlow.py
+-rw-rw-rw-   0        0        0      877 2024-04-16 07:34:12.000000 arch_flow-0.1.2/arch_flow/DirectoryCreator.py
+-rw-rw-rw-   0        0        0     3277 2024-04-21 05:43:57.000000 arch_flow-0.1.2/arch_flow/DirectoryExplorer.py
+-rw-rw-rw-   0        0        0     3130 2024-04-16 07:34:12.000000 arch_flow-0.1.2/arch_flow/StringManipulator.py
+-rw-rw-rw-   0        0        0       32 2024-04-16 07:33:26.000000 arch_flow-0.1.2/arch_flow/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 05:44:11.364681 arch_flow-0.1.2/arch_flow/exceptions/
+-rw-rw-rw-   0        0        0      594 2024-04-16 07:34:12.000000 arch_flow-0.1.2/arch_flow/exceptions/ExceptionHandler.py
+-rw-rw-rw-   0        0        0     1132 2024-04-16 07:34:12.000000 arch_flow-0.1.2/arch_flow/exceptions/FileOrDirectoryExistsError.py
+-rw-rw-rw-   0        0        0      631 2024-04-16 07:34:12.000000 arch_flow-0.1.2/arch_flow/exceptions/NotFoundException.py
+drwxrwxrwx   0        0        0        0 2024-04-21 05:44:11.376679 arch_flow-0.1.2/arch_flow/implementations/
+-rw-rw-rw-   0        0        0     2191 2024-04-16 07:34:12.000000 arch_flow-0.1.2/arch_flow/implementations/DirectoryCreatorImplementation.py
+-rw-rw-rw-   0        0        0     7196 2024-04-21 05:43:57.000000 arch_flow-0.1.2/arch_flow/implementations/DirectoryExplorerImplementation.py
+-rw-rw-rw-   0        0        0     7653 2024-03-15 22:56:29.000000 arch_flow-0.1.2/arch_flow/implementations/StringManipulatorImplementation.py
+drwxrwxrwx   0        0        0        0 2024-04-21 05:44:11.385681 arch_flow-0.1.2/arch_flow/output/
+-rw-rw-rw-   0        0        0     2372 2024-03-15 22:56:29.000000 arch_flow-0.1.2/arch_flow/output/OutputHandler.py
+drwxrwxrwx   0        0        0        0 2024-04-21 05:44:11.389681 arch_flow-0.1.2/arch_flow/utils/
+-rw-rw-rw-   0        0        0      470 2024-03-15 22:56:29.000000 arch_flow-0.1.2/arch_flow/utils/DirectoryExplorerUtil.py
+-rw-rw-rw-   0        0        0     1801 2024-04-16 07:34:12.000000 arch_flow-0.1.2/arch_flow/utils/Filter.py
+drwxrwxrwx   0        0        0        0 2024-04-21 05:44:11.391680 arch_flow-0.1.2/arch_flow.egg-info/
+-rw-rw-rw-   0        0        0      981 2024-04-21 05:44:11.000000 arch_flow-0.1.2/arch_flow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      743 2024-04-21 05:44:11.000000 arch_flow-0.1.2/arch_flow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 05:44:11.000000 arch_flow-0.1.2/arch_flow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-21 05:44:11.000000 arch_flow-0.1.2/arch_flow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-21 05:44:11.000000 arch_flow-0.1.2/arch_flow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 05:44:11.393680 arch_flow-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1182 2024-04-21 05:43:57.000000 arch_flow-0.1.2/setup.py
```

### Comparing `arch_flow-0.1.1/LICENCE` & `arch_flow-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.1/PKG-INFO` & `arch_flow-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arch-flow
-Version: 0.1.1
+Version: 0.1.2
 Summary: O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.
 Author: Carlos Vinicius Da Silva
 Author-email: vini989073599@gmail.com
 License: MIT License
 Keywords: arch flow
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `arch_flow-0.1.1/README.md` & `arch_flow-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.1/arch_flow/ArchFlow.py` & `arch_flow-0.1.2/arch_flow/ArchFlow.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,14 @@
         self.DirectoryCreator = DirectoryCreator()
         self.DirectoryExplorer = DirectoryExplorer()
         self.StringManipulator = StringManipulator()
         self.OutputHandler = OutputHandler()
         self.root_path = os.getcwd()
 
     @abstractmethod
-    def create_project(self, *args):
-        pass
-
-    @abstractmethod
     def functions_flow(self):
         pass
 
     def create_file_based_in_template(self, file_destination, file_name, template_file_name, args=None):
         file_destination = file_destination
         content = self.DirectoryExplorer.read_file_template(template_file_name)
         if args:
@@ -80,15 +76,15 @@
 
     def dictionary_of_standard_functions(self):
         dictionary_directory_creator = self.DirectoryCreator.dictionary_of_standard_functions()
         dictionary_directory_explorer = self.DirectoryExplorer.dictionary_of_standard_functions()
         dictionary_string_manipulator = self.StringManipulator.dictionary_of_standard_functions()
         dictionary_output_handler = self.OutputHandler.dictionary_of_standard_functions()
         functions_flow = self.functions_flow()
-        return {'create_project': self.create_project,
+        return {
                 'functions_flow': functions_flow,
                 'directory_creator': dictionary_directory_creator,
                 'directory_explorer': dictionary_directory_explorer,
                 'string_manipulator': dictionary_string_manipulator,
                 'output_handler': dictionary_output_handler,
                 'create_file_based_in_template': self.create_file_based_in_template
                 }
```

### Comparing `arch_flow-0.1.1/arch_flow/DirectoryCreator.py` & `arch_flow-0.1.2/arch_flow/DirectoryCreator.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.1/arch_flow/DirectoryExplorer.py` & `arch_flow-0.1.2/arch_flow/DirectoryExplorer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 from arch_flow.implementations.DirectoryExplorerImplementation import DirectoryExplorerImplementation
 
 
 class DirectoryExplorer:
-    def __init__(self, directory=None):
+    def __init__(self, directory=None, directory_template=None):
         self.implementation = DirectoryExplorerImplementation()
         self.directory = directory
+        self.directory_template = directory_template
         if directory is None:
             self.directory = os.getcwd()
 
     def set_directory(self, directory):
         self.directory = directory
 
     def get_directory(self):
```

### Comparing `arch_flow-0.1.1/arch_flow/StringManipulator.py` & `arch_flow-0.1.2/arch_flow/StringManipulator.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.1/arch_flow/exceptions/ExceptionHandler.py` & `arch_flow-0.1.2/arch_flow/exceptions/ExceptionHandler.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.1/arch_flow/exceptions/FileOrDirectoryExistsError.py` & `arch_flow-0.1.2/arch_flow/exceptions/FileOrDirectoryExistsError.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.1/arch_flow/exceptions/NotFoundException.py` & `arch_flow-0.1.2/arch_flow/exceptions/NotFoundException.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.1/arch_flow/implementations/DirectoryCreatorImplementation.py` & `arch_flow-0.1.2/arch_flow/implementations/DirectoryCreatorImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.1/arch_flow/implementations/DirectoryExplorerImplementation.py` & `arch_flow-0.1.2/arch_flow/implementations/DirectoryExplorerImplementation.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,19 +124,16 @@
             NotFoundException.fatal_not_found_error(f"Permission denied to access folder: {path_root}")
 
     @staticmethod
     def return_root_path(path_root):
         os.chdir(path_root)
         outuput.information_message(f"Returned to the original folder: {path_root}")
 
-    def read_file_template(self, name_template, required=False):
-        path_script = os.path.dirname(os.path.abspath(__file__))
-        root_base = os.path.abspath(os.path.join(path_script, '..', '..'))
-        root_path = os.path.join(root_base, 'use_cases')
-        file = self.find_only_one_file(root_path, name_template)
+    def read_file_template(self, name_template, directory_template, required=False):
+        file = self.find_only_one_file(directory_template, name_template)
         if file:
             return self.read_file(file[0], required)
         return ""
 
     @staticmethod
     def read_json_file(root_path_json):
         try:
```

### Comparing `arch_flow-0.1.1/arch_flow/implementations/StringManipulatorImplementation.py` & `arch_flow-0.1.2/arch_flow/implementations/StringManipulatorImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.1/arch_flow/output/OutputHandler.py` & `arch_flow-0.1.2/arch_flow/output/OutputHandler.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.1/arch_flow/utils/Filter.py` & `arch_flow-0.1.2/arch_flow/utils/Filter.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.1/arch_flow.egg-info/PKG-INFO` & `arch_flow-0.1.2/arch_flow.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arch-flow
-Version: 0.1.1
+Version: 0.1.2
 Summary: O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.
 Author: Carlos Vinicius Da Silva
 Author-email: vini989073599@gmail.com
 License: MIT License
 Keywords: arch flow
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `arch_flow-0.1.1/arch_flow.egg-info/SOURCES.txt` & `arch_flow-0.1.2/arch_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.1/setup.py` & `arch_flow-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='arch-flow',
-    version='0.1.1',
+    version='0.1.2',
     license='MIT License',
     author='Carlos Vinicius Da Silva',
     long_description="O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações. Inspirado no conceito de peças de Lego, o ArchFlow oferece uma variedade de módulos independentes, cada um com funcionalidades específicas. Esses módulos podem ser combinados de forma flexível para atender às necessidades de automação de diferentes projetos. Com uma arquitetura modular e uma ampla gama de funções, o ArchFlow permite aos desenvolvedores criar soluções eficientes e personalizadas, reduzindo o tempo e esforço necessários para o desenvolvimento de software.",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='arch flow',
     description=u'O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.',
```

