# Comparing `tmp/red_web_dashboard-1.4.0.tar.gz` & `tmp/red_web_dashboard-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "red_web_dashboard-1.4.0.tar", last modified: Thu Apr 18 11:51:23 2024, max compression
+gzip compressed data, was "red_web_dashboard-1.5.0.tar", last modified: Sun Apr 21 09:39:42 2024, max compression
```

## Comparing `red_web_dashboard-1.4.0.tar` & `red_web_dashboard-1.5.0.tar`

### file list

```diff
@@ -1,293 +1,293 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.512335 red_web_dashboard-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34625 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-18 11:51:23.512335 red_web_dashboard-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.512335 red_web_dashboard-1.4.0/Red_Web_Dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-18 11:51:23.000000 red_web_dashboard-1.4.0/Red_Web_Dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-04-18 11:51:23.000000 red_web_dashboard-1.4.0/Red_Web_Dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:51:23.000000 red_web_dashboard-1.4.0/Red_Web_Dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-18 11:51:23.000000 red_web_dashboard-1.4.0/Red_Web_Dashboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-18 11:51:23.000000 red_web_dashboard-1.4.0/Red_Web_Dashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 11:51:23.000000 red_web_dashboard-1.4.0/Red_Web_Dashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.456335 red_web_dashboard-1.4.0/reddash/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.456335 red_web_dashboard-1.4.0/reddash/app/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.460335 red_web_dashboard-1.4.0/reddash/app/base/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43308 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/base/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.460335 red_web_dashboard-1.4.0/reddash/app/login/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/login/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.452335 red_web_dashboard-1.4.0/reddash/app/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.464335 red_web_dashboard-1.4.0/reddash/app/static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/biometric-icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.468335 red_web_dashboard-1.4.0/reddash/app/static/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)   480516 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/css/argon-dashboard.css
--rw-r--r--   0 runner    (1001) docker     (127)  1218638 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/css/argon-dashboard.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   381006 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/css/argon-dashboard.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/css/nucleo-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/css/nucleo-svg.css
--rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/css/simplemde.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   635325 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/error-403.gif
--rw-r--r--   0 runner    (1001) docker     (127)   884014 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/error-404.gif
--rw-r--r--   0 runner    (1001) docker     (127)   824431 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/error-500.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.472335 red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo-icons.eot
--rw-r--r--   0 runner    (1001) docker     (127)   126098 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo-icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18292 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    26524 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo.eot
--rw-r--r--   0 runner    (1001) docker     (127)    26364 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/gulpfile.js
--rw-r--r--   0 runner    (1001) docker     (127)    34128 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/icon-documentation.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.472335 red_web_dashboard-1.4.0/reddash/app/static/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)    27200 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/js/argon-dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/js/argon-dashboard.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.472335 red_web_dashboard-1.4.0/reddash/app/static/assets/js/core/
--rw-r--r--   0 runner    (1001) docker     (127)    48944 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/js/core/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/js/core/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/js/core/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.472335 red_web_dashboard-1.4.0/reddash/app/static/assets/js/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/js/plugins/Chart.extension.js
--rw-r--r--   0 runner    (1001) docker     (127)    47524 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip
--rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/js/plugins/bootstrap-notify.js
--rw-r--r--   0 runner    (1001) docker     (127)   176853 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/js/plugins/chartjs.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19411 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    48421 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/js/plugins/utils.js
--rw-r--r--   0 runner    (1001) docker     (127)   140628 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/oauth.png
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/pdf.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/random.svg
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.472335 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.480335 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_cards.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_header.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_misc.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_nav.scss
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_popovers.scss
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_progress.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_tilt.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_tooltips.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_utilities-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)    16957 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)    68466 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.488335 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss
--rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_helpers.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_transitions.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss
--rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)    68547 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-reboot.scss
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.488335 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-text.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_validation.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.492335 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_color-bg.scss
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_colored-links.scss
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_ratio.scss
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stacks.scss
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stretched-link.scss
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_text-truncation.scss
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_visually-hidden.scss
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_vr.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.496335 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_backdrop.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_box-shadow.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_color-scheme.scss
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_container.scss
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_image.scss
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_reset-text.scss
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_resize.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_text-truncate.scss
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.496335 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.496335 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.496335 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-carousel.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.496335 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/custom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/custom/_styles.scss
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/custom/_variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.500335 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-select.scss
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/forms/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/forms/_inputs.scss
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/forms/_labels.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.500335 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_colored-shadows.scss
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_hover.scss
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/mixins/mixins.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.452335 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.500335 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/
--rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/plugins.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/theme.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.504335 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_breadcrumb.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_choices.scss
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_fixed-plugin.scss
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_form-switch.scss
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_full-calendar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_rtl.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_virtual-reality.scss
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/tasks_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.504335 red_web_dashboard-1.4.0/reddash/app/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.508335 red_web_dashboard-1.4.0/reddash/app/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/errors/403.html
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/errors/500.html
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/errors/blacklisted.html
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/errors/custom.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.508335 red_web_dashboard-1.4.0/reddash/app/templates/includes/
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/includes/fixed-plugin.html
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/includes/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/includes/navigation.html
--rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/includes/scripts.html
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/includes/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.508335 red_web_dashboard-1.4.0/reddash/app/templates/layouts/
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/layouts/base-fullscreen.html
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/layouts/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.508335 red_web_dashboard-1.4.0/reddash/app/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (127)    29014 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/pages/admin.html
--rw-r--r--   0 runner    (1001) docker     (127)    16881 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/pages/commands.html
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/pages/credits.html
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/pages/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (127)    30619 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/pages/dashboard_guild.html
--rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/pages/guild_profile.html
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/pages/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.508335 red_web_dashboard-1.4.0/reddash/app/templates/pages/login/
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/pages/login/login.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.508335 red_web_dashboard-1.4.0/reddash/app/templates/pages/third_parties/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/pages/third_parties/oauth.html
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/pages/third_parties/third_parties.html
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/pages/third_parties/third_parties_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/templates/pages/third_parties/third_party.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:51:23.512335 red_web_dashboard-1.4.0/reddash/app/third_parties/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/third_parties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/third_parties/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    26892 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/reddash/app/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-18 11:51:23.512335 red_web_dashboard-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-18 11:51:18.000000 red_web_dashboard-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.642760 red_web_dashboard-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34625 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-21 09:39:42.642760 red_web_dashboard-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.642760 red_web_dashboard-1.5.0/Red_Web_Dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-21 09:39:42.000000 red_web_dashboard-1.5.0/Red_Web_Dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-04-21 09:39:42.000000 red_web_dashboard-1.5.0/Red_Web_Dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:39:42.000000 red_web_dashboard-1.5.0/Red_Web_Dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 09:39:42.000000 red_web_dashboard-1.5.0/Red_Web_Dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-21 09:39:42.000000 red_web_dashboard-1.5.0/Red_Web_Dashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 09:39:42.000000 red_web_dashboard-1.5.0/Red_Web_Dashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.590760 red_web_dashboard-1.5.0/reddash/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.590760 red_web_dashboard-1.5.0/reddash/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.590760 red_web_dashboard-1.5.0/reddash/app/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43241 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/base/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.590760 red_web_dashboard-1.5.0/reddash/app/login/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/login/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.582760 red_web_dashboard-1.5.0/reddash/app/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.598760 red_web_dashboard-1.5.0/reddash/app/static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/biometric-icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.602760 red_web_dashboard-1.5.0/reddash/app/static/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   480516 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/css/argon-dashboard.css
+-rw-r--r--   0 runner    (1001) docker     (127)  1218638 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/css/argon-dashboard.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   381006 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/css/argon-dashboard.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/css/nucleo-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/css/nucleo-svg.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/css/simplemde.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   635325 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/error-403.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   884014 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/error-404.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   824431 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/error-500.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.602760 red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   126098 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18292 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    26524 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    26364 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/gulpfile.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34128 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/icon-documentation.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.602760 red_web_dashboard-1.5.0/reddash/app/static/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    27200 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/js/argon-dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/js/argon-dashboard.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.606760 red_web_dashboard-1.5.0/reddash/app/static/assets/js/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    48944 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/js/core/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/js/core/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/js/core/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.606760 red_web_dashboard-1.5.0/reddash/app/static/assets/js/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/js/plugins/Chart.extension.js
+-rw-r--r--   0 runner    (1001) docker     (127)    47524 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/js/plugins/bootstrap-notify.js
+-rw-r--r--   0 runner    (1001) docker     (127)   176853 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/js/plugins/chartjs.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19411 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    48421 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/js/plugins/utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)   140628 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/oauth.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/random.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.606760 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.614760 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_cards.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_misc.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_nav.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_popovers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_progress.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_tables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_tilt.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_tooltips.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_utilities-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    16957 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    68466 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.622760 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_helpers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_transitions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    68547 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-reboot.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.622760 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_validation.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.622760 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_clearfix.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_color-bg.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_colored-links.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_ratio.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stacks.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stretched-link.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_text-truncation.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_visually-hidden.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_vr.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.630760 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_backdrop.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_box-shadow.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_clearfix.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_color-scheme.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_container.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_image.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_list-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_reset-text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_resize.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_text-truncate.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.630760 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.630760 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.630760 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-carousel.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.630760 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/custom/_styles.scss
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/custom/_variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.630760 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-select.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/forms/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/forms/_inputs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/forms/_labels.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.630760 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_colored-shadows.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_hover.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/mixins/mixins.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.586760 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.634760 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/
+-rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/plugins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/theme.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.638760 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_breadcrumb.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_choices.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_fixed-plugin.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_form-switch.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_full-calendar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_rtl.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_virtual-reality.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/tasks_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.638760 red_web_dashboard-1.5.0/reddash/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.638760 red_web_dashboard-1.5.0/reddash/app/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/errors/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/errors/blacklisted.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/errors/custom.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.638760 red_web_dashboard-1.5.0/reddash/app/templates/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/includes/fixed-plugin.html
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/includes/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/includes/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/includes/scripts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/includes/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.638760 red_web_dashboard-1.5.0/reddash/app/templates/layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/layouts/base-fullscreen.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/layouts/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.642760 red_web_dashboard-1.5.0/reddash/app/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)    29444 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/pages/admin.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16966 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/pages/commands.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/pages/credits.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/pages/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)    30733 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/pages/dashboard_guild.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/pages/guild_profile.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/pages/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.642760 red_web_dashboard-1.5.0/reddash/app/templates/pages/login/
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/pages/login/login.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.642760 red_web_dashboard-1.5.0/reddash/app/templates/pages/third_parties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/pages/third_parties/oauth.html
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/pages/third_parties/third_parties.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/pages/third_parties/third_parties_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/templates/pages/third_parties/third_party.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:39:42.642760 red_web_dashboard-1.5.0/reddash/app/third_parties/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/third_parties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13477 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/third_parties/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27046 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/reddash/app/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-21 09:39:42.646760 red_web_dashboard-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-21 09:39:38.000000 red_web_dashboard-1.5.0/setup.py
```

### Comparing `red_web_dashboard-1.4.0/LICENSE` & `red_web_dashboard-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/PKG-INFO` & `red_web_dashboard-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Red-Web-Dashboard
-Version: 1.4.0
+Version: 1.5.0
 Summary: An easy-to-use interactive web Dashboard to control your Red bot!
 Home-page: https://github.com/AAA3A-AAA3A/Red-Dashboard
 Author: Neuro Assassin & AAA3A
 License: AGPL-3.0
 Project-URL: Third Party Discord Server, https://discord.gg/red-cog-support-240154543684321280
 Project-URL: Documentation, https://red-web-dashboard.readthedocs.io/en/latest/
 Project-URL: Donate on Buy Me a Coffee, https://www.buymeacoffee.com/aaa3a
