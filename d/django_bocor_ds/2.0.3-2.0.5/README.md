# Comparing `tmp/django_bocor_ds-2.0.3.tar.gz` & `tmp/django_bocor_ds-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_bocor_ds-2.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_bocor_ds-2.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_bocor_ds-2.0.3.tar` & `django_bocor_ds-2.0.5.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0     6148 2024-04-03 00:07:39.524906 django_bocor_ds-2.0.3/.DS_Store
--rw-r--r--   0        0        0       66 2024-03-21 05:49:50.372491 django_bocor_ds-2.0.3/.gitattributes
--rw-r--r--   0        0        0        7 2024-03-29 05:46:41.713784 django_bocor_ds-2.0.3/.gitignore
--rw-r--r--   0        0        0       52 2024-03-21 06:06:29.551428 django_bocor_ds-2.0.3/.idea/.gitignore
--rw-r--r--   0        0        0      405 2024-03-21 06:06:29.465715 django_bocor_ds-2.0.3/.idea/django-bocor-ds.iml
--rw-r--r--   0        0        0      174 2024-03-21 06:06:29.480874 django_bocor_ds-2.0.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      421 2024-03-21 06:08:26.611158 django_bocor_ds-2.0.3/.idea/misc.xml
--rw-r--r--   0        0        0      282 2024-03-21 06:06:29.471790 django_bocor_ds-2.0.3/.idea/modules.xml
--rw-r--r--   0        0        0      167 2024-03-21 06:06:29.484071 django_bocor_ds-2.0.3/.idea/vcs.xml
--rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_bocor_ds-2.0.3/LICENSE
--rw-r--r--   0        0        0     1758 2024-03-28 01:05:44.950188 django_bocor_ds-2.0.3/README.md
--rw-r--r--   0        0        0     6148 2024-04-03 00:07:39.525868 django_bocor_ds-2.0.3/django_bocor_ds/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-21 06:07:02.999245 django_bocor_ds-2.0.3/django_bocor_ds/__init__.py
--rw-r--r--   0        0        0      495 2024-03-26 07:24:10.511682 django_bocor_ds-2.0.3/django_bocor_ds/admin.py
--rw-r--r--   0        0        0      160 2024-03-21 06:07:03.001129 django_bocor_ds-2.0.3/django_bocor_ds/apps.py
--rw-r--r--   0        0        0      947 2024-03-24 12:14:35.423434 django_bocor_ds-2.0.3/django_bocor_ds/forms.py
--rw-r--r--   0        0        0     1915 2024-03-26 07:22:15.008801 django_bocor_ds-2.0.3/django_bocor_ds/migrations/0001_initial.py
--rw-r--r--   0        0        0      540 2024-03-26 08:05:25.492109 django_bocor_ds-2.0.3/django_bocor_ds/migrations/0002_remove_portfolio_image3_remove_portfolio_image4_and_more.py
--rw-r--r--   0        0        0      502 2024-03-27 02:55:50.933146 django_bocor_ds-2.0.3/django_bocor_ds/migrations/0003_portfolio_redirect_link.py
--rw-r--r--   0        0        0      351 2024-03-27 05:19:19.375307 django_bocor_ds-2.0.3/django_bocor_ds/migrations/0004_remove_portfolio_redirect_link.py
--rw-r--r--   0        0        0        0 2024-03-21 06:07:03.001526 django_bocor_ds-2.0.3/django_bocor_ds/migrations/__init__.py
--rw-r--r--   0        0        0      948 2024-03-27 05:06:04.714022 django_bocor_ds-2.0.3/django_bocor_ds/models.py
--rw-r--r--   0        0        0     6148 2024-03-21 08:10:33.959729 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/.DS_Store
--rwxr-xr-x   0        0        0    24397 2024-03-26 06:27:59.841052 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/css/style.css
--rwxr-xr-x   0        0        0   249630 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/img/footer-bg.jpg
--rwxr-xr-x   0        0        0     5114 2024-03-17 05:37:08.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/js/main.js
--rwxr-xr-x   0        0        0     2893 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/scss/_footer.scss
--rwxr-xr-x   0        0        0     1290 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/scss/_general.scss
--rwxr-xr-x   0        0        0      709 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/scss/_header.scss
--rwxr-xr-x   0        0        0     1422 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/scss/_hero.scss
--rwxr-xr-x   0        0        0     4101 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/scss/_nav.scss
--rwxr-xr-x   0        0        0    15555 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/scss/_sections.scss
--rwxr-xr-x   0        0        0      454 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/scss/_variables.scss
--rwxr-xr-x   0        0        0      136 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/scss/style.scss
--rw-r--r--   0        0        0    19941 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/aos/aos.cjs.js
--rw-r--r--   0        0        0    28765 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/aos/aos.css
--rw-r--r--   0        0        0    19768 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/aos/aos.esm.js
--rw-r--r--   0        0        0    13800 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/aos/aos.js
--rw-r--r--   0        0        0    56459 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/aos/aos.js.map
--rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.css
--rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.json
--rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.min.css
--rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.scss
--rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css
--rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css
--rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css
--rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css.map
--rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css
--rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css.map
--rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css
--rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css
--rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css.map
--rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css
--rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css.map
--rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css
--rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css.map
--rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css
--rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css.map
--rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js
--rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js
--rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js.map
--rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js.map
--rw-r--r--   0        0        0     7522 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/css/animations.css
--rw-r--r--   0        0        0    94202 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.css
--rw-r--r--   0        0        0    68028 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.min.css
--rw-r--r--   0        0        0      683 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/css/transformations.css
--rw-r--r--   0        0        0   405670 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.eot
--rw-r--r--   0        0        0  1242122 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.svg
--rw-r--r--   0        0        0   320944 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.ttf
--rw-r--r--   0        0        0   321020 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff
--rw-r--r--   0        0        0   115680 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff2
--rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.css
--rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.min.css
--rw-r--r--   0        0        0    52561 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.css
--rw-r--r--   0        0        0    45081 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.min.css
--rw-r--r--   0        0        0   109391 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.js
--rw-r--r--   0        0        0    55880 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.min.js
--rw-r--r--   0        0        0    91398 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.js
--rw-r--r--   0        0        0    35445 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.min.js
--rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/php-email-form/php-email-form.php
--rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/php-email-form/validate.js
--rw-r--r--   0        0        0    18436 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.css
--rw-r--r--   0        0        0   149147 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js
--rw-r--r--   0        0        0   201656 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js.map
--rw-r--r--   0        0        0     6148 2024-04-03 00:07:46.476654 django_bocor_ds-2.0.3/django_bocor_ds/templates/.DS_Store
--rwxr-xr-x   0        0        0     6381 2024-03-17 05:37:08.000000 django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/__inner-page.html
--rw-r--r--   0        0        0     8057 2024-03-26 07:30:05.640370 django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/__portfolio-details.html
--rw-r--r--   0        0        0     1220 2024-03-27 06:57:48.371319 django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_about.html
--rw-r--r--   0        0        0      735 2024-03-25 05:29:33.069856 django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_clients.html
--rw-r--r--   0        0        0     2808 2024-04-03 06:55:44.662722 django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_contact.html
--rw-r--r--   0        0        0      834 2024-03-27 06:19:40.055323 django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_faq.html
--rw-r--r--   0        0        0     1414 2024-03-27 06:27:58.932985 django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_features.html
--rw-r--r--   0        0        0      612 2024-03-26 01:35:37.535937 django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_hero.html
--rw-r--r--   0        0        0     1546 2024-03-27 06:25:38.395922 django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_portfolio.html
--rw-r--r--   0        0        0     1178 2024-03-27 06:19:40.048164 django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_pricing.html
--rw-r--r--   0        0        0     1142 2024-03-27 06:32:01.686698 django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_services.html
--rw-r--r--   0        0        0     1646 2024-03-27 06:24:03.103818 django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_team.html
--rw-r--r--   0        0        0     2370 2024-03-27 01:37:49.536434 django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/footer.html
--rw-r--r--   0        0        0     1398 2024-03-29 05:45:01.813266 django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/header.html
--rw-r--r--   0        0        0     3561 2024-03-26 06:02:21.891761 django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/index.html
--rw-r--r--   0        0        0     1893 2024-03-26 06:50:42.398917 django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/seo.html
--rw-r--r--   0        0        0        0 2023-03-21 07:32:09.033136 django_bocor_ds-2.0.3/django_bocor_ds/templatetags/__init__.py
--rw-r--r--   0        0        0     5223 2024-03-22 23:51:55.383813 django_bocor_ds-2.0.3/django_bocor_ds/templatetags/bocords_tags.py
--rw-r--r--   0        0        0       60 2024-03-21 06:07:03.001392 django_bocor_ds-2.0.3/django_bocor_ds/tests.py
--rw-r--r--   0        0        0      265 2024-03-27 05:05:51.517275 django_bocor_ds-2.0.3/django_bocor_ds/urls.py
--rw-r--r--   0        0        0     2469 2024-04-03 06:57:03.342404 django_bocor_ds-2.0.3/django_bocor_ds/views.py
--rw-r--r--   0        0        0      783 2024-04-03 06:58:08.579839 django_bocor_ds-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 django_bocor_ds-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     8196 2024-04-13 00:01:41.783512 django_bocor_ds-2.0.5/.DS_Store
+-rw-r--r--   0        0        0       66 2024-03-21 05:49:50.372491 django_bocor_ds-2.0.5/.gitattributes
+-rw-r--r--   0        0        0        7 2024-03-29 05:46:41.713784 django_bocor_ds-2.0.5/.gitignore
+-rw-r--r--   0        0        0       52 2024-03-21 06:06:29.551428 django_bocor_ds-2.0.5/.idea/.gitignore
+-rw-r--r--   0        0        0      405 2024-03-21 06:06:29.465715 django_bocor_ds-2.0.5/.idea/django-bocor-ds.iml
+-rw-r--r--   0        0        0      174 2024-03-21 06:06:29.480874 django_bocor_ds-2.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      421 2024-03-21 06:08:26.611158 django_bocor_ds-2.0.5/.idea/misc.xml
+-rw-r--r--   0        0        0      282 2024-03-21 06:06:29.471790 django_bocor_ds-2.0.5/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2024-03-21 06:06:29.484071 django_bocor_ds-2.0.5/.idea/vcs.xml
+-rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_bocor_ds-2.0.5/LICENSE
+-rw-r--r--   0        0        0     1759 2024-04-05 23:52:20.518931 django_bocor_ds-2.0.5/README.md
+-rw-r--r--   0        0        0     6148 2024-04-13 00:02:19.172196 django_bocor_ds-2.0.5/django_bocor_ds/.DS_Store
+-rw-r--r--   0        0        0        0 2024-03-21 06:07:02.999245 django_bocor_ds-2.0.5/django_bocor_ds/__init__.py
+-rw-r--r--   0        0        0      495 2024-03-26 07:24:10.511682 django_bocor_ds-2.0.5/django_bocor_ds/admin.py
+-rw-r--r--   0        0        0      160 2024-03-21 06:07:03.001129 django_bocor_ds-2.0.5/django_bocor_ds/apps.py
+-rw-r--r--   0        0        0      947 2024-03-24 12:14:35.423434 django_bocor_ds-2.0.5/django_bocor_ds/forms.py
+-rw-r--r--   0        0        0     1915 2024-03-26 07:22:15.008801 django_bocor_ds-2.0.5/django_bocor_ds/migrations/0001_initial.py
+-rw-r--r--   0        0        0      540 2024-03-26 08:05:25.492109 django_bocor_ds-2.0.5/django_bocor_ds/migrations/0002_remove_portfolio_image3_remove_portfolio_image4_and_more.py
+-rw-r--r--   0        0        0      502 2024-03-27 02:55:50.933146 django_bocor_ds-2.0.5/django_bocor_ds/migrations/0003_portfolio_redirect_link.py
+-rw-r--r--   0        0        0      351 2024-03-27 05:19:19.375307 django_bocor_ds-2.0.5/django_bocor_ds/migrations/0004_remove_portfolio_redirect_link.py
+-rw-r--r--   0        0        0        0 2024-03-21 06:07:03.001526 django_bocor_ds-2.0.5/django_bocor_ds/migrations/__init__.py
+-rw-r--r--   0        0        0      948 2024-03-27 05:06:04.714022 django_bocor_ds-2.0.5/django_bocor_ds/models.py
+-rw-r--r--   0        0        0     6148 2024-03-21 08:10:33.959729 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/.DS_Store
+-rwxr-xr-x   0        0        0    24429 2024-04-03 08:25:58.403114 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/css/style.css
+-rwxr-xr-x   0        0        0   249630 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/img/footer-bg.jpg
+-rwxr-xr-x   0        0        0     5114 2024-03-17 05:37:08.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/js/main.js
+-rwxr-xr-x   0        0        0     2893 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/scss/_footer.scss
+-rwxr-xr-x   0        0        0     1290 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/scss/_general.scss
+-rwxr-xr-x   0        0        0      709 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/scss/_header.scss
+-rwxr-xr-x   0        0        0     1422 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/scss/_hero.scss
+-rwxr-xr-x   0        0        0     4101 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/scss/_nav.scss
+-rwxr-xr-x   0        0        0    15555 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/scss/_sections.scss
+-rwxr-xr-x   0        0        0      454 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/scss/_variables.scss
+-rwxr-xr-x   0        0        0      136 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/scss/style.scss
+-rw-r--r--   0        0        0    19941 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/aos/aos.cjs.js
+-rw-r--r--   0        0        0    28765 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/aos/aos.css
+-rw-r--r--   0        0        0    19768 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/aos/aos.esm.js
+-rw-r--r--   0        0        0    13800 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/aos/aos.js
+-rw-r--r--   0        0        0    56459 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/aos/aos.js.map
+-rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.css
+-rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.json
+-rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.min.css
+-rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.scss
+-rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css
+-rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js
+-rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0     7522 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/css/animations.css
+-rw-r--r--   0        0        0    94202 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.css
+-rw-r--r--   0        0        0    68028 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.min.css
+-rw-r--r--   0        0        0      683 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/css/transformations.css
+-rw-r--r--   0        0        0   405670 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.eot
+-rw-r--r--   0        0        0  1242122 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.svg
+-rw-r--r--   0        0        0   320944 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.ttf
+-rw-r--r--   0        0        0   321020 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff
+-rw-r--r--   0        0        0   115680 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff2
+-rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.css
+-rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.min.css
+-rw-r--r--   0        0        0    52561 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.css
+-rw-r--r--   0        0        0    45081 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.min.css
+-rw-r--r--   0        0        0   109391 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.js
+-rw-r--r--   0        0        0    55880 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.min.js
+-rw-r--r--   0        0        0    91398 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.js
+-rw-r--r--   0        0        0    35445 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.min.js
+-rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/php-email-form/php-email-form.php
+-rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/php-email-form/validate.js
+-rw-r--r--   0        0        0    18436 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.css
+-rw-r--r--   0        0        0   149147 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js
+-rw-r--r--   0        0        0   201656 2024-03-12 00:49:58.000000 django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js.map
+-rw-r--r--   0        0        0     6148 2024-04-03 00:07:46.476654 django_bocor_ds-2.0.5/django_bocor_ds/templates/.DS_Store
+-rwxr-xr-x   0        0        0     6381 2024-03-17 05:37:08.000000 django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/__inner-page.html
+-rw-r--r--   0        0        0     8057 2024-03-26 07:30:05.640370 django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/__portfolio-details.html
+-rw-r--r--   0        0        0     1220 2024-03-27 06:57:48.371319 django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_about.html
+-rw-r--r--   0        0        0      735 2024-03-25 05:29:33.069856 django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_clients.html
+-rw-r--r--   0        0        0     2808 2024-04-03 06:55:44.662722 django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_contact.html
+-rw-r--r--   0        0        0      834 2024-03-27 06:19:40.055323 django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_faq.html
+-rw-r--r--   0        0        0     1414 2024-03-27 06:27:58.932985 django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_features.html
+-rw-r--r--   0        0        0      612 2024-03-26 01:35:37.535937 django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_hero.html
+-rw-r--r--   0        0        0     1546 2024-03-27 06:25:38.395922 django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_portfolio.html
+-rw-r--r--   0        0        0     1178 2024-03-27 06:19:40.048164 django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_pricing.html
+-rw-r--r--   0        0        0     1142 2024-03-27 06:32:01.686698 django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_services.html
+-rw-r--r--   0        0        0     1646 2024-03-27 06:24:03.103818 django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_team.html
+-rw-r--r--   0        0        0     2404 2024-04-04 04:41:10.261572 django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/footer.html
+-rw-r--r--   0        0        0     1452 2024-04-21 07:23:02.021277 django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/header.html
+-rw-r--r--   0        0        0     3561 2024-03-26 06:02:21.891761 django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/index.html
+-rw-r--r--   0        0        0     1914 2024-04-03 08:20:59.077335 django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/seo.html
+-rw-r--r--   0        0        0        0 2023-03-21 07:32:09.033136 django_bocor_ds-2.0.5/django_bocor_ds/templatetags/__init__.py
+-rw-r--r--   0        0        0     5223 2024-03-22 23:51:55.383813 django_bocor_ds-2.0.5/django_bocor_ds/templatetags/bocords_tags.py
+-rw-r--r--   0        0        0       60 2024-03-21 06:07:03.001392 django_bocor_ds-2.0.5/django_bocor_ds/tests.py
+-rw-r--r--   0        0        0      265 2024-03-27 05:05:51.517275 django_bocor_ds-2.0.5/django_bocor_ds/urls.py
+-rw-r--r--   0        0        0     2469 2024-04-03 06:57:03.342404 django_bocor_ds-2.0.5/django_bocor_ds/views.py
+-rw-r--r--   0        0        0      783 2024-04-21 07:25:36.561240 django_bocor_ds-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2261 1970-01-01 00:00:00.000000 django_bocor_ds-2.0.5/PKG-INFO
```

### Comparing `django_bocor_ds-2.0.3/.DS_Store` & `django_bocor_ds-2.0.5/django_bocor_ds/.DS_Store`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 040a 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0007  ................
-00000050: 0000 0001 0000 1000 0061 6277 7370 626c  .........abwspbl
-00000060: 6f62 0000 0000 0000 0000 0000 0000 0000  ob..............
+00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
+00000050: 0000 0001 0000 1000 006c 0061 0074 0065  .........l.a.t.e
+00000060: 0073 6277 0000 0000 0000 0000 0000 0000  .sbw............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -58,67 +58,67 @@
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000400: 0000 0000 0000 0000 0000 0007 0000 0005  ................
-00000410: 005f 0064 0061 0074 0061 6277 7370 626c  ._.d.a.t.abwspbl
-00000420: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
-00000430: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
-00000440: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
-00000450: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00000460: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00000470: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00000480: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00000490: 7208 0908 095f 1018 7b7b 3130 352c 2038  r...._..{{105, 8
-000004a0: 3730 7d2c 207b 3932 302c 2034 3336 7d7d  70}, {920, 436}}
-000004b0: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
-000004c0: 0000 0000 0101 0000 0000 0000 000d 0000  ................
-000004d0: 0000 0000 0000 0000 0000 0000 008b 0000  ................
-000004e0: 0005 005f 0064 0061 0074 0061 7653 726e  ..._.d.a.t.avSrn
-000004f0: 6c6f 6e67 0000 0001 0000 0009 005f 006d  long........._.m
-00000500: 0079 0074 0065 0073 0074 0065 0072 6469  .y.t.e.s.t.e.rdi
-00000510: 6c63 626c 6f62 0000 0020 0000 0000 0001  lcblob... ......
-00000520: 21cd ffff ffbf 0000 00b1 0001 7f3e 0000  !............>..
-00000530: 3003 ffff ffff ffff 0000 0000 0007 005f  0.............._
-00000540: 0073 0074 0061 0074 0069 0063 6277 7370  .s.t.a.t.i.cbwsp
-00000550: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
-00000560: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
-00000570: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-00000580: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
-00000590: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
-000005a0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
-000005b0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-000005c0: 6261 7208 0908 095f 1018 7b7b 3130 352c  bar...._..{{105,
-000005d0: 2038 3730 7d2c 207b 3932 302c 2034 3336   870}, {920, 436
-000005e0: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
-000005f0: 0000 0000 0000 0101 0000 0000 0000 000d  ................
-00000600: 0000 0000 0000 0000 0000 0000 0000 008b  ................
-00000610: 0000 0007 005f 0073 0074 0061 0074 0069  ....._.s.t.a.t.i
-00000620: 0063 7653 726e 6c6f 6e67 0000 0001 0000  .cvSrnlong......
-00000630: 000f 0064 006a 0061 006e 0067 006f 005f  ...d.j.a.n.g.o._
-00000640: 0062 006f 0063 006f 0072 005f 0064 0073  .b.o.c.o.r._.d.s
-00000650: 6277 7370 626c 6f62 0000 00b9 6270 6c69  bwspblob....bpli
-00000660: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
-00000670: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
-00000680: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00000690: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-000006a0: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-000006b0: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-000006c0: 5369 6465 6261 7208 0908 095f 1019 7b7b  Sidebar...._..{{
-000006d0: 3133 3239 2c20 3534 317d 2c20 7b39 3230  1329, 541}, {920
-000006e0: 2c20 3433 367d 7d09 0815 232f 3b52 5f6b  , 436}}...#/;R_k
-000006f0: 6c6d 6e6f 8b00 0000 0000 0001 0100 0000  lmno............
-00000700: 0000 0000 0d00 0000 0000 0000 0000 0000  ................
-00000710: 0000 0000 8c00 0000 0f00 6400 6a00 6100  ..........d.j.a.
-00000720: 6e00 6700 6f00 5f00 6200 6f00 6300 6f00  n.g.o._.b.o.c.o.
-00000730: 7200 5f00 6400 7376 5372 6e6c 6f6e 6700  r._.d.svSrnlong.
-00000740: 0000 0100 0000 0000 0000 0000 0000 0000  ................
+00000400: 0000 0000 0000 0000 0000 0004 0000 0009  ................
+00000410: 0074 0065 006d 0070 006c 0061 0074 0065  .t.e.m.p.l.a.t.e
+00000420: 0073 6277 7370 626c 6f62 0000 00b9 6270  .sbwspblob....bp
+00000430: 6c69 7374 3030 d601 0203 0405 0607 0807  list00..........
+00000440: 080b 085d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
+00000450: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
+00000460: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+00000470: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+00000480: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+00000490: 6f77 5369 6465 6261 7208 0908 095f 1019  owSidebar...._..
+000004a0: 7b7b 3233 3633 2c20 3737 327d 2c20 7b39  {{2363, 772}, {9
+000004b0: 3230 2c20 3433 367d 7d09 0815 232f 3b52  20, 436}}...#/;R
+000004c0: 5f6b 6c6d 6e6f 8b00 0000 0000 0001 0100  _klmno..........
+000004d0: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
+000004e0: 0000 0000 0000 8c00 0000 0900 7400 6500  ............t.e.
+000004f0: 6d00 7000 6c00 6100 7400 6500 7376 5372  m.p.l.a.t.e.svSr
+00000500: 6e6c 6f6e 6700 0000 0100 0000 0c00 7400  nlong.........t.
+00000510: 6500 6d00 7000 6c00 6100 7400 6500 7400  e.m.p.l.a.t.e.t.
+00000520: 6100 6700 7362 7773 7062 6c6f 6200 0000  a.g.sbwspblob...
+00000530: b962 706c 6973 7430 30d6 0102 0304 0506  .bplist00.......
+00000540: 0708 0708 0b08 5d53 686f 7753 7461 7475  ......]ShowStatu
+00000550: 7342 6172 5b53 686f 7754 6f6f 6c62 6172  sBar[ShowToolbar
+00000560: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
+00000570: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
+00000580: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
+00000590: 5b53 686f 7753 6964 6562 6172 0809 0809  [ShowSidebar....
+000005a0: 5f10 197b 7b32 3336 332c 2037 3732 7d2c  _..{{2363, 772},
+000005b0: 207b 3932 302c 2034 3336 7d7d 0908 1523   {920, 436}}...#
+000005c0: 2f3b 525f 6b6c 6d6e 6f8b 0000 0000 0000  /;R_klmno.......
+000005d0: 0101 0000 0000 0000 000d 0000 0000 0000  ................
+000005e0: 0000 0000 0000 0000 008c 0000 000c 0074  ...............t
+000005f0: 0065 006d 0070 006c 0061 0074 0065 0074  .e.m.p.l.a.t.e.t
+00000600: 0061 0067 0073 7653 726e 6c6f 6e67 0000  .a.g.svSrnlong..
+00000610: 0001 0000 0000 0000 0000 0000 0000 0000  ................
+00000620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `django_bocor_ds-2.0.3/LICENSE` & `django_bocor_ds-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/README.md` & `django_bocor_ds-2.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 ]
 
 MEDIA_URL = '/media/'  
 MEDIA_ROOT = os.path.join(BASE_DIR, 'media/')  
 X_FRAME_OPTIONS = 'SAMEORIGIN'  
   
 STATIC_ROOT = os.path.join(BASE_DIR, 'staticfiles')  
