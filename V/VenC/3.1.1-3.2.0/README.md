# Comparing `tmp/VenC-3.1.1.tar.gz` & `tmp/VenC-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VenC-3.1.1.tar", last modified: Thu Jan 25 13:25:35 2024, max compression
+gzip compressed data, was "VenC-3.2.0.tar", last modified: Sun Apr 21 11:05:31 2024, max compression
```

## Comparing `VenC-3.1.1.tar` & `VenC-3.2.0.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.970920 VenC-3.1.1/
--rw-rw-r--   0 denis     (1000) denis     (1000)      451 2024-01-25 13:25:35.970920 VenC-3.1.1/PKG-INFO
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.966920 VenC-3.1.1/VenC.egg-info/
--rw-rw-r--   0 denis     (1000) denis     (1000)      451 2024-01-25 13:25:35.000000 VenC-3.1.1/VenC.egg-info/PKG-INFO
--rw-rw-r--   0 denis     (1000) denis     (1000)     2451 2024-01-25 13:25:35.000000 VenC-3.1.1/VenC.egg-info/SOURCES.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)        1 2024-01-25 13:25:35.000000 VenC-3.1.1/VenC.egg-info/dependency_links.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)       17 2024-01-25 13:25:35.000000 VenC-3.1.1/VenC.egg-info/requires.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)        6 2024-01-25 13:25:35.000000 VenC-3.1.1/VenC.egg-info/top_level.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)       38 2024-01-25 13:25:35.970920 VenC-3.1.1/setup.cfg
--rwxrwxr-x   0 denis     (1000) denis     (1000)     3163 2024-01-25 13:20:53.000000 VenC-3.1.1/setup.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.962920 VenC-3.1.1/share/
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.966920 VenC-3.1.1/share/embed_providers/
--rw-rw-r--   0 denis     (1000) denis     (1000)   123306 2023-12-19 14:41:00.000000 VenC-3.1.1/share/embed_providers/oembed.json
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.962920 VenC-3.1.1/share/themes/
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.966920 VenC-3.1.1/share/themes/concrete/
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.966920 VenC-3.1.1/share/themes/concrete/assets/
--rw-rw-r--   0 denis     (1000) denis     (1000)     3543 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes/concrete/assets/style.css
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.966920 VenC-3.1.1/share/themes/concrete/chunks/
--rw-rw-r--   0 denis     (1000) denis     (1000)      356 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes/concrete/chunks/atomEntry.xml
--rw-rw-r--   0 denis     (1000) denis     (1000)        8 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes/concrete/chunks/atomFooter.xml
--rw-rw-r--   0 denis     (1000) denis     (1000)      707 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes/concrete/chunks/atomHeader.xml
--rw-rw-r--   0 denis     (1000) denis     (1000)      105 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes/concrete/chunks/audio.html
--rw-rw-r--   0 denis     (1000) denis     (1000)      762 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes/concrete/chunks/entry.html
--rw-rw-r--   0 denis     (1000) denis     (1000)     1193 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes/concrete/chunks/footer.html
--rw-rw-r--   0 denis     (1000) denis     (1000)     2988 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes/concrete/chunks/header.html
--rw-rw-r--   0 denis     (1000) denis     (1000)      318 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes/concrete/chunks/rssEntry.xml
--rw-rw-r--   0 denis     (1000) denis     (1000)       18 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes/concrete/chunks/rssFooter.xml
--rw-rw-r--   0 denis     (1000) denis     (1000)      256 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes/concrete/chunks/rssHeader.xml
--rw-rw-r--   0 denis     (1000) denis     (1000)      119 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes/concrete/chunks/video.html
--rw-rw-r--   0 denis     (1000) denis     (1000)      209 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes/concrete/config.yaml
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.966920 VenC-3.1.1/share/themes_assets/
--rw-rw-r--   0 denis     (1000) denis     (1000)     6552 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes_assets/VenC-Infinite-Scroll-1.2.0.js
--rw-rw-r--   0 denis     (1000) denis     (1000)      950 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes_assets/VenC-Scripts-Bootstrap-0.0.0.js
--rw-rw-r--   0 denis     (1000) denis     (1000)     5436 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes_assets/VenC-Tree-0.2.0.js
--rw-rw-r--   0 denis     (1000) denis     (1000)    85831 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes_assets/concrete.png
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.966920 VenC-3.1.1/share/themes_templates/
--rw-rw-r--   0 denis     (1000) denis     (1000)      188 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes_templates/images
--rw-rw-r--   0 denis     (1000) denis     (1000)      138 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes_templates/kroki
--rw-rw-r--   0 denis     (1000) denis     (1000)      132 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes_templates/oEmbed
--rw-rw-r--   0 denis     (1000) denis     (1000)      151 2023-12-19 14:41:00.000000 VenC-3.1.1/share/themes_templates/pygmentize
--rwxrwxr-x   0 denis     (1000) denis     (1000)     2992 2023-12-19 14:41:00.000000 VenC-3.1.1/venc
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.966920 VenC-3.1.1/venc3/
--rw-rw-r--   0 denis     (1000) denis     (1000)      799 2024-01-25 13:20:53.000000 VenC-3.1.1/venc3/__init__.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.966920 VenC-3.1.1/venc3/commands/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-01-12 18:30:07.000000 VenC-3.1.1/venc3/commands/__init__.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)    10934 2024-01-25 13:20:53.000000 VenC-3.1.1/venc3/commands/export.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     1815 2024-01-25 13:20:53.000000 VenC-3.1.1/venc3/commands/install.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     7854 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/commands/new.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     4459 2024-01-25 13:20:53.000000 VenC-3.1.1/venc3/commands/print.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     3492 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/commands/remote.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2321 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/commands/serv.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.966920 VenC-3.1.1/venc3/datastore/
--rw-rw-r--   0 denis     (1000) denis     (1000)     9240 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/datastore/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2487 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/datastore/archives.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     5477 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/datastore/configuration.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     4093 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/datastore/entries.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     7006 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/datastore/entry.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1346 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/datastore/hardcoded_assets.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     1675 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/datastore/metadata.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     4852 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/datastore/taxonomy.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     5487 2024-01-25 13:20:53.000000 VenC-3.1.1/venc3/datastore/theme.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     6619 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/exceptions.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     4355 2024-01-25 13:20:53.000000 VenC-3.1.1/venc3/helpers.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.966920 VenC-3.1.1/venc3/l10n/
--rw-rw-r--   0 denis     (1000) denis     (1000)     1529 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/l10n/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     8238 2023-12-30 11:29:51.000000 VenC-3.1.1/venc3/l10n/en.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     9164 2023-12-30 11:29:51.000000 VenC-3.1.1/venc3/l10n/fr.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.970920 VenC-3.1.1/venc3/markup_languages/
--rw-rw-r--   0 denis     (1000) denis     (1000)     2778 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/markup_languages/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1641 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/markup_languages/asciidoc.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2019 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/markup_languages/markdown.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1644 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/markup_languages/restructuredtext.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.970920 VenC-3.1.1/venc3/parallelism/
--rw-rw-r--   0 denis     (1000) denis     (1000)     2443 2023-01-12 18:30:07.000000 VenC-3.1.1/venc3/parallelism/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2702 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/parallelism/build_entries.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     5405 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/parallelism/export_entries.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.970920 VenC-3.1.1/venc3/patterns/
--rw-rw-r--   0 denis     (1000) denis     (1000)        1 2023-01-12 18:30:07.000000 VenC-3.1.1/venc3/patterns/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)    25125 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/patterns/datastore.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     4444 2024-01-25 13:20:53.000000 VenC-3.1.1/venc3/patterns/non_contextual.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     9637 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/patterns/patterns_map.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)    12375 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/patterns/processor.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1536 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/patterns/theme.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.970920 VenC-3.1.1/venc3/patterns/third_party_wrapped_features/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-01-12 18:30:07.000000 VenC-3.1.1/venc3/patterns/third_party_wrapped_features/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2610 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/patterns/third_party_wrapped_features/kroki.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1232 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/patterns/third_party_wrapped_features/latex2mathml.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     3783 2024-01-25 13:20:53.000000 VenC-3.1.1/venc3/patterns/third_party_wrapped_features/oembed.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     3255 2024-01-25 13:20:53.000000 VenC-3.1.1/venc3/patterns/third_party_wrapped_features/pygmentize.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1975 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/prompt.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-01-25 13:25:35.970920 VenC-3.1.1/venc3/threads/
--rw-rw-r--   0 denis     (1000) denis     (1000)    14363 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/threads/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2701 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/threads/archives.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     4739 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/threads/categories.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     3903 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/threads/chapters.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     6307 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/threads/entries.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1935 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/threads/feed.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2709 2023-12-19 14:41:00.000000 VenC-3.1.1/venc3/threads/main.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.469176 VenC-3.2.0/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      451 2024-04-21 11:05:31.469176 VenC-3.2.0/PKG-INFO
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.461176 VenC-3.2.0/VenC.egg-info/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      451 2024-04-21 11:05:31.000000 VenC-3.2.0/VenC.egg-info/PKG-INFO
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2489 2024-04-21 11:05:31.000000 VenC-3.2.0/VenC.egg-info/SOURCES.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)        1 2024-04-21 11:05:31.000000 VenC-3.2.0/VenC.egg-info/dependency_links.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)       17 2024-04-21 11:05:31.000000 VenC-3.2.0/VenC.egg-info/requires.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)        6 2024-04-21 11:05:31.000000 VenC-3.2.0/VenC.egg-info/top_level.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)       38 2024-04-21 11:05:31.469176 VenC-3.2.0/setup.cfg
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     3163 2024-04-21 10:17:35.000000 VenC-3.2.0/setup.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.461176 VenC-3.2.0/share/
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.461176 VenC-3.2.0/share/embed_providers/
+-rw-rw-r--   0 denis     (1000) denis     (1000)   123306 2023-12-19 14:41:00.000000 VenC-3.2.0/share/embed_providers/oembed.json
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.461176 VenC-3.2.0/share/themes/
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.461176 VenC-3.2.0/share/themes/concrete/
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.461176 VenC-3.2.0/share/themes/concrete/assets/
+-rw-rw-r--   0 denis     (1000) denis     (1000)     5109 2024-04-21 10:17:35.000000 VenC-3.2.0/share/themes/concrete/assets/style.css
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.461176 VenC-3.2.0/share/themes/concrete/chunks/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      356 2024-02-17 16:56:20.000000 VenC-3.2.0/share/themes/concrete/chunks/atomEntry.xml
+-rw-rw-r--   0 denis     (1000) denis     (1000)        8 2024-02-17 16:56:20.000000 VenC-3.2.0/share/themes/concrete/chunks/atomFooter.xml
+-rw-rw-r--   0 denis     (1000) denis     (1000)      706 2024-04-21 10:17:35.000000 VenC-3.2.0/share/themes/concrete/chunks/atomHeader.xml
+-rw-rw-r--   0 denis     (1000) denis     (1000)      105 2024-02-17 16:56:20.000000 VenC-3.2.0/share/themes/concrete/chunks/audio.html
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1810 2024-04-21 10:17:35.000000 VenC-3.2.0/share/themes/concrete/chunks/entry.html
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1208 2024-04-21 10:17:35.000000 VenC-3.2.0/share/themes/concrete/chunks/footer.html
+-rw-rw-r--   0 denis     (1000) denis     (1000)     6088 2024-04-21 10:17:35.000000 VenC-3.2.0/share/themes/concrete/chunks/header.html
+-rw-rw-r--   0 denis     (1000) denis     (1000)      318 2024-02-17 16:56:20.000000 VenC-3.2.0/share/themes/concrete/chunks/rssEntry.xml
+-rw-rw-r--   0 denis     (1000) denis     (1000)       18 2024-02-17 16:56:20.000000 VenC-3.2.0/share/themes/concrete/chunks/rssFooter.xml
+-rw-rw-r--   0 denis     (1000) denis     (1000)      256 2024-02-17 16:56:20.000000 VenC-3.2.0/share/themes/concrete/chunks/rssHeader.xml
+-rw-rw-r--   0 denis     (1000) denis     (1000)      119 2024-02-17 16:56:20.000000 VenC-3.2.0/share/themes/concrete/chunks/video.html
+-rw-rw-r--   0 denis     (1000) denis     (1000)      233 2024-04-21 10:17:35.000000 VenC-3.2.0/share/themes/concrete/config.yaml
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.465176 VenC-3.2.0/share/themes_assets/
+-rw-rw-r--   0 denis     (1000) denis     (1000)     6552 2023-12-19 14:41:00.000000 VenC-3.2.0/share/themes_assets/VenC-Infinite-Scroll-1.2.0.js
+-rw-rw-r--   0 denis     (1000) denis     (1000)      951 2024-04-21 10:17:35.000000 VenC-3.2.0/share/themes_assets/VenC-Scripts-Bootstrap-0.0.0.js
+-rw-rw-r--   0 denis     (1000) denis     (1000)     5436 2024-02-18 15:13:05.000000 VenC-3.2.0/share/themes_assets/VenC-Tree-0.2.0.js
+-rw-rw-r--   0 denis     (1000) denis     (1000)    97152 2024-04-21 10:17:35.000000 VenC-3.2.0/share/themes_assets/concrete-dark.png
+-rw-rw-r--   0 denis     (1000) denis     (1000)    64283 2024-04-21 10:17:35.000000 VenC-3.2.0/share/themes_assets/concrete.png
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.465176 VenC-3.2.0/share/themes_templates/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      188 2023-12-19 14:41:00.000000 VenC-3.2.0/share/themes_templates/images
+-rw-rw-r--   0 denis     (1000) denis     (1000)      138 2023-12-19 14:41:00.000000 VenC-3.2.0/share/themes_templates/kroki
+-rw-rw-r--   0 denis     (1000) denis     (1000)      132 2023-12-19 14:41:00.000000 VenC-3.2.0/share/themes_templates/oEmbed
+-rw-rw-r--   0 denis     (1000) denis     (1000)      151 2023-12-19 14:41:00.000000 VenC-3.2.0/share/themes_templates/pygmentize
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     2992 2023-12-19 14:41:00.000000 VenC-3.2.0/venc
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.465176 VenC-3.2.0/venc3/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      799 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/__init__.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.465176 VenC-3.2.0/venc3/commands/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/commands/__init__.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)    10723 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/commands/export.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     1815 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/commands/install.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     7094 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/commands/new.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     4459 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/commands/print.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     9275 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/commands/remote.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     4195 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/commands/serv.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.465176 VenC-3.2.0/venc3/datastore/
+-rw-rw-r--   0 denis     (1000) denis     (1000)     9560 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/datastore/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2515 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/datastore/archives.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     6612 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/datastore/configuration.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     4116 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/datastore/entries.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     6920 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/datastore/entry.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1346 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/datastore/hardcoded_assets.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     1675 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/datastore/metadata.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     4838 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/datastore/taxonomy.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     5487 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/datastore/theme.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     6619 2024-04-11 16:07:13.000000 VenC-3.2.0/venc3/exceptions.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     5027 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/helpers.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.465176 VenC-3.2.0/venc3/l10n/
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1529 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/l10n/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     8277 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/l10n/en.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     9225 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/l10n/fr.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.465176 VenC-3.2.0/venc3/markup_languages/
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2808 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/markup_languages/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1641 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/markup_languages/asciidoc.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2019 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/markup_languages/markdown.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1644 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/markup_languages/restructuredtext.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.469176 VenC-3.2.0/venc3/parallelism/
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2443 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/parallelism/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2702 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/parallelism/build_entries.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     5405 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/parallelism/export_entries.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.469176 VenC-3.2.0/venc3/patterns/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        1 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/patterns/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)    33331 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/patterns/datastore.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     4645 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/patterns/non_contextual.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)    11160 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/patterns/patterns_map.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)    12375 2024-03-08 02:35:29.000000 VenC-3.2.0/venc3/patterns/processor.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1536 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/patterns/theme.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.469176 VenC-3.2.0/venc3/patterns/third_party_wrapped_features/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/patterns/third_party_wrapped_features/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2611 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/patterns/third_party_wrapped_features/kroki.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1232 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/patterns/third_party_wrapped_features/latex2mathml.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     3783 2024-02-11 16:20:57.000000 VenC-3.2.0/venc3/patterns/third_party_wrapped_features/oembed.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     3256 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/patterns/third_party_wrapped_features/pygmentize.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1975 2024-04-04 17:42:26.000000 VenC-3.2.0/venc3/prompt.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-21 11:05:31.469176 VenC-3.2.0/venc3/threads/
+-rw-rw-r--   0 denis     (1000) denis     (1000)    14691 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/threads/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2703 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/threads/archives.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     4745 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/threads/categories.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     6225 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/threads/chapters.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     6309 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/threads/entries.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2136 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/threads/feed.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2707 2024-04-21 10:17:35.000000 VenC-3.2.0/venc3/threads/main.py
```

### Comparing `VenC-3.1.1/VenC.egg-info/SOURCES.txt` & `VenC-3.2.0/VenC.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 share/themes/concrete/chunks/rssEntry.xml
 share/themes/concrete/chunks/rssFooter.xml
 share/themes/concrete/chunks/rssHeader.xml
 share/themes/concrete/chunks/video.html
 share/themes_assets/VenC-Infinite-Scroll-1.2.0.js
 share/themes_assets/VenC-Scripts-Bootstrap-0.0.0.js
 share/themes_assets/VenC-Tree-0.2.0.js