```

### Comparing `red_web_dashboard-1.4.0/README.md` & `red_web_dashboard-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/Red_Web_Dashboard.egg-info/PKG-INFO` & `red_web_dashboard-1.5.0/Red_Web_Dashboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Red-Web-Dashboard
-Version: 1.4.0
+Version: 1.5.0
 Summary: An easy-to-use interactive web Dashboard to control your Red bot!
 Home-page: https://github.com/AAA3A-AAA3A/Red-Dashboard
 Author: Neuro Assassin & AAA3A
 License: AGPL-3.0
 Project-URL: Third Party Discord Server, https://discord.gg/red-cog-support-240154543684321280
 Project-URL: Documentation, https://red-web-dashboard.readthedocs.io/en/latest/
 Project-URL: Donate on Buy Me a Coffee, https://www.buymeacoffee.com/aaa3a
```

### Comparing `red_web_dashboard-1.4.0/Red_Web_Dashboard.egg-info/SOURCES.txt` & `red_web_dashboard-1.5.0/Red_Web_Dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/pyproject.toml` & `red_web_dashboard-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/__main__.py` & `red_web_dashboard-1.5.0/reddash/__main__.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/app.py` & `red_web_dashboard-1.5.0/reddash/app/app.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/base/routes.py` & `red_web_dashboard-1.5.0/reddash/app/base/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,19 +189,15 @@
             request.args.get("query"),
             request.args.get("filter"),
         ],
     }
     with app.lock:
         result = await get_result(app, requeststr)
 
-    guilds = Pagination(result["guilds"])
-    guilds.total = result["total"]
-    guilds.per_page = result["per_page"]
-    guilds.pages = result["pages"]
-    guilds.page = result["page"]
+    guilds = Pagination(result.pop("items"), **result)
 
     redirecting_to: str = (
         request.args.get("next") if not app.config["USE_SESSION_FOR_NEXT"] else session.get("next")
     ) or url_for("base_blueprint.dashboard_guild", guild_id="GUILD_ID")
     # `url_has_allowed_host_and_scheme` should check if the url is safe for redirects, meaning it matches the request host.
     if not url_has_allowed_host_and_scheme(redirecting_to, request.host):
         return abort(400)
@@ -218,20 +214,20 @@
 class LeaveGuildForm(FlaskForm):
     def __init__(self) -> None:
         super().__init__(prefix="leave_guild_form_")
 
     submit: wtforms.SubmitField = wtforms.SubmitField(_("Leave Guild"))
 
 
