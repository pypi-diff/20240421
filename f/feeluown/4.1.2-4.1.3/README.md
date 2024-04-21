# Comparing `tmp/feeluown-4.1.2.tar.gz` & `tmp/feeluown-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feeluown-4.1.2.tar", last modified: Wed Mar 13 03:00:52 2024, max compression
+gzip compressed data, was "feeluown-4.1.3.tar", last modified: Sun Apr 21 10:24:43 2024, max compression
```

## Comparing `feeluown-4.1.2.tar` & `feeluown-4.1.3.tar`

### file list

```diff
@@ -1,284 +1,286 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:52.015683 feeluown-4.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-13 03:00:50.000000 feeluown-4.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-03-13 03:00:52.015683 feeluown-4.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-03-13 03:00:50.000000 feeluown-4.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:51.979683 feeluown-4.1.2/feeluown/
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      158 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:51.979683 feeluown-4.1.2/feeluown/app/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/app/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/app/cli_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/app/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/app/gui_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/app/mixed_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/app/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/app/once_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/app/server_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:51.979683 feeluown-4.1.2/feeluown/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/cli/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4208 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (127)    13819 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:51.983683 feeluown-4.1.2/feeluown/entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/entry_points/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/entry_points/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/entry_points/run_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/entry_points/run_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/excs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:51.983683 feeluown-4.1.2/feeluown/fuoexec/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/fuoexec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/fuoexec/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/fuoexec/fuoexec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/fuoexec/signal_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:51.983683 feeluown-4.1.2/feeluown/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:51.971683 feeluown-4.1.2/feeluown/gui/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:51.987683 feeluown-4.1.2/feeluown/gui/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/icons/already_download.png
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/icons/already_downloaded_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/icons/cur_playlist.png
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/icons/cur_playlist_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/icons/download.png
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/icons/download_dark.png
--rwxr-xr-x   0 runner    (1001) docker     (127)   303153 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/icons/feeluown.icns
--rw-r--r--   0 runner    (1001) docker     (127)   112526 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/icons/feeluown.ico
--rw-r--r--   0 runner    (1001) docker     (127)    35773 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/icons/feeluown.png
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/icons/like.png
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/icons/like_checked.png
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/icons/like_checked_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/icons/like_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/icons/tray-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)     7712 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/icons/tray-light.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:51.987683 feeluown-4.1.2/feeluown/gui/assets/themes/
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/themes/common.qss
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/themes/dark.qss
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/themes/light.qss
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/assets/themes/macos_dark.colors
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/base_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:51.991683 feeluown-4.1.2/feeluown/gui/components/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/components/avatar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/components/btns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/components/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/components/line_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/components/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/components/nowplaying.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/components/player_playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/components/player_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/components/playlist_btn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/components/song_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/components/volume_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/drawers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20550 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/hotkey.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/mimedata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:51.991683 feeluown-4.1.2/feeluown/gui/page_containers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/page_containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/page_containers/scroll_area.py
--rw-r--r--   0 runner    (1001) docker     (127)    20407 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/page_containers/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:51.991683 feeluown-4.1.2/feeluown/gui/pages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/pages/coll_mixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/pages/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/pages/my_fav.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/pages/provider_home.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/pages/recently_played.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/pages/recommendation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/pages/recommendation_daily_songs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/pages/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    13654 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/pages/song_explore.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/pages/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/provider_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/tips.py
--rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/tray.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:51.995683 feeluown-4.1.2/feeluown/gui/uimain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/uimain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/uimain/floating_box.py
--rw-r--r--   0 runner    (1001) docker     (127)    14382 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/uimain/lyric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/uimain/nowplaying_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/uimain/page_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/uimain/player_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/uimain/playlist_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    12831 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/uimain/sidebar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/uimain/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:51.995683 feeluown-4.1.2/feeluown/gui/uimodels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/uimodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/uimodels/my_music.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/uimodels/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/uimodels/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:51.999683 feeluown-4.1.2/feeluown/gui/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/accordion.py
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/comment_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/cover_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/frameless.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/header.py
--rw-r--r--   0 runner    (1001) docker     (127)    16619 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/img_card_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/lyric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/magicbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/messageline.py
--rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/mpv_.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/my_music.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/playlist_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/progress_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/selfpaint_btn.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/separator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/size_grip.py
--rw-r--r--   0 runner    (1001) docker     (127)    10285 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/song_minicard_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    27444 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/songs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/statusline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:51.999683 feeluown-4.1.2/feeluown/gui/widgets/statusline_items/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/statusline_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/statusline_items/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/statusline_items/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/tabbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/table_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/textbtn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/textlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/volume_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/gui/widgets/weblogin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:52.003683 feeluown-4.1.2/feeluown/library/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/library/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/library/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/library/excs.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/library/flags.py
--rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/library/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/library/model_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/library/model_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/library/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/library/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/library/provider_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/library/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:52.003683 feeluown-4.1.2/feeluown/local/
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/local/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/local/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/local/provider_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/local/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/local/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    79466 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/mpv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:52.003683 feeluown-4.1.2/feeluown/nowplaying/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/nowplaying/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:52.003683 feeluown-4.1.2/feeluown/nowplaying/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/nowplaying/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/nowplaying/linux/introspect.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/nowplaying/linux/mpris2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/nowplaying/macos.py
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/nowplaying/nowplaying.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:52.007683 feeluown-4.1.2/feeluown/player/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/player/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/player/base_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/player/delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/player/fm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/player/lyric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/player/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/player/mpvplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    25849 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/player/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/player/radio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/player/recently_played.py
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:52.007683 feeluown-4.1.2/feeluown/pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/pyinstaller/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/pyinstaller/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:52.007683 feeluown-4.1.2/feeluown/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/serializers/_plain_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/serializers/json_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/serializers/model_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/serializers/objs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/serializers/plain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/serializers/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/serializers/typename.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:52.007683 feeluown-4.1.2/feeluown/server/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/data_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:52.007683 feeluown-4.1.2/feeluown/server/dslv1/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/dslv1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/dslv1/codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/dslv1/lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/dslv1/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/dslv2.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/excs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:52.011683 feeluown-4.1.2/feeluown/server/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/handlers/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/handlers/excs.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/handlers/exec_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/handlers/handle.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/handlers/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/handlers/player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/handlers/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/handlers/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/handlers/set_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/handlers/show.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/handlers/status.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/handlers/sub.py
--rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:52.011683 feeluown-4.1.2/feeluown/server/pubsub/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/pubsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/pubsub/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/pubsub/publishers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:52.011683 feeluown-4.1.2/feeluown/server/rpc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/server/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:52.011683 feeluown-4.1.2/feeluown/uimodels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/uimodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/uimodels/my_music.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/uimodels/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/uimodels/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:52.015683 feeluown-4.1.2/feeluown/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/utils/aio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/utils/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/utils/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/utils/lang.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/utils/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12691 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/utils/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/utils/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    13634 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/utils/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/utils/typing_.py
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    54535 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/utils/yt_dlp_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:52.015683 feeluown-4.1.2/feeluown/webserver/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/webserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/webserver/jsonrpc_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-03-13 03:00:50.000000 feeluown-4.1.2/feeluown/webserver/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 03:00:51.979683 feeluown-4.1.2/feeluown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-03-13 03:00:51.000000 feeluown-4.1.2/feeluown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-03-13 03:00:51.000000 feeluown-4.1.2/feeluown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 03:00:51.000000 feeluown-4.1.2/feeluown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-13 03:00:51.000000 feeluown-4.1.2/feeluown.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-13 03:00:51.000000 feeluown-4.1.2/feeluown.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-13 03:00:51.000000 feeluown-4.1.2/feeluown.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-13 03:00:52.015683 feeluown-4.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-03-13 03:00:50.000000 feeluown-4.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.329369 feeluown-4.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-21 10:24:42.000000 feeluown-4.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-21 10:24:43.329369 feeluown-4.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-21 10:24:42.000000 feeluown-4.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.297368 feeluown-4.1.3/feeluown/
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      158 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.297368 feeluown-4.1.3/feeluown/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/cli_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/gui_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/mixed_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/once_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/app/server_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.297368 feeluown-4.1.3/feeluown/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/cli/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4208 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.297368 feeluown-4.1.3/feeluown/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/entry_points/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/entry_points/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/entry_points/run_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/entry_points/run_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/excs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.297368 feeluown-4.1.3/feeluown/fuoexec/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/fuoexec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/fuoexec/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/fuoexec/fuoexec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/fuoexec/signal_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.301368 feeluown-4.1.3/feeluown/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.293368 feeluown-4.1.3/feeluown/gui/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.305369 feeluown-4.1.3/feeluown/gui/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/already_download.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/already_downloaded_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/cur_playlist.png
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/cur_playlist_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/download.png
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/download_dark.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)   303153 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/feeluown.icns
+-rw-r--r--   0 runner    (1001) docker     (127)   112526 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/feeluown.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    35773 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/feeluown.png
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/like.png
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/like_checked.png
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/like_checked_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/like_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/tray-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7712 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/icons/tray-light.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.305369 feeluown-4.1.3/feeluown/gui/assets/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/themes/common.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/themes/dark.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/themes/light.qss
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/assets/themes/macos_dark.colors
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/base_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.305369 feeluown-4.1.3/feeluown/gui/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/avatar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/btns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/line_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/nowplaying.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/player_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/player_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/playlist_btn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/song_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/components/volume_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/drawers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20611 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/hotkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/mimedata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.305369 feeluown-4.1.3/feeluown/gui/page_containers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/page_containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/page_containers/scroll_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20407 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/page_containers/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.309368 feeluown-4.1.3/feeluown/gui/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/coll_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/homepage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/my_fav.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/provider_home.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/recently_played.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/recommendation_daily_songs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13654 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/song_explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/pages/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/provider_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/tips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/tray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.309368 feeluown-4.1.3/feeluown/gui/uimain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/floating_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15321 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/lyric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/nowplaying_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12168 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/page_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/player_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/playlist_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimain/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.309368 feeluown-4.1.3/feeluown/gui/uimodels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimodels/my_music.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimodels/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/uimodels/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.317369 feeluown-4.1.3/feeluown/gui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/accordion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/comment_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/cover_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/frameless.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16619 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/img_card_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/lyric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/magicbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/messageline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/mpv_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/my_music.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/playlist_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/progress_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/selfpaint_btn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/separator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/size_grip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/song_minicard_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27444 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/songs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/statusline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.317369 feeluown-4.1.3/feeluown/gui/widgets/statusline_items/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/statusline_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/statusline_items/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/statusline_items/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/tabbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/table_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/textbtn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/textlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/volume_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/gui/widgets/weblogin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.317369 feeluown-4.1.3/feeluown/library/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/excs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/model_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/model_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10825 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/provider_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/library/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.317369 feeluown-4.1.3/feeluown/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/local/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/local/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/local/provider_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/local/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/local/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79978 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/mpv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.321369 feeluown-4.1.3/feeluown/nowplaying/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/nowplaying/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.321369 feeluown-4.1.3/feeluown/nowplaying/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/nowplaying/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/nowplaying/linux/introspect.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/nowplaying/linux/mpris2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/nowplaying/macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/nowplaying/nowplaying.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.321369 feeluown-4.1.3/feeluown/player/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/base_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/fm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/lyric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/mpvplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25849 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/player/recently_played.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.321369 feeluown-4.1.3/feeluown/pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/pyinstaller/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/pyinstaller/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.321369 feeluown-4.1.3/feeluown/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/_plain_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/json_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/model_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/objs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/plain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/serializers/typename.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.325369 feeluown-4.1.3/feeluown/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/data_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.325369 feeluown-4.1.3/feeluown/server/dslv1/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/dslv1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/dslv1/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/dslv1/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/dslv1/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/dslv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/excs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.325369 feeluown-4.1.3/feeluown/server/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/excs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/exec_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/set_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/handlers/sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.329369 feeluown-4.1.3/feeluown/server/pubsub/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/pubsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/pubsub/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/pubsub/publishers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.329369 feeluown-4.1.3/feeluown/server/rpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/server/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.329369 feeluown-4.1.3/feeluown/uimodels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/uimodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/uimodels/my_music.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/uimodels/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/uimodels/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.329369 feeluown-4.1.3/feeluown/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/aio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12691 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13634 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/typing_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54535 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/utils/yt_dlp_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.329369 feeluown-4.1.3/feeluown/webserver/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/webserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/webserver/jsonrpc_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-21 10:24:42.000000 feeluown-4.1.3/feeluown/webserver/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:24:43.297368 feeluown-4.1.3/feeluown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-21 10:24:43.000000 feeluown-4.1.3/feeluown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-21 10:24:43.000000 feeluown-4.1.3/feeluown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 10:24:43.000000 feeluown-4.1.3/feeluown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-21 10:24:43.000000 feeluown-4.1.3/feeluown.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-21 10:24:43.000000 feeluown-4.1.3/feeluown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 10:24:43.000000 feeluown-4.1.3/feeluown.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-21 10:24:43.333369 feeluown-4.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-21 10:24:42.000000 feeluown-4.1.3/setup.py
```

### Comparing `feeluown-4.1.2/LICENSE` & `feeluown-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/PKG-INFO` & `feeluown-4.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feeluown
-Version: 4.1.2
+Version: 4.1.3
 Summary: *nix music player
 Home-page: https://github.com/feeluown/FeelUOwn
 Author: feeluown
 Author-email: yinshaowen241@gmail.com
 License: GPL-3.0
 Description: ## FeelUOwn - feel your own