+
 ```
 
 in the shell
 ```
 >> pip install django-bocor-ds
 >> python manage.py makemigrations django_calendards django_modalds
 >> python manage.py migrate
```

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/.DS_Store` & `django_bocor_ds-2.0.5/django_bocor_ds/templates/.DS_Store`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0108 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 0000 0002 0000 0000 0000 0002  ................
-00000050: 0000 0001 0000 1000 006c 0061 0074 0065  .........l.a.t.e
-00000060: 0073 6277 0000 0000 0000 0000 0000 0000  .sbw............
+00000050: 0000 0001 0000 1000 0072 0064 0073 6277  .........r.d.sbw
+00000060: 7370 626c 0000 0000 0000 0000 0000 0000  spbl............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0002 0000 0009  ................
-00000210: 0074 0065 006d 0070 006c 0061 0074 0065  .t.e.m.p.l.a.t.e
-00000220: 0073 6277 7370 626c 6f62 0000 00b9 6270  .sbwspblob....bp
-00000230: 6c69 7374 3030 d601 0203 0405 0607 0807  list00..........
-00000240: 080b 085d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
-00000250: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
-00000260: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
-00000270: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
-00000280: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-00000290: 6f77 5369 6465 6261 7208 0908 095f 1019  owSidebar...._..
-000002a0: 7b7b 3133 3239 2c20 3534 317d 2c20 7b39  {{1329, 541}, {9
-000002b0: 3230 2c20 3433 367d 7d09 0815 232f 3b52  20, 436}}...#/;R
-000002c0: 5f6b 6c6d 6e6f 8b00 0000 0000 0001 0100  _klmno..........
-000002d0: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
-000002e0: 0000 0000 0000 8c00 0000 0900 7400 6500  ............t.e.
-000002f0: 6d00 7000 6c00 6100 7400 6500 7376 5372  m.p.l.a.t.e.svSr
-00000300: 6e6c 6f6e 6700 0000 0100 0000 0000 0000  nlong...........
+00000100: 0000 0000 0000 0000 0000 0002 0000 0007  ................
+00000110: 0062 006f 0063 006f 0072 0064 0073 6277  .b.o.c.o.r.d.sbw
+00000120: 7370 626c 6f62 0000 00b9 6270 6c69 7374  spblob....bplist
+00000130: 3030 d601 0203 0405 0607 0807 080b 085d  00.............]
+00000140: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
+00000150: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
+00000160: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
+00000170: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
+00000180: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
+00000190: 6465 6261 7208 0908 095f 1019 7b7b 3133  debar...._..{{13
+000001a0: 3239 2c20 3534 317d 2c20 7b39 3230 2c20  29, 541}, {920, 
+000001b0: 3433 367d 7d09 0815 232f 3b52 5f6b 6c6d  436}}...#/;R_klm
+000001c0: 6e6f 8b00 0000 0000 0001 0100 0000 0000  no..............
+000001d0: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
+000001e0: 0000 8c00 0000 0700 6200 6f00 6300 6f00  ........b.o.c.o.
+000001f0: 7200 6400 7376 5372 6e6c 6f6e 6700 0000  r.d.svSrnlong...
+00000200: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0108 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -318,15 +318,15 @@
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
+00001440: 0100 0000 8000 0000 0000 0000 0100 0002  ................
 00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