-async def get_guild(guild_id: int):
+async def get_guild(guild_id: int, for_third_parties: bool = False):
     requeststr = {
         "jsonrpc": "2.0",
         "id": 0,
         "method": "DASHBOARDRPC__GET_GUILD",
-        "params": [current_user.id, guild_id],
+        "params": [current_user.id, guild_id, for_third_parties],
     }
     with app.lock:
         guild = await get_result(app, requeststr)
     if guild["status"] == 1:
         return abort(404, description=_("Guild not found or missing access to it."))
     guild["created_at"] = datetime.datetime.fromtimestamp(
         guild["created_at"], tz=datetime.timezone.utc
@@ -377,20 +373,20 @@
     )
     embeds: wtforms.BooleanField = wtforms.BooleanField(_("Use embeds in responses."))
     use_bot_color: wtforms.BooleanField = wtforms.BooleanField(_("Use bot set color in embeds."))
     fuzzy: wtforms.BooleanField = wtforms.BooleanField(_("Use fuzzy command search."))
     delete_delay: wtforms.IntegerField = wtforms.IntegerField(
         _("Delay before deleting invocation messages (-1 to disable):"),
         validators=[
-            wtforms.validators.DataRequired(),
+            wtforms.validators.InputRequired(),
             wtforms.validators.NumberRange(min=-1, max=60),
         ],
     )
     locale: wtforms.StringField = wtforms.StringField(
-        _("Locale:"), validators=[wtforms.validators.DataRequired(), BabelCheck(check_reset=True)]
+        _("Locale:"), validators=[wtforms.validators.InputRequired(), BabelCheck(check_reset=True)]
     )
     regional_format: wtforms.StringField = wtforms.StringField(
         _("Regional Format:"), validators=[wtforms.validators.Optional(), BabelCheck(check_reset=True)]
     )
     submit: wtforms.SubmitField = wtforms.SubmitField(_("Save Modifications"))
 
 
@@ -412,16 +408,16 @@
             kwargs["class"] += " markdown-text-area-field-max-height"
         if disable_toolbar:
             kwargs["class"] += " markdown-text-area-field-toolbar-disabled"
         return super().__call__(**kwargs)
 
 
 class AliasForm(FlaskForm):
-    alias_name: wtforms.StringField = wtforms.StringField(_("Name"), validators=[wtforms.validators.DataRequired(), wtforms.validators.Regexp(r"^[^\s]+$"), wtforms.validators.Length(max=300)])
-    command: MarkdownTextAreaField = MarkdownTextAreaField(_("Command"), validators=[wtforms.validators.DataRequired(), wtforms.validators.Length(max=1700)])
+    alias_name: wtforms.StringField = wtforms.StringField(_("Name"), validators=[wtforms.validators.InputRequired(), wtforms.validators.Regexp(r"^[^\s]+$"), wtforms.validators.Length(max=300)])
+    command: MarkdownTextAreaField = MarkdownTextAreaField(_("Command"), validators=[wtforms.validators.InputRequired(), wtforms.validators.Length(max=1700)])
 
 
 class AliasesForm(FlaskForm):
     def __init__(self, aliases: typing.Dict[str, str]) -> None:
         super().__init__(prefix="aliases_form_")
         for name, command in aliases.items():
             self.aliases.append_entry({"alias_name": name, "command": command})
@@ -429,27 +425,27 @@
         self.aliases.entries = [entry for entry in self.aliases.entries if entry.csrf_token.data is not None]
 
     aliases: wtforms.FieldList = wtforms.FieldList(wtforms.FormField(AliasForm))
     submit: wtforms.SubmitField = wtforms.SubmitField(_("Save Modifications"))
 
 
 class CustomCommandResponseForm(FlaskForm):
-    response: MarkdownTextAreaField = MarkdownTextAreaField(_("Response"), validators=[wtforms.validators.DataRequired(), wtforms.validators.Length(max=2000)])
+    response: MarkdownTextAreaField = MarkdownTextAreaField(_("Response"), validators=[wtforms.validators.InputRequired(), wtforms.validators.Length(max=2000)])
 
 
 class CustomCommandForm(FlaskForm):
     def __init__(self, *args, **kwargs) -> None:
         responses = kwargs.pop("responses", {})
         super().__init__(*args, **kwargs)
         for response in responses:
             self.responses.append_entry({"response": response})
         self.responses.default = [entry for entry in self.responses.entries if entry.response.data and entry.csrf_token.data is None]
         self.responses.entries = [entry for entry in self.responses.entries if not entry.response.data or entry.csrf_token.data is not None]
 
-    command: wtforms.StringField = wtforms.StringField(_("Name"), validators=[wtforms.validators.DataRequired(), wtforms.validators.Regexp(r"^[^\sA-Z]+$"), wtforms.validators.Length(max=300)])
+    command: wtforms.StringField = wtforms.StringField(_("Name"), validators=[wtforms.validators.InputRequired(), wtforms.validators.Regexp(r"^[^\sA-Z]+$"), wtforms.validators.Length(max=300)])
     responses: wtforms.FieldList = wtforms.FieldList(wtforms.FormField(CustomCommandResponseForm), _("Responses"), min_entries=1)
 
 
 class CustomCommandsForm(FlaskForm):
     def __init__(self, custom_commands: typing.Dict[str, typing.List[str]]) -> None:
         super().__init__(prefix="custom_commands_form_")
         for command, responses in custom_commands.items():
@@ -715,25 +711,25 @@
     icon: wtforms.StringField = wtforms.StringField(_("Icon:"))
     website_description: wtforms.StringField = wtforms.StringField(_("Website (Short) Description:"))
     description: MarkdownTextAreaField = MarkdownTextAreaField(_("Description:"))
     support_server: wtforms.URLField = wtforms.URLField(_("Support Server URL:"))
     default_color: wtforms.SelectField = wtforms.SelectField(
         _("Default Color:"),
         choices=[(color, color.capitalize()) for color in AVAILABLE_COLORS],
-        validators=[wtforms.validators.DataRequired()],
+        validators=[wtforms.validators.InputRequired()],
     )
     default_background_theme: wtforms.SelectField = wtforms.SelectField(
         _("Default Background Theme:"),
         choices=[("light", "Light"), ("dark", "Dark")],
-        validators=[wtforms.validators.DataRequired()],
+        validators=[wtforms.validators.InputRequired()],
     )
     default_sidebar_theme: wtforms.SelectField = wtforms.SelectField(
         _("Default Sidebar Theme:"),
         choices=[("light", "Light"), ("dark", "Dark")],
-        validators=[wtforms.validators.DataRequired()],
+        validators=[wtforms.validators.InputRequired()],
     )
     disabled_third_parties: wtforms.SelectMultipleField = wtforms.SelectMultipleField(
         _("Disabled Third Parties:"), choices=[]
     )
     submit: wtforms.SubmitField = wtforms.SubmitField(_("Save Modifications"))
 
 