```

### Comparing `feeluown-4.1.2/README.md` & `feeluown-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/__init__.py` & `feeluown-4.1.3/feeluown/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 import logging.config
 
 from .consts import LOG_FILE
 
 
-__version__ = '4.1.2'
+__version__ = '4.1.3'
 
 
 dict_config = {
     'version': 1,
     'disable_existing_loggers': False,
     'formatters': {
         'standard': {
```

### Comparing `feeluown-4.1.2/feeluown/app/app.py` & `feeluown-4.1.3/feeluown/app/app.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/app/cli_app.py` & `feeluown-4.1.3/feeluown/app/cli_app.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/app/config.py` & `feeluown-4.1.3/feeluown/app/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     config.deffield('VERBOSE', default=0, type_=int, desc='日志详细程度')
     config.deffield('RPC_PORT', default=23333, type_=int, desc='RPC 端口')
     config.deffield('PUBSUB_PORT', default=23334, type_=int, desc='PUBSUB 端口')
     config.deffield('WEB_PORT', default=23332, type_=int, desc='WEB 服务端口')
     config.deffield('ENABLE_WEB_SERVER', default=False, type_=bool)
     config.deffield('MODE', default=0x0000, desc='CLI or GUI 模式')
     config.deffield('THEME', default='auto', desc='auto/light/dark')
+    config.deffield('ENABLE_NEW_HOMEPAGE', default=False, type_=bool)
     config.deffield('MPV_AUDIO_DEVICE', default='auto', desc='MPV 播放设备')
     config.deffield('COLLECTIONS_DIR',  desc='本地收藏所在目录')
     config.deffield('FORCE_MAC_HOTKEY', desc='强制开启 macOS 全局快捷键功能',
                     warn='Will be remove in version 3.0')
     config.deffield('LOG_TO_FILE', desc='将日志输出到文件中')
     config.deffield('AUDIO_SELECT_POLICY', default='hq<>')
     config.deffield('VIDEO_SELECT_POLICY', default='hd<>')
```

### Comparing `feeluown-4.1.2/feeluown/app/gui_app.py` & `feeluown-4.1.3/feeluown/app/gui_app.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/app/server_app.py` & `feeluown-4.1.3/feeluown/app/server_app.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/argparser.py` & `feeluown-4.1.3/feeluown/argparser.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/cli/cli.py` & `feeluown-4.1.3/feeluown/cli/cli.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/cli/install.py` & `feeluown-4.1.3/feeluown/cli/install.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/collection.py` & `feeluown-4.1.3/feeluown/collection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import base64
 import itertools
 import logging
 import os
 from datetime import datetime
-from enum import Enum
 from pathlib import Path
 from typing import Dict, Iterable, List
 
 import tomlkit
 
 from feeluown.consts import COLLECTIONS_DIR
 from feeluown.utils.dispatch import Signal
 from feeluown.library import resolve, reverse, ResolverNotFound, \
-    ResolveFailed, ModelState
+    ResolveFailed, ModelState, CollectionType
 from feeluown.utils.utils import elfhash
 
 logger = logging.getLogger(__name__)
 
 COLL_LIBRARY_IDENTIFIER = 'library'
 COLL_POOL_IDENTIFIER = 'pool'
 # for backward compat, we should never change these filenames
@@ -29,22 +28,18 @@
 TOML_DELIMLF = "+++\n"
 
 
 class CollectionAlreadyExists(Exception):
     pass
 
 
-class CollectionType(Enum):
-    sys_library = 16
-    sys_pool = 13
-
-    mixed = 8
-
-
 class Collection:
+    """
+    TODO: This collection should be moved into local provider.
+    """
 
     def __init__(self, fpath):
         # TODO: 以后考虑添加 identifier 字段，identifier
         # 字段应该尽量设计成可以跨电脑使用
         self.fpath = str(fpath)
         # TODO: 目前还没想好 collection identifier 计算方法，故添加这个函数
         # 现在把 fpath 当作 identifier 使用，但对外透明
```

### Comparing `feeluown-4.1.2/feeluown/config.py` & `feeluown-4.1.3/feeluown/config.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/entry_points/base.py` & `feeluown-4.1.3/feeluown/entry_points/base.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/entry_points/run.py` & `feeluown-4.1.3/feeluown/entry_points/run.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/entry_points/run_app.py` & `feeluown-4.1.3/feeluown/entry_points/run_app.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/excs.py` & `feeluown-4.1.3/feeluown/excs.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/fuoexec/functions.py` & `feeluown-4.1.3/feeluown/fuoexec/functions.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/fuoexec/fuoexec.py` & `feeluown-4.1.3/feeluown/fuoexec/fuoexec.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/fuoexec/signal_manager.py` & `feeluown-4.1.3/feeluown/fuoexec/signal_manager.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/icons/already_download.png` & `feeluown-4.1.3/feeluown/gui/assets/icons/already_download.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/icons/already_downloaded_dark.png` & `feeluown-4.1.3/feeluown/gui/assets/icons/already_downloaded_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/icons/cur_playlist.png` & `feeluown-4.1.3/feeluown/gui/assets/icons/cur_playlist.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/icons/cur_playlist_dark.png` & `feeluown-4.1.3/feeluown/gui/assets/icons/cur_playlist_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/icons/download.png` & `feeluown-4.1.3/feeluown/gui/assets/icons/download.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/icons/download_dark.png` & `feeluown-4.1.3/feeluown/gui/assets/icons/download_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/icons/feeluown.icns` & `feeluown-4.1.3/feeluown/gui/assets/icons/feeluown.icns`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/icons/feeluown.ico` & `feeluown-4.1.3/feeluown/gui/assets/icons/feeluown.ico`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/icons/feeluown.png` & `feeluown-4.1.3/feeluown/gui/assets/icons/feeluown.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/icons/like.png` & `feeluown-4.1.3/feeluown/gui/assets/icons/like.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/icons/like_checked.png` & `feeluown-4.1.3/feeluown/gui/assets/icons/like_checked.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/icons/like_checked_dark.png` & `feeluown-4.1.3/feeluown/gui/assets/icons/like_checked_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/icons/like_dark.png` & `feeluown-4.1.3/feeluown/gui/assets/icons/like_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/icons/tray-dark.png` & `feeluown-4.1.3/feeluown/gui/assets/icons/tray-dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/icons/tray-light.png` & `feeluown-4.1.3/feeluown/gui/assets/icons/tray-light.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/themes/common.qss` & `feeluown-4.1.3/feeluown/gui/assets/themes/common.qss`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/themes/dark.qss` & `feeluown-4.1.3/feeluown/gui/assets/themes/dark.qss`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/themes/light.qss` & `feeluown-4.1.3/feeluown/gui/assets/themes/light.qss`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/assets/themes/macos_dark.colors` & `feeluown-4.1.3/feeluown/gui/assets/themes/macos_dark.colors`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/base_renderer.py` & `feeluown-4.1.3/feeluown/gui/base_renderer.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/browser.py` & `feeluown-4.1.3/feeluown/gui/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,15 @@
         from feeluown.gui.pages.song_explore import render as render_song_explore
         from feeluown.gui.pages.provider_home import render as render_provider_home
         from feeluown.gui.pages.recently_played import render as render_recently_played
         from feeluown.gui.pages.recommendation import render as render_rec
         from feeluown.gui.pages.recommendation_daily_songs import \
             render as render_rec_daily_songs
         from feeluown.gui.pages.my_fav import render as render_my_fav
+        from feeluown.gui.pages.homepage import render as render_homepage
 
         model_prefix = f'{MODEL_PAGE_PREFIX}<provider>'
 
         async def dummy_render(req, *args, **kwargs):
             warnings.warn(f'This route:{req.rule} will be removed.')
 
         urlpatterns = [
@@ -210,12 +211,13 @@
             (f'{model_prefix}/songs/<identifier>/hot_comments', dummy_render),
             (f'{model_prefix}/songs/<identifier>/explore', render_song_explore),
             ('/colls/<identifier>', render_coll_mixed),
             ('/providers/<identifier>', render_provider_home),
             ('/recently_played', render_recently_played),
             ('/search', render_search),
             ('/rec', render_rec),
+            ('/homepage', render_homepage),
             ('/rec/daily_songs', render_rec_daily_songs),
             ('/my_fav', render_my_fav),
         ]
         for url, renderer in urlpatterns:
             self.route(url)(renderer)
```

### Comparing `feeluown-4.1.2/feeluown/gui/components/__init__.py` & `feeluown-4.1.3/feeluown/gui/components/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/components/avatar.py` & `feeluown-4.1.3/feeluown/gui/components/avatar.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/components/btns.py` & `feeluown-4.1.3/feeluown/gui/components/btns.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/components/collections.py` & `feeluown-4.1.3/feeluown/gui/components/collections.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/components/line_song.py` & `feeluown-4.1.3/feeluown/gui/components/line_song.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/components/menu.py` & `feeluown-4.1.3/feeluown/gui/components/menu.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/components/nowplaying.py` & `feeluown-4.1.3/feeluown/gui/components/nowplaying.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/components/player_playlist.py` & `feeluown-4.1.3/feeluown/gui/components/player_playlist.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,17 @@
     SongMiniCardListView,
     SongMiniCardListModel,
 )
 from feeluown.utils.reader import create_reader
 
 
 class PlayerPlaylistModel(SongMiniCardListModel):
-    # FIXME: make this singleton
+    """
+    this is a singleton class (ensured by PlayerPlaylistView)
+    """
 
     def __init__(self, playlist, *args, **kwargs):
         reader = create_reader(playlist.list())
         super().__init__(reader, *args, **kwargs)
 
         self._playlist = playlist
         self._playlist.songs_added.connect(self.on_songs_added)
@@ -43,25 +45,27 @@
             self._items.pop(index + count - 1)
             count -= 1
         self.endRemoveRows()
 
 
 class PlayerPlaylistView(SongMiniCardListView):
 
+    _model = None
+
     def __init__(self, app, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._app = app
 
         self.play_song_needed.connect(self._app.playlist.play_model)
-        self.setModel(
-            PlayerPlaylistModel(
+        if PlayerPlaylistView._model is None:
+            PlayerPlaylistView._model = PlayerPlaylistModel(
                 self._app.playlist,
                 fetch_cover_wrapper(self._app),
             )
-        )
+        self.setModel(PlayerPlaylistView._model)
 
     def contextMenuEvent(self, e):
         index = self.indexAt(e.pos())
         if not index.isValid():
             return
 
         song = index.data(Qt.UserRole)[0]
```

### Comparing `feeluown-4.1.2/feeluown/gui/components/player_progress.py` & `feeluown-4.1.3/feeluown/gui/components/player_progress.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/components/playlist_btn.py` & `feeluown-4.1.3/feeluown/gui/components/playlist_btn.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/components/song_tag.py` & `feeluown-4.1.3/feeluown/gui/components/song_tag.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/consts.py` & `feeluown-4.1.3/feeluown/gui/consts.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/debug.py` & `feeluown-4.1.3/feeluown/gui/debug.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/drawers.py` & `feeluown-4.1.3/feeluown/gui/drawers.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/helpers.py` & `feeluown-4.1.3/feeluown/gui/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,16 +239,17 @@
                 # inside the viewport, so we always hide the last
                 # two row to ensure fetch-more will not be
                 # triggered automatically.
                 #
                 # qt triggers fetchMore when user scrolls down to bottom.
                 index = self._last_visible_index()
                 rect = self.visualRect(index)
-                height = self.sizeHint().height() - int(rect.height() * 1.5) - \
-                    self._reserved
+                height = self.sizeHint().height()
+                if self._no_scroll_v is False:
+                    height = height - int(rect.height() * 1.5) - self._reserved
                 self.setFixedHeight(max(height, self.min_height()))
             else:
                 self.setFixedHeight(self._row_height * self._fixed_row_count)
         else:
             height = self.sizeHint().height()
             self.setFixedHeight(height)
         self.updateGeometry()
```

### Comparing `feeluown-4.1.2/feeluown/gui/hotkey.py` & `feeluown-4.1.3/feeluown/gui/hotkey.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/image.py` & `feeluown-4.1.3/feeluown/gui/image.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/mimedata.py` & `feeluown-4.1.3/feeluown/gui/mimedata.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/page_containers/scroll_area.py` & `feeluown-4.1.3/feeluown/gui/page_containers/scroll_area.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/page_containers/table.py` & `feeluown-4.1.3/feeluown/gui/page_containers/table.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/pages/coll_mixed.py` & `feeluown-4.1.3/feeluown/gui/pages/coll_mixed.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/pages/model.py` & `feeluown-4.1.3/feeluown/gui/pages/model.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/pages/my_fav.py` & `feeluown-4.1.3/feeluown/gui/pages/my_fav.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/pages/provider_home.py` & `feeluown-4.1.3/feeluown/gui/pages/provider_home.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/pages/recently_played.py` & `feeluown-4.1.3/feeluown/gui/pages/recently_played.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/pages/recommendation.py` & `feeluown-4.1.3/feeluown/gui/pages/recommendation.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/pages/recommendation_daily_songs.py` & `feeluown-4.1.3/feeluown/gui/pages/recommendation_daily_songs.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/pages/search.py` & `feeluown-4.1.3/feeluown/gui/pages/search.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/pages/song_explore.py` & `feeluown-4.1.3/feeluown/gui/pages/song_explore.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/provider_ui.py` & `feeluown-4.1.3/feeluown/gui/provider_ui.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/theme.py` & `feeluown-4.1.3/feeluown/gui/theme.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/tips.py` & `feeluown-4.1.3/feeluown/gui/tips.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     ('Thearas', ''),
     ('reaink', ''),
     ('wenLiangcan', ''),
     ('leedagee', ''),
     ('hanchanli', ''),
     ('xssss1', ''),
     ('williamherry', ''),
+    ('seiuneko', ''),
 ]
 
 
 class TipsManager:
     """在合适的时候展示一些使用 Tip"""
 
     tips = [
```

### Comparing `feeluown-4.1.2/feeluown/gui/tray.py` & `feeluown-4.1.3/feeluown/gui/tray.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/ui.py` & `feeluown-4.1.3/feeluown/gui/ui.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/uimain/floating_box.py` & `feeluown-4.1.3/feeluown/gui/uimain/floating_box.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/uimain/lyric.py` & `feeluown-4.1.3/feeluown/gui/uimain/lyric.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     QMenu, QAction, QFontDialog, QShortcut, QSpacerItem
 
 from feeluown.gui.helpers import esc_hide_widget, resize_font, elided_text
 from feeluown.player import LyricLine
 
 
 IS_MACOS = sys.platform == 'darwin'
+IS_WINDOWS = sys.platform == 'win32'
 
 
 def set_bg_color(palette, color):
     palette.setColor(QPalette.Active, QPalette.Window, color)
     palette.setColor(QPalette.Active, QPalette.Base, color)
     palette.setColor(QPalette.Inactive, QPalette.Window, color)
     palette.setColor(QPalette.Inactive, QPalette.Base, color)
@@ -33,14 +34,46 @@
 * Ctrl+= 或者 Ctrl++ 可以增大字体
 * Ctrl+- 可以减小字体
 * 鼠标前进后退键可以播放前一首/下一首
 * ESC 键可以关闭此歌词窗口
 """
 
 
+class SizeGrip(QSizeGrip):
+    """
+    On windows, when the user drags the size grip, the lyric window is
+    resized and the lyric window also moves. This is not the expected.
+    So override the mouse event to fix this issue.
+
+    Check https://github.com/feeluown/FeelUOwn/issues/752 for more details.
+    """
+    def mousePressEvent(self, e):
+        super().mousePressEvent(e)
+        if IS_WINDOWS:
+            e.accept()
+
+    def mouseMoveEvent(self, e):
+        super().mouseMoveEvent(e)
+        if IS_WINDOWS:
+            e.accept()
+
+    def mouseReleaseEvent(self, e):
+        super().mouseReleaseEvent(e)
+        if IS_WINDOWS:
+            e.accept()
+
+    def paintEvent(self, _):
+        """
+        On windows, it draws a icon on the corner. On other platforms, it does not.
+        So let LyricWindow draw the icon for the SizeGrip.
+        """
+        if IS_WINDOWS:
+            return
+
+
 class LyricWindow(QWidget):
     """LyricWindow is a transparent container which contains a real lyric window.
 
     LyricWindow acts as a transparent container, so the inner window can has
     semi-transparent background. It is also responsible for handling the
     window flags and geometry. It also provides a few APIs for communicating
     with other widgets
@@ -226,15 +259,15 @@
         super().__init__(parent=parent)
         self._app = app
 
         self._border_radius = 0
         # When _auto_resize is True,
         # the window size adapts to the lyric sentence width.
         self._auto_resize = True
-        self._size_grip = QSizeGrip(self)
+        self._size_grip = SizeGrip(self)
         self.line_label = LineLabel(self)
 
         self._app.live_lyric.line_changed.connect(self.set_line)
         self._app.live_lyric.lyrics_changed.connect(self.on_lyrics_changed)
         QShortcut(QKeySequence.ZoomIn, self).activated.connect(self.zoomin)
         QShortcut(QKeySequence.ZoomOut, self).activated.connect(self.zoomout)
         QShortcut(QKeySequence('Ctrl+='), self).activated.connect(self.zoomin)
```

### Comparing `feeluown-4.1.2/feeluown/gui/uimain/nowplaying_overlay.py` & `feeluown-4.1.3/feeluown/gui/uimain/nowplaying_overlay.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/uimain/page_view.py` & `feeluown-4.1.3/feeluown/gui/uimain/page_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import sys
 
 from PyQt5.QtCore import Qt, QRect, QSize, QEasingCurve, QEvent
 from PyQt5.QtGui import QPainter, QBrush, QColor, QLinearGradient, QPalette
-from PyQt5.QtWidgets import QFrame, QVBoxLayout, QStackedLayout
+from PyQt5.QtWidgets import QAbstractScrollArea, QFrame, QVBoxLayout, QStackedLayout
 
 from feeluown.utils import aio
 from feeluown.library import ModelType
 from feeluown.utils.reader import wrap
 
 from feeluown.gui.theme import Light
 from feeluown.gui.helpers import BgTransparentMixin, BaseScrollAreaForNoScrollItemView
@@ -51,19 +51,15 @@
     def height_for_itemview(self):
         height = self.height()
         for w in self._other_widgets:
             if w.isVisible():
                 height -= w.height()
         return height
 
-    def wheelEvent(self, e):
-        super().wheelEvent(e)
-        self._app.ui.bottom_panel.update()
-
-    def eventFilter(self, obj, event):
+    def eventFilter(self, _, event):
         if event.type() == QEvent.Resize:
             self.maybe_resize_itemview()
         return False
 
     def fillable_bg_height(self):
         """Implement VFillableBg protocol"""
         height = 0
@@ -118,17 +114,27 @@
 
         # remove tmp widgets
         for i in range(self._stacked_layout.count()):
             w = self._stacked_layout.widget(i)
             if w not in (self.scrollarea, ):
                 self._stacked_layout.removeWidget(w)
 
+        widget.installEventFilter(self)
+        if isinstance(widget, QAbstractScrollArea):
+            widget.verticalScrollBar().installEventFilter(self)
+
         self._stacked_layout.addWidget(widget)
         self._stacked_layout.setCurrentWidget(widget)
 
+    def eventFilter(self, _, event):
+        # Refresh when the body is scrolled.
+        if event.type() == QEvent.Wheel:
+            self.update()
+        return False
+
     def show_collection(self, coll, model_type):
 
         def _show_pure_albums_coll(coll):
             self.set_body(self.scrollarea)
             reader = wrap(coll.models)
             self.table_container.show_albums_coll(reader)
 
@@ -172,15 +178,19 @@
         # calculate available size
         draw_width = self.width()
         draw_height = self.bottom_panel.height()
         current_widget = self._stacked_layout.currentWidget()
         if isinstance(current_widget, VFillableBg):
             draw_height += current_widget.fillable_bg_height()
 
-        scrolled = self.scrollarea.verticalScrollBar().value()
+        widget = self._stacked_layout.currentWidget()
+        if isinstance(widget, QAbstractScrollArea):
+            scrolled = widget.verticalScrollBar().value()
+        else:
+            scrolled = 0
         max_scroll_height = draw_height - self.bottom_panel.height()
 
         # Draw the whole background with QPalette.Base color.
         painter.save()
         painter.setBrush(self.palette().brush(QPalette.Base))
         painter.drawRect(self.rect())
         painter.restore()
```

### Comparing `feeluown-4.1.2/feeluown/gui/uimain/player_bar.py` & `feeluown-4.1.3/feeluown/gui/uimain/player_bar.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/uimain/playlist_overlay.py` & `feeluown-4.1.3/feeluown/gui/uimain/playlist_overlay.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/uimain/sidebar.py` & `feeluown-4.1.3/feeluown/gui/uimain/sidebar.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,20 @@
         # 让各个音乐库来决定是否显示这些组件
         self.playlists_con.hide()
         self.my_music_con.hide()
         self.discovery_btn.setDisabled(True)
         self.fav_btn.setDisabled(True)
         self.discovery_btn.setToolTip('当前资源提供方未知')
 
-        self.home_btn.clicked.connect(self.show_library)
+        if self._app.config.ENABLE_NEW_HOMEPAGE is True:
+            self.home_btn.clicked.connect(
+                lambda: self._app.browser.goto(page='/homepage'))
+        else:
+            self.home_btn.clicked.connect(self.show_library)
+
         self.discovery_btn.clicked.connect(self.show_pool)
         self.playlists_view.show_playlist.connect(
             lambda pl: self._app.browser.goto(model=pl))
         self.collections_view.show_collection.connect(
             lambda coll: self._app.browser.goto(page=f'/colls/{coll.identifier}'))
         self.collections_view.remove_collection.connect(self._remove_coll)
         self.playlists_view.remove_playlist.connect(self._remove_playlist)
```

### Comparing `feeluown-4.1.2/feeluown/gui/uimain/toolbar.py` & `feeluown-4.1.3/feeluown/gui/uimain/toolbar.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/uimodels/my_music.py` & `feeluown-4.1.3/feeluown/gui/uimodels/my_music.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/uimodels/playlist.py` & `feeluown-4.1.3/feeluown/gui/uimodels/playlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/watch.py` & `feeluown-4.1.3/feeluown/gui/watch.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/accordion.py` & `feeluown-4.1.3/feeluown/gui/widgets/accordion.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/comment_list.py` & `feeluown-4.1.3/feeluown/gui/widgets/comment_list.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/cover_label.py` & `feeluown-4.1.3/feeluown/gui/widgets/cover_label.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/frameless.py` & `feeluown-4.1.3/feeluown/gui/widgets/frameless.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/header.py` & `feeluown-4.1.3/feeluown/gui/widgets/header.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from PyQt5.QtGui import QFont
 from PyQt5.QtWidgets import QLabel
 
 
 class BaseHeader(QLabel):
-    def __init__(self, font_size, *args, **kwargs):
+    def __init__(self, *args, font_size=13, **kwargs):
         super().__init__(*args, **kwargs)
 
         font = self.font()
         font.setPixelSize(font_size)
         self.setFont(font)
 
 
 class LargeHeader(BaseHeader):
     def __init__(self, *args, **kwargs):
-        super().__init__(20, *args, **kwargs)
+        super().__init__(*args, font_size=20, **kwargs)
 
         font = self.font()
         font.setWeight(QFont.DemiBold)
         self.setFont(font)
 
 
 class MidHeader(BaseHeader):
     def __init__(self, *args, **kwargs):
-        super().__init__(16, *args, **kwargs)
+        super().__init__(*args, font_size=16, **kwargs)
```

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/img_card_list.py` & `feeluown-4.1.3/feeluown/gui/widgets/img_card_list.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/labels.py` & `feeluown-4.1.3/feeluown/gui/widgets/labels.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/login.py` & `feeluown-4.1.3/feeluown/gui/widgets/login.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/lyric.py` & `feeluown-4.1.3/feeluown/gui/widgets/lyric.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/magicbox.py` & `feeluown-4.1.3/feeluown/gui/widgets/magicbox.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/messageline.py` & `feeluown-4.1.3/feeluown/gui/widgets/messageline.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/meta.py` & `feeluown-4.1.3/feeluown/gui/widgets/meta.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/mpv_.py` & `feeluown-4.1.3/feeluown/gui/widgets/mpv_.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/my_music.py` & `feeluown-4.1.3/feeluown/gui/widgets/my_music.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/playlist_button.py` & `feeluown-4.1.3/feeluown/gui/widgets/playlist_button.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/playlists.py` & `feeluown-4.1.3/feeluown/gui/widgets/playlists.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/progress_slider.py` & `feeluown-4.1.3/feeluown/gui/widgets/progress_slider.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/provider.py` & `feeluown-4.1.3/feeluown/gui/widgets/provider.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/selfpaint_btn.py` & `feeluown-4.1.3/feeluown/gui/widgets/selfpaint_btn.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/separator.py` & `feeluown-4.1.3/feeluown/gui/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/settings.py` & `feeluown-4.1.3/feeluown/gui/widgets/settings.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/song_minicard_list.py` & `feeluown-4.1.3/feeluown/gui/widgets/song_minicard_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,29 +27,30 @@
 class BaseSongMiniCardListModel(QAbstractListModel):
     def __init__(self, fetch_image, parent=None):
         super().__init__(parent)
 
         self._items = []
         self.fetch_image = fetch_image
         self.pixmaps = {}  # {uri: (Option<pixmap>, Option<color>)}
+        self.rowsAboutToBeRemoved.connect(self.on_rows_about_to_be_removed)
 
     def rowCount(self, _=QModelIndex()):
         return len(self._items)
 
     def flags(self, index):
         if not index.isValid():
             return 0
         flags = Qt.ItemIsSelectable | Qt.ItemIsEnabled
         return flags
 
     def _fetch_image_callback(self, item):
         # TODO: duplicate code with ImgListModel
         def cb(content):
             uri = reverse(item)
-            if content is None:
+            if content is None and uri in self.pixmaps:
                 self.pixmaps[uri] = (self.pixmaps[uri][1], None)
                 return
 
             img = QImage()
             img.loadFromData(content)
             pixmap = QPixmap(img)
             self.pixmaps[uri] = (pixmap, None)
@@ -83,16 +84,23 @@
             return self._items[offset].title_display
         elif role == Qt.UserRole:
             song = self._items[offset]
             pixmap = self.get_pixmap_unblocking(song)
             return (song, pixmap)
         return None
 
+    def on_rows_about_to_be_removed(self, _, first, last):
+        for i in range(first, last+1):
+            item = self._items[i]
+            uri = reverse(item)
+            # clear pixmap cache
+            self.pixmaps.pop(uri, None)
+
 
-class SongMiniCardListModel(BaseSongMiniCardListModel, ReaderFetchMoreMixin):
+class SongMiniCardListModel(ReaderFetchMoreMixin, BaseSongMiniCardListModel):
     def __init__(self, reader, fetch_image, parent=None):
         super().__init__(fetch_image, parent)
 
         self._reader = reader
         self._fetch_more_step = 10
         self._is_fetching = False
```

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/songs.py` & `feeluown-4.1.3/feeluown/gui/widgets/songs.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/statusline.py` & `feeluown-4.1.3/feeluown/gui/widgets/statusline.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/statusline_items/notify.py` & `feeluown-4.1.3/feeluown/gui/widgets/statusline_items/notify.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/statusline_items/plugin.py` & `feeluown-4.1.3/feeluown/gui/widgets/statusline_items/plugin.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/tabbar.py` & `feeluown-4.1.3/feeluown/gui/widgets/tabbar.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/table_toolbar.py` & `feeluown-4.1.3/feeluown/gui/widgets/table_toolbar.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/textlist.py` & `feeluown-4.1.3/feeluown/gui/widgets/textlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/video.py` & `feeluown-4.1.3/feeluown/gui/widgets/video.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/volume_button.py` & `feeluown-4.1.3/feeluown/gui/widgets/volume_button.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/gui/widgets/weblogin.py` & `feeluown-4.1.3/feeluown/gui/widgets/weblogin.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/library/__init__.py` & `feeluown-4.1.3/feeluown/library/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,7 +24,8 @@
 from .excs import NoUserLoggedIn, ModelNotFound, \
     ProviderAlreadyExists, ResourceNotFound, MediaNotFound
 from .provider_protocol import *
 from .uri import (
     Resolver, reverse, resolve, ResolverNotFound, ResolveFailed,
     parse_line, NS_TYPE_MAP,
 )
+from .collection import Collection, CollectionType
```

### Comparing `feeluown-4.1.2/feeluown/library/base.py` & `feeluown-4.1.3/feeluown/library/base.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/library/flags.py` & `feeluown-4.1.3/feeluown/library/flags.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/library/library.py` & `feeluown-4.1.3/feeluown/library/library.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/library/model_protocol.py` & `feeluown-4.1.3/feeluown/library/model_protocol.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/library/model_state.py` & `feeluown-4.1.3/feeluown/library/model_state.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/library/models.py` & `feeluown-4.1.3/feeluown/library/models.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/library/provider.py` & `feeluown-4.1.3/feeluown/library/provider.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/library/provider_protocol.py` & `feeluown-4.1.3/feeluown/library/provider_protocol.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from feeluown.media import Quality, Media
 from feeluown.excs import NoUserLoggedIn
 from .models import (
     BriefCommentModel, SongModel, VideoModel, AlbumModel, ArtistModel,
     PlaylistModel, UserModel, ModelType, BriefArtistModel, BriefSongModel,
     LyricModel, BriefVideoModel,
 )
+from .collection import Collection
 
 from .flags import Flags as PF
 
 
 ID = str
 _FlagProtocolMapping: Dict[Tuple[ModelType, PF], type] = {}
 
@@ -381,14 +382,26 @@
 class SupportsRecListDailySongs(Protocol):
     @abstractmethod
     def rec_list_daily_songs(self) -> List[SongModel]:
         pass
 
 
 @runtime_checkable
+class SupportsRecACollectionOfSongs(Protocol):
+    @abstractmethod
+    def rec_a_collection_of_songs(self) -> Collection:
+        """
+        For example, providers may provider a list of songs,
+        and the title looks like “大家都在听” / “红心歌曲”.
+
+        For different user, this API may return different result.
+        """
+
+
+@runtime_checkable
 class SupportsRecListDailyPlaylists(Protocol):
     @abstractmethod
     def rec_list_daily_playlists(self) -> List[PlaylistModel]:
         pass
 
 
 @runtime_checkable
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `feeluown-4.1.2/feeluown/library/uri.py` & `feeluown-4.1.3/feeluown/library/uri.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/local/__init__.py` & `feeluown-4.1.3/feeluown/local/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/local/db.py` & `feeluown-4.1.3/feeluown/local/db.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/local/provider.py` & `feeluown-4.1.3/feeluown/local/provider.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/local/provider_ui.py` & `feeluown-4.1.3/feeluown/local/provider_ui.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/local/schemas.py` & `feeluown-4.1.3/feeluown/local/schemas.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/local/ui.py` & `feeluown-4.1.3/feeluown/local/ui.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/media.py` & `feeluown-4.1.3/feeluown/media.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/mpv.py` & `feeluown-4.1.3/feeluown/mpv.py`

 * *Files 1% similar despite different names*

```diff
@@ -859,14 +859,16 @@
             self.set_loglevel(loglevel or 'terminal-default')
         if start_event_thread:
             self._event_thread = threading.Thread(target=self._loop, name='MPVEventHandlerThread')
             self._event_thread.setDaemon(True)
             self._event_thread.start()
         else:
             self._event_thread = None
+        if m := re.search(r'(\d+)\.(\d+)\.(\d+)', self.mpv_version):
+            self.mpv_version_tuple = tuple(map(int, m.groups()))
 
     def _loop(self):
         for event in _event_generator(self._event_handle):
             try:
                 devent = event.as_dict(decoder=lazy_decoder) # copy data from ctypes
                 eid = devent['event_id']
 
@@ -1148,17 +1150,24 @@
         """Mapped mpv playlist-play-index command, see man mpv(1)."""
         self.command('playlist-play-index', idx)
 
     @staticmethod
     def _encode_options(options):
         return ','.join('{}={}'.format(_py_to_mpv(str(key)), str(val)) for key, val in options.items())
 
-    def loadfile(self, filename, mode='replace', **options):
+    def loadfile(self, filename, mode='replace', index=None, **options):
         """Mapped mpv loadfile command, see man mpv(1)."""
-        self.command('loadfile', filename.encode(fs_enc), mode, MPV._encode_options(options))
+        if self.mpv_version_tuple >= (0, 38, 0):
+            if index is None:
+                index = -1
+            self.command('loadfile', filename.encode(fs_enc), mode, index, MPV._encode_options(options))
+        else:
+            if index is not None:
+                warn(f'The index argument to the loadfile command is only supported on mpv >= 0.38.0')
+            self.command('loadfile', filename.encode(fs_enc), mode, MPV._encode_options(options))
 
     def loadlist(self, playlist, mode='replace'):
         """Mapped mpv loadlist command, see man mpv(1)."""
         self.command('loadlist', playlist.encode(fs_enc), mode)
 
     def playlist_clear(self):
         """Mapped mpv playlist_clear command, see man mpv(1)."""
```

### Comparing `feeluown-4.1.2/feeluown/nowplaying/__init__.py` & `feeluown-4.1.3/feeluown/nowplaying/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/nowplaying/linux/__init__.py` & `feeluown-4.1.3/feeluown/nowplaying/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/nowplaying/linux/introspect.xml` & `feeluown-4.1.3/feeluown/nowplaying/linux/introspect.xml`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/nowplaying/linux/mpris2.py` & `feeluown-4.1.3/feeluown/nowplaying/linux/mpris2.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/nowplaying/macos.py` & `feeluown-4.1.3/feeluown/nowplaying/macos.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/nowplaying/nowplaying.py` & `feeluown-4.1.3/feeluown/nowplaying/nowplaying.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/player/__init__.py` & `feeluown-4.1.3/feeluown/player/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/player/base_player.py` & `feeluown-4.1.3/feeluown/player/base_player.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/player/delegate.py` & `feeluown-4.1.3/feeluown/player/delegate.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/player/fm.py` & `feeluown-4.1.3/feeluown/player/fm.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/player/lyric.py` & `feeluown-4.1.3/feeluown/player/lyric.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,18 +45,20 @@
     return None, None
 
 
 def parse_lyric_text(content: str) -> Dict[int, str]:
     """
     Reference: https://github.com/osdlyrics/osdlyrics/blob/master/python/lrc.py
 
-    >>> parse_lyric_text("[00:00.00] 作曲 : 周杰伦\\n[00:01.00] 作词 : 周杰伦\\n")
-    OrderedDict([(0, ' 作曲 : 周杰伦'), (1000, ' 作词 : 周杰伦')])
-    >>> parse_lyric_text("[01:30][00:01:10][01:00]再等直至再吻到你")
-    OrderedDict([(60000, '再等直至再吻到你'), (70000, '再等直至再吻到你'), (90000, '再等直至再吻到你')])
+    >>> r = parse_lyric_text("[00:00.00] 作曲 : 周杰伦\\n[00:01.00] 作词 : 周杰伦\\n")
+    >>> list(r.items())[0]
+    (0, ' 作曲 : 周杰伦')
+    >>> r = parse_lyric_text("[01:30][00:01:10][01:00]再等直至再吻到你")
+    >>> list(r.items())[-1]
+    (90000, '再等直至再吻到你')
     """
     def to_mileseconds(time_str):
         mileseconds = 0
         unit = 1000
         t_seq = time_str.split(':')
         t_seq.reverse()
         for num in t_seq:
```

### Comparing `feeluown-4.1.2/feeluown/player/metadata.py` & `feeluown-4.1.3/feeluown/player/metadata.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/player/mpvplayer.py` & `feeluown-4.1.3/feeluown/player/mpvplayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,20 +41,20 @@
         # https://github.com/cosven/FeelUOwn/issues/246
         locale.setlocale(locale.LC_NUMERIC, 'C')
         mpvkwargs = {}
         if winid is not None:
             mpvkwargs['wid'] = winid
         self._version = _mpv_client_api_version()
 
-        # old version libmpv can use opengl-cb
-        if self._version < (1, 107):
-            mpvkwargs['vo'] = 'opengl-cb'
-            self.use_opengl_cb = True
-        else:
-            self.use_opengl_cb = False
+        # From libmpv 0.38, libmpv is not the default vo.
+        # Note if vo is not set to libmpv, the video is rendered in mpv's
+        # native window instead of feeluown's mpvwidget (tested on KDE+wayland).
+        # On macOS, this option is optional. I believe the option is also required
+        # on Windows.
+        mpvkwargs['vo'] = 'libmpv'
 
         # set log_handler if you want to debug
         # mpvkwargs['log_handler'] = self.__log_handler
         # mpvkwargs['msg_level'] = 'all=v'
         # the default version of libmpv on Ubuntu 18.04 is (1, 25)
         self._mpv = MPV(ytdl=False,
                         input_default_bindings=True,
```

### Comparing `feeluown-4.1.2/feeluown/player/playlist.py` & `feeluown-4.1.3/feeluown/player/playlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/player/radio.py` & `feeluown-4.1.3/feeluown/player/radio.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/player/recently_played.py` & `feeluown-4.1.3/feeluown/player/recently_played.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/plugin.py` & `feeluown-4.1.3/feeluown/plugin.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/serializers/__init__.py` & `feeluown-4.1.3/feeluown/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/serializers/_plain_formatter.py` & `feeluown-4.1.3/feeluown/serializers/_plain_formatter.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/serializers/base.py` & `feeluown-4.1.3/feeluown/serializers/base.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/serializers/json_.py` & `feeluown-4.1.3/feeluown/serializers/json_.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/serializers/model_helpers.py` & `feeluown-4.1.3/feeluown/serializers/model_helpers.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/serializers/objs.py` & `feeluown-4.1.3/feeluown/serializers/objs.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/serializers/plain.py` & `feeluown-4.1.3/feeluown/serializers/plain.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/serializers/python.py` & `feeluown-4.1.3/feeluown/serializers/python.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/serializers/typename.py` & `feeluown-4.1.3/feeluown/serializers/typename.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/__init__.py` & `feeluown-4.1.3/feeluown/server/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/data_structure.py` & `feeluown-4.1.3/feeluown/server/data_structure.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/dslv1/codegen.py` & `feeluown-4.1.3/feeluown/server/dslv1/codegen.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/dslv1/lexer.py` & `feeluown-4.1.3/feeluown/server/dslv1/lexer.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/dslv1/parser.py` & `feeluown-4.1.3/feeluown/server/dslv1/parser.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/dslv2.py` & `feeluown-4.1.3/feeluown/server/dslv2.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/excs.py` & `feeluown-4.1.3/feeluown/server/excs.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/handlers/base.py` & `feeluown-4.1.3/feeluown/server/handlers/base.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/handlers/exec_.py` & `feeluown-4.1.3/feeluown/server/handlers/exec_.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/handlers/handle.py` & `feeluown-4.1.3/feeluown/server/handlers/handle.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/handlers/help.py` & `feeluown-4.1.3/feeluown/server/handlers/help.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/handlers/player.py` & `feeluown-4.1.3/feeluown/server/handlers/player.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/handlers/playlist.py` & `feeluown-4.1.3/feeluown/server/handlers/playlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/handlers/search.py` & `feeluown-4.1.3/feeluown/server/handlers/search.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/handlers/show.py` & `feeluown-4.1.3/feeluown/server/handlers/show.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/handlers/sub.py` & `feeluown-4.1.3/feeluown/server/handlers/sub.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/protocol.py` & `feeluown-4.1.3/feeluown/server/protocol.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/pubsub/gateway.py` & `feeluown-4.1.3/feeluown/server/pubsub/gateway.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/pubsub/publishers.py` & `feeluown-4.1.3/feeluown/server/pubsub/publishers.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/server/server.py` & `feeluown-4.1.3/feeluown/server/server.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/task.py` & `feeluown-4.1.3/feeluown/task.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/utils/aio.py` & `feeluown-4.1.3/feeluown/utils/aio.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,20 @@
 
 #: sleep is an alias of `asyncio.sleep`.
 sleep = asyncio.sleep
 
 #: run is an alias of `asyncio.run`.
 run = asyncio.run
 
+#: wait is an alias of `asyncio.wait`.
+wait = asyncio.wait
+
+#: gather is an alias of `asyncio.gather`.
+gather = asyncio.gather
+
 
 def run_in_executor(executor, func, *args):
     """alias for loop.run_in_executor"""
     loop = asyncio.get_running_loop()
     return loop.run_in_executor(executor, func, *args)
```

### Comparing `feeluown-4.1.2/feeluown/utils/audio.py` & `feeluown-4.1.3/feeluown/utils/audio.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/utils/cache.py` & `feeluown-4.1.3/feeluown/utils/cache.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/utils/dispatch.py` & `feeluown-4.1.3/feeluown/utils/dispatch.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/utils/lang.py` & `feeluown-4.1.3/feeluown/utils/lang.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/utils/patch.py` & `feeluown-4.1.3/feeluown/utils/patch.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/utils/reader.py` & `feeluown-4.1.3/feeluown/utils/reader.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/utils/request.py` & `feeluown-4.1.3/feeluown/utils/request.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/utils/router.py` & `feeluown-4.1.3/feeluown/utils/router.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/utils/sync.py` & `feeluown-4.1.3/feeluown/utils/sync.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/utils/utils.py` & `feeluown-4.1.3/feeluown/utils/utils.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/utils/yt_dlp_cookies.py` & `feeluown-4.1.3/feeluown/utils/yt_dlp_cookies.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/version.py` & `feeluown-4.1.3/feeluown/version.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/webserver/jsonrpc_.py` & `feeluown-4.1.3/feeluown/webserver/jsonrpc_.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown/webserver/server.py` & `feeluown-4.1.3/feeluown/webserver/server.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/feeluown.egg-info/PKG-INFO` & `feeluown-4.1.3/feeluown.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feeluown
-Version: 4.1.2
+Version: 4.1.3
 Summary: *nix music player
 Home-page: https://github.com/feeluown/FeelUOwn
 Author: feeluown
 Author-email: yinshaowen241@gmail.com
 License: GPL-3.0
 Description: ## FeelUOwn - feel your own
```

### Comparing `feeluown-4.1.2/feeluown.egg-info/SOURCES.txt` & `feeluown-4.1.3/feeluown.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 feeluown/gui/components/song_tag.py
 feeluown/gui/components/volume_slider.py
 feeluown/gui/page_containers/__init__.py
 feeluown/gui/page_containers/scroll_area.py
 feeluown/gui/page_containers/table.py
 feeluown/gui/pages/__init__.py
 feeluown/gui/pages/coll_mixed.py
+feeluown/gui/pages/homepage.py
 feeluown/gui/pages/model.py
 feeluown/gui/pages/my_fav.py
 feeluown/gui/pages/provider_home.py
 feeluown/gui/pages/recently_played.py
 feeluown/gui/pages/recommendation.py
 feeluown/gui/pages/recommendation_daily_songs.py
 feeluown/gui/pages/search.py
@@ -150,14 +151,15 @@
 feeluown/gui/widgets/weblogin.py
 feeluown/gui/widgets/statusline_items/__init__.py
 feeluown/gui/widgets/statusline_items/notify.py
 feeluown/gui/widgets/statusline_items/plugin.py
 feeluown/library/__init__.py
 feeluown/library/abc.py
 feeluown/library/base.py
+feeluown/library/collection.py
 feeluown/library/excs.py
 feeluown/library/flags.py
 feeluown/library/library.py
 feeluown/library/model_protocol.py
 feeluown/library/model_state.py
 feeluown/library/models.py
 feeluown/library/provider.py
```

### Comparing `feeluown-4.1.2/setup.cfg` & `feeluown-4.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.2/setup.py` & `feeluown-4.1.3/setup.py`

 * *Files identical despite different names*