```

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/forms.py` & `django_bocor_ds-2.0.5/django_bocor_ds/forms.py`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/migrations/0001_initial.py` & `django_bocor_ds-2.0.5/django_bocor_ds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/migrations/0002_remove_portfolio_image3_remove_portfolio_image4_and_more.py` & `django_bocor_ds-2.0.5/django_bocor_ds/migrations/0002_remove_portfolio_image3_remove_portfolio_image4_and_more.py`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/models.py` & `django_bocor_ds-2.0.5/django_bocor_ds/models.py`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/.DS_Store` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/css/style.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/css/style.css`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 h1,
 h2,
 h3,
 h4,
 h5,
 h6 {
-  font-family: "Raleway", sans-serif;
+  font-family: "Noto Sans KR", "Raleway", sans-serif;
 }
 
 /*--------------------------------------------------------------
 # Back to top button
 --------------------------------------------------------------*/
 .back-to-top {
   position: fixed;
@@ -1060,15 +1060,15 @@
   display: inline-block;
   padding: 6px 30px;
   border-radius: 20px;
   color: #fff;
   transition: none;
   font-size: 14px;
   font-weight: 400;
-  font-family: "Raleway", sans-serif;
+  font-family: "Noto Sans KR", "Raleway", sans-serif;
   transition: 0.3s;
 }
 
 .pricing .get-started-btn:hover {
   background: #fdc134;
 }
