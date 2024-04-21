# Comparing `tmp/pyseoanalyzer-4.0.6.tar.gz` & `tmp/pyseoanalyzer-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyseoanalyzer-4.0.6.tar", last modified: Sun Jan 16 01:03:46 2022, max compression
+gzip compressed data, was "pyseoanalyzer-4.0.7.tar", last modified: Sat Oct  1 16:43:42 2022, max compression
```

## Comparing `pyseoanalyzer-4.0.6.tar` & `pyseoanalyzer-4.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 sethblack   (501) staff       (20)        0 2022-01-16 01:03:46.903131 pyseoanalyzer-4.0.6/
--rw-r--r--   0 sethblack   (501) staff       (20)     1479 2021-01-12 17:32:28.000000 pyseoanalyzer-4.0.6/LICENSE
--rw-r--r--   0 sethblack   (501) staff       (20)       63 2021-01-12 17:21:33.000000 pyseoanalyzer-4.0.6/MANIFEST.in
--rw-r--r--   0 sethblack   (501) staff       (20)     3984 2022-01-16 01:03:46.903010 pyseoanalyzer-4.0.6/PKG-INFO
--rw-r--r--   0 sethblack   (501) staff       (20)     2170 2021-12-03 23:08:28.000000 pyseoanalyzer-4.0.6/README.md
-drwxr-xr-x   0 sethblack   (501) staff       (20)        0 2022-01-16 01:03:46.899530 pyseoanalyzer-4.0.6/pyseoanalyzer.egg-info/
--rw-r--r--   0 sethblack   (501) staff       (20)     3984 2022-01-16 01:03:46.000000 pyseoanalyzer-4.0.6/pyseoanalyzer.egg-info/PKG-INFO
--rw-r--r--   0 sethblack   (501) staff       (20)      568 2022-01-16 01:03:46.000000 pyseoanalyzer-4.0.6/pyseoanalyzer.egg-info/SOURCES.txt
--rw-r--r--   0 sethblack   (501) staff       (20)        1 2022-01-16 01:03:46.000000 pyseoanalyzer-4.0.6/pyseoanalyzer.egg-info/dependency_links.txt
--rw-r--r--   0 sethblack   (501) staff       (20)       58 2022-01-16 01:03:46.000000 pyseoanalyzer-4.0.6/pyseoanalyzer.egg-info/entry_points.txt
--rw-r--r--   0 sethblack   (501) staff       (20)        1 2021-01-18 20:38:11.000000 pyseoanalyzer-4.0.6/pyseoanalyzer.egg-info/not-zip-safe
--rw-r--r--   0 sethblack   (501) staff       (20)       52 2022-01-16 01:03:46.000000 pyseoanalyzer-4.0.6/pyseoanalyzer.egg-info/requires.txt
--rw-r--r--   0 sethblack   (501) staff       (20)       18 2022-01-16 01:03:46.000000 pyseoanalyzer-4.0.6/pyseoanalyzer.egg-info/top_level.txt
-drwxr-xr-x   0 sethblack   (501) staff       (20)        0 2022-01-16 01:03:46.901194 pyseoanalyzer-4.0.6/seoanalyzer/
--rwxr-xr-x   0 sethblack   (501) staff       (20)       79 2021-01-12 17:21:33.000000 pyseoanalyzer-4.0.6/seoanalyzer/__init__.py
--rw-r--r--   0 sethblack   (501) staff       (20)     1356 2021-01-12 17:21:33.000000 pyseoanalyzer-4.0.6/seoanalyzer/__main__.py
--rw-r--r--   0 sethblack   (501) staff       (20)     1656 2021-12-03 23:08:28.000000 pyseoanalyzer-4.0.6/seoanalyzer/analyzer.py
--rw-r--r--   0 sethblack   (501) staff       (20)      463 2021-04-10 21:03:49.000000 pyseoanalyzer-4.0.6/seoanalyzer/http.py
--rw-r--r--   0 sethblack   (501) staff       (20)    16279 2021-12-03 23:08:28.000000 pyseoanalyzer-4.0.6/seoanalyzer/page.py
--rw-r--r--   0 sethblack   (501) staff       (20)     4362 2021-01-12 17:21:33.000000 pyseoanalyzer-4.0.6/seoanalyzer/stemmer.py
-drwxr-xr-x   0 sethblack   (501) staff       (20)        0 2022-01-16 01:03:46.901414 pyseoanalyzer-4.0.6/seoanalyzer/templates/
--rw-r--r--   0 sethblack   (501) staff       (20)     4937 2021-01-12 18:12:35.000000 pyseoanalyzer-4.0.6/seoanalyzer/templates/index.html
--rw-r--r--   0 sethblack   (501) staff       (20)     2868 2021-12-03 23:08:28.000000 pyseoanalyzer-4.0.6/seoanalyzer/website.py
--rw-r--r--   0 sethblack   (501) staff       (20)       38 2022-01-16 01:03:46.903168 pyseoanalyzer-4.0.6/setup.cfg
--rwxr-xr-x   0 sethblack   (501) staff       (20)     1753 2022-01-16 01:03:35.000000 pyseoanalyzer-4.0.6/setup.py
-drwxr-xr-x   0 sethblack   (501) staff       (20)        0 2022-01-16 01:03:46.902701 pyseoanalyzer-4.0.6/tests/
--rw-r--r--   0 sethblack   (501) staff       (20)        0 2021-01-12 17:21:33.000000 pyseoanalyzer-4.0.6/tests/__init__.py
--rw-r--r--   0 sethblack   (501) staff       (20)      491 2021-01-12 17:31:20.000000 pyseoanalyzer-4.0.6/tests/test_analyzer.py
--rw-r--r--   0 sethblack   (501) staff       (20)      118 2021-01-12 17:21:33.000000 pyseoanalyzer-4.0.6/tests/test_http.py
--rw-r--r--   0 sethblack   (501) staff       (20)      636 2021-01-12 17:24:22.000000 pyseoanalyzer-4.0.6/tests/test_page.py
+drwxr-xr-x   0 sethblack   (501) staff       (20)        0 2022-10-01 16:43:42.266293 pyseoanalyzer-4.0.7/
+-rw-r--r--   0 sethblack   (501) staff       (20)     1479 2022-10-01 16:40:01.000000 pyseoanalyzer-4.0.7/LICENSE
+-rw-r--r--   0 sethblack   (501) staff       (20)       63 2022-10-01 16:40:01.000000 pyseoanalyzer-4.0.7/MANIFEST.in
+-rw-r--r--   0 sethblack   (501) staff       (20)     3222 2022-10-01 16:43:42.266181 pyseoanalyzer-4.0.7/PKG-INFO
+-rw-r--r--   0 sethblack   (501) staff       (20)     2170 2022-10-01 16:40:01.000000 pyseoanalyzer-4.0.7/README.md
+drwxr-xr-x   0 sethblack   (501) staff       (20)        0 2022-10-01 16:43:42.264035 pyseoanalyzer-4.0.7/pyseoanalyzer.egg-info/
+-rw-r--r--   0 sethblack   (501) staff       (20)     3222 2022-10-01 16:43:42.000000 pyseoanalyzer-4.0.7/pyseoanalyzer.egg-info/PKG-INFO
+-rw-r--r--   0 sethblack   (501) staff       (20)      568 2022-10-01 16:43:42.000000 pyseoanalyzer-4.0.7/pyseoanalyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 sethblack   (501) staff       (20)        1 2022-10-01 16:43:42.000000 pyseoanalyzer-4.0.7/pyseoanalyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 sethblack   (501) staff       (20)       57 2022-10-01 16:43:42.000000 pyseoanalyzer-4.0.7/pyseoanalyzer.egg-info/entry_points.txt
+-rw-r--r--   0 sethblack   (501) staff       (20)        1 2022-10-01 16:43:42.000000 pyseoanalyzer-4.0.7/pyseoanalyzer.egg-info/not-zip-safe
+-rw-r--r--   0 sethblack   (501) staff       (20)       52 2022-10-01 16:43:42.000000 pyseoanalyzer-4.0.7/pyseoanalyzer.egg-info/requires.txt
+-rw-r--r--   0 sethblack   (501) staff       (20)       18 2022-10-01 16:43:42.000000 pyseoanalyzer-4.0.7/pyseoanalyzer.egg-info/top_level.txt
+drwxr-xr-x   0 sethblack   (501) staff       (20)        0 2022-10-01 16:43:42.265129 pyseoanalyzer-4.0.7/seoanalyzer/
+-rwxr-xr-x   0 sethblack   (501) staff       (20)       79 2022-10-01 16:40:01.000000 pyseoanalyzer-4.0.7/seoanalyzer/__init__.py
+-rw-r--r--   0 sethblack   (501) staff       (20)     1356 2022-10-01 16:40:01.000000 pyseoanalyzer-4.0.7/seoanalyzer/__main__.py
+-rw-r--r--   0 sethblack   (501) staff       (20)     1656 2022-10-01 16:40:01.000000 pyseoanalyzer-4.0.7/seoanalyzer/analyzer.py
+-rw-r--r--   0 sethblack   (501) staff       (20)      463 2022-10-01 16:40:01.000000 pyseoanalyzer-4.0.7/seoanalyzer/http.py
+-rw-r--r--   0 sethblack   (501) staff       (20)    16507 2022-10-01 16:40:01.000000 pyseoanalyzer-4.0.7/seoanalyzer/page.py
+-rw-r--r--   0 sethblack   (501) staff       (20)     4362 2022-10-01 16:40:01.000000 pyseoanalyzer-4.0.7/seoanalyzer/stemmer.py
+drwxr-xr-x   0 sethblack   (501) staff       (20)        0 2022-10-01 16:43:42.265399 pyseoanalyzer-4.0.7/seoanalyzer/templates/
+-rw-r--r--   0 sethblack   (501) staff       (20)     4937 2022-10-01 16:40:01.000000 pyseoanalyzer-4.0.7/seoanalyzer/templates/index.html
+-rw-r--r--   0 sethblack   (501) staff       (20)     2868 2022-10-01 16:40:01.000000 pyseoanalyzer-4.0.7/seoanalyzer/website.py
+-rw-r--r--   0 sethblack   (501) staff       (20)       38 2022-10-01 16:43:42.266326 pyseoanalyzer-4.0.7/setup.cfg
+-rwxr-xr-x   0 sethblack   (501) staff       (20)     1753 2022-10-01 16:40:20.000000 pyseoanalyzer-4.0.7/setup.py
+drwxr-xr-x   0 sethblack   (501) staff       (20)        0 2022-10-01 16:43:42.266009 pyseoanalyzer-4.0.7/tests/
+-rw-r--r--   0 sethblack   (501) staff       (20)        0 2022-10-01 16:40:01.000000 pyseoanalyzer-4.0.7/tests/__init__.py
+-rw-r--r--   0 sethblack   (501) staff       (20)      491 2022-10-01 16:40:01.000000 pyseoanalyzer-4.0.7/tests/test_analyzer.py
+-rw-r--r--   0 sethblack   (501) staff       (20)      118 2022-10-01 16:40:01.000000 pyseoanalyzer-4.0.7/tests/test_http.py
+-rw-r--r--   0 sethblack   (501) staff       (20)      636 2022-10-01 16:40:01.000000 pyseoanalyzer-4.0.7/tests/test_page.py
```

### Comparing `pyseoanalyzer-4.0.6/LICENSE` & `pyseoanalyzer-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyseoanalyzer-4.0.6/PKG-INFO` & `pyseoanalyzer-4.0.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,115 @@
 Metadata-Version: 2.1
 Name: pyseoanalyzer