@@ -774,15 +770,15 @@
         self.invite_commands_scope.default = self.invite_commands_scope.checked = settings["invite_commands_scope"]
         self.invite_perms.validators.append(wtforms.validators.NumberRange(min=0, max=app.variables["constants"]["MAX_DISCORD_PERMISSIONS_VALUE"]))
         self.invite_perms.default = settings["invite_perms"]
         self.locale.default = settings["locale"]
         self.regional_format.default = settings["regional_format"]
 
     prefixes: wtforms.StringField = wtforms.StringField(
-        _("Prefixes:"), validators=[wtforms.validators.DataRequired(), PrefixesCheck()]
+        _("Prefixes:"), validators=[wtforms.validators.InputRequired(), PrefixesCheck()]
     )
     invoke_error_msg: wtforms.StringField = wtforms.StringField(
         _("Invoke Error Message:"), validators=[wtforms.validators.Length(max=1000)]
     )
     disabled_commands: wtforms.SelectMultipleField = wtforms.SelectMultipleField(
         _("Disabled Commands:"), choices=[]
     )
@@ -798,19 +794,19 @@
     fuzzy: wtforms.BooleanField = wtforms.BooleanField(_("Use Fuzzy Search when command invokation."))
     use_buttons: wtforms.BooleanField = wtforms.BooleanField(_("Use Buttons instead of Reactions."))
     invite_public: wtforms.BooleanField = wtforms.BooleanField(_("Make the invite public."))
     invite_commands_scope: wtforms.BooleanField = wtforms.BooleanField(_("Use the Commands Scope in the invite."))
     invite_perms: wtforms.IntegerField = wtforms.IntegerField(
         _("Invite Permissions (0 for nothing):"),
         validators=[
-            wtforms.validators.DataRequired(),
+            wtforms.validators.InputRequired(),
         ],
     )
     locale: wtforms.StringField = wtforms.StringField(
-        _("Locale:"), validators=[wtforms.validators.DataRequired(), BabelCheck()]
+        _("Locale:"), validators=[wtforms.validators.InputRequired(), BabelCheck()]
     )
     regional_format: wtforms.StringField = wtforms.StringField(
         _("Regional Format:"),
         validators=[wtforms.validators.Optional(), BabelCheck(check_reset=True)],
     )
     submit: wtforms.SubmitField = wtforms.SubmitField(_("Save Modifications"))
```

### Comparing `red_web_dashboard-1.4.0/reddash/app/login/routes.py` & `red_web_dashboard-1.5.0/reddash/app/login/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         ) as r:
             new_data = await r.json()
             try:
                 user: User = User(
                     id=int(new_data["id"]),
                     name=new_data["username"],
                     global_name=new_data["global_name"],
-                    avatar_url=f"https://cdn.discordapp.com/avatars/{new_data['id']}/{new_data['avatar']}.png",
+                    avatar_url=f"https://cdn.discordapp.com/avatars/{new_data['id']}/{new_data['avatar']}.png" if new_data["avatar"] is not None else None,
                 )
                 login_user(
                     user=user,
                     remember=False,
                     duration=datetime.timedelta(weeks=1),
                 )
             except KeyError as e:
```

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/biometric-icon.svg` & `red_web_dashboard-1.5.0/reddash/app/static/assets/biometric-icon.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/css/argon-dashboard.css` & `red_web_dashboard-1.5.0/reddash/app/static/assets/css/argon-dashboard.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/css/argon-dashboard.css.map` & `red_web_dashboard-1.5.0/reddash/app/static/assets/css/argon-dashboard.css.map`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/css/argon-dashboard.min.css` & `red_web_dashboard-1.5.0/reddash/app/static/assets/css/argon-dashboard.min.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/css/nucleo-icons.css` & `red_web_dashboard-1.5.0/reddash/app/static/assets/css/nucleo-icons.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/css/nucleo-svg.css` & `red_web_dashboard-1.5.0/reddash/app/static/assets/css/nucleo-svg.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/css/simplemde.min.css` & `red_web_dashboard-1.5.0/reddash/app/static/assets/css/simplemde.min.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/error-403.gif` & `red_web_dashboard-1.5.0/reddash/app/static/assets/error-403.gif`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/error-404.gif` & `red_web_dashboard-1.5.0/reddash/app/static/assets/error-404.gif`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/error-500.gif` & `red_web_dashboard-1.5.0/reddash/app/static/assets/error-500.gif`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo-icons.eot` & `red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo-icons.eot`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo-icons.svg` & `red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo-icons.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo-icons.ttf` & `red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo-icons.ttf`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo-icons.woff` & `red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo-icons.woff`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo-icons.woff2` & `red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo-icons.woff2`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo.eot` & `red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo.eot`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo.ttf` & `red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo.ttf`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo.woff` & `red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo.woff`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/fonts/nucleo.woff2` & `red_web_dashboard-1.5.0/reddash/app/static/assets/fonts/nucleo.woff2`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/gulpfile.js` & `red_web_dashboard-1.5.0/reddash/app/static/assets/gulpfile.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/icon-documentation.svg` & `red_web_dashboard-1.5.0/reddash/app/static/assets/icon-documentation.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/js/argon-dashboard.js` & `red_web_dashboard-1.5.0/reddash/app/static/assets/js/argon-dashboard.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/js/argon-dashboard.js.map` & `red_web_dashboard-1.5.0/reddash/app/static/assets/js/argon-dashboard.js.map`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/js/core/bootstrap.min.js` & `red_web_dashboard-1.5.0/reddash/app/static/assets/js/core/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/js/core/jquery.min.js` & `red_web_dashboard-1.5.0/reddash/app/static/assets/js/core/jquery.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/js/core/popper.min.js` & `red_web_dashboard-1.5.0/reddash/app/static/assets/js/core/popper.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/js/plugins/Chart.extension.js` & `red_web_dashboard-1.5.0/reddash/app/static/assets/js/plugins/Chart.extension.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip` & `red_web_dashboard-1.5.0/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/js/plugins/bootstrap-notify.js` & `red_web_dashboard-1.5.0/reddash/app/static/assets/js/plugins/bootstrap-notify.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/js/plugins/chartjs.min.js` & `red_web_dashboard-1.5.0/reddash/app/static/assets/js/plugins/chartjs.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js` & `red_web_dashboard-1.5.0/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js` & `red_web_dashboard-1.5.0/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/js/plugins/utils.js` & `red_web_dashboard-1.5.0/reddash/app/static/assets/js/plugins/utils.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/oauth.png` & `red_web_dashboard-1.5.0/reddash/app/static/assets/oauth.png`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/pdf.svg` & `red_web_dashboard-1.5.0/reddash/app/static/assets/pdf.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/random.svg` & `red_web_dashboard-1.5.0/reddash/app/static/assets/random.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_cards.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_cards.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_forms.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_forms.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_header.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_header.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_misc.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_misc.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_nav.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_nav.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_tables.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_tables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_typography.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_typography.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/_variables.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/_variables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/theme.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/theme.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/static/assets/scss/argon-dashboard.scss` & `red_web_dashboard-1.5.0/reddash/app/static/assets/scss/argon-dashboard.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/tasks_manager.py` & `red_web_dashboard-1.5.0/reddash/app/tasks_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                                 continue
 
                         result = await secure_send(self.app, request)
                         if not result:
                             continue
                         if "error" in result:
                             continue
-                        if "disconnected" in result["result"]:
+                        if "disconnected" in result["result"] or "version" not in result["result"]:
                             continue
                         if result["result"]["version"] != version != 0:
                             self.ignore_disconnect: bool = True
                             self.app.logger.info("RPC websocket behind. Closing and restarting...")
                             self.app.ws.close()
                             initialize_websocket(self.app)
                             self.ignore_disconnect: bool = False
```

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/errors/403.html` & `red_web_dashboard-1.5.0/reddash/app/templates/errors/403.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/errors/404.html` & `red_web_dashboard-1.5.0/reddash/app/templates/errors/404.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/errors/500.html` & `red_web_dashboard-1.5.0/reddash/app/templates/errors/500.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/errors/blacklisted.html` & `red_web_dashboard-1.5.0/reddash/app/templates/errors/blacklisted.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/errors/custom.html` & `red_web_dashboard-1.5.0/reddash/app/templates/errors/custom.html`

 * *Files 7% similar despite different names*

```diff
@@ -13,16 +13,16 @@
         <div class="card card-chart">
           <div class="row">
             <div class="col-md-12">
               <div class="card">
                 <div class="card-header">
                   <div class="card-body">
                     <h1><bold>{{ error_title }}</bold></h1>