```

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/img/footer-bg.jpg` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/img/footer-bg.jpg`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/js/main.js` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/js/main.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/scss/_footer.scss` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/scss/_footer.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/scss/_general.scss` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/scss/_general.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/scss/_header.scss` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/scss/_hero.scss` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/scss/_hero.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/scss/_nav.scss` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/scss/_sections.scss` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/scss/_sections.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/aos/aos.cjs.js` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/aos/aos.cjs.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/aos/aos.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/aos/aos.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/aos/aos.esm.js` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/aos/aos.esm.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/aos/aos.js` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/aos/aos.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/aos/aos.js.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/aos/aos.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.json` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.min.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.scss` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/css/animations.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/css/animations.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.min.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/css/transformations.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/css/transformations.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.eot` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.eot`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.svg` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.svg`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.ttf` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.ttf`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff2` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff2`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.min.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.min.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.js` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.min.js` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.js` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.min.js` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/php-email-form/php-email-form.php` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/php-email-form/php-email-form.php`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/php-email-form/validate.js` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/php-email-form/validate.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.css` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js.map` & `django_bocor_ds-2.0.5/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/__inner-page.html` & `django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/__inner-page.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/__portfolio-details.html` & `django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/__portfolio-details.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_about.html` & `django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_about.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_clients.html` & `django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_clients.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_contact.html` & `django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_contact.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_faq.html` & `django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_faq.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_features.html` & `django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_features.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_hero.html` & `django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_hero.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_portfolio.html` & `django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_portfolio.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_pricing.html` & `django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_pricing.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_services.html` & `django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_services.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/_team.html` & `django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/_team.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/footer.html` & `django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/footer.html`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,23 @@
         <div class="row  justify-content-center">
           <div class="col-lg-6">
             <h3>{{ footer.h3 }}</h3>
             <p>{{ footer.p }}</p>
           </div>
         </div>
 
