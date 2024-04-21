# Comparing `tmp/entelecheia-0.3.1.tar.gz` & `tmp/entelecheia-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entelecheia-0.3.1.tar", max compression
+gzip compressed data, was "entelecheia-0.3.2.tar", max compression
```

## Comparing `entelecheia-0.3.1.tar` & `entelecheia-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2024-03-25 00:07:59.945327 entelecheia-0.3.1/LICENSE
--rw-r--r--   0        0        0     2681 2024-03-25 00:07:59.945327 entelecheia-0.3.1/README.md
--rw-r--r--   0        0        0     3298 2024-03-25 00:08:24.173304 entelecheia-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      187 2024-03-25 00:07:59.945327 entelecheia-0.3.1/src/entelecheia/__cli__.py
--rw-r--r--   0        0        0      533 2024-03-25 00:07:59.945327 entelecheia-0.3.1/src/entelecheia/__init__.py
--rw-r--r--   0        0        0       22 2024-03-25 00:08:24.141304 entelecheia-0.3.1/src/entelecheia/_version.py
--rw-r--r--   0        0        0        0 2024-03-25 00:07:59.945327 entelecheia-0.3.1/src/entelecheia/conf/__init__.py
--rw-r--r--   0        0        0      322 2024-03-25 00:07:59.945327 entelecheia-0.3.1/src/entelecheia/conf/about/entelecheia.yaml
--rw-r--r--   0        0        0        0 2024-03-25 00:07:59.945327 entelecheia-0.3.1/src/entelecheia/py.typed
--rw-r--r--   0        0        0     3489 1970-01-01 00:00:00.000000 entelecheia-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-21 02:00:56.768545 entelecheia-0.3.2/LICENSE
+-rw-r--r--   0        0        0     4092 2024-04-21 02:00:56.768545 entelecheia-0.3.2/README.md
+-rw-r--r--   0        0        0     3298 2024-04-21 02:01:18.072736 entelecheia-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      187 2024-04-21 02:00:56.768545 entelecheia-0.3.2/src/entelecheia/__cli__.py
+-rw-r--r--   0        0        0      516 2024-04-21 02:00:56.768545 entelecheia-0.3.2/src/entelecheia/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-21 02:01:18.040736 entelecheia-0.3.2/src/entelecheia/_version.py
+-rw-r--r--   0        0        0        0 2024-04-21 02:00:56.768545 entelecheia-0.3.2/src/entelecheia/conf/__init__.py
+-rw-r--r--   0        0        0      322 2024-04-21 02:00:56.768545 entelecheia-0.3.2/src/entelecheia/conf/about/entelecheia.yaml
+-rw-r--r--   0        0        0        0 2024-04-21 02:00:56.768545 entelecheia-0.3.2/src/entelecheia/py.typed
+-rw-r--r--   0        0        0     4900 1970-01-01 00:00:00.000000 entelecheia-0.3.2/PKG-INFO
```

### Comparing `entelecheia-0.3.1/LICENSE` & `entelecheia-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `entelecheia-0.3.1/pyproject.toml` & `entelecheia-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "entelecheia"
-version = "0.3.1"
+version = "0.3.2"
 description = "ἐντελέχεια is coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”)."
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.me"
 repository = "https://github.com/entelecheia/entelecheia"
 readme = "README.md"
 packages = [{ include = "entelecheia", from = "src" }]
```

### Comparing `entelecheia-0.3.1/src/entelecheia/__init__.py` & `entelecheia-0.3.2/src/entelecheia/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 
 
 def get_version() -> str:
     """Get the package version."""
     return __version__
 
 
-__all__ = ["HyFI", "get_version", "open_homepage"]
+__all__ = ["HyFI", "get_version"]
```

### Comparing `entelecheia-0.3.1/PKG-INFO` & `entelecheia-0.3.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,16 @@
-Metadata-Version: 2.1
-Name: entelecheia
-Version: 0.3.1
-Summary: ἐντελέχεια is coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”).
-Home-page: https://entelecheia.me
-License: MIT
-Author: Young Joon Lee
-Author-email: entelecheia@hotmail.com
-Requires-Python: >=3.9,<3.13
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: hyfi (>=1.36.3,<2.0.0)
-Project-URL: Repository, https://github.com/entelecheia/entelecheia
-Description-Content-Type: text/markdown
-
 # ἐντελέχεια 【en.te.lé.kʰeː.a】
 
 [![stai-img]][stai-url]
 [![halla-img]][halla-url]
 [![home-img]][home-url]
 [![lecture-img]][lecture-url]
 [![research-img]][research-url]
 [![playground-img]][playground-url]