-                    {% if error_description %}
-                      <p>{{ error_description }}</p>
+                    {% if error_message %}
+                      <p>{{ error_message }}</p>
                     {% endif %}
                     <br />
                     <a class="btn bg-gradient-success mb-1 w-30" href="{{ url_for("base_blueprint.index") }}">{{ _("Back to Home") }}</a>
                   </div>
                 </div>
               </div>
             </div>
```

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/includes/fixed-plugin.html` & `red_web_dashboard-1.5.0/reddash/app/templates/includes/fixed-plugin.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/includes/footer.html` & `red_web_dashboard-1.5.0/reddash/app/templates/includes/footer.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/includes/navigation.html` & `red_web_dashboard-1.5.0/reddash/app/templates/includes/navigation.html`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
       <ul class="navbar-nav justify-content-end">
         <li class="nav-item d-flex align-items-center">
             {% if current_user.is_authenticated %}
               <div class="show">
                 <div class="dropdown">
                   <a class="nav-link" href="javascript:void(0);" role="button" id="user_dropdown" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                     <div class="photo">
-                      <img src="{{ current_user.avatar_url }}" style="height: 35px; width: 35px; border-radius: 50%; margin: auto;" alt="User Avatar">
+                      <img src="{{ current_user.display_avatar }}" style="height: 35px; width: 35px; border-radius: 50%; margin: auto;" alt="User Avatar">
                       <b class="text-white" style="margin-left: 2px">{{ current_user.display_name }}</b>
                       <span class="text-white" style="margin-left: 0.5px"><i class="ni ni-bold-down"></i></span>
                     </div>
                     <b class="caret d-none d-lg-block d-xl-block"></b>
                   </a>
                   <ul class="dropdown-menu" aria-labelledby="user_dropdown">
                     <li class="nav-link"><a href="{{ url_for("login_blueprint.logout") }}" class="nav-item dropdown-item text-danger"><i class="ni ni-user-run" style="width: 1.3em; vertical-align: -2px;"></i> {{ _("Logout") }}</a></li>
```

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/includes/scripts.html` & `red_web_dashboard-1.5.0/reddash/app/templates/includes/scripts.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/includes/sidenav.html` & `red_web_dashboard-1.5.0/reddash/app/templates/includes/sidenav.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/layouts/base-fullscreen.html` & `red_web_dashboard-1.5.0/reddash/app/templates/layouts/base-fullscreen.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/layouts/base.html` & `red_web_dashboard-1.5.0/reddash/app/templates/layouts/base.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/pages/admin.html` & `red_web_dashboard-1.5.0/reddash/app/templates/pages/admin.html`

 * *Files 1% similar despite different names*

```diff
@@ -342,16 +342,16 @@
                                 <img class="profile-pic" src="{{ variables["bot"]["avatar"] }}" />
                                 <div class="upload-button" onclick='$(this).next(".file-upload").click();'>
                                     <i class="fa fa-arrow-circle-up" aria-hidden="true"></i>
                                 </div>
                                 {{ bot_profile_form.avatar(class="file-upload", accept="image/png, image/jpg, image/jpeg, image/gif", onchange="readURL(this);", style="display: none;") }}
                             </div>
                             <div class="text-center">
-                                <a class="text-danger text-xs" href="javascript:void(0);" onclick='this.parentElement.parentElement.parentElement.parentElement.querySelector("input[type=hidden]").value = "default"; this.parentElement.parentElement.parentElement.parentElement.querySelector("input[type=file]").value = null; $(".profile-pic").attr("src", "{{ variables["bot"]["default_avatar"] }}"); this.style.display = "none"; this.parentElement.children[1].style.display = "";'>{{ _("Use default") }}</a>
-                                <a class="text-danger text-xs" href="javascript:void(0);" onclick='this.parentElement.parentElement.parentElement.parentElement.querySelector("input[type=hidden]").value = "keep"; this.parentElement.parentElement.parentElement.parentElement.querySelector("input[type=file]").value = null; $(".profile-pic").attr("src", "{{ variables["bot"]["avatar"] }}"); this.style.display = "none"; this.parentElement.children[0].style.display = "";' style="display: none; margin-left: 8px;">{{ _("Keep current") }}</a>
+                                <a class="text-danger text-xs" href="javascript:void(0);" onclick='this.parentElement.parentElement.parentElement.parentElement.querySelector("input[type=hidden]").value = "default"; this.parentElement.parentElement.parentElement.parentElement.querySelector("input[type=file]").value = null; $(".profile-pic").attr("src", "{{ variables["bot"]["default_avatar"] }}"); this.style.display = "none"; this.parentElement.children[1].style.display = "";'{% if variables["bot"]["avatar"] != variables["bot"]["default_avatar"] %} style="display: none;"{% endif %}>{{ _("Use default") }}</a>
+                                <a class="text-danger text-xs" href="javascript:void(0);" onclick='this.parentElement.parentElement.parentElement.parentElement.querySelector("input[type=hidden]").value = "keep"; this.parentElement.parentElement.parentElement.parentElement.querySelector("input[type=file]").value = null; $(".profile-pic").attr("src", "{{ variables["bot"]["avatar"] }}"); this.style.display = "none";{% if variables["bot"]["avatar"] != variables["bot"]["default_avatar"] %} this.parentElement.children[0].style.display = "";{% endif %}' style="display: none; margin-left: 8px;">{{ _("Keep current") }}</a>
                             </div>
                         </div>
                         <div class="mb-3">
                             <div class="form-group">
                                 <label class="form-group-label">{{ bot_profile_form.username.label.text }}</label>
                                 {{ bot_profile_form.username(class="form-control form-control-default") }}
                             </div>
@@ -408,24 +408,29 @@
             if (!(window.location.pathname.startsWith(new_url)) || (target_id == "overview" && !(window.location.pathname == base_url))) {
                 // window.location.pathname = new_url;
                 window.history.pushState({}, "", new_url);
             }
         })
     </script>
     <script>
+        document.addEventListener("DOMContentLoaded", function() {
+            changePage("{{ page }}");
+        });
         var readURL = function(input) {
             if (input.files && input.files[0]) {
                 var reader = new FileReader();
                 reader.onload = function (e) {
                     $(".profile-pic").attr("src", e.target.result);
                 }
                 reader.readAsDataURL(input.files[0]);
                 var avatar_options = input.parentElement.parentElement.parentElement.parentElement.querySelector("div .text-center");
-                avatar_options.children[0].style.display = "";
-                if (avatar_options.children.leghth > 1) {
+                {% if variables["bot"]["avatar"] != variables["bot"]["default_avatar"] %}
+                    avatar_options.children[0].style.display = "";
+                {% endif %}
+                if (avatar_options.children.length > 1) {
                     avatar_options.children[1].style.display = "";
                 }
             }
         }
     </script>
     <script>
         async function confirmLock(event) {
```