-        <!--
+        {% if footer.use_newsletter %}
         <div class="row footer-newsletter justify-content-center">
           <div class="col-lg-6">
             <form action="" method="post">
               <input type="email" name="email" placeholder="Enter your Email"><input type="submit" value="Subscribe">
             </form>
           </div>
         </div>
-        -->
+        {% endif %}
 
         <div class="social-links">
           {% if social.twitter %}
           <a href="{{ footer.social.twitter }}" class="twitter" title="{{ basic_info.clinic }} 트위터 바로가기" target="_blank"><i class="bi bi-twitter"></i></a>
           {% endif %}
           {% if social.facebook %}
           <a href="{{ footer.social.facebook }}" class="facebook" title="{{ basic_info.clinic }} 페이스북 바로가기" target="_blank"><i class="bi bi-facebook"></i></a>
```

#### html2text {}

```diff
@@ -1,7 +1,10 @@
 {% load static %}
 ******** {{{{ ffooootteerr..hh33 }}}} ********
 {{ footer.p }}
+{% if footer.use_newsletter %}
+[Unknown INPUT type][Subscribe]
+{% endif %}
 {% if social.twitter %} {% endif %} {% if social.facebook %} {% endif %} {% if
 social.instagram %} {% endif %} {% if social.youtube %} {% endif %} {% if
 social.blog %} {% endif %}
 © Copyright _DD_ee_mm_ii_aa_nn_ss_oo_ff_tt_. All Rights Reserved