+
 <!-- [![stateful-img]][stateful-url]
 [![stateful_dnd-img]][stateful-url] -->
 
 [stai-img]: https://img.shields.io/badge/STAI-jeju.ai-blue
 [stai-url]: https://stai.jeju.ai
 [playground-img]: https://img.shields.io/badge/playground-app_launcher-blue
 [playground-url]: https://entelecheia.cloudflareaccess.com
@@ -46,22 +28,55 @@
 [linkedin-url]: https://www.linkedin.com/in/entelecheia/
 [stateful-img]: https://badge.stateful.com/entelecheia/status.svg
 [stateful-url]: https://app.stateful.com/status/entelecheia
 [stateful_dnd-img]: https://badge.stateful.com/entelecheia/dnd.svg
 
 Coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”).
 
-[![GitHub Streak](http://github-readme-streak-stats.entelecheia.me/?user=entelecheia&theme=transparent&hide_border=true)](https://entelecheia.me/repositories/) 
-<!-- [![entelecheia's wakatime stats](https://github-readme-stats.entelecheia.me/api/wakatime?username=entelecheia&layout=compact&theme=transparent&hide_border=true&hide=other,browsing,shell,writing,reviewing,searching,researching,github,ai,text)](https://wakatime.com/@entelecheia) -->
-
-[![entelecheia's github activity graph](https://github-readme-activity-graph.entelecheia.me/graph?username=entelecheia&theme=react-dark&area=true&hide_border=true)](https://entelecheia.me/repositories/)
+[![entelecheia](https://github.com/entelecheia/entelecheia/assets/1177283/0a67c698-8c9e-4006-b131-d0593cd7c256)](https://entelecheia.me)
 
-[![trophy](https://github-profile-trophy.entelecheia.me/?username=entelecheia&theme=darkhub&rank=-C,-B&column=-1&no-bg=true&no-frame=true)](https://entelecheia.me/repositories/)
+### Hi there, I'm Young Joon Lee 👋
 
+🏫 I am an Assistant Professor of Artificial Intelligence Engineering at Cheju Halla University in Jeju, Korea. I specialize in integrating Artificial Intelligence, Machine Learning, and Natural Language Processing to transform finance and economics.
 
-<a href="https://www.quine.sh/user/entelecheia">
-  <img width=49% align="center" src="https://stats.quine.sh/entelecheia/topics-over-time?theme=dark" />
-</a>
-<a href="https://www.quine.sh/user/entelecheia">
-  <img width=49% align="center" src="https://stats.quine.sh/entelecheia/languages-over-time?theme=dark" />
-</a>
+🔍 My research involves creating sophisticated AI models that enhance decision-making accuracy and efficiency in financial sectors.
 
+🌱 I’m committed to educating and inspiring the next generation of AI professionals, preparing them to excel at the forefront of AI and finance intersections.
+
+🤝 I'm eager to collaborate with peers, industry experts, and organizations interested in utilizing AI to revolutionize financial practices and drive innovation.
+
+💬 Feel free to connect with me to explore how we can shape the future of finance together with cutting-edge AI solutions.
+
+#### 📈 GitHub Statistics
+
+<details>
+  <summary>📊 GitHub Stats</summary>
+
+  <a href="https://entelecheia.me/repositories/">
+    <img width=49% align="center" src="http://github-readme-streak-stats.entelecheia.me/?user=entelecheia&theme=transparent&hide_border=true" />
+    <img width=49% align="center" src="http://github-readme-stats.entelecheia.me/api?username=entelecheia&theme=transparent&show_icons=true&hide_border=true&hide_title=true" />
+  </a>
+  
+  [![trophy](https://github-profile-trophy.entelecheia.me/?username=entelecheia&theme=darkhub&rank=-C,-B&column=-1&no-bg=true&no-frame=true)](https://entelecheia.me/repositories/)
+
+</details>
+  
+<details>
+  <summary>🔥 Recent Contributions</summary>
+  
+  [![entelecheia's github activity graph](https://github-readme-activity-graph.entelecheia.me/graph?username=entelecheia&theme=react-dark&area=true&hide_border=true)](https://entelecheia.me/repositories/)
+
+[![3d contributions](https://raw.githubusercontent.com/entelecheia/metrics/main/profile-3d-contrib/profile-entelecheia.svg)](https://github.com/entelecheia/entelecheia/edit/main/README.md)
+
+</details>
+  
+  
+<details>
+  <summary>🌐 Language and Topics Trajectory</summary>
+  
+  <a href="https://www.quine.sh/user/entelecheia">
+    <img width=49% align="center" src="https://stats.quine.sh/entelecheia/topics-over-time?theme=dark" />
+  </a>
+  <a href="https://www.quine.sh/user/entelecheia">
+    <img width=49% align="center" src="https://stats.quine.sh/entelecheia/languages-over-time?theme=dark" />
+  </a>
+</details>
```

#### html2text {}

```diff
@@ -1,40 +1,48 @@
-Metadata-Version: 2.1 Name: entelecheia Version: 0.3.1 Summary:
-á¼Î½ÏÎµÎ»Î­ÏÎµÎ¹Î± is coined by Aristotle from á¼Î½ÏÎµÎ»Î®Ï (entelá¸s,
-âcomplete, full, accomplishedâ) + á¼ÏÎµÎ¹Î½ (Ã©khein, âhave, holdâ).
-Home-page: https://entelecheia.me License: MIT Author: Young Joon Lee Author-
-email: entelecheia@hotmail.com Requires-Python: >=3.9,<3.13 Classifier: License
-:: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Requires-Dist: hyfi
-(>=1.36.3,<2.0.0) Project-URL: Repository, https://github.com/entelecheia/
-entelecheia Description-Content-Type: text/markdown # á¼Î½ÏÎµÎ»Î­ÏÎµÎ¹Î±
-ãen.te.lÃ©.kÊ°eË.aã [![stai-img]][stai-url] [![halla-img]][halla-url] [!
-[home-img]][home-url] [![lecture-img]][lecture-url] [![research-img]][research-
-url] [![playground-img]][playground-url] [stai-img]: https://img.shields.io/
-badge/STAI-jeju.ai-blue [stai-url]: https://stai.jeju.ai [playground-img]:
-https://img.shields.io/badge/playground-app_launcher-blue [playground-url]:
-https://entelecheia.cloudflareaccess.com [halla-img]: https://img.shields.io/
-badge/CHU-halla.ai-blue [halla-url]: https://halla.ai [home-img]: https://
-img.shields.io/badge/home-entelecheia.me-blue [home-url]: https://
-entelecheia.me [course-img]: https://img.shields.io/badge/course-
+# á¼Î½ÏÎµÎ»Î­ÏÎµÎ¹Î± ãen.te.lÃ©.kÊ°eË.aã [![stai-img]][stai-url] [!
+[halla-img]][halla-url] [![home-img]][home-url] [![lecture-img]][lecture-url]
+[![research-img]][research-url] [![playground-img]][playground-url] [stai-img]:
+https://img.shields.io/badge/STAI-jeju.ai-blue [stai-url]: https://stai.jeju.ai
+[playground-img]: https://img.shields.io/badge/playground-app_launcher-blue
+[playground-url]: https://entelecheia.cloudflareaccess.com [halla-img]: https:/
+/img.shields.io/badge/CHU-halla.ai-blue [halla-url]: https://halla.ai [home-
+img]: https://img.shields.io/badge/home-entelecheia.me-blue [home-url]: https:/
+/entelecheia.me [course-img]: https://img.shields.io/badge/course-
 entelecheia.ai-blue [course-url]: https://course.entelecheia.ai [lecture-img]:
 https://img.shields.io/badge/lecture-entelecheia.ai-blue [lecture-url]: https:/
 /lecture.entelecheia.ai [research-img]: https://img.shields.io/badge/research-
 entelecheia.ai-blue [research-url]: https://research.entelecheia.ai [linkedin-
 img]: https://img.shields.io/badge/LinkedIn-blue?logo=linkedin [linkedin-url]:
 https://www.linkedin.com/in/entelecheia/ [stateful-img]: https://
 badge.stateful.com/entelecheia/status.svg [stateful-url]: https://
 app.stateful.com/status/entelecheia [stateful_dnd-img]: https://
 badge.stateful.com/entelecheia/dnd.svg Coined by Aristotle from á¼Î½ÏÎµÎ»Î®Ï
 (entelá¸s, âcomplete, full, accomplishedâ) + á¼ÏÎµÎ¹Î½ (Ã©khein,
-âhave, holdâ). [![GitHub Streak](http://github-readme-streak-
-stats.entelecheia.me/?user=entelecheia&theme=transparent&hide_border=true)]
-(https://entelecheia.me/repositories/) [![entelecheia's github activity graph]
-(https://github-readme-activity-graph.entelecheia.me/
-graph?username=entelecheia&theme=react-dark&area=true&hide_border=true)](https:
-//entelecheia.me/repositories/) [![trophy](https://github-profile-
-trophy.entelecheia.me/?username=entelecheia&theme=darkhub&rank=-C,-B&column=-
-1&no-bg=true&no-frame=true)](https://entelecheia.me/repositories/)_[_h_t_t_p_s_:_/_/
+âhave, holdâ). [![entelecheia](https://github.com/entelecheia/entelecheia/
+assets/1177283/0a67c698-8c9e-4006-b131-d0593cd7c256)](https://entelecheia.me)
+### Hi there, I'm Young Joon Lee ð ð« I am an Assistant Professor of
+Artificial Intelligence Engineering at Cheju Halla University in Jeju, Korea. I
+specialize in integrating Artificial Intelligence, Machine Learning, and
+Natural Language Processing to transform finance and economics. ð My
+research involves creating sophisticated AI models that enhance decision-making
+accuracy and efficiency in financial sectors. ð± Iâm committed to educating
+and inspiring the next generation of AI professionals, preparing them to excel
+at the forefront of AI and finance intersections. ð¤ I'm eager to collaborate
+with peers, industry experts, and organizations interested in utilizing AI to
+revolutionize financial practices and drive innovation. ð¬ Feel free to
+connect with me to explore how we can shape the future of finance together with
+cutting-edge AI solutions. #### ð GitHub Statistics ð GitHub Stats _[_h_t_t_p_:
+_/_/_g_i_t_h_u_b_-_r_e_a_d_m_e_-_s_t_r_e_a_k_-_s_t_a_t_s_._e_n_t_e_l_e_c_h_e_i_a_._m_e_/
+_?_u_s_e_r_=_e_n_t_e_l_e_c_h_e_i_a_&_t_h_e_m_e_=_t_r_a_n_s_p_a_r_e_n_t_&_h_i_d_e___b_o_r_d_e_r_=_t_r_u_e_]_[_h_t_t_p_:_/_/_g_i_t_h_u_b_-_r_e_a_d_m_e_-
+_s_t_a_t_s_._e_n_t_e_l_e_c_h_e_i_a_._m_e_/
+_a_p_i_?_u_s_e_r_n_a_m_e_=_e_n_t_e_l_e_c_h_e_i_a_&_t_h_e_m_e_=_t_r_a_n_s_p_a_r_e_n_t_&_s_h_o_w___i_c_o_n_s_=_t_r_u_e_&_h_i_d_e___b_o_r_d_e_r_=_t_r_u_e_&_h_i_d_e___t_i_t_l_e_=_t_r_u_e_]
+[![trophy](https://github-profile-trophy.entelecheia.me/
+?username=entelecheia&theme=darkhub&rank=-C,-B&column=-1&no-bg=true&no-
+frame=true)](https://entelecheia.me/repositories/) ð¥ Recent Contributions [!
+[entelecheia's github activity graph](https://github-readme-activity-
+graph.entelecheia.me/graph?username=entelecheia&theme=react-
+dark&area=true&hide_border=true)](https://entelecheia.me/repositories/) [![3d
+contributions](https://raw.githubusercontent.com/entelecheia/metrics/main/
+profile-3d-contrib/profile-entelecheia.svg)](https://github.com/entelecheia/
+entelecheia/edit/main/README.md) ð Language and Topics Trajectory_[_h_t_t_p_s_:_/_/
 _s_t_a_t_s_._q_u_i_n_e_._s_h_/_e_n_t_e_l_e_c_h_e_i_a_/_t_o_p_i_c_s_-_o_v_e_r_-_t_i_m_e_?_t_h_e_m_e_=_d_a_r_k_]_[_h_t_t_p_s_:_/_/_s_t_a_t_s_._q_u_i_n_e_._s_h_/
 _e_n_t_e_l_e_c_h_e_i_a_/_l_a_n_g_u_a_g_e_s_-_o_v_e_r_-_t_i_m_e_?_t_h_e_m_e_=_d_a_r_k_]
```