#### html2text {}

```diff
@@ -110,15 +110,17 @@
 my-4 mb-2") }}
 **** {{{{ __((""EEddiitt DDiissccoorrdd BBoott PPrrooffiillee"")) }}}} ****
 ×
 {{ bot_profile_form.hidden_tag() }}
 }" />
 {{ bot_profile_form.avatar(class="file-upload", accept="image/png, image/jpg,
 image/jpeg, image/gif", onchange="readURL(this);", style="display: none;") }}
-_{_{_ ___(_"_U_s_e_ _d_e_f_a_u_l_t_"_)_ _}_} _{_{_ ___(_"_K_e_e_p_ _c_u_r_r_e_n_t_"_)_ _}_}
+% if variables["bot"]["avatar"] != variables["bot"]["default_avatar"] %}
+style="display: none;"{% endif %}>{{ _("Use default") }}
+ _{_{_ ___(_"_K_e_e_p_ _c_u_r_r_e_n_t_"_)_ _}_}
 {{ bot_profile_form.username.label.text }} {{ bot_profile_form.username
 (class="form-control form-control-default") }}
 {{ bot_profile_form.description.label.text }} {{ bot_profile_form.description
 (class="form-control form-control-default") }}
 {{ _("Fermer") }} {{ bot_profile_form.submit(class="btn mb-0 bg-gradient-
 success btn-md w-30 mt-2 mb-4") }}
 {% endblock %} {% block javascripts %}
```

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/pages/commands.html` & `red_web_dashboard-1.5.0/reddash/app/templates/pages/commands.html`

 * *Files 4% similar despite different names*

```diff
@@ -89,18 +89,21 @@
                                                           </tr>
                                                           {% if command.signature or command.aliases %}
                                                             <tr>
                                                               <td colspan="2" style="border: none; padding: 0px;">
                                                                 <div class="collapse" id="collapse_{{ command.name }}">
                                                                   <div class="d-flex card card-body text-wrap">
                                                                     {% if command.signature %}
-                                                                      <strong>{{ _("Usage:") }}</stro> <code>{{ prefixes[0] }}{{ command.name }} {{ command.signature }}</code> <a href="javascript:copyTextToClipboard('{{ prefixes[0] }}{{ command.name }} {{ command.signature }}');" title="{{ _("Copy to clipboard") }}"><i class="far fa-copy me-2"></i></a>
+                                                                      <strong>{{ _("Usage:") }}</strong>
+                                                                      <div class="d-flex"><code>{{ prefixes[0] }}{{ command.name }} {{ command.signature }}</code> <a href="javascript:copyTextToClipboard('{{ prefixes[0] }}{{ command.name }} {{ command.signature }}');" title="{{ _("Copy to clipboard") }}"><i class="far fa-copy me-2"></i></a></div>
                                                                     {% endif %}
+                                                                    <br />
                                                                     {% if command.aliases %}
-                                                                      <strong>{{ _("Aliases:") }}</strong> <code>{{ command.aliases|join(", ") }}</code>
+                                                                      <strong>{{ _("Aliases:") }}</strong>
+                                                                      <code>{{ command.aliases|join(", ") }}</code>
                                                                     {% endif %}
                                                                   </div>
                                                                 </div>
                                                               </td>
                                                             </tr>
                                                           {% endif %}
                                                           {% if command.subs %}
@@ -152,29 +155,28 @@
                                           {% if (not tab_name or cogs[cog]["name"] == tab_name) and query.lower() in command["name"].lower() %}
                                             <tr data-toggle="collapse" href="#collapse_{{ command.name }}" role="button" aria-expanded="false" aria-controls="collapse_{{ command.name }}">
                                               <td class="text-{{ variables["meta"]["color"] }}" style="padding-left: {{ loop.depth0 * 40 + 24 }}px" title="{{ command.name }} {{ command.signature }}">
                                                 <span class="prefix">{{ prefixes[0] }}</span>{{ command.name }}
                                               </td>
                                               <td style="padding-left: 24px" class="text-wrap">{{ command.short_description|markdown }}</td>
                                             </tr>
-                                            {% if command.signature or command.aliases or command.description %}
+                                            {% if command.signature or command.aliases %}
                                               <tr>
                                                 <td colspan="2" style="border: none; padding: 0px;">
                                                   <div class="collapse" id="collapse_{{ command.name }}">
                                                     <div class="d-flex card card-body text-wrap">
-                                                      {% if command.signature or command.aliases %}
-                                                        {% if command.signature %}
-                                                          <strong>{{ _("Usage:") }}</stro> <code>{{ prefixes[0] }}{{ command.name }} {{ command.signature }}</code> <a href="javascript:copyTextToClipboard('{{ prefixes[0] }}{{ command.name }} {{ command.signature }}');" title="{{ _("Copy to clipboard") }}"><i class="far fa-copy me-2"></i></a>
-                                                        {% endif %}
-                                                        {% if command.aliases %}
-                                                          <strong>{{ _("Aliases:") }}</strong> <code>{{ command.aliases|join(", ") }}</code>
-                                                        {% endif %}
-                                                        <br /><br />
+                                                      {% if command.signature %}
+                                                        <strong>{{ _("Usage:") }}</strong>
+                                                        <div class="d-flex"><code>{{ prefixes[0] }}{{ command.name }} {{ command.signature }}</code> <a href="javascript:copyTextToClipboard('{{ prefixes[0] }}{{ command.name }} {{ command.signature }}');" title="{{ _("Copy to clipboard") }}"><i class="far fa-copy me-2"></i></a></div>
+                                                      {% endif %}
+                                                      <br />
+                                                      {% if command.aliases %}
+                                                        <strong>{{ _("Aliases:") }}</strong>
+                                                        <code>{{ command.aliases|join(", ") }}</code>
                                                       {% endif %}
-                                                      {{ command.description|markdown }}
                                                     </div>
                                                   </div>
                                                 </td>
                                               </tr>
                                             {% endif %}
                                             {% if command.subs %}
                                               {{ loop(command.subs) }}
```

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/pages/credits.html` & `red_web_dashboard-1.5.0/reddash/app/templates/pages/credits.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/pages/dashboard.html` & `red_web_dashboard-1.5.0/reddash/app/templates/pages/dashboard.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/pages/dashboard_guild.html` & `red_web_dashboard-1.5.0/reddash/app/templates/pages/dashboard_guild.html`

 * *Files 1% similar despite different names*