```

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/header.html` & `django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/header.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% load static %}
+{% load django_utilsds_tags %}
 
 <header id="header">
   <div class="container d-flex align-items-center justify-content-between">
 
     <!-- 로고 -->
     <div class="logo">
       {% if use_logo %}
@@ -17,15 +18,15 @@
         <li><a class="nav-link scrollto active" href="#hero">Home</a></li>
         <!-- 메뉴 -->
         {% for component, etc, title, is_show in components %}
           {% if is_show %}
             {% if component == 'direct_link' %}
               <li><a class="nav-link scrollto" href="{{ etc }}" target="_blank">{{ title }}</a></li>
             {% else %}
-              <li><a class="nav-link scrollto" href="{% url 'bocords:home' %}#{{ component }}">{{ title }}</a></li>
+              <li><a class="nav-link scrollto" href="{% url 'bocords:home' %}#{{ component | underscore_to_hyphen }}">{{ title }}</a></li>
             {% endif %}
           {% endif %}
         {% endfor %}
 
         {% for component, is_use, _, _ in components %}
         {% if component == menu_btn.component and is_use %}
         <li><a class="getstarted scrollto" href="#{{ menu_btn.component }}">{{ menu_btn.title }}</a></li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% load static %}
+{% load static %} {% load django_utilsds_tags %}
 {% if use_logo %} {% else %}
 ************ _{{_{{_ _ll_oo_gg_oo____tt_ee_xx_tt_ _}}_}}_.. ************
 {% endif %}
     * _H_o_m_e
     * {% for component, etc, title, is_show in components %} {% if is_show %}
       {% if component == 'direct_link' %}
     * _{_{_ _t_i_t_l_e_ _}_}
```

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/index.html` & `django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/index.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/templates/bocords/seo.html` & `django_bocor_ds-2.0.5/django_bocor_ds/templates/bocords/seo.html`

 * *Files 9% similar despite different names*

```diff
@@ -32,9 +32,10 @@
 =Open+Sans:300,300i,400,400i,600,600i,700,700i
 |Raleway:300,300i,400,400i,500,500i,600,600i,700,700i
 |Poppins:300,300i,400,400i,500,500i,600,600i,700,700i" rel="stylesheet">
 
 <!-- noto sans kr 폰트 추가 css 파일에 font-family: "Noto Sans KR", sans-serif; 추가해 준다. -->
 <link rel="preconnect" href="https://fonts.googleapis.com">
 <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
