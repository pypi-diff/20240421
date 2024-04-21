# Comparing `tmp/zimo-web-screenshot-0.1.3.tar.gz` & `tmp/zimo-web-screenshot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimo-web-screenshot-0.1.3.tar", last modified: Mon Apr 15 11:52:42 2024, max compression
+gzip compressed data, was "zimo-web-screenshot-0.2.0.tar", last modified: Sun Apr 21 14:51:49 2024, max compression
```

## Comparing `zimo-web-screenshot-0.1.3.tar` & `zimo-web-screenshot-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-15 11:52:42.635949 zimo-web-screenshot-0.1.3/
--rw-r--r--   0 zimoluo    (501) staff       (20)     1057 2024-04-15 05:14:35.000000 zimo-web-screenshot-0.1.3/LICENSE
--rw-r--r--   0 zimoluo    (501) staff       (20)     2162 2024-04-15 11:52:42.636048 zimo-web-screenshot-0.1.3/PKG-INFO
--rw-r--r--   0 zimoluo    (501) staff       (20)     1657 2024-04-15 11:41:59.000000 zimo-web-screenshot-0.1.3/README.md
--rw-r--r--   0 zimoluo    (501) staff       (20)       79 2024-04-15 11:52:42.636227 zimo-web-screenshot-0.1.3/setup.cfg
--rw-r--r--   0 zimoluo    (501) staff       (20)      888 2024-04-15 11:52:33.000000 zimo-web-screenshot-0.1.3/setup.py
-drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-15 11:52:42.635106 zimo-web-screenshot-0.1.3/zimo_web_screenshot/
--rw-r--r--   0 zimoluo    (501) staff       (20)        0 2024-04-15 10:38:36.000000 zimo-web-screenshot-0.1.3/zimo_web_screenshot/__init__.py
--rw-r--r--   0 zimoluo    (501) staff       (20)     2307 2024-04-15 11:51:26.000000 zimo-web-screenshot-0.1.3/zimo_web_screenshot/screenshot.py
-drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-15 11:52:42.635839 zimo-web-screenshot-0.1.3/zimo_web_screenshot.egg-info/
--rw-r--r--   0 zimoluo    (501) staff       (20)     2162 2024-04-15 11:52:42.000000 zimo-web-screenshot-0.1.3/zimo_web_screenshot.egg-info/PKG-INFO
--rw-r--r--   0 zimoluo    (501) staff       (20)      362 2024-04-15 11:52:42.000000 zimo-web-screenshot-0.1.3/zimo_web_screenshot.egg-info/SOURCES.txt
--rw-r--r--   0 zimoluo    (501) staff       (20)        1 2024-04-15 11:52:42.000000 zimo-web-screenshot-0.1.3/zimo_web_screenshot.egg-info/dependency_links.txt
--rw-r--r--   0 zimoluo    (501) staff       (20)       76 2024-04-15 11:52:42.000000 zimo-web-screenshot-0.1.3/zimo_web_screenshot.egg-info/entry_points.txt
--rw-r--r--   0 zimoluo    (501) staff       (20)        9 2024-04-15 11:52:42.000000 zimo-web-screenshot-0.1.3/zimo_web_screenshot.egg-info/requires.txt
--rw-r--r--   0 zimoluo    (501) staff       (20)       20 2024-04-15 11:52:42.000000 zimo-web-screenshot-0.1.3/zimo_web_screenshot.egg-info/top_level.txt
+drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-21 14:51:49.452212 zimo-web-screenshot-0.2.0/
+-rw-r--r--   0 zimoluo    (501) staff       (20)     1057 2024-04-15 05:14:35.000000 zimo-web-screenshot-0.2.0/LICENSE
+-rw-r--r--   0 zimoluo    (501) staff       (20)     2162 2024-04-21 14:51:49.452296 zimo-web-screenshot-0.2.0/PKG-INFO
+-rw-r--r--   0 zimoluo    (501) staff       (20)     1657 2024-04-15 11:41:59.000000 zimo-web-screenshot-0.2.0/README.md
+-rw-r--r--   0 zimoluo    (501) staff       (20)       79 2024-04-21 14:51:49.452510 zimo-web-screenshot-0.2.0/setup.cfg
+-rw-r--r--   0 zimoluo    (501) staff       (20)      888 2024-04-21 14:46:41.000000 zimo-web-screenshot-0.2.0/setup.py
+drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-21 14:51:49.451124 zimo-web-screenshot-0.2.0/zimo_web_screenshot/
+-rw-r--r--   0 zimoluo    (501) staff       (20)        0 2024-04-15 10:38:36.000000 zimo-web-screenshot-0.2.0/zimo_web_screenshot/__init__.py
+-rw-r--r--   0 zimoluo    (501) staff       (20)     2753 2024-04-21 14:49:44.000000 zimo-web-screenshot-0.2.0/zimo_web_screenshot/screenshot.py
+drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-21 14:51:49.452094 zimo-web-screenshot-0.2.0/zimo_web_screenshot.egg-info/
+-rw-r--r--   0 zimoluo    (501) staff       (20)     2162 2024-04-21 14:51:49.000000 zimo-web-screenshot-0.2.0/zimo_web_screenshot.egg-info/PKG-INFO
+-rw-r--r--   0 zimoluo    (501) staff       (20)      362 2024-04-21 14:51:49.000000 zimo-web-screenshot-0.2.0/zimo_web_screenshot.egg-info/SOURCES.txt
+-rw-r--r--   0 zimoluo    (501) staff       (20)        1 2024-04-21 14:51:49.000000 zimo-web-screenshot-0.2.0/zimo_web_screenshot.egg-info/dependency_links.txt
+-rw-r--r--   0 zimoluo    (501) staff       (20)       76 2024-04-21 14:51:49.000000 zimo-web-screenshot-0.2.0/zimo_web_screenshot.egg-info/entry_points.txt
+-rw-r--r--   0 zimoluo    (501) staff       (20)        9 2024-04-21 14:51:49.000000 zimo-web-screenshot-0.2.0/zimo_web_screenshot.egg-info/requires.txt
+-rw-r--r--   0 zimoluo    (501) staff       (20)       20 2024-04-21 14:51:49.000000 zimo-web-screenshot-0.2.0/zimo_web_screenshot.egg-info/top_level.txt
```

### Comparing `zimo-web-screenshot-0.1.3/LICENSE` & `zimo-web-screenshot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zimo-web-screenshot-0.1.3/PKG-INFO` & `zimo-web-screenshot-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimo-web-screenshot
-Version: 0.1.3
+Version: 0.2.0
 Summary: A simple CLI tool to take screenshots of Zimo Web pages with Selenium.
 Home-page: https://github.com/zimoluo/zimo-web-screenshot-tool
 Author: Zimo Luo
 Author-email: abgkings0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zimo-web-screenshot-0.1.3/README.md` & `zimo-web-screenshot-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `zimo-web-screenshot-0.1.3/setup.py` & `zimo-web-screenshot-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zimo-web-screenshot',
-    version='0.1.3',
+    version='0.2.0',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'selenium',
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `zimo-web-screenshot-0.1.3/zimo_web_screenshot/screenshot.py` & `zimo-web-screenshot-0.2.0/zimo_web_screenshot/screenshot.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,41 +4,47 @@
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.by import By
 import time
 
 
 def take_screenshot(width, height, theme_name, pathname, delay, filename):