-Version: 4.0.6
+Version: 4.0.7
 Summary: An SEO tool that analyzes the structure of a site, crawls the site, count words in the body of the site and warns of any technical SEO issues.
 Home-page: https://github.com/sethblack/python-seo-analyzer
 Author: Seth Black
 Author-email: sblack@sethserver.com
-License: UNKNOWN
-Description: Python SEO Analyzer
-        ===================
-        
-        [![Googling Google by taleas.com](https://www.taleas.com/static/images/comics/googling-google.jpg "Googling Google by taleas.com")](https://www.taleas.com/comics/googling-google.html)
-        
-        An SEO tool that analyzes the structure of a site, crawls the site, counts words in the body of the site and warns of any technical SEO issues.
-        
-        Requires Python 3.6+, BeautifulSoup4 and urllib3.
-        
-        Installation
-        ------------
-        
-        ### PIP
-        
-        ```
-        pip3 install pyseoanalyzer
-        ```
-        
-        ### Docker
-        
-        ```
-        docker run sethblack/python-seo-analyzer [ARGS ...]
-        ```
-        
-        Command-line Usage
-        ------------------
-        
-        If you run without a sitemap it will start crawling at the homepage.
-        
-        ```sh
-        seoanalyze http://www.domain.com/
-        ```
-        
-        Or you can specify the path to a sitmap to seed the urls to scan list.
-        
-        ```sh
-        seoanalyze http://www.domain.com/ --sitemap path/to/sitemap.xml
-        ```
-        
-        HTML output can be generated from the analysis instead of json.
-        
-        ```sh
-        seoanalyze http://www.domain.com/ --output-format html
-        ```
-        
-        API
-        ---
-        
-        The `analyze` function returns a dictionary with the results of the crawl.
-        
-        ```python
-        from seoanalyzer import analyze
-        
-        output = analyze(site, sitemap)
-        
-        print(output)
-        ```
-        
-        In order to analyze heading tags (h1-h6) and other extra additional tags as well, the following options can be passed to the `analyze` function
-        ```python
-        from seoanalyzer import analyze
-        
-        output = analyze(site, sitemap, analyze_headings=True, analyze_extra_tags=True)
-        
-        print(output)
-        ```
-        
-        By default, the `analyze` function analyzes all the existing inner links as well, which might be time consuming.
-        This default behaviour can be changed to analyze only the provided URL by passing the following option to the `analyze` function
-        ```python
-        from seoanalyzer import analyze
-        
-        output = analyze(site, sitemap, follow_links=False)
-        
-        print(output)
-        ```
-        
-        Alternatively, you can run the analysis as a script from the seoanalyzer folder.
-        
-        ```sh
-        python analyzer.py https://www.sethserver.com/ -f html > results.html
-        ```
-        
-        Notes
-        -----
-        
-        If you get `requests.exceptions.SSLError` at either the command-line or via the python-API, try using:
-         - http://www.foo.bar
-         
-         **instead** of..
-         
-         -  https://www.foo.bar
-        
 Keywords: search engine optimization,seo,website parser,crawler,scraper
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Python SEO Analyzer
+===================
+
+[![Googling Google by taleas.com](https://www.taleas.com/static/images/comics/googling-google.jpg "Googling Google by taleas.com")](https://www.taleas.com/comics/googling-google.html)
+
+An SEO tool that analyzes the structure of a site, crawls the site, counts words in the body of the site and warns of any technical SEO issues.
+
+Requires Python 3.6+, BeautifulSoup4 and urllib3.
+
+Installation
+------------
+
+### PIP
+
+```
+pip3 install pyseoanalyzer
+```
+
+### Docker
+
+```
+docker run sethblack/python-seo-analyzer [ARGS ...]
+```
+
+Command-line Usage
+------------------
+
+If you run without a sitemap it will start crawling at the homepage.
+
+```sh
+seoanalyze http://www.domain.com/
+```
+
+Or you can specify the path to a sitmap to seed the urls to scan list.
+
+```sh
+seoanalyze http://www.domain.com/ --sitemap path/to/sitemap.xml
+```
+
+HTML output can be generated from the analysis instead of json.
+
+```sh
+seoanalyze http://www.domain.com/ --output-format html
+```
+
+API
+---
+
+The `analyze` function returns a dictionary with the results of the crawl.
+
+```python
+from seoanalyzer import analyze
+
+output = analyze(site, sitemap)
+
+print(output)
+```
+
+In order to analyze heading tags (h1-h6) and other extra additional tags as well, the following options can be passed to the `analyze` function
+```python
+from seoanalyzer import analyze
+
+output = analyze(site, sitemap, analyze_headings=True, analyze_extra_tags=True)
+
+print(output)
+```
+
+By default, the `analyze` function analyzes all the existing inner links as well, which might be time consuming.
+This default behaviour can be changed to analyze only the provided URL by passing the following option to the `analyze` function
+```python
+from seoanalyzer import analyze
+
+output = analyze(site, sitemap, follow_links=False)
+
+print(output)
+```
+
+Alternatively, you can run the analysis as a script from the seoanalyzer folder.
+
+```sh
+python analyzer.py https://www.sethserver.com/ -f html > results.html
+```
+
+Notes
+-----
+
+If you get `requests.exceptions.SSLError` at either the command-line or via the python-API, try using:
+ - http://www.foo.bar
+ 
+ **instead** of..
+ 
+ -  https://www.foo.bar
```

### Comparing `pyseoanalyzer-4.0.6/README.md` & `pyseoanalyzer-4.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyseoanalyzer-4.0.6/pyseoanalyzer.egg-info/PKG-INFO` & `pyseoanalyzer-4.0.7/pyseoanalyzer.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,115 @@
 Metadata-Version: 2.1
 Name: pyseoanalyzer
-Version: 4.0.6
+Version: 4.0.7
 Summary: An SEO tool that analyzes the structure of a site, crawls the site, count words in the body of the site and warns of any technical SEO issues.
 Home-page: https://github.com/sethblack/python-seo-analyzer
 Author: Seth Black
 Author-email: sblack@sethserver.com
-License: UNKNOWN
-Description: Python SEO Analyzer
-        ===================
-        
-        [![Googling Google by taleas.com](https://www.taleas.com/static/images/comics/googling-google.jpg "Googling Google by taleas.com")](https://www.taleas.com/comics/googling-google.html)
-        
-        An SEO tool that analyzes the structure of a site, crawls the site, counts words in the body of the site and warns of any technical SEO issues.
-        
-        Requires Python 3.6+, BeautifulSoup4 and urllib3.
-        
-        Installation
-        ------------
-        
-        ### PIP
-        
-        ```
-        pip3 install pyseoanalyzer
-        ```
-        
-        ### Docker
-        
-        ```
-        docker run sethblack/python-seo-analyzer [ARGS ...]
-        ```
-        
-        Command-line Usage
-        ------------------
-        
-        If you run without a sitemap it will start crawling at the homepage.
-        
-        ```sh
-        seoanalyze http://www.domain.com/
-        ```
-        
-        Or you can specify the path to a sitmap to seed the urls to scan list.
-        
-        ```sh
-        seoanalyze http://www.domain.com/ --sitemap path/to/sitemap.xml
-        ```
-        
-        HTML output can be generated from the analysis instead of json.
-        
-        ```sh
-        seoanalyze http://www.domain.com/ --output-format html
-        ```
-        
-        API
-        ---
-        
-        The `analyze` function returns a dictionary with the results of the crawl.
-        
-        ```python
-        from seoanalyzer import analyze
-        
-        output = analyze(site, sitemap)
-        
-        print(output)
-        ```
-        
-        In order to analyze heading tags (h1-h6) and other extra additional tags as well, the following options can be passed to the `analyze` function
-        ```python
-        from seoanalyzer import analyze
-        
-        output = analyze(site, sitemap, analyze_headings=True, analyze_extra_tags=True)
-        
-        print(output)
-        ```
-        
-        By default, the `analyze` function analyzes all the existing inner links as well, which might be time consuming.
-        This default behaviour can be changed to analyze only the provided URL by passing the following option to the `analyze` function
-        ```python
-        from seoanalyzer import analyze
-        
-        output = analyze(site, sitemap, follow_links=False)
-        
-        print(output)
-        ```
-        
-        Alternatively, you can run the analysis as a script from the seoanalyzer folder.
-        
-        ```sh
-        python analyzer.py https://www.sethserver.com/ -f html > results.html
-        ```
-        
-        Notes
-        -----
-        
-        If you get `requests.exceptions.SSLError` at either the command-line or via the python-API, try using:
-         - http://www.foo.bar
-         
-         **instead** of..
-         
-         -  https://www.foo.bar
-        
 Keywords: search engine optimization,seo,website parser,crawler,scraper
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Python SEO Analyzer
+===================
+
+[![Googling Google by taleas.com](https://www.taleas.com/static/images/comics/googling-google.jpg "Googling Google by taleas.com")](https://www.taleas.com/comics/googling-google.html)
+
+An SEO tool that analyzes the structure of a site, crawls the site, counts words in the body of the site and warns of any technical SEO issues.
+
+Requires Python 3.6+, BeautifulSoup4 and urllib3.
+
+Installation
+------------
+
+### PIP
+
+```
+pip3 install pyseoanalyzer
+```
+
+### Docker
+
+```
+docker run sethblack/python-seo-analyzer [ARGS ...]
+```
+
+Command-line Usage
+------------------
+
+If you run without a sitemap it will start crawling at the homepage.
+
+```sh
+seoanalyze http://www.domain.com/
+```
+
+Or you can specify the path to a sitmap to seed the urls to scan list.
+
+```sh
+seoanalyze http://www.domain.com/ --sitemap path/to/sitemap.xml
+```
+
+HTML output can be generated from the analysis instead of json.
+
+```sh
+seoanalyze http://www.domain.com/ --output-format html
+```
+
+API
+---
+
+The `analyze` function returns a dictionary with the results of the crawl.
+
+```python
+from seoanalyzer import analyze
+
+output = analyze(site, sitemap)
+
+print(output)
+```
+
+In order to analyze heading tags (h1-h6) and other extra additional tags as well, the following options can be passed to the `analyze` function
+```python
+from seoanalyzer import analyze
+
+output = analyze(site, sitemap, analyze_headings=True, analyze_extra_tags=True)
+
+print(output)
+```
+
+By default, the `analyze` function analyzes all the existing inner links as well, which might be time consuming.
+This default behaviour can be changed to analyze only the provided URL by passing the following option to the `analyze` function
+```python
+from seoanalyzer import analyze
+
+output = analyze(site, sitemap, follow_links=False)
+
+print(output)
+```
+
+Alternatively, you can run the analysis as a script from the seoanalyzer folder.
+
+```sh
+python analyzer.py https://www.sethserver.com/ -f html > results.html
+```
+
+Notes
+-----
+
+If you get `requests.exceptions.SSLError` at either the command-line or via the python-API, try using:
+ - http://www.foo.bar
+ 
+ **instead** of..
+ 
+ -  https://www.foo.bar
```

### Comparing `pyseoanalyzer-4.0.6/pyseoanalyzer.egg-info/SOURCES.txt` & `pyseoanalyzer-4.0.7/pyseoanalyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyseoanalyzer-4.0.6/seoanalyzer/__main__.py` & `pyseoanalyzer-4.0.7/seoanalyzer/__main__.py`

 * *Files identical despite different names*

### Comparing `pyseoanalyzer-4.0.6/seoanalyzer/analyzer.py` & `pyseoanalyzer-4.0.7/seoanalyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `pyseoanalyzer-4.0.6/seoanalyzer/page.py` & `pyseoanalyzer-4.0.7/seoanalyzer/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,18 @@
     'title': '//title/text()',
     'meta_desc': '//meta[@name="description"]/@content',
     'viewport': '//meta[@name="viewport"]/@content',
     'charset': '//meta[@charset]/@charset',
     'canonical': '//link[@rel="canonical"]/@href',
     'alt_href': '//link[@rel="alternate"]/@href',
     'alt_hreflang': '//link[@rel="alternate"]/@hreflang',
+    'og_title': '//meta[@property="og:title"]/@content',
+    'og_desc': '//meta[@property="og:description"]/@content',
+    'og_url': '//meta[@property="og:url"]/@content',
+    'og_image': '//meta[@property="og:image"]/@content'
 }
 
 IMAGE_EXTENSIONS = set(['.img', '.png', '.jpg', '.jpeg', '.gif', '.bmp', '.svg', '.webp', '.avif',])
 
 
 class Page():
     """
```

### Comparing `pyseoanalyzer-4.0.6/seoanalyzer/stemmer.py` & `pyseoanalyzer-4.0.7/seoanalyzer/stemmer.py`

 * *Files identical despite different names*

### Comparing `pyseoanalyzer-4.0.6/seoanalyzer/templates/index.html` & `pyseoanalyzer-4.0.7/seoanalyzer/templates/index.html`

 * *Files identical despite different names*

### Comparing `pyseoanalyzer-4.0.6/seoanalyzer/website.py` & `pyseoanalyzer-4.0.7/seoanalyzer/website.py`

 * *Files identical despite different names*

### Comparing `pyseoanalyzer-4.0.6/setup.py` & `pyseoanalyzer-4.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyseoanalyzer',
-    version='4.0.6',
+    version='4.0.7',
     description='An SEO tool that analyzes the structure of a site, crawls the site, count words in the body of the site and warns of any technical SEO issues.',
     author='Seth Black',
     author_email='sblack@sethserver.com',
     url='https://github.com/sethblack/python-seo-analyzer',
     packages=find_packages(),
     keywords=['search engine optimization', 'seo', 'website parser', 'crawler', 'scraper',],
     package_data={'seoanalyzer': ['templates/index.html',]},
```

### Comparing `pyseoanalyzer-4.0.6/tests/test_page.py` & `pyseoanalyzer-4.0.7/tests/test_page.py`

 * *Files identical despite different names*