-<link href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@100..900&display=swap" rel="stylesheet">
-
+<link href="https://fonts.googleapis.com/css2?
+family=Noto+Sans+KR:wght@100..900&
+family=Noto+Serif+KR&display=swap" rel="stylesheet">
```

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/templatetags/bocords_tags.py` & `django_bocor_ds-2.0.5/django_bocor_ds/templatetags/bocords_tags.py`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/django_bocor_ds/views.py` & `django_bocor_ds-2.0.5/django_bocor_ds/views.py`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.0.3/pyproject.toml` & `django_bocor_ds-2.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django_bocor_ds"
-version = "2.0.3"
+version = "2.0.5"
 description = "my demiansoft templates"
 authors = [{name = "Hyungjin Kim", email = "hj3415@gmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dependencies = [
     "Django >= 5.0.3",
     "libsass>=0.23.0",
     "django-analyticsds >= 0.3.1",
     "django-calendards >= 0.4.0",
     "django-modalds >= 0.1.0",
-    "django-utilsds >= 0.4.0",
+    "django-utilsds >= 0.5.1",
 ]
 
 [project.urls]
 Home = "https://www.demiansoft.com"
 
 [tool.flit.sdist]
 # include = ["analyticsds/","calendards/","popupds/"]
```

### Comparing `django_bocor_ds-2.0.3/PKG-INFO` & `django_bocor_ds-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: django_bocor_ds
-Version: 2.0.3
+Version: 2.0.5
 Summary: my demiansoft templates
 Author-email: Hyungjin Kim <hj3415@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django >= 5.0.3
 Requires-Dist: libsass>=0.23.0
 Requires-Dist: django-analyticsds >= 0.3.1
 Requires-Dist: django-calendards >= 0.4.0
 Requires-Dist: django-modalds >= 0.1.0
-Requires-Dist: django-utilsds >= 0.4.0
+Requires-Dist: django-utilsds >= 0.5.1
 Project-URL: Home, https://www.demiansoft.com
 
 ### django-bocor-ds
 
 #### Introduction 
 demiansoft homepage templates
 
@@ -50,14 +50,15 @@
 ]
 
 MEDIA_URL = '/media/'  
 MEDIA_ROOT = os.path.join(BASE_DIR, 'media/')  
 X_FRAME_OPTIONS = 'SAMEORIGIN'  
   
 STATIC_ROOT = os.path.join(BASE_DIR, 'staticfiles')  
+
 ```
 
 in the shell
 ```
 >> pip install django-bocor-ds
 >> python manage.py makemigrations django_calendards django_modalds
 >> python manage.py migrate
```