-    chrome_options = Options()
-    chrome_options.add_argument(f"--window-size={width},{height}")
-    chrome_options.add_argument("--headless")
-    chrome_options.add_argument("--hide-scrollbars")
-
-    driver = webdriver.Chrome(options=chrome_options)
-    driver.get(f"https://www.zimoluo.me/{pathname}")
-
-    WebDriverWait(driver, 10).until(
-        EC.element_to_be_clickable((By.ID, "menu-button"))).click()
-
-    time.sleep(0.4)
-
-    button_xpath = f"//button[.//img[@alt='Use {theme_name} theme']]"
-    WebDriverWait(driver, 10).until(
-        EC.element_to_be_clickable((By.XPATH, button_xpath))).click()
-    time.sleep(0.4)
-
-    WebDriverWait(driver, 10).until(
-        EC.element_to_be_clickable((By.ID, "menu-button"))).click()
-
-    time.sleep(1)
-
-    time.sleep(delay)
-
-    driver.save_screenshot(f'{filename}.png')
-    driver.quit()
+    try:
+        chrome_options = Options()
+        chrome_options.add_argument(f"--window-size={width},{height}")
+        chrome_options.add_argument("--headless")
+        chrome_options.add_argument("--hide-scrollbars")
+
+        driver = webdriver.Chrome(options=chrome_options)
+        driver.get(f"https://www.zimoluo.me/{pathname}")
+
+        WebDriverWait(driver, 10).until(
+            EC.element_to_be_clickable((By.ID, "menu-button"))).click()
+
+        time.sleep(0.4)
+
+        button_xpath = f"//button[.//img[@alt='Use {theme_name} theme']]"
+        WebDriverWait(driver, 10).until(
+            EC.element_to_be_clickable((By.XPATH, button_xpath))).click()
+        time.sleep(0.4)
+
+        WebDriverWait(driver, 10).until(
+            EC.element_to_be_clickable((By.ID, "menu-button"))).click()
+
+        time.sleep(1)
+
+        time.sleep(delay)
+
+        driver.save_screenshot(f'{filename}.png')
+    except KeyboardInterrupt:
+        print("Screenshot taking was aborted by the user.")
+    except Exception as e:
+        print(f"An error occurred: {e}")
+    finally:
+        driver.quit()
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Take a screenshot of a Zimo Web's page with specified settings.")
     parser.add_argument('-w', '--width', type=int,
                         default=1600, help='Width of the browser window')
@@ -51,13 +57,19 @@
     parser.add_argument('-d', '--delay', type=float,
                         default=0, help='Delay before taking the screenshot')
     parser.add_argument('-f', '--filename', type=str,
                         default='webpage_screenshot', help='Output filename without suffix')
 
     args = parser.parse_args()
 
-    take_screenshot(args.width, args.height, args.theme,
-                    args.pathname, args.delay, args.filename)
+    try:
+        take_screenshot(args.width, args.height, args.theme,
+                        args.pathname, args.delay, args.filename)
+    except Exception as e:
+        print(f"Failed to take screenshot: {e}")
 
 
 if __name__ == "__main__":
-    main()
+    try:
+        main()
+    except KeyboardInterrupt:
+        print("Program was interrupted by the user.")
```

### Comparing `zimo-web-screenshot-0.1.3/zimo_web_screenshot.egg-info/PKG-INFO` & `zimo-web-screenshot-0.2.0/zimo_web_screenshot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimo-web-screenshot
-Version: 0.1.3
+Version: 0.2.0
 Summary: A simple CLI tool to take screenshots of Zimo Web pages with Selenium.
 Home-page: https://github.com/zimoluo/zimo-web-screenshot-tool
 Author: Zimo Luo
 Author-email: abgkings0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