```diff
@@ -44,22 +44,22 @@
                                     </div>
                                     <div class="mt-4">
 
                                         {% if aliases_form %}
                                             <div id="Alias">
                                                 <div class="card">
                                                     <div class="card-header" id="headingAlias">
-                                                        <a class="btn btn-link" data-toggle="collapse" data-target="#collapseAlias" aria-expanded="true" aria-controls="collapseAlias" style="width: 100%;">
+                                                        <a class="btn btn-link mb-0" data-toggle="collapse" data-target="#collapseAlias" aria-expanded="true" aria-controls="collapseAlias" style="width: 100%;">
                                                             <div class="d-flex justify-content-between align-items-center">
                                                                 <h4 class="mb-0">{{ _("Alias") }}</h4>
                                                                 <h4><i class="fa fa-arrow-circle-o-down"></i></h4>
                                                             </div>
                                                         </a>
                                                     </div>
-                                                    <div id="collapseAlias" class="collapse card-body" aria-labelledby="headingAlias" data-parent="#accordion">
+                                                    <div id="collapseAlias" class="collapse card-body" aria-labelledby="headingAlias">
                                                         <form action="" method="POST" role="form" enctype="multipart/form-data">
                                                             {{ aliases_form.hidden_tag() }}
                                                             {% for alias_form in aliases_form.aliases.default %}
                                                                 <div class="row mb-3">
                                                                     {% if loop.index0 > 0 %}
                                                                         <hr class="horizontal dark" />
                                                                     {% endif %}
@@ -90,22 +90,22 @@
                                         {% endif %}
 
                                         {% if custom_commands_form %}
                                             <br />
                                             <div id="CustomCommands">
                                                 <div class="card">
                                                     <div class="card-header" id="headingCustomCommands">
-                                                        <a class="btn btn-link" data-toggle="collapse" data-target="#collapseCustomCommands" aria-expanded="true" aria-controls="collapseCustomCommands" style="width: 100%;">
+                                                        <a class="btn btn-link mb-0" data-toggle="collapse" data-target="#collapseCustomCommands" aria-expanded="true" aria-controls="collapseCustomCommands" style="width: 100%;">
                                                             <div class="d-flex justify-content-between align-items-center">
                                                                 <h4 class="mb-0">{{ _("CustomCommands") }}</h4>
                                                                 <h4><i class="fa fa-arrow-circle-o-down"></i></h4>
                                                             </div>
                                                         </a>
                                                     </div>
-                                                    <div id="collapseCustomCommands" class="collapse card-body" aria-labelledby="headingCustomCommands" data-parent="#accordion">
+                                                    <div id="collapseCustomCommands" class="collapse card-body" aria-labelledby="headingCustomCommands">
                                                         <form action="" method="POST" role="form" enctype="multipart/form-data">
                                                             {{ custom_commands_form.hidden_tag() }}
                                                             {% for custom_command_form in custom_commands_form.custom_commands.default %}
                                                                 <div class="row mb-3">
                                                                     {% if loop.index0 > 0 %}
                                                                         <hr class="horizontal dark" />
                                                                     {% endif %}
@@ -283,14 +283,17 @@
         $('#guild-content a[data-toggle="pill"]').on("shown.bs.tab", function (e) {
             var base_url = '{{ url_for("base_blueprint.dashboard_guild", guild_id=guild.id) }}';
             var target_id = e.target.id.slice(0, -4);
             if (target_id == "third-parties") {
                 resize_event = new Event("resize");
                 window.dispatchEvent(resize_event);
             }
+            if (!["overview", "settings", "third-parties"].includes(target_id)) {
+                target_id = "third-parties/" + target_id;
+            }
             if (target_id == "overview") {
                 var new_url = base_url;
             } else {
                 var new_url = base_url + "/" + target_id;
             }
             if (!(window.location.pathname.startsWith(new_url)) || (target_id == "overview" && !(window.location.pathname == base_url))) {
                 // window.location.pathname = new_url;
```

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/pages/guild_profile.html` & `red_web_dashboard-1.5.0/reddash/app/templates/pages/guild_profile.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <div id="profile" class="card card-body col-md-3 mt-4 align-items-center" style="margin-left: 10px; margin-right: 10px;">
     <div {% if False %}class="row"{% endif %}>
         <br />
         <div class="col-sm-auto col-4 text-center">
-            <div class="avatar avatar-xl"><img src="{{ guild.icon_url }}"{% if guild.icon_animated %} onmouseover="playGif(this);" onmouseout="stopGif(this);"{% endif %} class="shadow-sm border-radius-lg" style="height: 170%; width: 170%;" /></div>
+            <div class="avatar avatar-xl"><img src={% if guild.icon_animated %}"{{ guild.icon_url[:-3] + "png" }}" onmouseover='this.src = this.src.slice(0, -3) + "gif";' onmouseout='this.src = this.src.slice(0, -3) + "png";'{% else %}"{{ guild.icon_url }}"{% endif %} class="shadow-sm border-radius-lg" style="height: 170%; width: 170%;" /></div>
         </div>
         <div class="col-sm-auto col-8 my-auto">
             <div class="h-100">
                 <h3 class="col mb-1 font-weight-bolder text-center">
                     {{ guild.name }}
                     <div class="dropdown" style="display: unset;">
                         <a class="nav-link text-lg text-dark" role="button" id="guild_dropdown" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false" style="display: unset; vertical-align: 2.6px; margin-left: 2px;">
@@ -51,27 +51,14 @@
     <h6 class="text-secondary" style="margin-bottom: 0rem;">{{ _("Created at:") }} {{ moment(guild.created_at).format("Do MMMM YYYY") }}</h6>
     {% if guild.joined_at %}
         <h6 class="text-secondary">{{ _("Bot joined at:") }} {{ moment(guild.joined_at).format("Do MMMM YYYY") }}</h6>
     {% endif %}
 </div>
             
 {% block javascripts %}