+share/themes_assets/concrete-dark.png
 share/themes_assets/concrete.png
 share/themes_templates/images
 share/themes_templates/kroki
 share/themes_templates/oEmbed
 share/themes_templates/pygmentize
 venc3/__init__.py
 venc3/exceptions.py
```

### Comparing `VenC-3.1.1/setup.py` & `VenC-3.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         dst_prefix+"share/VenC/themes_templates/",
         ["share/themes_templates/"+filename for filename in listdir("share/themes_templates")]
     )
 )
 
 setup(
     name='VenC',
-    version='3.1.1',
+    version='3.2.0',
     description='A static blog generator.',
     author='Denis Salem',
     author_email='denissalem@tuxfamily.org',
     url='https://github.com/DenisSalem/VenC',
     packages=[
         'venc3',
         'venc3.commands',
```

### Comparing `VenC-3.1.1/share/embed_providers/oembed.json` & `VenC-3.2.0/share/embed_providers/oembed.json`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/share/themes/concrete/chunks/atomHeader.xml` & `VenC-3.2.0/share/themes/concrete/chunks/atomHeader.xml`

 * *Files 2% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 <feed xmlns="http://www.w3.org/2005/Atom">
  <link href=".:GetBlogURL:..:GetRelativeLocation:./atom_feed.xml" rel="self" type="application/atom+xml"/>
  <link href=".:GetBlogURL:." rel="alternate" type="text/html" />
  
  <title>.:GetBlogName:. .:GetThreadName::| {value}:.</title>
     .:GetBlogMetadataIfNotNull::blog_description::<subtitle>{value}</subtitle>:.
     .:GetBlogMetadataIfNotNull::blog_url::<id>{value}.:GetRelativeLocation:.</id>:.
- <updated>.:GetGenerationTimestamp::%Y-%m-%dT%H:%M:%SZ:.</updated>
+ <updated>.:GetLastEntryTimestamp::%Y-%m-%dT%H:%M:%SZ:.</updated>
  <author>
    .:GetBlogMetadataIfNotNull::author_name::<name>{value}</name>:.
    .:GetBlogMetadataIfNotNull::author_email::<email>{value}</email>:.
  </author>
```

### Comparing `VenC-3.1.1/share/themes/concrete/chunks/footer.html` & `VenC-3.2.0/share/themes/concrete/chunks/footer.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
         </div>
         <footer class="box engrave">
             .:IfInfiniteScrollEnabled::
                 .:IfInThread::
                     .:GetBlogMetadataIfExists::loading_image::
-                        <img id="__VENC_LOADING__" src=".:GetRelativeRoot:.{value}" />
+                        <img id="__VENC_LOADING__" src=".:GetRelativeRoot:..:IfInMainThread::%2e/::/:.{value}" />
                       :.
                 :.
             :.
-            .:IncludeFileIfExists::
-                .:GetBlogMetadataIfNotNull::include_in_footer:.        
-            :.
             <div id="__VENC_NAVIGATION__">
                 .:GetPreviousPage::<a id="previous_link" href="{path}">.:IfInThread::←::{entry_title} ←:.</a>:.
                 .:IfInThread::
                     .:IfPages::
                         <ul id="navigation_pages_list">
                             .:ForPages::5::<li class="page_list_item">
                                 <a href="{path}">{page_number}</a>
                             </li>:: . :.
                         </ul>
                     :.
                 :.
                 .:GetNextPage::<a id="next_link" href="{path}" data-venc-api-infinite-scroll-hook="{path}">.:IfInThread::→::→ {entry_title}:.</a>:.
             </div>
         </footer>
+        .:IncludeFileIfExists::
+            .:GetBlogMetadataIfNotNull::include_in_footer:.        
+        :.
     </body>
 </html>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 .:IfInfiniteScrollEnabled:: .:IfInThread:: .:GetBlogMetadataIfExists::
-loading_image:: [.:GetRelativeRoot:.{value}]:. :. :. .:IncludeFileIfExists:: .:
-GetBlogMetadataIfNotNull::include_in_footer:. :.
+loading_image:: [.:GetRelativeRoot:..:IfInMainThread::%2e/::/:.{value}]:. :. :.
 .:GetPreviousPage::_._:_I_f_I_n_T_h_r_e_a_d_:_:_â___:_:_{_e_n_t_r_y___t_i_t_l_e_}_ _â___:_.:. .:IfInThread:: .:
 IfPages::
     * .:ForPages::5::
     * _{_p_a_g_e___n_u_m_b_e_r_}
     * :: . :.
 :. :. .:GetNextPage::_._:_I_f_I_n_T_h_r_e_a_d_:_:_â___:_:_â___ _{_e_n_t_r_y___t_i_t_l_e_}_:_.:.
+.:IncludeFileIfExists:: .:GetBlogMetadataIfNotNull::include_in_footer:. :.
```

### Comparing `VenC-3.1.1/share/themes_assets/VenC-Infinite-Scroll-1.2.0.js` & `VenC-3.2.0/share/themes_assets/VenC-Infinite-Scroll-1.2.0.js`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/share/themes_assets/VenC-Scripts-Bootstrap-0.0.0.js` & `VenC-3.2.0/share/themes_assets/VenC-Scripts-Bootstrap-0.0.0.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -22,8 +22,8 @@
 function VENC_ON_LOAD_CALLBACK() {
     var i;
     for (i = 0; i < VENC_ON_LOAD_CALLBACK_REGISTER.length; i++) {
         VENC_ON_LOAD_CALLBACK_REGISTER[i]();
     }
 }
 
-window.onload = VENC_ON_LOAD_CALLBACK
+window.onload = VENC_ON_LOAD_CALLBACK;
```

### Comparing `VenC-3.1.1/share/themes_assets/VenC-Tree-0.2.0.js` & `VenC-3.2.0/share/themes_assets/VenC-Tree-0.2.0.js`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc` & `VenC-3.2.0/venc`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/__init__.py` & `VenC-3.2.0/venc3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with VenC.  If not, see <http://www.gnu.org/licenses/>.
 
-venc_version = "3.1.1"
+venc_version = "3.2.0"
 __version__ = venc_version # PEP396
```

### Comparing `VenC-3.1.1/venc3/commands/export.py` & `VenC-3.2.0/venc3/commands/export.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,38 +20,14 @@
 import subprocess
 
 from venc3.exceptions import VenCException, MalformedPatterns
 from venc3.helpers import rm_tree_error_handler
 from venc3.patterns.non_contextual import theme_includes_dependencies
 from venc3.patterns.processor import Processor, Pattern
 from venc3.prompt import notify
-
-def copy_recursively(src, dest):
-    import errno, os, shutil
-    try:
-        listdir = os.listdir(src)
-    except Exception as e:
-        from venc3.exceptions import VenCException
-        VenCException(("exception_place_holder", e)).die()
-        
-    for filename in listdir:
-        try:
-            shutil.copytree(src+filename, dest+filename)
-    
-        except shutil.Error as e:
-            from venc3.prompt import notify
-            notify(("directory_not_copied", str(e)), "YELLOW")
-            
-        except OSError as e:
-            if e.errno == errno.ENOTDIR:
-                shutil.copy(src+filename, dest+filename)
-
-            else:
-                from venc3.prompt import notify
-                notify(("directory_not_copied", str(e)), "YELLOW")
                 
 def export_via_ftp(params):
     export_blog(params)
     from venc3.commands.remote import remote_copy
     remote_copy(None)
 
 def setup_pattern_processor(parallel=False):        
@@ -169,47 +145,60 @@
         pattern_processor.process(theme.rss_footer, flags)
         pattern_processor.process(theme.atom_header, flags)
         pattern_processor.process(theme.atom_footer, flags)
 
     except VenCException as e:    
         e.die()
 
-def export_blog(params):
-    theme_name = params[0] if len(params) else ''
+def export_blog(params):    
     import time
         
     start_timestamp = time.time()
     from venc3.datastore import init_datastore
     datastore = init_datastore()
     
     notify(("pre_process",), prepend="├─ ")
     
     from venc3.datastore.theme import init_theme
+    theme_name = params[0] if len(params) else datastore.blog_configuration["default_theme"]
     init_theme(theme_name)
     from venc3.patterns.third_party_wrapped_features.pygmentize import init_code_highlight
     init_code_highlight()
     from venc3.patterns.patterns_map import init_pattern_map
     init_pattern_map()
     
+    # cleaning and setup directories
+    import os, shutil
+    if not os.path.exists('extra'):
+        os.makedirs("extra")
+        
+    if not os.path.exists('blog'):
+        os.makedirs("blog")
+    else:
+        for filename in os.listdir('blog'):
+            if os.path.isfile("blog/"+filename):
+                try:
+                    os.remove("blog/"+filename)
+                except Exception as e:
+                    rm_tree_error_handler("os.remove", "blog/"+filename, [e])
+            else:
+                shutil.rmtree("blog/"+filename, ignore_errors=False, onerror=rm_tree_error_handler)    
+    
     process_non_contextual_patterns()
+    
     if not datastore.blog_configuration["disable_single_entries"]:
         notify(("link_entries",), prepend="├─ ")
         # Add required link between entries
         entries = datastore.entries
         for entry_index in range(0, len(entries)):
             current_entry = entries[entry_index]
             if entry_index > 0:
                 entries[entry_index-1].next_entry = current_entry
                 current_entry.previous_entry = entries[entry_index-1]
 
-    # cleaning directory
-    import os, shutil
-    shutil.rmtree("blog", ignore_errors=False, onerror=rm_tree_error_handler)
-    os.makedirs("blog")
-
     try:
         # Starting second pass and exporting
         from venc3.threads.main import MainThread
         thread = MainThread()
         thread.do()
         
         if not datastore.blog_configuration["disable_archives"]:
@@ -236,16 +225,16 @@
         e.die()
         
     # Copy assets and extra files
     notify(("copy_assets_and_extra_files",), prepend="└─ ")
     from venc3.patterns.third_party_wrapped_features.pygmentize import code_highlight
     from venc3.datastore.theme import theme, theme_assets_dependencies
     from venc3.helpers import get_base_dir
-
     code_highlight.export_style_sheets()
+    from venc3.helpers import copy_recursively
     copy_recursively("extra/","blog/")
     copy_recursively(theme.theme_folder+"assets/","blog/")
     for depenpency in theme_assets_dependencies:
         try:
             shutil.copyfile(get_base_dir()+"/share/VenC/themes_assets/"+depenpency, "blog/"+depenpency)
         
         except IsADirectoryError:
```

### Comparing `VenC-3.1.1/venc3/commands/install.py` & `VenC-3.2.0/venc3/commands/install.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/commands/new.py` & `VenC-3.2.0/venc3/commands/new.py`

 * *Files 24% similar despite different names*

```diff
@@ -123,79 +123,67 @@
             os.remove(output_filename)
             e.die()
     
     stream.write(output)
     stream.close()
 
     try:
-        if not "text_editor" in blog_configuration.keys():
-            from venc3.prompt import notify
-            notify(("missing_mandatory_field_in_blog_conf", "text_editor"), "YELLOW")
-        
-        elif type(blog_configuration["text_editor"]) != list:
-            from venc3.prompt import notify
-            notify(("blog_metadata_is_not_a_list", "text_editor"), "YELLOW")
-            
-        else:
+        if "text_editor" in blog_configuration.keys():
             command = [str(arg) for arg in blog_configuration["text_editor"] if arg != '']
-            command.append(output_filename)
-            subprocess.call(command) 
+
+        elif "EDITOR" in os.environ.keys():
+            command = [str(arg) for arg in os.environ["EDITOR"].split(' ') if arg != '']
+
+        else:
+            command = None
+
+        if command != None:
+            if len(command):
+                command.append(output_filename)
+                subprocess.call(command)
+                
+            else:
+                from venc3.prompt import die
+                die(("invalid_value_in_setting", str(blog_configuration["text_editor"]), "text_editor"))
 
     except FileNotFoundError:
         os.remove(output_filename)
         from venc3.prompt import die
         die(("unknown_command", blog_configuration["text_editor"]))
         
     from venc3.prompt import notify
-    notify(("entry_written",))
+    notify(("entry_written", output_filename))
 
 def new_blog(blog_names):
     if len(blog_names) < 1:
         from venc3.prompt import die
         die(("missing_params", "--new-blog"))
         
     from venc3.l10n import messages
     default_configuration =	{
-        "blog_name":			              messages.blog_name,
-        "disable_threads":              [],
-        "disable_archives":             False,
-        "disable_categories":           False,
-        "disable_chapters":             True,
-        "disable_single_entries":       False,
-        "disable_main_thread":          False,
-        "disable_rss_feed":             False,
-        "disable_atom_feed":            False,
-        "text_editor":                  ["nano"],
-        "date_format":                  "%A %d. %B %Y",
-        "blog_url":			                messages.blog_url,
-        "ftp_host":                     messages.ftp_host,
-        "code_highlight_css_override":  False,
-        "path":	{
-            "ftp":                      messages.ftp_path,
+        "blog_name":            messages.blog_name,
+        "date_format":          "%A %d. %B %Y",
+        "entries_per_pages":    10,
+        "columns":              1,
+        "feed_length":          5,
+        "reverse_thread_order": True,
+        "markup_language":      "none",
+        "paths":	{
             "entries_sub_folders":      "{entry_title}",
             "categories_sub_folders":   "",
             "archives_sub_folders":     "",
             "chapters_sub_folders":     "chapters",
             "index_file_name":		        "index{page_number}.html",
             "category_directory_name":	"{category}",
             "chapter_directory_name": 	"{chapter_name}",
 			      "archives_directory_name":	"%Y-%m",
 			      "entry_file_name":		        "index.html",
 			      "rss_file_name":		          "rss.xml",
 			      "atom_file_name":		        "atom.xml"
         },
-        "entries_per_pages":		    10,
-        "columns":			            1,
-        "feed_length":	        	    5,
-        "reverse_thread_order":		    True,
-        "markup_language":              "Markdown",
-        "path_encoding":                "",
-        "server_port":                  8888,
-        "sort_by":                      "id",
-        "parallel_processing": 1
     }
     for folder_name in blog_names:
         try:
             os.mkdir(folder_name)
 
         except OSError:
             from venc3.prompt import die
```

### Comparing `VenC-3.1.1/venc3/commands/print.py` & `VenC-3.2.0/venc3/commands/print.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/datastore/__init__.py` & `VenC-3.2.0/venc3/datastore/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,16 +39,14 @@
     def __init__(self):
         self.requested_entry = None
         self.embed_providers = {}
         self.in_child_process = False
         self.root_page = None
         self.blog_configuration = get_blog_configuration()
         self.sort_by = self.blog_configuration["sort_by"]
-
-        self.blog_url = self.blog_configuration["blog_url"]
         self.disable_threads = self.blog_configuration["disable_threads"]
         
         try:
             from multiprocessing import cpu_count
             cpu_c = cpu_count()
             self.workers_count = cpu_c if cpu_c > 0 else 1
             
@@ -77,28 +75,27 @@
         
         # TODO : Cache should be voided when usage is complete
         
         self.cache_blog_archives = {}
         self.cache_entries_subset = {}
         self.cache_get_entry_attribute_by_id = {}
         self.cache_get_chapter_attribute_by_index = {}
-        # ~ self.cache_entry_tocs = {}
         
         self.generation_timestamp = datetime.datetime.now()
         self.raw_chapters = {}
         self.chapters_index = []
 
         self.init_entries()
         self.init_archives()
         self.init_taxonomy()
                 
     def build_chapter_indexes(self):
         # build chapters index
-        path_chapters_sub_folders = self.blog_configuration["path"]["chapters_sub_folders"]
-        path_chapter_folder_name = self.blog_configuration["path"]["chapter_directory_name"]
+        path_chapters_sub_folders = self.blog_configuration["paths"]["chapters_sub_folders"]
+        path_chapter_folder_name = self.blog_configuration["paths"]["chapter_directory_name"]
         
         for chapter in sorted(self.raw_chapters.keys(), key = lambda x : int(x.replace('.', ''))):
             top = self.chapters_index
             index = ''
             levels = [str(level) for level in chapter.split('.') if level != '']
             len_levels = len(levels)
                     
@@ -114,15 +111,15 @@
                 try:
                     top = next(f).sub_chapters
                 
                 except StopIteration:
                     if index in self.raw_chapters.keys():
                         entry = self.raw_chapters[index]
                         try:
-                            path = "\x1a"+path_chapters_sub_folders+quirk_encoding(
+                            path = "\x1a/"+path_chapters_sub_folders+quirk_encoding(
                                 path_chapter_folder_name.format(**{
                                     "chapter_name" : entry.title,
                                     "chapter_index" : index
                                 })
                             )
                             
                         except KeyError as e:
@@ -167,53 +164,62 @@
         return output+close_ul
 
     def build_html_chapters(self, lo, io, ic, lc, top, level):          
         if top == []:
             return ''
             
         output = lo.format(**{"level" :level})
-
+        
+        from venc3.helpers import quirk_encoding
+        
         for sub_chapter in top:
             output += io.format(**{
                 "index": sub_chapter.index,
                 "title": self.entries[sub_chapter.entry_index].title,
+                "html_id" : quirk_encoding(self.entries[sub_chapter.entry_index].title),
                 "path":  sub_chapter.path,
                 "level": level
             })
             output += self.build_html_chapters(lo, io, ic, lc, sub_chapter.sub_chapters, level+1)
             output += ic
         output += lc
 
         return output
 
     def build_html_categories_tree(self, pattern, opening_node, opening_branch, closing_branch, closing_node, tree):
+        if not len(tree):
+            return ""
+            
         output_string = opening_node
         for node in sorted(tree, key = lambda x : x.value):
             if node.value in self.disable_threads:
                 continue
 
-            variables = {
-                "value" : node.value,
-                "count" : node.count,
-                "weight" : round(node.count / node.weight_tracker.value,2),
-                "path" : node.path,
-                "childs" : self.build_html_categories_tree(
-                    pattern,
-                    opening_node,
-                    opening_branch,
-                    closing_branch,
-                    closing_node,
-                    node.childs
-                ) if len(node.childs) else ''
-            }
-
-            output_string += opening_branch.format(**variables) +closing_branch.format(**variables)
+            variables = self.node_to_dictionnary(pattern, node, opening_node, opening_branch, closing_branch, closing_node, node.childs)
+            output_string += opening_branch.format(**variables) + closing_branch.format(**variables)
 
         return output_string + closing_node
-        
+
+    def node_to_dictionnary(self, pattern, node, opening_node, opening_branch, closing_branch, closing_node, childs):
+        return {
+            "value" : node.value,
+            "html_id": quirk_encoding(node.value),
+            "count" : node.count,
+            "weight" : round(node.count / node.weight_tracker.value,2),
+            "path" : node.path,
+            "childs" : self.build_html_categories_tree(
+                pattern,
+                opening_node,
+                opening_branch,
+                closing_branch,
+                closing_node,
+                childs
+            )
+        }
+
     def update_chapters(self, entry):
         try:
             if type(entry.chapter) == float:
                 notify(("chapter_type_is_ambiguous", entry.id), color="YELLOW")
                 
             chapter = str(entry.chapter)
             [ int(level) for level in chapter.split('.') if level != '']
@@ -233,14 +239,14 @@
                 entry.id,
                 self.raw_chapters[chapter].title,
                 self.raw_chapters[chapter].id,
                 chapter
             ))
         else:
             self.raw_chapters[chapter] = entry
-            
+        
 datastore = None
 
 def init_datastore():
     global datastore
     datastore = DataStore()
     return datastore
```

### Comparing `VenC-3.1.1/venc3/datastore/archives.py` & `VenC-3.2.0/venc3/datastore/archives.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 from venc3.helpers import quirk_encoding
 
 class Archives:
     def init_archives(self):
         self.entries_per_archives = []
         self.archives_weight_tracker = WeightTracker()
 
-        path_archives_sub_folders = self.blog_configuration["path"]["archives_sub_folders"]
-        compute_archives = self.blog_configuration["path"]["archives_directory_name"] != '' and not self.blog_configuration["disable_archives"]
+        path_archives_sub_folders = self.blog_configuration["paths"]["archives_sub_folders"]
+        compute_archives = self.blog_configuration["paths"]["archives_directory_name"] != '' and not self.blog_configuration["disable_archives"]
 
         if compute_archives:
             for entry_index in range(0, len(self.entries)):
                 current_entry = self.entries[entry_index]
                 formatted_date = current_entry.formatted_date
                 archives_index = self.get_archives_index_for_given_date(formatted_date)
                 if archives_index != None:
@@ -40,15 +40,15 @@
                     self.entries_per_archives[archives_index].related_to.append(entry_index)
 
                 else:
                     self.entries_per_archives.append(
                         MetadataNode(
                             formatted_date,
                             entry_index,
-                            path="\x1a"+path_archives_sub_folders+quirk_encoding(formatted_date),
+                            path= ("\x1a/"+path_archives_sub_folders+'/'+quirk_encoding(formatted_date)).replace('//','/'),
                             weight_tracker=self.archives_weight_tracker
                         )
                     )
 
     def get_archives_index_for_given_date(self, value):
         index = 0
         for metadata in self.entries_per_archives:
```

### Comparing `VenC-3.1.1/venc3/datastore/configuration.py` & `VenC-3.2.0/venc3/datastore/configuration.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,26 +15,91 @@
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with VenC.  If not, see <http://www.gnu.org/licenses/>.
 
 BLOG_CONFIGURATION = None
 
-def setup_sub_folder(blog_configuration, key):
-    from venc3.helpers import quirk_encoding
-    try:
-        path = quirk_encoding(blog_configuration["path"][key])
+def sanitize_optional_fields(blog_configuration):
+    fields = {
+        "blog_keywords": list,
+        "blog_url": str,
+        "code_highlight_css_override": bool,
+        "columns": int,
+        "default_theme": str,
+        "disable_archives": bool,
+        "disable_atom_feed": bool,
+        "disable_categories": bool,
+        "disable_chapters": bool,
+        "disable_infinite_scroll" : bool,
+        "disable_main_thread": bool,
+        "disable_rss_feed" : bool,
+        "disable_single_entries": bool,
+        "disable_threads": list,
+        "ftp_encoding": str,
+        "ftp_host": str,
+        "ftp_port": int,
+        "ftp_sessions": int,
+        "path_encoding": str, 
+        "parallel_processing": int,
+        "pipe_flow": int,
+        "server_port": int,
+        "sort_by": str,
+        "text_editor": list
+    }
+
+    for field in fields.keys():
+        if field in blog_configuration.keys():
+            if not type(blog_configuration[field]) == fields[field]:
+                from venc3.prompt import die
+                die(("field_is_not_of_type", field, "blog_configuration.yaml", fields[field].__name__))
+                
+    if "ftp" in blog_configuration["paths"].keys():
+        if not type(blog_configuration["paths"]["ftp"]) == str:  # TODO: check when used
+            from venc3.prompt import die
+            die(("field_is_not_of_type", field, "blog_configuration.yaml", fields[field].__name__))
+        else:
+            blog_configuration["paths"]["ftp"] = '/'.join([directory for directory in blog_configuration["paths"]["ftp"].split('/') if len(directory) ])
+                
+def setup_optional_fields(blog_configuration):
+        sanitize_optional_fields(blog_configuration)
+    
+        default_values = {
+            "default_theme" : '',
+            "sort_by" : "id",
+            "pipe_flow" : 512,
+            "path_encoding": "", # TODO: plz, what da fuck is this shit ?
+            "disable_threads" : [],
+            "parallel_processing" : 1,
+            "columns" : 1,
+            "server_port" : 8888,
+            "ftp_port": 21,
+            "ftp_encoding": "latin-1",
+            "ftp_sessions": 4
+        }
             
-    except UnicodeEncodeError as e:
-        from venc3.exceptions import VenCException
-        raise VenCException(("encoding_error_in_sub_folder_path", key))
-                    
-    blog_configuration["path"][key] = (path if path[-1] == '/' else path+'/' ) if (path != '/' and len(path)) else ''
-
-# TODO : Datastructure parsing sux so bad. Need advanced type check and content validation
+        for field in default_values.keys():
+            if not field in blog_configuration.keys():
+                blog_configuration[field] = default_values[field]
+                        
+        fields_set_to_false = [
+          "code_highlight_css_override",
+          "disable_archives",
+          "disable_atom_feed",
+          "disable_categories",
+          "disable_chapters",
+          "disable_main_thread",
+          "disable_rss_feed",
+          "disable_single_entries",
+        ]
+        
+        for field in fields_set_to_false:
+            if not field in blog_configuration.keys():
+                blog_configuration[field] = False
+                
 def get_blog_configuration():
     global BLOG_CONFIGURATION
     if BLOG_CONFIGURATION != None:
         return BLOG_CONFIGURATION
   
     import os
     import yaml
@@ -44,90 +109,64 @@
             open(
                 os.getcwd()+"/blog_configuration.yaml",
                 'r'
             ).read(),
             Loader=yaml.FullLoader
         )
         
-        mandatory_fields = [
-            "blog_name",
-            "blog_url",
-            "date_format",
-            "ftp_host",
-            "entries_per_pages",
-            "columns",
-            "feed_length",
-            "reverse_thread_order",
-            "markup_language",
-            "disable_main_thread",
-            "disable_archives",
-            "disable_categories",
-            "disable_chapters",
-            "disable_single_entries",
-            "code_highlight_css_override",
-            "server_port",
-            "disable_rss_feed",
-            "disable_atom_feed",
-            "sort_by",
-        ]
+        #TODO: update doc about mandatory fields
 
-        for field in mandatory_fields:
+        mandatory_fields = {
+            "blog_name" : str,
+            "date_format" : str,
+            "entries_per_pages" : int,
+            "feed_length" : int,
+            "reverse_thread_order" : bool,
+            "markup_language" : str,
+            "paths": dict
+        }
+
+        for field in mandatory_fields.keys():
             if not field in blog_configuration.keys():
                 from venc3.prompt import die
                 die(("missing_mandatory_field_in_blog_conf", field))
-                
-        if "blog_keywords" in blog_configuration.keys() and type(blog_configuration["blog_keywords"]) != list and not blog_configuration["blog_keywords"] == None:
-            from venc3.prompt import die
-            die(("blog_metadata_is_not_a_list", "blog_keywords"))
+            
+            if not type(blog_configuration[field]) == mandatory_fields[field]:
+                from venc3.prompt import die
+                die(("field_is_not_of_type", field, "blog_configuration.yaml", mandatory_fields[field].__name__))
         
-        mandatory_fields = [
-            "index_file_name",
-            "category_directory_name",
-            "chapter_directory_name",
-            "archives_directory_name",
-            "entry_file_name",
-            "rss_file_name",
-            "atom_file_name",
-            "ftp",
-            "entries_sub_folders",
-            "categories_sub_folders",
-            "archives_sub_folders",
-            "chapters_sub_folders",
-        ]
+        mandatory_fields = {
+            "index_file_name" : str,
+            "category_directory_name" : str,
+            "chapter_directory_name" : str,
+            "archives_directory_name" : str,
+            "entry_file_name" : str,
+            "rss_file_name" : str,
+            "atom_file_name" : str,
+            "entries_sub_folders" : str,
+            "categories_sub_folders" : str,
+            "archives_sub_folders" : str,
+            "chapters_sub_folders" : str,
+        }
 
         for field in mandatory_fields:
-            if not field in blog_configuration["path"].keys():
+            if not field in blog_configuration["paths"].keys():
                 from venc3.prompt import die
                 die(("missing_mandatory_field_in_blog_conf", field))
                 
-            elif not field in ["index_file_name","ftp","rss_file_name","atom_file_name","entry_file_name","archives_directory_name"]:
-                setup_sub_folder(blog_configuration, field)
-                
-        if not "https://schema.org" in blog_configuration.keys():
-            blog_configuration["https://schema.org"] = {}
-            
+            if not type(blog_configuration["paths"][field]) == mandatory_fields[field]:
+                from venc3.prompt import die
+                die(("field_is_not_of_type", field, "blog_configuration.yaml", mandatory_fields[field].__name__))
+
         if not blog_configuration["markup_language"] in ["none", "Markdown", "reStructuredText", "asciidoc"]:
             from venc3.prompt import die
             die(("unknown_markup_language", blog_configuration["markup_language"], "blog_configuration.yaml"))
-
-        if (not "sort_by" in blog_configuration.keys() ) or blog_configuration["sort_by"] in ['', None]:
-            blog_configuration["sort_by"] = "id"
-
-        if type(blog_configuration["blog_url"]) == str and blog_configuration["blog_url"][-1:] == '/':
-            blog_configuration["blog_url"] = blog_configuration["blog_url"][:-1]
-
-        if "disable_threads" in blog_configuration.keys() and type(blog_configuration["disable_threads"]) != list and blog_configuration["disable_threads"] != None:
-            from venc3.prompt import die
-            die(("blog_metadata_is_not_a_list", "disable_threads"))
-        else:
-            blog_configuration["disable_threads"] = []
-
-        if not "pipe_flow" in blog_configuration.keys():
-            blog_configuration["pipe_flow"] = 512
-            
+        
+        setup_optional_fields(blog_configuration)
+                        
         BLOG_CONFIGURATION = blog_configuration
         return BLOG_CONFIGURATION
 
     except FileNotFoundError:
         from venc3.prompt import die
         die(("no_blog_configuration",))
 
@@ -135,10 +174,7 @@
         from venc3.prompt import die
         die(("no_blog_configuration",))
 
     except yaml.scanner.ScannerError as e:
         from venc3.prompt import die, notify
         notify(("in_", "blog_configuration.yaml"), color="RED")
         die(("exception_place_holder", str(e)))
-
-    except VenCException as e:
-        e.die()
```

### Comparing `VenC-3.1.1/venc3/datastore/entries.py` & `VenC-3.2.0/venc3/datastore/entries.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,31 +24,30 @@
 class Entries:
     def init_entries(self):
       
         self.entries = []
 
         from venc3.prompt import notify
         notify(("loading_entries",), prepend="┌─ ")
-
-        from venc3.datastore.entry import yield_entries_content
-        filenames = [filename for filename in yield_entries_content()]
-        
-        self.chunks_len = (len(filenames)//self.workers_count)+1
         
         from venc3.exceptions import VenCException
         
         try:
+            from venc3.datastore.entry import yield_entries_content
+            filenames = [filename for filename in yield_entries_content()]
+            
+            self.chunks_len = (len(filenames)//self.workers_count)+1      
             if self.workers_count > 1:
                 # There we setup chunks of entries send to workers throught dispatchers
                 global multiprocessing_thread_params
                 multiprocessing_thread_params = {
                     "chunked_filenames" :[],
                     "workers_count" : self.workers_count,
                     "entries": self.entries,
-                    "paths": self.blog_configuration["path"],
+                    "paths": self.blog_configuration["paths"],
                     "cut_threads_kill_workers" : False
                 }
                 for i in range(0, self.workers_count):
                     multiprocessing_thread_params["chunked_filenames"].append(filenames[:self.chunks_len])
                     filenames = filenames[self.chunks_len:]
                     
                 filenames = None
@@ -69,15 +68,15 @@
                 parallelism.start()
                 parallelism.join()
                     
             else:
                 for filename in filenames:
                     self.entries.append(Entry(
                         filename,
-                        self.blog_configuration["path"],
+                        self.blog_configuration["paths"],
                     ))
                     
         except VenCException as e:
             if self.workers_count > 1:
                 parallelism.kill()
                 
             e.die()
```

### Comparing `VenC-3.1.1/venc3/datastore/entry.py` & `VenC-3.2.0/venc3/datastore/entry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /usr/bin/env python3
 
-#    Copyright 2016, 2023 Denis Salem
+#    Copyright 2016, 2024 Denis Salem
 #
 #    This file is part of VenC.
 #
 #    VenC is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
@@ -24,28 +24,27 @@
 from venc3.patterns.processor import PatternTree
 
 class Entry:  
     def __init__(self, filename, paths):
         date_format = paths["archives_directory_name"]
         self.previous_entry = None
         self.next_entry = None
-        self.chapter = None  # will be overriden at chapters datastructure generation
         self.title = ''
 
         # Loading
         raw_data = open(os.getcwd()+"/entries/"+filename,'r').read()
         entry_parted = raw_data.split("---VENC-BEGIN-PREVIEW---\n")
         if len(entry_parted) == 2:
             entry_parted = [entry_parted[0]] + entry_parted[1].split("---VENC-END-PREVIEW---\n")
             if len(entry_parted) == 3:
                 import yaml
                 try:
                     metadata = yaml.load(entry_parted[0], Loader=yaml.FullLoader)
 
-                except yaml.scanner.ScannerError as e:
+                except Exception as e:
                     from venc3.exceptions import VenCException
                     raise VenCException(("possible_malformed_entry", filename, ''), context=filename, extra=str(e))
                     
                 if "markup_language" in metadata.keys():
                     markup_language = metadata["markup_language"]
                 else:
                     from venc3.datastore.configuration import get_blog_configuration
@@ -113,17 +112,15 @@
         params = {
             "entry_id": self.id,
             "entry_title": self.title
         }
 
         sf = quirk_encoding(paths["entries_sub_folders"].format(**params))
         self.sub_folder = (sf+'/' if sf[-1] != '/' else sf) if len(sf) else ''
-        self.path = "\x1a"+self.sub_folder+quirk_encoding(
-            paths["entry_file_name"].format(**params)
-        )
+        self.path = "\x1a/"+quirk_encoding(self.sub_folder+paths["entry_file_name"].format(**params)).replace('//','/')
         
         if type(metadata["categories"]) != list:
             from venc3.exceptions import VenCException
             raise VenCException(("entry_metadata_is_not_a_list", "categories", self.id), context=filename)
 
         self.raw_categories = metadata["categories"]
         
@@ -157,17 +154,17 @@
                 from venc3.prompt import notify
                 notify(("invalid_entry_filename", filename), "YELLOW")
 
             except IndexError:
                 from venc3.prompt import notify
                 notify(("invalid_entry_filename", filename), "YELLOW")
     
-    except FileNotFoundError:
-        from venc3.prompt import die
-        die(("file_not_found", os.getcwd()+"/entries"))
+    except FileNotFoundError as e:
+        from venc3.exceptions import VenCException
+        raise VenCException(("file_not_found", str(e)))
 
 def get_latest_entryID():
     entries_list = sorted(yield_entries_content(), key = lambda entry : int(entry.split("__")[0]))
     if len(entries_list) != 0:
         return int(entries_list[-1].split("__")[0])
     else:
         return 0
```

### Comparing `VenC-3.1.1/venc3/datastore/hardcoded_assets.py` & `VenC-3.2.0/venc3/datastore/hardcoded_assets.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/datastore/metadata.py` & `VenC-3.2.0/venc3/datastore/metadata.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/datastore/taxonomy.py` & `VenC-3.2.0/venc3/datastore/taxonomy.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,56 +55,56 @@
         self.categories_weight_tracker = WeightTracker()
         self.html_categories_tree = {}
         self.html_categories_leaves = {}
         
         if self.entries_per_categories == None:
             self.entries_per_categories = []
             self.categories_leaves = []
-            path = self.blog_configuration["path"]["categories_sub_folders"]
+            path = self.blog_configuration["paths"]["categories_sub_folders"]
             for entry_index in range(0, len(self.entries)):
                 current_entry = self.entries[entry_index]
                 self.build_tree(
                     current_entry.id,
                     current_entry.raw_categories,
                     self.entries_per_categories,
                     self.categories_leaves,
                     self.categories_weight_tracker,
-                    sub_folders="\x1a"+path
+                    sub_folders="\x1a/"+path
                 )
                 
             self.categories_leaves = self.extract_leaves(None)
     
-    def build_tree(self, entry_id, input_list, blog_output_tree, blog_output_leaves, weight_tracker, sub_folders=''):     
-        from venc3.datastore.configuration import get_blog_configuration
-        category_directory_name = get_blog_configuration()["path"]["category_directory_name"]
+    def build_tree(self, entry_id, input_list, blog_output_tree, blog_output_leaves, weight_tracker, sub_folders):     
+        category_directory_name = self.blog_configuration["paths"]["category_directory_name"]
 
         for item, sub_items in flatten_current_level(input_list):
-            if not len(item):
+            if not len(str(item)):
                 continue
     
             match = None
             try:
-                path = sub_folders+quirk_encoding(category_directory_name.format(**{"category":item}))
+                path = quirk_encoding(sub_folders + ('/' if len(sub_folders) > 1 else '') + category_directory_name.format(**{"category":item})).replace('//','/')
+
             except KeyError as e:
                 from venc3.prompt import die
                 die(("invalid_variable_name_in_setting", str(e), "category_directory_name"))
                 
             for node in blog_output_tree:
-                if node.value == item:
+                if node.value == str(item):
                     node.count +=1
                     node.weight_tracker.update()
                     node.related_to.append(entry_id)
                     match = node
                     break
     
             if match == None:
                 metadata = MetadataNode(
-                    item, 
+                    str(item), 
                     entry_id,
-                    quirk_encoding(path),
+                    path,
                     weight_tracker
                 )
     
                 blog_output_tree.append(metadata) 
                 blog_output_leaves.append(metadata)
                 
             if len(sub_items):
```

### Comparing `VenC-3.1.1/venc3/datastore/theme.py` & `VenC-3.2.0/venc3/datastore/theme.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/exceptions.py` & `VenC-3.2.0/venc3/exceptions.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/helpers.py` & `VenC-3.2.0/venc3/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,14 +21,39 @@
 import sys
 
 # Sometimes format fail with {something} not found in given dict.
 class SafeFormatDict(dict):
     def __missing__(self, key):
         return '{'+key+'}'
 
+def copy_recursively(src, dest):
+    import errno, os, shutil
+    
+    try:
+        listdir = os.listdir(src)
+    except Exception as e:
+        from venc3.exceptions import VenCException
+        VenCException(("exception_place_holder", e)).die()
+        
+    for filename in listdir:
+        try:
+            shutil.copytree(src+filename, dest+filename)
+    
+        except shutil.Error as e:
+            from venc3.prompt import notify
+            notify(("directory_not_copied", str(e)), "YELLOW")
+            
+        except OSError as e:
+            if e.errno == errno.ENOTDIR:
+                shutil.copy(src+filename, dest+filename)
+
+            else:
+                from venc3.prompt import notify
+                notify(("directory_not_copied", str(e)), "YELLOW")
+                
 def export_extra_data(origin, destination=""):
     import os
     import shutil
 
     try:
         folder = os.listdir(origin)
         for item in folder:
@@ -45,29 +70,17 @@
         raise
 
 def get_base_dir():
     return sys.prefix if sys.prefix != sys.base_prefix else os.path.expanduser("~")+"/.local"
 
 def quirk_encoding(string):
     import unidecode
-    return unidecode.unidecode(
-        string.replace(
-            '\'',
-            '-'
-        ).replace(
-            ' ',
-            '-'
-        ).replace(
-            '%',
-            '-'
-        ).replace(
-            ':',
-            '-'
-        )
-    )
+    for char in ['\'',' ','%',':','&','\\']:
+        string = string.replace(char,'-')
+    return unidecode.unidecode(string)
 
 def rm_tree_error_handler(function, path, excinfo):
     from venc3.prompt import notify
     
     if path == "blog" and excinfo[0] == FileNotFoundError:
         notify(("blog_folder_doesnt_exists",),"YELLOW")
         return
@@ -96,15 +109,15 @@
                 from venc3.l10n import messages; 
                 cause = messages.missing_separator_in_entry.format("---VENC-BEGIN-PREVIEW---")
                 from venc3.exceptions import VenCException
                 raise VenCException(("possible_malformed_entry", template_path, cause), context=template_path)
             
             import yaml
             try:
-                parted[0] = yaml.dump(yaml.load(parted[0], Loader=yaml.FullLoader))
+                parted[0] = yaml.dump(yaml.load(parted[0], Loader=yaml.FullLoader),allow_unicode=True)
                 
             except yaml.scanner.ScannerError as e:
                 from venc3.exceptions import VenCException
                 raise VenCException(("possible_malformed_entry",template_path, ''), context=template_path, extra=str(e))
                 
             return "---VENC-BEGIN-PREVIEW---".join(parted)
             
@@ -119,8 +132,7 @@
             from venc3.exceptions import VenCException
             raise VenCException(("wrong_permissions", template_path))
     
     from venc3.exceptions import VenCException
     from venc3.l10n import messages
     msg = "\n"+ messages.file_not_found.format(templates_paths[0])+"\n"+ messages.file_not_found.format(templates_paths[1])
     raise VenCException(("exception_place_holder", msg))
-
```

### Comparing `VenC-3.1.1/venc3/l10n/__init__.py` & `VenC-3.2.0/venc3/l10n/__init__.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/l10n/en.py` & `VenC-3.2.0/venc3/l10n/en.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,31 +19,30 @@
 
 class Messages:
     cannot_get_current_locale = "Cannot get current locale. Language set to English."
     blog_created = "Your blog has been created!"
     blogs_created = "Your blogs have been created!"
     chapter_has_a_wrong_index = "In entry #{0}, chapter index format is wrong: {1}."
     theme_installed = "Theme has been installed!"
-    entry_written = "Entry has been saved!"
+    entry_written = "Entry has been saved: {0}"
     file_not_found = "{0}: this file or directory does not exist."
     file_already_exists = "{0}: {1}: file or directory already exists."
     invalid_entry_filename = "{0}: invalid entry filename."
     blog_name = "Blog name"
     blog_url = "The URL of your blog"
     missing_params = "{0}: missing arguments."
     cannot_read_in = "{0}: cannot read into {1}."
     nothing_to_do = "Nothing to do."
     unknown_command = "{0}: unknown command."
     no_blog_configuration = "Blog's configuration file doesn't exist or you do not have right permissions."
     missing_mandatory_field_in_blog_conf = "Warning, the field \"{0}\" is missing in the blog's configuration file."
     username="Username: "
     ftp_host="FTP hostname"
     ftp_path="Absolute path of your blog on FTP server."
-    clean_ftp_directory="Cleaning target FTP directory..."
-    copy_to_ftp_directory="Copying your blog to target FTP directory..."
+    sync_ftp_directory="Syncing remote target with local data..."
     possible_malformed_entry="Possible malformed entry {0}. {1} Abort."
     export_single_entries="Exporting single entries locally..."
     export_archives="Exporting entries grouped by dates locally..."
     export_main_thread="Exporting main entries thread locally."
     export_categories="Exporting entries grouped by categories locally..."
     export_chapters="Exporting chapters locally..."
     wrong_args_number="Wrong arguments number: expected {0}, got {1}."
@@ -80,15 +79,15 @@
     chapter_already_exists = "Chapters \"{0}\" (id = {1}) and \"{2}\" (id = {3}) have the same index \"{4}\"."
     copy_assets_and_extra_files = "Copying extra files..."
     task_done_in_n_seconds = "Task done in {0} seconds."
     nothing_to_serv = "Nothing to do. Try venc -xb before."
     theme_has_no_description = "This theme has no description."
     undefined_variable = "{0} is undefined in {1}."
     entry_has_no_metadata_like = "Entry has no metadata identified by \"{0}\"."
-    blog_has_no_metadata_like = "Blog has no metadata identified by {0}."
+    blog_has_no_metadata_like = "Blog has no metadata identified by \"{0}\"."
     invalid_range = "Invalid range {0}:{1}."
     entry_metadata_is_not_a_list = "Metadata identified by \"{0}\" from entry {1} is not a list."
     blog_metadata_is_not_a_list = "Metadata identified by \"{0}\" blog configuration file is not a list."
     item_deleted_from_server = "Deleted from server: {0}"
     item_uploaded_to_server = "Uploaded to server: {0}"
     cannot_retrieve_entry_attribute_because_wrong_id = "Cannot retrieve entry attribute because the given id is unknown."
     id_must_be_an_integer = "Identifier must be an integer."
@@ -117,11 +116,11 @@
     this_pattern_is_embed_in_the_name_of_another_one = "This pattern {0} is embedded in the name of another one."
     not_installed = "is not installed."
     chapter_type_is_ambiguous = "Chapter index from entry is of type float #{0} and ambiguous. It should be str or int."
     current_python_implementation_doesnt_support_parallelism = "Current Python implementation doesn't support parallelism."
     no_parallel_processing_default_value = "No explicit value is defined for \"parallel_processing\" in your configuration file.\nBy default VenC will run {0} parallel processes."
     wrong_value_for_parallel_processing = "Wrong value for \"parallel_processing\" in your configuration file. It must be a non zero positive integer."
     invalid_variable_name_in_setting = "Invalid variable name {0} in \"{1}\" within your configuration file."
-
+    invalid_value_in_setting = "Invalid value \"{0}\" in \"{1}\" within your configuration file."
     # Will not be hooked by l10n_cleanup
     generating_rss = "Generating RSS feed..."
     generating_atom = "Generating Atom feed..."
```

### Comparing `VenC-3.1.1/venc3/l10n/fr.py` & `VenC-3.2.0/venc3/l10n/fr.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #    along with VenC.  If not, see <http://www.gnu.org/licenses/>.
 
 class Messages:
     blog_created = "Votre blog a été créé !"
     blogs_created = "Vos blogs ont été créés !"
     chapter_has_a_wrong_index = "Dans la publication #{0}, le format de l'index du chapitre n'est pas correct : {1}."
     theme_installed = "Le thème a bien été installé !"
-    entry_written = "La publication a bien été ajoutée !"
+    entry_written = "La publication a bien été ajoutée : {0}"
     file_not_found = "{0} : ce fichier ou ce dossier n'existe pas."
     file_already_exists = "{0} : {1} : le fichier existe déjà."
     invalid_entry_filename = "{0} : nom de fichier invalide pour une publication."
     blog_name = "Nom du blog"
     blog_url = "L'URL du blog"
     missing_params = "{0} : paramètres manquants."
     cannot_read_in = "{0} : impossible de lire dans {1}."
@@ -34,16 +34,15 @@
     unknown_command = "{0} : commande inconnue."
     no_blog_configuration = "Le fichier de configuration du blog n'existe pas ou vous n'avez pas les bonnes permissions."
     missing_mandatory_field_in_blog_conf = "Attention, le champ \"{0}\" est manquant dans le fichier de configuration principal du blog."
     username="Nom d'utilisateur : "
     user_passwd="Mot de passe utilisateur : "
     ftp_host="Nom d'hôte FTP"
     ftp_path="Chemin absolu de votre blog sur l'hôte FTP."
-    clean_ftp_directory="Nettoyage du répertoire FTP de destination..."
-    copy_to_ftp_directory="Copie du blog vers le répertoire FTP de destination..."
+    sync_ftp_directory="Synchronisation de la destination avec les données locales..."
     possible_malformed_entry="La publication {0} est probablement mal formée... {1} Abandon."
     export_single_entries="Exportation locale des publications individuelles..."
     export_archives="Exportation locale des publications groupées par dates..."
     export_main_thread="Exportation locale du principal fil de publications."
     export_categories="Exportation locale des publications groupées par catégories..."
     export_chapters="Exportation locale des chapitres..."
     wrong_args_number="Mauvais nombre d'arguments : attendu {0}, reçu {1}."
@@ -79,15 +78,15 @@
     loading_entries = "Chargement des publications..."
     chapter_already_exists = "Les chapitres \"{0}\" (id = {1}) et \"{2}\" (id = {3}) ont le même index \"{4}\"."
     copy_assets_and_extra_files = "Copie des fichiers additionnels..."
     task_done_in_n_seconds = "Tâche réalisée en {0} secondes."
     nothing_to_serv = "Rien à faire. Essayez venc -xb d'abord."
     theme_has_no_description = "Ce thème n'a pas de description."
     undefined_variable = "{0} n'est  pas défini dans \"{1}\"."
-    entry_has_no_metadata_like = "La publication ne possède pas la métadonnée identifiée par \"{0}\"."
+    entry_has_no_metadata_like = "La publication \"{0}\" ne possède pas la métadonnée identifiée par \"{1}\"."
     blog_has_no_metadata_like = "Le blog ne possède pas la métadonnée identifiée par {0}."
     invalid_range = "Plage de nombres invalide {0}:{1}."
     entry_metadata_is_not_a_list = "La métadonnée \"{0}\" de la publication {1} n'est pas une liste."
     blog_metadata_is_not_a_list = "La métadonnée \"{0}\" dans le fichier de configuration du blog n'est pas une liste."
     item_deleted_from_server = "Supprimé du serveur : {0}"
     item_uploaded_to_server = "Transféré sur le serveur : {0}"
     cannot_retrieve_entry_attribute_because_wrong_id = "Impossible de récupérer l'attribut de la publication parce que l'id renseigné est inconnu."
@@ -117,11 +116,12 @@
     this_pattern_is_embed_in_the_name_of_another_one = "Le pattern {0} est intégré dans le nom d'un autre."
     not_installed = "n'est pas installé."
     chapter_type_is_ambiguous = "L'index du chapitre de la publication #{0} est de type float et est donc ambigu. Le type devrait être str ou int."
     current_python_implementation_doesnt_support_parallelism = "L'implémentation courante de Python ne supporte pas le parallélisme."
     no_parallel_processing_default_value = "Aucune valeur définie explicitement pour \"parallel_processing\" dans votre fichier de configuration.\nPar défaut, VenC utilisera {0} processus parallèles."
     wrong_value_for_parallel_processing = "La valeur de \"parallel_processing\" dans votre fichier de configuration est incorrecte, il doit s'agir d'un nombre entier supérieur à 0."
     invalid_variable_name_in_setting = "Variable {0} incorrecte dans \"{1}\" dans votre fichier de configuration."
+    invalid_value_in_setting = "La valeur \"{0}\" dans \"{1}\", dans votre fichier de configuration, est incorrecte."
     # Will not be hooked by l10n_cleanup
     generating_rss = "Génération du flux RSS..."
     generating_atom = "Génération du flux Atom..."
```

### Comparing `VenC-3.1.1/venc3/markup_languages/__init__.py` & `VenC-3.2.0/venc3/markup_languages/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,16 +40,16 @@
     }
     
     try:
         m = importlib.import_module("venc3.markup_languages."+key[markup_language][0])
         return getattr(m, key[markup_language][1])
         
     except ModuleNotFoundError:
-        from venc3.prompt import die
-        die(("module_not_found", key[markup_language][2]))  
+        from venc3.exceptions import VenCException
+        raise VenCException(("module_not_found", key[markup_language][2]))  
 
 def process_markup_language(source, markup_language, entry):
     if markup_language == "Markdown":
         do_table_of_content = ":content" == source.context[-8:]
         venc_markdown = import_wrapper(markup_language)(do_table_of_content)
         string = venc_markdown.render(source.string)
         if do_table_of_content:
```

### Comparing `VenC-3.1.1/venc3/markup_languages/asciidoc.py` & `VenC-3.2.0/venc3/markup_languages/asciidoc.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/markup_languages/markdown.py` & `VenC-3.2.0/venc3/markup_languages/markdown.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/markup_languages/restructuredtext.py` & `VenC-3.2.0/venc3/markup_languages/restructuredtext.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/parallelism/__init__.py` & `VenC-3.2.0/venc3/parallelism/__init__.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/parallelism/build_entries.py` & `VenC-3.2.0/venc3/parallelism/build_entries.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/parallelism/export_entries.py` & `VenC-3.2.0/venc3/parallelism/export_entries.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/patterns/datastore.py` & `VenC-3.2.0/venc3/patterns/datastore.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,14 +24,61 @@
         return separator.join([string.format(**something) for something in iterable])
     
     except KeyError as e:
         from venc3.exceptions import VenCException
         raise VenCException(("unknown_contextual", str(e)), pattern)
 
 class DatastorePatterns:
+    def cherry_pick_metadata(self, pattern, source, if_exists,  path):
+        from venc3.datastore.entry import Entry
+
+        if not len(path):
+            from venc3.exceptions import VenCException
+            raise VenCException(("wrong_args_number", ">= 1", "0"), context=self)
+            
+        try:
+            node = getattr(source, path[0]) if type(source) == Entry else source[path[0]]
+            previous_key = path[0]
+            for key in path[1:]:
+                node = node[key]
+                previous_key = key
+
+            return str(node)
+            
+        except TypeError:
+            from venc3.exceptions import VenCException
+            raise VenCException(("field_is_not_of_type", previous_key, source.title if type(source) == Entry else"blog_configuration.yaml", dict), pattern)
+            
+        except Exception as e:
+            if not type(e) in[KeyError, AttributeError]:
+                raise e
+            
+            if if_exists:
+                return ""
+                
+            if type(source) == Entry:
+                exception_params = ("entry_has_no_metadata_like", source.title, ' -> '.join(path))
+            else:
+                exception_params = ("blog_has_no_metadata_like", ' -> '.join(path))
+                
+            from venc3.exceptions import VenCException
+            raise VenCException(exception_params, pattern)
+            
+    def cherry_pick_blog_metadata(self, pattern, *branch):
+        return self.cherry_pick_metadata(pattern, self.blog_configuration, False, branch)
+
+    def cherry_pick_blog_metadata_if_exists(self, pattern, *branch):
+        return self.cherry_pick_metadata(pattern, self.blog_configuration, True, branch)
+
+    def cherry_pick_entry_metadata(self, pattern, *branch):
+        return self.cherry_pick_metadata(pattern, self.requested_entry, False, branch)
+
+    def cherry_pick_entry_metadata_if_exists(self, pattern, *branch):
+        return self.cherry_pick_metadata(pattern, self.requested_entry, True, branch)
+        
     def if_categories(self, pattern, if_true, if_false=''):
         if self.entries_per_categories != [] and not self.blog_configuration["disable_categories"]:
             return if_true
             
         else:
             return if_false
     
@@ -90,15 +137,15 @@
             else:
                 return if_true
                     
         except KeyError:
             return if_true
                         
     def get_chapters(self, pattern, list_open, item_open, item_close, list_close):
-        '''index,title,path,level'''
+        '''index,title,path,level,html_id'''
         key = list_open+item_open+item_close+list_close
         if not key in self.html_chapters.keys():
             self.html_chapters[key] = self.build_html_chapters(list_open, item_open, item_close, list_close, self.chapters_index, 0)
 
         return self.html_chapters[key]
 
     def get_entry_toc(self, pattern, open_ul, open_li, content, close_li, close_ul):
@@ -115,33 +162,36 @@
             
     def get_blog_metadata(self, pattern, metadata_name):
         # if exception is raised it will be automatically be catch by processor.
         try:
             return str(self.blog_configuration[metadata_name])
             
         except KeyError:
-            raise VenCException(("blog_has_no_metadata_like", metadata_name), context=self)
+            from venc3.exceptions import VenCException
+            raise VenCException(("blog_has_no_metadata_like", metadata_name), pattern)
             
     def get_blog_metadata_if_exists(self, pattern, metadata_name, if_true='', if_false='', ok_if_null=True):
+        '''value'''
         try:
             value = self.blog_configuration[metadata_name]
             
         except KeyError:
             return if_false
         
         if len(if_true):
             if ok_if_null or (value != None and len(str(value))):
-                return if_true.format(**{"value" : value,"{relative_origin}":"\x1a"})
+                return if_true.format(**{"value" : value})
                   
             else:
                 return if_false
         else:
             return value
             
     def get_blog_metadata_if_not_null(self, pattern, metadata_name, if_true='', if_false=''):
+        '''value'''
         try:
             return self.get_blog_metadata_if_exists(pattern, metadata_name, if_true, if_false, ok_if_null=False)
             
         except Exception as e:
             import traceback
             print(traceback.format_exc())
             
@@ -154,15 +204,15 @@
             
             except ValueError:
                 from venc3.exceptions import VenCException
                 raise VenCException(("id_must_be_an_integer",), pattern)
                 
             except AttributeError as e:
                 from venc3.exceptions import VenCException
-                raise VenCException(("entry_has_no_metadata_like", attribute), pattern)
+                raise VenCException(("entry_has_no_metadata_like", entry.id), pattern)
 
             except IndexError:
                 from venc3.exceptions import VenCException
                 raise VenCException(("cannot_retrieve_entry_attribute_because_wrong_id",), pattern)
             
         return self.cache_get_entry_attribute_by_id[key]
     
@@ -183,15 +233,15 @@
     def get_entry_metadata(self, pattern, metadata_name):
         try:
             return str(getattr(self.requested_entry, metadata_name))
             
         except AttributeError:
             from venc3.exceptions import VenCException
             raise VenCException(
-                ("entry_has_no_metadata_like", metadata_name),
+                ("entry_has_no_metadata_like", self.requested_entry.id, metadata_name),
                 pattern
             )
             
     def get_entry_metadata_if_exists(self, pattern, metadata_name, string='', string2='', ok_if_null=True):
         '''value'''
         try:
             value = str(getattr(self.requested_entry,metadata_name ))
@@ -235,16 +285,16 @@
 
     def get_entry_date(self, pattern, date_format=''):
         return self.requested_entry.date.strftime(
             date_format if len(date_format) else self.blog_configuration["date_format"]
         )
 
     def get_entry_archive_path(self, pattern):
-        return "\x1a"+self.requested_entry.date.strftime(
-            self.blog_configuration["path"]["archives_directory_name"]
+        return "\x1a/"+self.requested_entry.date.strftime(
+            self.blog_configuration["paths"]["archives_directory_name"]
         )
     
     def get_chapter_attribute_by_index(self, pattern, attribute, index):
         if self.blog_configuration["disable_chapters"]:
             return ""
         
         key = attribute+index
@@ -285,30 +335,30 @@
         return self.get_blog_metadata_if_exists(pattern, "author_description")
 
         
     def get_blog_license(self, pattern):
         return self.get_blog_metadata_if_exists(pattern, "license")
     
     def get_blog_url(self, pattern):
-        return self.blog_configuration["blog_url"]
-    
+        return self.get_blog_metadata_if_exists(pattern, "blog_url")
+
     def get_blog_language(self, pattern):
         return self.get_blog_metadata_if_exists(pattern, "blog_language")
     
     def get_author_email(self, pattern):
         return self.get_blog_metadata_if_exists(pattern, "author_email")
 
     def get_root_page(self, pattern):
         if self.root_page == None:
-            self.root_page =  "\x1a"+self.blog_configuration["path"]["index_file_name"].format(**{"page_number":''})
+            self.root_page =  "\x1a/"+self.blog_configuration["paths"]["index_file_name"].format(**{"page_number":''})
             
         return self.root_page
         
     def get_entry_categories_tree(self, pattern, open_node, open_branch, close_branch, clode_node):
-        '''value,count,weight,path,childs'''
+        '''value,html_id,count,weight,path,childs'''
         key = open_node+open_branch+close_branch+clode_node
         entry = self.requested_entry
 
         if not key in self.requested_entry.html_categories_tree.keys():
             if self.blog_configuration["disable_categories"]:
                 entry.html_categories_tree[key] = ''
 
@@ -320,73 +370,95 @@
                     close_branch,
                     clode_node,
                     self.extract_leaves(entry.id)
                 )
 
         
         return entry.html_categories_tree[key]
-            
-    def get_blog_categories_tree(self, pattern, open_node, open_branch, close_branch, clode_node):
-        '''value,count,weight,path,childs'''
-        key = open_node+open_branch+close_branch+clode_node
+
+    def get_blog_categories_tree_from_branches(self, pattern, branches, sub_tree_string, separator, open_node, open_branch, close_branch, close_node):
+        '''value,html_id,count,weight,path,childs'''
+
+        return self.get_categories_tree_from_branches(
+            pattern,
+            branches,
+            sub_tree_string,
+            separator,
+            open_node,
+            open_branch,
+            close_branch,
+            close_node,
+            None
+        )
+
+    def get_entry_categories_tree_from_branches(self, pattern, branches, sub_tree_string, separator, open_node, open_branch, close_branch, close_node):
+        '''value,html_id,count,weight,path,childs'''
+
+        return self.get_categories_tree_from_branches(
+            pattern,
+            branches,
+            sub_tree_string,
+            separator,
+            open_node,
+            open_branch,
+            close_branch,
+            close_node,
+            self.requested_entry
+        )
+
+        
+    def get_categories_tree_from_branches(self, pattern, branches, sub_tree_string, sub_tree_separator, open_node, open_branch, close_branch, close_node, from_entry):
+        branches = branches.strip()
+        self.test_blog_configuration_field(pattern, branches, list)
+        
+        output = []
+        
+        for branch_name in self.blog_configuration[branches]:
+            node = self.pick_branch(branch_name, None)
+            if node != None and len(node.childs):
+                if from_entry != None:
+                    extracted_branches = self.extract_leaves(from_entry.id, node.childs)
+                    if not len(extracted_branches):
+                        continue
+                        
+                output.append(
+                    sub_tree_string.format(
+                        **self.node_to_dictionnary(
+                            pattern,
+                            node,
+                            open_node,
+                            open_branch,
+                            close_branch,
+                            close_node,
+                            node.childs if from_entry == None else extracted_branches
+                        )
+                    )
+                )
+        
+        return sub_tree_separator.join(output)
+                
+    def get_blog_categories_tree(self, pattern, open_node, open_branch, close_branch, close_node):
+        '''value,html_id,count,weight,path,childs'''
+        key = open_node+open_branch+close_branch+close_node
         # compute once categories tree and deliver baked html
         if not key in self.html_categories_tree.keys():
             if self.blog_configuration["disable_categories"]:
                 self.html_categories_tree[key] = ''
 
             else:
                 self.html_categories_tree[key] = self.build_html_categories_tree(
                     pattern, 
                     open_node,
                     open_branch,
                     close_branch,
-                    clode_node,
+                    close_node,
                     self.entries_per_categories
                 )
 
         return self.html_categories_tree[key]
-        
-    def range_entries_by_id(self, pattern, begin_at, end_at):
-        key = 'rang_entries_by_id,'+begin_at+','+end_at
-        if not str(id(key)) in self.cache_entries_subset.keys():
-            try:
-                begin_at= int(begin_at)
-                
-            except ValueError:
-                from venc3.exceptions import VenCException
-                from venc3.l10n import messages
-                raise VenCException(
-                    ("wrong_pattern_argument", "begin_at", begin_at, "RangeEntriesByID", messages.pattern_argument_must_be_integer),
-                    pattern
-                )
-            
-            try:
-                end_at = int(end_at)
-                
-            except ValueError:
-                from venc3.exceptions import VenCException
-                from venc3.l10n import messages
-                raise VenCException(
-                    ("wrong_pattern_argument", "end_at", end_at, "RangeEntriesByID", messages.pattern_argument_must_be_integer),
-                    pattern
-                )
-            
-            entries = []
-            if end_at > begin_at:
-                entries = [entry for entry in self.entries if end_at >= entry.id >= begin_at]
-                
-            elif end_at < begin_at:
-                entries = [entry for entry in self.entries[::-1] if end_at <= entry.id <= begin_at]
-    
-            else:
-                entries = []
-            
-            self.cache_entries_subset[str(id(key))] = entries
-            
-        return str(id(key))
             
     def for_entries_set(self, pattern, entries_subset_key, string):
         '''id,title,path,archive_path,chapter_path,...'''
         output = ""
         try:
             entries = self.cache_entries_subset[entries_subset_key.strip()]
             
@@ -395,21 +467,21 @@
             from venc3.l10n import messages
             raise VenCException(
                 ("wrong_pattern_argument", "entries_subset_key", entries_subset_key, "ForEntriesSet", messages.argument_does_not_match_with_any_entries_subset),
                 pattern
             )
         
         date_format = self.blog_configuration["date_format"]
-        archives_directory_name = self.blog_configuration["path"]["archives_directory_name"]
+        archives_directory_name = self.blog_configuration["paths"]["archives_directory_name"]
         for entry in entries:
             dataset = {
                 "id" : entry.id,
                 "title": entry.title,
                 "path": entry.path,
-                "archive_path": "\x1a"+entry.date.strftime(archives_directory_name),
+                "archive_path": "\x1a/"+entry.date.strftime(archives_directory_name),
                 "chapter_path": entry.chapter.path if entry.chapter != None else ""
             }
             dataset.update({ 
                 attr: getattr(entry, attr) for attr in dir(entry) if type(getattr(entry, attr)) in [str, int, float]
             })
             while '∞':
                 try:
@@ -417,103 +489,105 @@
                     break
                 except KeyError as e:
                     dataset.update({str(e)[1:-1]:''})
                     
         return output
 
     def for_blog_archives(self, pattern, string, separator):
-        '''value,path,count,weight'''
+        '''value,path,count,weight,html_id'''
+        from venc3.helpers import quirk_encoding
         key = string+','+separator
         if not key in self.cache_blog_archives.keys():
             if self.blog_configuration["disable_archives"]:
                 self.cache_blog_archives[key] = ''
 
             else:
                 archives = [{
                     "value" : o.value,
+                    "html_id" : quirk_encoding(o.value),
                     "path" : o.path,
                     "count" : o.count,
                     "weight" : round(o.count / o.weight_tracker.value,2)
                 } for o in self.entries_per_archives if o.value not in self.disable_threads]
                 self.cache_blog_archives[key] = merge(archives, string, separator, pattern)
 
         return self.cache_blog_archives[key]
 
     def for_blog_metadata(self, pattern, metadata_name, string, separator=''):
-        '''value'''
+        '''value,html_id'''
         return self.for_blog_metadata_if_exists(pattern, metadata_name, string, separator, raise_exception=True)
 
     def for_blog_metadata_if_exists(self, pattern, metadata_name, string, separator='', raise_exception=False):
-        '''value'''
+        '''value,html_id'''
         key = metadata_name+','+string+','+separator+','+str(raise_exception)
         if not key in self.html_for_metadata:
             if not metadata_name in self.blog_configuration.keys():
                 if raise_exception:
                     from venc3.exceptions import VenCException
                     raise VenCException(("blog_has_no_metadata_like", metadata_name), pattern)
                     
                 self.html_for_metadata[key] = ""
                 return ""
                 
             if type(self.blog_configuration[metadata_name]) != list:
                 if raise_exception:
                     from venc3.exceptions import VenCException
                     raise VenCException(("blog_metadata_is_not_a_list", metadata_name), pattern)
-                    
-                self.html_for_metadata[key] = ""
-                
-            self.html_for_metadata[key] = merge([{"value": v} for v in self.blog_configuration[metadata_name]], string, separator, pattern)
+
+            from venc3.helpers import quirk_encoding
+            self.html_for_metadata[key] = merge([{"value": v.strip(),"html_id":quirk_encoding(v.strip())} for v in self.blog_configuration[metadata_name]], string, separator, pattern)
         
         return self.html_for_metadata[key]
 
     def for_entry_metadata(self, pattern, metadata_name, string, separator=''):
-        '''value'''
+        '''value,html_id'''
         return self.for_entry_metadata_if_exists(pattern, metadata_name, string, separator, raise_exception=True)
 
     def for_entry_metadata_if_exists(self, pattern, metadata_name, string, separator='', raise_exception=False):    
-        '''value'''    
+        '''value,html_id'''    
         entry = self.requested_entry
         key = metadata_name+string+separator
             
         if not key in entry.html_for_metadata:
             try:
                 l = getattr(entry, metadata_name)
                 if not type(l) in [list, tuple]:
                     from venc3.exceptions import VenCException
                     raise VenCException(("entry_metadata_is_not_a_list", metadata_name, entry), pattern)
                 
             except AttributeError as e:
                 if raise_exception:
                     from venc3.exceptions import VenCException
-                    raise VenCException(("entry_has_no_metadata_like", metadata_name), pattern)
+                    raise VenCException(("entry_has_no_metadata_like", entry.id, metadata_name), pattern)
                 else:
                     entry.html_for_metadata[key] = ""
                     return ""
                 
             try:
+                from venc3.helpers import quirk_encoding
                 entry.html_for_metadata[key] = separator.join([
-                     string.format(**{"value": item.strip()}) for item in l
+                     string.format(**{"value": item.strip(),"html_id":quirk_encoding(item.strip())}) for item in l
                 ])
                 
             except KeyError as e:
                 from venc3.exceptions import VenCException
                 raise VenCException(("unknown_contextual", str(e)), pattern)
             
         return entry.html_for_metadata[key]
             
     def for_entry_authors(self, pattern, string, separator=' '):
-        '''value'''
+        '''value,html_id'''
         return self.for_entry_metadata(pattern, "authors", string, separator)
 
     def get_blog_metadata_tree(self, pattern, metadata_name, open_node, open_branch, value_childs, value, close_branch, close_node):
-        '''value,tree'''
+        '''value,tree,html_id'''
         return self.get_blog_metadata_tree_if_exists(pattern, metadata_name, open_node, open_branch, value_childs, value, close_branch, close_node, raise_exception=True)
 
     def get_blog_metadata_tree_if_exists(self, pattern, metadata_name, open_node, open_branch, value_childs, value, close_branch, close_node, raise_exception=False):
-        '''value,childs'''
+        '''value,childs,html_id'''
         metadata_name = metadata_name.strip()
         key = metadata_name+','+open_node+','+open_branch+value_childs+','+value+','+close_branch+','+close_node+','+str(raise_exception)
         if key in self.html_tree_for_blog_metadata.keys():
             return self.html_tree_for_blog_metadata[key]
             
         if not metadata_name in self.blog_configuration.keys():
             if raise_exception:
@@ -524,74 +598,183 @@
                 self.html_tree_for_blog_metadata[key] = ""
                 return ""
                 
         self.html_tree_for_blog_metadata[key] = self.tree_for_metadata(self.blog_configuration[metadata_name], open_node, open_branch, value_childs, value, close_branch, close_node)
         return self.html_tree_for_blog_metadata[key]
         
     def get_entry_metadata_tree(self, pattern, metadata_name, open_node, open_branch, value_childs, value, close_branch, close_node):
-        '''value,childs'''
+        '''value,childs,html_id'''
         return self.get_entry_metadata_tree_if_exists(pattern, metadata_name, open_node, open_branch, value_childs, value, close_branch, close_node, raise_exception=True)
         
     def get_entry_metadata_tree_if_exists(self, pattern, metadata_name, open_node, open_branch, value_childs, value, close_branch, close_node, raise_exception=False):
-        '''value,childs'''
+        '''value,childs,html_id'''
         entry = self.requested_entry
         source = metadata_name.strip()
         if not hasattr(entry, metadata_name):
             if raise_exception:
                 from venc3.exceptions import VenCException
-                raise VenCException(("entry_has_no_metadata_like", metadata_name), pattern)
+                raise VenCException(("entry_has_no_metadata_like", entry.id, metadata_name), pattern)
                 
             else:
                 return ""
                 
         return self.tree_for_metadata(getattr(entry, metadata_name), open_node, open_branch, value_childs, value, close_branch, close_node)
-                    
-    def tree_for_metadata(self, source, open_node, open_branch, value_childs, value, close_branch, close_node):
-        try:
-            items = [
-                open_branch+value.format(
-                    **{"value":item}
-                )+close_branch if type(item) != dict else open_branch+value_childs.format(
-                    **{
-                        "value" : tuple(item.keys())[0],
-                        "childs": self.tree_for_metadata(tuple(item.values())[0], open_node, open_branch, value_childs, value, close_branch, close_node)
-                    }
-                )+close_branch for item in source
-            ]
-            
-        except KeyError as e:
-            from venc3.exceptions import VenCException
-            raise VenCException(("unknown_contextual", str(e)), pattern)
-            
-        return open_node + (''.join(items))+ close_node
 
-    def get_flattened_categories(self, pattern, string, separator, from_entry = False):
+
+    def get_flattened_categories(self, pattern, string, separator, from_entry = False, from_branch = None):
+        '''value,count,weight,path,html_id'''
+
         if self.blog_configuration["disable_categories"]:
             return ''
             
-        key = string+'::'+separator+'::'+str(self.requested_entry.id if from_entry else None)
+        key = string+'::'+separator+'::'+str(self.requested_entry.id if from_entry else None)+(("::"+str(from_branch.value)) if from_branch != None else '' ) 
         cache = self.requested_entry.html_categories_leaves if from_entry else self.html_categories_leaves
 
         if not key in cache.keys():
+            from venc3.helpers import quirk_encoding
             output = merge(
-                [ {
-                    "value" : node.value,
-                    "count" : node.count,
-                    "weight" : round(node.count / self.categories_weight_tracker.value, 2),
-                    "path" : node.path
-                } for node in self.extract_leaves( self.requested_entry.id if from_entry else None) ],
+                sorted(
+                    [{
+                        "value" : node.value,
+                        "html_id": quirk_encoding(node.value),
+                        "count" : node.count,
+                        "weight" : round(node.count / self.categories_weight_tracker.value, 2),
+                        "path" : node.path
+                    } for node in self.extract_leaves(
+                        self.requested_entry.id if from_entry else None,
+                        from_branch.childs if from_branch != None else None
+                    )],
+                    key = lambda d : d["value"]
+                ),
                 string,
                 separator,
                 pattern
             )
         
             cache[key] = output
         
-        return cache[key]
+        return cache[key]             
+
+    def get_flattened_categories_from_branches(self, pattern, branches, sub_tree_string, sub_tree_separator, string, separator, from_entry):
+        '''value,count,weight,path,html_id'''
+
+        branches = branches.strip()
+        self.test_blog_configuration_field(pattern, branches, list)
+        
+        output = []
+        
+        from venc3.helpers import quirk_encoding
+        
+        for branch_name in self.blog_configuration[branches]:
+            node = self.pick_branch(branch_name, None)
+            # TODO: self.extract_leaves will be called twice ... Boooooo not coooool
+            if node != None and len(self.extract_leaves(self.requested_entry.id if from_entry else None, node.childs)):
+                output.append(sub_tree_string.format(**{
+                    "value"  : node.value,
+                    "html_id": quirk_encoding(node.value),
+                    "count"  : node.count,
+                    "weight" : round(node.count / self.categories_weight_tracker.value, 2),
+                    "path"   : node.path,
+                    "childs" : self.get_flattened_categories(pattern, string, separator, from_entry, node)
+                }))
+                
+        return sub_tree_separator.join(output)
+                
+    def get_flattened_blog_categories(self, pattern, string, separator):
+        '''value,html_id,count,weight,path'''
+        return self.get_flattened_categories(pattern, string, separator)
+
+    def get_flattened_blog_categories_from_branches(self, pattern, branches, sub_tree_string, sub_tree_separator, string, separator):
+        '''value,html_id,count,weight,path,childs'''
+        
+        return self.get_flattened_categories_from_branches(pattern, branches, sub_tree_string, sub_tree_separator, string, separator, False)         
         
     def get_flattened_entry_categories(self, pattern, string, separator):
-        '''value,count,weight,path'''
+        '''value,html_id,count,weight,path'''
+
         return self.get_flattened_categories(pattern, string, separator, True)
 
-    def get_flattened_blog_categories(self, pattern, string, separator):
-        '''value,count,weight,path'''
-        return self.get_flattened_categories(pattern, string, separator)
+    def get_flattened_entry_categories_from_branches(self, pattern, branches, sub_tree_string, sub_tree_separator, string, separator):
+        '''value,html_id,count,weight,path,childs'''
+        return self.get_flattened_categories_from_branches(pattern, branches, sub_tree_string, sub_tree_separator, string, separator, True)
+        
+    def pick_branch(self, branch_name, extracted_branch):
+        for node in self.entries_per_categories if extracted_branch == None else extracted_branch:
+            if branch_name == node.value:
+                return node
+                
+        return None
+         
+    def range_entries_by_id(self, pattern, begin_at, end_at):
+        key = 'rang_entries_by_id,'+begin_at+','+end_at
+        if not str(id(key)) in self.cache_entries_subset.keys():
+            try:
+                begin_at= int(begin_at)
+                
+            except ValueError:
+                from venc3.exceptions import VenCException
+                from venc3.l10n import messages
+                raise VenCException(
+                    ("wrong_pattern_argument", "begin_at", begin_at, "RangeEntriesByID", messages.pattern_argument_must_be_integer),
+                    pattern
+                )
+            
+            try:
+                end_at = int(end_at)
+                
+            except ValueError:
+                from venc3.exceptions import VenCException
+                from venc3.l10n import messages
+                raise VenCException(
+                    ("wrong_pattern_argument", "end_at", end_at, "RangeEntriesByID", messages.pattern_argument_must_be_integer),
+                    pattern
+                )
+            
+            entries = []
+            if end_at > begin_at:
+                entries = [entry for entry in self.entries if end_at >= entry.id >= begin_at]
+                
+            elif end_at < begin_at:
+                entries = [entry for entry in self.entries[::-1] if end_at <= entry.id <= begin_at]
+    
+            else:
+                entries = []
+            
+            self.cache_entries_subset[str(id(key))] = entries
+            
+        return str(id(key))
+        
+    def test_blog_configuration_field(self, pattern, field_name, field_type):
+        if not field_name in self.blog_configuration.keys():
+            from venc3.exceptions import VenCException
+            raise VenCException(
+                ("undefined_variable", field_name, "blog_configuration.yaml"),
+                pattern
+            )
+            
+        if type(self.blog_configuration[field_name]) != field_type:
+            from venc3.exceptions import VenCException
+            raise VenCException(
+                ("field_is_not_of_type", field_name, field_type),
+                pattern
+            )
+            
+    def tree_for_metadata(self, source, open_node, open_branch, value_childs, value, close_branch, close_node):
+        from venc3.helpers import quirk_encoding
+        try:
+            items = [
+                open_branch+value.format(
+                    **{"value":item}
+                )+close_branch if type(item) != dict else open_branch+value_childs.format(
+                    **{
+                        "value" : tuple(item.keys())[0],
+                        "html_id" : quirk_encoding(tuple(item.keys())[0]),
+                        "childs": self.tree_for_metadata(tuple(item.values())[0], open_node, open_branch, value_childs, value, close_branch, close_node)
+                    }
+                )+close_branch for item in source
+            ]
+            
+        except KeyError as e:
+            from venc3.exceptions import VenCException
+            raise VenCException(("unknown_contextual", str(e)), pattern)
+            
+        return open_node + (''.join(items))+ close_node
```

### Comparing `VenC-3.1.1/venc3/patterns/non_contextual.py` & `VenC-3.2.0/venc3/patterns/non_contextual.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,18 @@
     return '::'.join(content)
     
 def html(pattern, *content):
     return "</p>"+('::'.join(content))+"<p>" if pattern.root.has_markup_language else '::'.join(content)
     
 def get_venc_version(pattern):
     return venc_version
-    
+
+def set_background_color(pattern, color, string):        
+    return "<span class=\"__VENC_TEXT_COLOR__\" style=\"background-color: "+color+";\">"+string+"</span>"
+        
 def set_color(pattern, color, string):        
     return "<span class=\"__VENC_TEXT_COLOR__\" style=\"color: "+color+";\">"+string+"</span>"
 
 def set_style(pattern, tag_id, tag_class, *string):
     return "<span id=\""+tag_id.strip()+"\" class=\""+tag_class.strip()+"\">"+('::'.join(string).strip())+"</span>"
 
 def include_file(pattern, filename, *argv, raise_error=True):
@@ -46,14 +49,15 @@
             return ""
 
         from venc3.exceptions import VenCException
         raise VenCException(("wrong_pattern_argument", "path", filename, "include_file"), pattern, pattern.root.string)
     
     include_string = None
     from venc3.helpers import get_base_dir
+    filename = filename.strip()
     paths = ("includes/"+filename, get_base_dir()+"/share/VenC/themes_includes/"+filename)
     for path in paths:
         if shutil.os.path.exists(path):
             try:
                 include_string = open(path, 'r').read()
                 break
```

### Comparing `VenC-3.1.1/venc3/patterns/patterns_map.py` & `VenC-3.2.0/venc3/patterns/patterns_map.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # TODO : Replace all argument name "node" by "pattern" to avoid confusion
 
 class PatternsMap():    
     CONTEXTUALS = { # All of the below is loaded from Thread instanciated classes
         "ForPages":	                    "for_pages",
         "GetEntryContent":              "get_entry_content",
         "GetEntryPreview":              "get_entry_preview",
+        "GetLastEntryTimestamp":	      "get_last_entry_timestamp",
         "GetNextPage":	                "get_next_page",
         "GetPreviousPage":	            "get_previous_page",
         "GetRandomNumber":	            "get_random_number",
         "GetRelativeLocation":	        "get_relative_location",
         "GetRelativeRoot":	            "get_relative_root",
         "GetStyleSheets":	              "get_style_sheets",
         "GetThreadName":	              "get_thread_name",
@@ -41,88 +42,97 @@
         "IfInThread":	                  "if_in_thread",
         "IfInThreadAndHasFeeds":	      "if_in_thread_and_has_feeds",
         "IfPages":	                    "if_pages",
         "PreviewIfInThreadElseContent": "preview_if_in_thread_else_content",
     }
 
     NON_CONTEXTUALS = { # all of the below is loaded from datastore
-        "entries" : { 
-            "ForEntryAuthors":	            "for_entry_authors",
-            "ForEntryMetadata":	            "for_entry_metadata",
-            "ForEntryMetadataIfExists":	    "for_entry_metadata_if_exists",   
-            "GetEntryArchivePath":	        "get_entry_archive_path",
-            "GetEntryCategoriesTree":	      "get_entry_categories_tree",
-            "GetEntryChapterLevel":         "get_entry_chapter_level",
-            "GetEntryChapterPath":          "get_entry_chapter_path",
-            "GetEntryDate":	                "get_entry_date",
-            "GetEntryDay":	                "get_entry_day",
-            "GetEntryHour":	                "get_entry_hour",
-            "GetEntryID":	                  "get_entry_id",
-            "GetEntryMetadata":	            "get_entry_metadata",
-            "GetEntryMetadataIfExists":     "get_entry_metadata_if_exists",
-            "GetEntryMetadataIfNotNull":    "get_entry_metadata_if_not_null",
-            "GetEntryMetadataTree":         "get_entry_metadata_tree",
-            "GetEntryMetadataTreeIfExists": "get_entry_metadata_tree_if_exists",
-            "GetEntryMinute":	              "get_entry_minute",
-            "GetEntryMonth":	              "get_entry_month",
-            "GetEntryPath":	                "get_entry_path",
-            "GetEntryTitle":	              "get_entry_title",
-            "GetEntryToC":                  "get_entry_toc",
-            "GetEntryYear":	                "get_entry_year",
-            "GetFlattenedEntryCategories":	"get_flattened_entry_categories",
-            "IfEntryMetadataIsTrue":	      "if_entry_metadata_is_true",
-        },
         "blog": {
-            "ForBlogArchives":	            "for_blog_archives",
-            "ForBlogMetadata":              "for_blog_metadata",
-            "ForBlogMetadataIfExists":      "for_blog_metadata_if_exists",
-            "ForEntriesSet":	              "for_entries_set",
-            "GetAuthorDescription":	        "get_author_description",
-            "GetAuthorEmail":               "get_author_email",
-            "GetAuthorName":	              "get_author_name",
-            "GetBlogCategoriesTree":	      "get_blog_categories_tree",
-            "GetBlogDescription":	          "get_blog_description",
-            "GetBlogLanguage":	            "get_blog_language",
-            "GetBlogLicense":	              "get_blog_license",
-            "GetBlogMetadata":	            "get_blog_metadata",
-            "GetBlogMetadataIfExists":	    "get_blog_metadata_if_exists",
-            "GetBlogMetadataIfNotNull":	    "get_blog_metadata_if_not_null",
-            "GetBlogMetadataTree":          "get_blog_metadata_tree",
-            "GetBlogMetadataTreeIfExists":  "get_blog_metadata_tree_if_exists",
-            "GetBlogName":	                "get_blog_name",
-            "GetBlogURL":	                  "get_blog_url",
-            "GetChapterAttributeByIndex" :  "get_chapter_attribute_by_index",
-            "GetChapters" :                 "get_chapters",
-            "GetEntryAttributeByID" :       "get_entry_attribute_by_id",
-            "GetFlattenedBlogCategories":	  "get_flattened_blog_categories",
-            "GetRootPage":	                "get_root_page",
-            "GetGenerationTimestamp":	      "get_generation_timestamp",
-            "IfAtomEnabled":	              "if_atom_enabled",
-            "IfBlogMetadataIsTrue":	        "if_blog_metadata_is_true",
-            "IfCategories":	                "if_categories",
-            "IfChapters":	                  "if_chapters",
-            "IfFeedsEnabled":	              "if_feeds_enabled",
-            "IfInfiniteScrollEnabled":	      "if_infinite_scroll_enabled",
-            "IfRSSEnabled":	                "if_rss_enabled",
-            "RangeEntriesByID":             "range_entries_by_id",
+            "CherryPickBlogMetadata":                 "cherry_pick_blog_metadata",
+            "CherryPickBlogMetadataIfExists":         "cherry_pick_blog_metadata_if_exists",
+            "ForBlogArchives":	                      "for_blog_archives",
+            "ForBlogMetadata":                        "for_blog_metadata",
+            "ForBlogMetadataIfExists":                "for_blog_metadata_if_exists",
+            "ForEntriesSet":	                        "for_entries_set",
+            "GetAuthorDescription":	                  "get_author_description",
+            "GetAuthorEmail":                         "get_author_email",
+            "GetAuthorName":	                        "get_author_name",
+            "GetBlogCategoriesTree":	                "get_blog_categories_tree",
+            "GetBlogCategoriesTreeFromBranches":      "get_blog_categories_tree_from_branches",
+            "GetBlogDescription":	                    "get_blog_description",
+            "GetBlogLanguage":	                      "get_blog_language",
+            "GetBlogLicense":	                        "get_blog_license",
+            "GetBlogMetadata":	                      "get_blog_metadata",
+            "GetBlogMetadataIfExists":	              "get_blog_metadata_if_exists",
+            "GetBlogMetadataIfNotNull":	              "get_blog_metadata_if_not_null",
+            "GetBlogMetadataTree":                    "get_blog_metadata_tree",
+            "GetBlogMetadataTreeIfExists":            "get_blog_metadata_tree_if_exists",
+            "GetBlogName":	                          "get_blog_name",
+            "GetBlogURL":	                            "get_blog_url",
+            "GetChapterAttributeByIndex" :            "get_chapter_attribute_by_index",
+            "GetChapters" :                           "get_chapters",
+            "GetEntryAttributeByID" :                 "get_entry_attribute_by_id",
+            "GetFlattenedBlogCategories":	            "get_flattened_blog_categories",
+            "GetFlattenedBlogCategoriesFromBranches":	"get_flattened_blog_categories_from_branches",
+            "GetRootPage":	                          "get_root_page",
+            "GetGenerationTimestamp":	                "get_generation_timestamp",
+            "IfAtomEnabled":	                        "if_atom_enabled",
+            "IfBlogMetadataIsTrue":	                  "if_blog_metadata_is_true",
+            "IfCategories":	                          "if_categories",
+            "IfChapters":	                            "if_chapters",
+            "IfFeedsEnabled":	                        "if_feeds_enabled",
+            "IfInfiniteScrollEnabled":	                "if_infinite_scroll_enabled",
+            "IfRSSEnabled":	                          "if_rss_enabled",
+            "RangeEntriesByID":                       "range_entries_by_id",
+        },
+        "entries" : { 
+            "CherryPickEntryMetadata":                  "cherry_pick_entry_metadata",
+            "CherryPickEntryMetadataIfExists":          "cherry_pick_entry_metadata_if_exists",
+            "ForEntryAuthors":	                        "for_entry_authors",
+            "ForEntryMetadata":	                        "for_entry_metadata",
+            "ForEntryMetadataIfExists":	                "for_entry_metadata_if_exists",   
+            "GetEntryArchivePath":	                    "get_entry_archive_path",
+            "GetEntryCategoriesTree":	                  "get_entry_categories_tree",
+            "GetEntryCategoriesTreeFromBranches":	      "get_entry_categories_tree_from_branches",
+            "GetEntryChapterLevel":                     "get_entry_chapter_level",
+            "GetEntryChapterPath":                      "get_entry_chapter_path",
+            "GetEntryDate":	                            "get_entry_date",
+            "GetEntryDay":	                            "get_entry_day",
+            "GetEntryHour":	                            "get_entry_hour",
+            "GetEntryID":	                              "get_entry_id",
+            "GetEntryMetadata":	                        "get_entry_metadata",
+            "GetEntryMetadataIfExists":                 "get_entry_metadata_if_exists",
+            "GetEntryMetadataIfNotNull":                "get_entry_metadata_if_not_null",
+            "GetEntryMetadataTree":                     "get_entry_metadata_tree",
+            "GetEntryMetadataTreeIfExists":             "get_entry_metadata_tree_if_exists",
+            "GetEntryMinute":	                          "get_entry_minute",
+            "GetEntryMonth":	                          "get_entry_month",
+            "GetEntryPath":	                            "get_entry_path",
+            "GetEntryTitle":	                          "get_entry_title",
+            "GetEntryToC":                              "get_entry_toc",
+            "GetEntryYear":	                            "get_entry_year",
+            "GetFlattenedEntryCategories":	            "get_flattened_entry_categories",
+            "GetFlattenedEntryCategoriesFromBranches":	"get_flattened_entry_categories_from_branches",
+            "IfEntryMetadataIsTrue":	                  "if_entry_metadata_is_true",
         },
         "extra": { # Loaded from function localy imported
             "Audio":	                  "venc3.patterns.theme.get_audio",
             "CodeHighlight":	          "venc3.patterns.third_party_wrapped_features.pygmentize.highlight",
             "CodeHighlightInclude":	    "venc3.patterns.third_party_wrapped_features.pygmentize.highlight_include",
             "DisableMarkup":	          "venc3.patterns.non_contextual.disable_markup",
             "Escape":                   "venc3.patterns.non_contextual.escape",
-            "GetEmbedContent":	           "venc3.patterns.third_party_wrapped_features.oembed.wrapper_embed_content",
+            "GetEmbedContent":	        "venc3.patterns.third_party_wrapped_features.oembed.wrapper_embed_content",
             "GetVenCVersion":	          "venc3.patterns.non_contextual.get_venc_version",
             "HTML":                     "venc3.patterns.non_contextual.html",
             "IncludeFile":	            "venc3.patterns.non_contextual.include_file",
             "IncludeFileIfExists":	    "venc3.patterns.non_contextual.include_file_if_exists",
             "Kroki":	                  "venc3.patterns.third_party_wrapped_features.kroki.kroki",
             "KrokiFromFile":	          "venc3.patterns.third_party_wrapped_features.kroki.kroki_from_file",
             "Latex2MathML":	            "venc3.patterns.third_party_wrapped_features.latex2mathml.latex_2_mathml",
+            "SetBackgroundColor":	      "venc3.patterns.non_contextual.set_background_color",
             "SetColor":	                "venc3.patterns.non_contextual.set_color",
             "SetStyle":	                "venc3.patterns.non_contextual.set_style",
             "Table":	                  "venc3.patterns.non_contextual.table",
             "Video":	                  "venc3.patterns.theme.get_video",
         },
     }
```

### Comparing `VenC-3.1.1/venc3/patterns/processor.py` & `VenC-3.2.0/venc3/patterns/processor.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/patterns/theme.py` & `VenC-3.2.0/venc3/patterns/theme.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/patterns/third_party_wrapped_features/kroki.py` & `VenC-3.2.0/venc3/patterns/third_party_wrapped_features/kroki.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,8 +54,8 @@
                 with open("extra/"+filename,"wb") as f:
                     f.write(content)
                         
             except Exception as e:
                 from venc3.exceptions import VenCException
                 raise VenCException(("exception_place_holder", str(e)), pattern)
               
-    return "<img class=\"__VENC_KROKI__\" src=\"\x1a"+filename+"\">"
+    return "<img class=\"__VENC_KROKI__\" src=\"\x1a/"+filename+"\">"
```

### Comparing `VenC-3.1.1/venc3/patterns/third_party_wrapped_features/latex2mathml.py` & `VenC-3.2.0/venc3/patterns/third_party_wrapped_features/latex2mathml.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/patterns/third_party_wrapped_features/oembed.py` & `VenC-3.2.0/venc3/patterns/third_party_wrapped_features/oembed.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/patterns/third_party_wrapped_features/pygmentize.py` & `VenC-3.2.0/venc3/patterns/third_party_wrapped_features/pygmentize.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             if key not in extra or self._override:    
                 stream = open(os.getcwd()+"/extra/"+key,'w')
                 stream.write(self.includes[key])
 
 def get_style_sheets(pattern):
     output = str()
     for filename in code_highlight.includes.keys():
-        output += "<link rel=\"stylesheet\" href=\"\x1a"+filename+"\" type=\"text/css\" >\n"
+        output += "<link rel=\"stylesheet\" href=\"\x1a/"+filename+"\" type=\"text/css\" >\n"
 
     return output
         
 def highlight_include(pattern, langage, display_line_numbers, filename):
     from venc3.patterns.non_contextual import include_file
     string = include_file(pattern, filename, [])
     return highlight(pattern, langage, display_line_numbers, string)
```

### Comparing `VenC-3.1.1/venc3/prompt.py` & `VenC-3.2.0/venc3/prompt.py`

 * *Files identical despite different names*

### Comparing `VenC-3.1.1/venc3/threads/__init__.py` & `VenC-3.2.0/venc3/threads/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /usr/bin/env python3
 
-#    Copyright 2016, 2022 Denis Salem
+#    Copyright 2016, 2024 Denis Salem
 #
 #    This file is part of VenC.
 #
 #    VenC is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
@@ -111,34 +111,41 @@
         '''value'''
         if len(self.thread_name):
             return string1.format(**{"value":self.thread_name})
         
         else:
             return string2
                 
-            
     # Must be called in child class
     def organize_entries(self, entries):
         self.pages = list()
         for i in range(0, ceil(len(entries)/self.entries_per_page)):
             self.pages.append(
                 entries[i*self.entries_per_page:(i+1)*self.entries_per_page]
             )
 
         self.pages_count = len(self.pages)
 
+    def get_last_entry_timestamp(self, pattern, time_format):
+        from venc3.exceptions import VenCException
+        raise VenCException(
+            ("you_cannot_use_this_pattern_here", "GetLastEntryTimestamp", pattern.root.context),
+            pattern
+        )
+        
     # Must be called in child class
     def get_next_page(self, pattern, string):
         '''page_number,entry_id,entry_title,path'''
         if self.current_page < self.pages_count - 1:
             params = {
                 "page_number" : str(self.current_page + 1),
                 "entry_id" : '',
                 "entry_title": '',
-                "path" : ''
+                "path" : '',
+                "chapter": ''
             }
 
             if self.in_thread:
                 params["path"] = self.filename.format(**params)
 
             else:
                 params["path"] = self.current_entry.next_entry.path
@@ -162,15 +169,16 @@
     def get_previous_page(self, pattern, string):
         '''page_number,entry_id,entry_title,path'''
         if self.current_page > 0:
             params = {
                 "page_number" : str(self.current_page - 1) if self.current_page - 1 != 0 else '',
                 "entry_id" : '',
                 "entry_title": '',
-                "path" : ''
+                "path" : '',
+                "chapter" : ''
             }
 
             if self.in_thread:
                 params["path"] = self.filename.format(**params)
 
             else:
                     params["entry_id"] = self.current_entry.previous_entry.id
```

### Comparing `VenC-3.1.1/venc3/threads/archives.py` & `VenC-3.2.0/venc3/threads/archives.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 from venc3.helpers import quirk_encoding
 from venc3.threads import Thread
 
 class ArchivesThread(Thread):
     def __init__(self):
         from venc3.l10n import messages
         super().__init__(messages.export_archives)
-        self.filename = self.datastore.blog_configuration["path"]["index_file_name"]
-        self.sub_folders = self.datastore.blog_configuration["path"]["archives_sub_folders"]
+        self.filename = self.datastore.blog_configuration["paths"]["index_file_name"]
+        self.sub_folders = self.datastore.blog_configuration["paths"]["archives_sub_folders"]
         if len(self.sub_folders) and self.sub_folders[-1] != '/':
             self.sub_folders += '/'
             
-        self.relative_origin = str("../"+''.join([ "../" for p in self.sub_folders.split('/') if p != ''])).replace("//",'/')
+        self.relative_origin = str(".."+'/'.join([ "/.." for p in self.sub_folders.split('/') if p != ''])).replace("//",'/')
         self.in_thread = True
         self.thread_has_feeds = False
 
     def if_in_archives(self, node, string1, string2=''):
         return string1.strip()
 
     def setup_archive_context(self, i, len_archives):
```

### Comparing `VenC-3.1.1/venc3/threads/categories.py` & `VenC-3.2.0/venc3/threads/categories.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 from venc3.helpers import quirk_encoding
 from venc3.threads import Thread
 
 class CategoriesThread(Thread):
     def __init__(self):
         from venc3.l10n import messages
         super().__init__(messages.export_categories)
-        self.filename = self.datastore.blog_configuration["path"]["index_file_name"]
-        self.sub_folders = self.datastore.blog_configuration["path"]["categories_sub_folders"]
-        self.export_path = "blog/"+self.sub_folders
+        self.filename = self.datastore.blog_configuration["paths"]["index_file_name"]
+        self.sub_folders = self.datastore.blog_configuration["paths"]["categories_sub_folders"]
+        self.export_path = "blog/"+self.sub_folders+'/'
         self.category_value = ""
         self.relative_origin = ""
         self.in_thread = True
         self.thread_has_feeds = True
 
         self.disable_rss_feed = self.datastore.blog_configuration["disable_rss_feed"]
         self.disable_atom_feed = self.datastore.blog_configuration["disable_atom_feed"]
@@ -73,15 +73,15 @@
         from venc3.prompt import notify
         notify(("exception_place_holder", node.value+"..."), prepend=self.indentation_level+tree_special_char+"─ ")
 
         export_path = self.export_path
         category_value = self.category_value
         self.category_value += node.value+'/'
         self.export_path += quirk_encoding(node.value)+'/'
-        self.relative_origin = ''.join([ '../' for f in self.export_path.split("/")[1:] if f != '' ]).replace("//",'/')
+        self.relative_origin = '/'.join([ '..' for f in self.export_path.split("/")[1:] if f != '' ]).replace("//",'/')
 
         try:
             os.makedirs(self.export_path)
 
         except FileExistsError:
             pass
```

### Comparing `VenC-3.1.1/venc3/threads/chapters.py` & `VenC-3.2.0/venc3/threads/chapters.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,21 +21,75 @@
 
 from venc3.threads import Thread
 
 class ChaptersThread(Thread):
     def __init__(self):
         from venc3.l10n import messages
         super().__init__(messages.export_chapters)
-        self.filename = self.datastore.blog_configuration["path"]["index_file_name"]
+        self.filename = self.datastore.blog_configuration["paths"]["index_file_name"]
         self.entries_per_page = self.datastore.blog_configuration["entries_per_pages"]
-        self.folder_name = self.datastore.blog_configuration["path"]["chapter_directory_name"]
-        self.sub_folders = self.datastore.blog_configuration["path"]["chapters_sub_folders"]
+        self.folder_name = self.datastore.blog_configuration["paths"]["chapter_directory_name"]
+        self.sub_folders = self.datastore.blog_configuration["paths"]["chapters_sub_folders"]
         self.relative_origin = str(''.join([ "../" for p in self.sub_folders.split('/') if p != ''])).replace("//",'/')
         self.in_thread = True
         self.thread_has_feeds = False
+        self.chapters_list = [ [int(v) for v in key.split('.')] for key in self.datastore.raw_chapters.keys() ]
+        self.chapters_list.sort()
+        self.chapters_list = ['.'.join([str(v) for v in l]) for l in self.chapters_list]
+
+    def get_next_page(self, pattern, string): #TODO : Any chance to factorize this in parent class ?
+        '''page_number,entry_id,entry_title,path,chapter'''
+        index = self.chapters_list.index(self.pages[self.current_page][-1].chapter.index) + 1
+        if index  < len(self.chapters_list):
+            entry = self.datastore.raw_chapters[self.chapters_list[index]]
+            params = {
+                "page_number" : '', #TODO: not implemented yet
+                "entry_id" : entry.id,
+                "entry_title": entry.title,
+                "path" : entry.chapter.path,
+                "chapter" : entry.chapter.index
+            }
+
+            try:
+                return string.format(**params)
+                
+            except KeyError as e:
+                from venc3.exceptions import VenCException
+                raise VenCException(
+                    ("unknown_contextual", str(e)[1:-1]),
+                    pattern
+                )
+
+        else:
+            return str()
+            
+    def get_previous_page(self, pattern, string): #TODO : Any chance to factorize this in parent class ?
+        '''page_number,entry_id,entry_title,path,chapter'''
+        index = self.chapters_list.index(self.pages[self.current_page][0].chapter.index) - 1
+        if index >= 0:
+            entry = self.datastore.raw_chapters[self.chapters_list[index]]
+            params = {
+                "page_number" : '', #TODO: not implemented yet
+                "entry_id" : entry.id,
+                "entry_title": entry.title,
+                "path" : entry.chapter.path,
+                "chapter" : entry.chapter.index
+            }
+            try:
+                return string.format(**params)
+
+            except KeyError as e:
+                from venc3.exceptions import VenCException
+                raise VenCException(
+                    ("unknown_contextual", str(e)[1:-1]),
+                    pattern
+                )
+                
+        else:
+            return str()
 
     def if_in_first_page(self, node, string1, string2=''):
         return string2.strip()
     
     def if_in_last_page(self, node, string1, string2=''):
         return string2.strip()
         
@@ -55,36 +109,35 @@
         folder_name = quirk_encoding(
             self.folder_name.format(**{
               "chapter_name" : entry.title,
               "chapter_index": node.index
           })
         )
         self.export_path = "blog/"+self.sub_folders+'/'+folder_name
-        self.relative_origin = ''.join([ '../' for f in self.export_path.split("/")[1:] if f != '' ])
+        self.relative_origin = '/'.join([ '..' for f in self.export_path.split("/")[1:] if f != '' ]).replace('//','/')
 
         try:
             os.makedirs(self.export_path)
 
         except FileExistsError:
             pass
             
         return (node)
     
-    def extract_sub_chapters(self, sub_chapters):
+    def extract_sub_chapters(self, sub_chapters): # TODO : Investigate yielding usage here for better efficiency
         output = []
         output_append = output.append
         for c in sub_chapters:
             output_append(self.datastore.entries[c.entry_index])
             if len(c.sub_chapters):
                 for sc_entries in self.extract_sub_chapters(c.sub_chapters):
                     output_append(sc_entries)
         
         return output
-        
-        
+            
     def do(self, top=None):          
         if top == None:
             top = self.datastore.chapters_index
             
         for chapter_index in range(0, len(top)):
             chapter = top[chapter_index]
             entry = self.datastore.entries[chapter.entry_index]
```

### Comparing `VenC-3.1.1/venc3/threads/entries.py` & `VenC-3.2.0/venc3/threads/entries.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     def __init__(self):
         from venc3.l10n import messages
         super().__init__(messages.export_single_entries)
         self.entries_per_page = 1 #override value
         self.organize_entries(self.datastore.entries)
         self.current_entry_index=-1
         self.entries = self.datastore.entries
-        self.filename = self.datastore.blog_configuration["path"]["entry_file_name"]
-        self.sub_folders = self.datastore.blog_configuration["path"]["entries_sub_folders"]
+        self.filename = self.datastore.blog_configuration["paths"]["entry_file_name"]
+        self.sub_folders = self.datastore.blog_configuration["paths"]["entries_sub_folders"]
         self.export_path = "blog/"+self.sub_folders
-        self.relative_origin = str(''.join([ "../" for p in self.sub_folders.split('/') if p != ''])).replace("//",'/')
+        self.relative_origin = str('/'.join([ ".." for p in self.sub_folders.split('/') if p != ''])).replace("//",'/')
         self.in_thread = False
         self.thread_has_feeds = False
         self.known_written_path = []
 
     def format_filename(self, value=None): #value ignored
         try:
             return self.filename.format(**{
@@ -115,15 +115,15 @@
         export_path = quirk_encoding(
             self.export_path.format(**{
                     'entry_id': self.current_entry.id,
                     'entry_title': self.current_entry.title
             })
         )
         self.thread_name = self.current_entry.title
-        self.relative_origin = str(''.join([ "../" for p in export_path.split('/')[1:] if p != ''])).replace("//",'/')
+        self.relative_origin = str('/'.join([ ".." for p in export_path.split('/')[1:] if p != ''])).replace("//",'/')
         os.makedirs(export_path, exist_ok=True)
 
 
     def write_file(self, output, file_id):
         export_path = quirk_encoding(self.export_path.format(**{
             'entry_id': self.current_entry.id,
             'entry_title': self.current_entry.title
```

### Comparing `VenC-3.1.1/venc3/threads/feed.py` & `VenC-3.2.0/venc3/threads/feed.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /usr/bin/env python3
 
-#    Copyright 2016, 2022 Denis Salem
+#    Copyright 2016, 2024 Denis Salem
 #
 #    This file is part of VenC.
 #
 #    VenC is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
@@ -27,22 +27,25 @@
         self.header = getattr(self.theme, feed_type+"_header")
         self.entry = getattr(self.theme, feed_type+"_entry")
         self.context_header = feed_type+"Header.xml"
         self.context_footer = feed_type+"Footer.xml"
         self.column_opening = ''
         self.column_closing = ''
         self.columns_number = 1
-        self.filename = self.datastore.blog_configuration["path"][feed_type+"_file_name"]
+        self.filename = self.datastore.blog_configuration["paths"][feed_type+"_file_name"]
         self.entries_per_page = self.datastore.blog_configuration["feed_length"]
         self.in_thread = True
         self.content_type = feed_type
 
     def do(self, entries, export_path, relative_origin):
+        self.last_entry = entries[-1]
         self.export_path = export_path
         self.relative_origin = relative_origin
         self.organize_entries(entries)
         super().do()
 
     def if_in_feed(self, node, string1, string2=''):
         return string1.strip()
             
-
+    def get_last_entry_timestamp(self, pattern, time_format):
+        import datetime
+        return datetime.datetime.strftime(self.last_entry.date, time_format)
```

### Comparing `VenC-3.1.1/venc3/threads/main.py` & `VenC-3.2.0/venc3/threads/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         else:
             self.organize_entries([
                 entry for entry in datastore.get_entries(
                     datastore.blog_configuration["reverse_thread_order"]
                 )
             ])
 
-        self.filename = self.datastore.blog_configuration["path"]["index_file_name"]
-        self.relative_origin = str()
+        self.filename = self.datastore.blog_configuration["paths"]["index_file_name"]
+        self.relative_origin = ""
         self.export_path = "blog/"
         self.in_thread = True
         self.thread_has_feeds = True
 
             
     def get_feed_entries(self):
         entries = []
```