-    {% if guild.icon_animated %}
-        <script>
-            function playGif(element) {
-                element.src = element.src.replace(".png", ".gif");
-            }
-            function stopGif(element) {
-                element.src = element.src.replace(".gif", ".png");
-            }
-            document.addEventListener("DOMContentLoaded", function() {
-                stopGif(document.querySelector("#profile img"));
-            });
-        </script>
-    {% endif %}
     <script>
         async function confirmLeaveGuild(event) {
             if (confirmationDone) {
                 return true;
             }
             let target_button = event.target;
             event.preventDefault();
```

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/pages/index.html` & `red_web_dashboard-1.5.0/reddash/app/templates/pages/index.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/pages/login/login.html` & `red_web_dashboard-1.5.0/reddash/app/templates/pages/login/login.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/pages/third_parties/oauth.html` & `red_web_dashboard-1.5.0/reddash/app/templates/pages/third_parties/oauth.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/pages/third_parties/third_parties_list.html` & `red_web_dashboard-1.5.0/reddash/app/templates/pages/third_parties/third_parties_list.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.4.0/reddash/app/templates/pages/third_parties/third_party.html` & `red_web_dashboard-1.5.0/reddash/app/templates/pages/third_parties/third_party.html`

 * *Files 8% similar despite different names*

```diff
@@ -40,20 +40,20 @@
                         <div class="card card-chart">
                             <div class="card-body">
                                 <div class="row">
                                     <div class="col-sm-12 text-left">
                                         <div class="d-flex justify-content-between mb-4">
                                             {% if guild %}
                                                 {% if not fullscreen %}
-                                                    <h2 class="card-title"><a href="{{ url_for("base_blueprint.dashboard_guild", guild_id=guild.id, page="third-parties", third_party=name) }}">🔙 {{ name }}</a></h2>
+                                                    <h2 class="card-title"><a href="{{ url_for("base_blueprint.dashboard_guild", guild_id=guild.id, page="third-parties", third_party=name) }}">🔙 {{ name }}</a>{% if page %} / {{ page|replace("_", " ")|replace("-", " ")|title }}{% endif %}</h2>
                                                 {% else %}
-                                                    <h2 class="card-title"><a href="{{ url_for("base_blueprint.dashboard_guild", guild_id=guild.id) }}"><img src="{{ guild.icon_url }}" style="height: 50px; vertical-align: -13px; border-radius: 50%; margin: none; display: inline;" /> {{ guild.name }}</a> / <a href="{{ url_for("base_blueprint.dashboard_guild", guild_id=guild.id, page="third-parties", third_party=name) }}">🔙 {{ name }}</a></h2>
+                                                    <h2 class="card-title"><a href="{{ url_for("base_blueprint.dashboard_guild", guild_id=guild.id) }}"><img src="{{ guild.icon_url }}" style="height: 50px; vertical-align: -13px; border-radius: 50%; margin: none; display: inline;" /> {{ guild.name }}</a> / <a href="{{ url_for("base_blueprint.dashboard_guild", guild_id=guild.id, page="third-parties", third_party=name) }}">🔙 {{ name }}</a>{% if page %} / {{ page|replace("_", " ")|replace("-", " ")|title }}{% endif %}</h2>
                                                 {% endif %}
                                             {% else %}
-                                                <h2 class="card-title"><a href="{{ url_for("third_parties_blueprint.third_parties", third_party=name) }}">🔙 {{ name }}</a></h2>
+                                                <h2 class="card-title"><a href="{{ url_for("third_parties_blueprint.third_parties", third_party=name) }}">🔙 {{ name }}</a>{% if page %} / {{ page|replace("_", " ")|replace("-", " ")|title }}{% endif %}</h2>
                                             {% endif %}
                                         </div>
                                     </div>
                                 </div>
                                 <div class="container mt-4">
                                     {{ source_content|safe }}
                                 </div>
```

#### html2text {}

```diff
@@ -8,17 +8,20 @@
     * }" class="nav-link"> {{ _("Overview") }}
 }}" class="nav-link"> {{ _("Settings") }}
 }}" class="nav-link show active" id="third-parties-tab"> {{ _("Third Parties")
 }}
 
 {% endif %}
 {% if guild %} {% if not fullscreen %}
-********** tthhiirrdd__ppaarrttyy==nnaammee)) }}}}"">>?ð??? {{{{ nnaammee }}}} **********
+********** tthhiirrdd__ppaarrttyy==nnaammee)) }}}}"">>?ð??? {{{{ nnaammee }}}}{{%% iiff ppaaggee %%}} // {{{{ ppaaggee||rreeppllaaccee((""__"",,
+"" ""))||rreeppllaaccee((""--"",, "" ""))||ttiittllee }}}}{{%% eennddiiff %%}} **********
 {% else %}
 ********** }}"">>[[{{{{ gguuiilldd..iiccoonn__uurrll }}}}]] {{{{ gguuiilldd..nnaammee }}}} // tthhiirrdd__ppaarrttyy==nnaammee)) }}}}"">>?ð??? {{
-{{ nnaammee }}}} **********
+{{ nnaammee }}}}{{%% iiff ppaaggee %%}} // {{{{ ppaaggee||rreeppllaaccee((""__"",, "" ""))||rreeppllaaccee((""--"",, "" ""))||ttiittllee }}}}{{%%
+eennddiiff %%}} **********
 {% endif %} {% else %}
-********** }}"">>?ð??? {{{{ nnaammee }}}} **********
+********** }}"">>?ð??? {{{{ nnaammee }}}}{{%% iiff ppaaggee %%}} // {{{{ ppaaggee||rreeppllaaccee((""__"",, "" ""))||rreeppllaaccee((""--"",,
+"" ""))||ttiittllee }}}}{{%% eennddiiff %%}} **********
 {% endif %}
 {{ source_content|safe }}
 {% endblock %} {% block javascripts %}
 {% endblock %}
```

### Comparing `red_web_dashboard-1.4.0/reddash/app/utils.py` & `red_web_dashboard-1.5.0/reddash/app/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,20 +56,20 @@
     USERS: typing.Dict[str, "User"] = {}
 
     def __init__(
         self,
         id: int,
         name: str,
         global_name: typing.Optional[str] = None,
-        avatar_url: str = "https://cdn.discordapp.com/embed/avatars/2.png",
+        avatar_url: typing.Optional[str] = None,
     ) -> None:
         self.id: int = id
         self.name: str = name
         self.global_name: typing.Optional[str] = global_name
-        self.avatar_url: str = avatar_url
+        self.avatar_url: typing.Optional[str] = avatar_url
 
         self.devices: typing.List[str] = []
 
         self.__class__.USERS[self.id] = self
 
     def get_id(self) -> str:
         token = self.generate_token(
@@ -86,14 +86,18 @@
         return f"<User id={self.id!r} name={self.name!r} global_name={self.global_name!r} avatar_url={self.avatar_url!r}>"
 
     @property
     def display_name(self) -> str:
         return self.global_name or self.name
 
     @property
+    def display_avatar(self) -> str:
+        return self.avatar_url or f"https://cdn.discordapp.com/embed/avatars/{(self.id >> 22) % 6}.png"
+
+    @property
     def is_owner(self) -> bool:
         return self.id in app.variables["bot"]["owner_ids"]
 
     @property
     def is_active(self) -> bool:
         return not self.is_blacklisted
 
@@ -218,16 +222,16 @@
     def init_field(field, *args, **kwargs):
         initial_init_field(field, *args, **kwargs)
         if isinstance(field, FormField):
             return
         if hasattr(field, "_value"):
             field._real_value = field._value
         field._value = lambda: (field._real_value() if hasattr(field, "_real_value") else "") or (
-            (str(field.default) if not isinstance(field.default, typing.List) else field.default)
-            if field.default
+            (field.default if isinstance(field.default, typing.List) else str(field.default))
+            if field.default is not None
             else ""
         )
         if isinstance(field, SelectFieldBase):
             old_choices_generator = field._choices_generator
 
             def _choices_generator(choices):
                 for value, label, selected, render_kw in old_choices_generator(choices):
```

### Comparing `red_web_dashboard-1.4.0/setup.cfg` & `red_web_dashboard-1.5.0/setup.cfg`

 * *Files identical despite different names*

