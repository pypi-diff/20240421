# Comparing `tmp/practical_astronomy-0.0.4.tar.gz` & `tmp/practical_astronomy-1.0.0.tar.gz`

## Comparing `practical_astronomy-0.0.4.tar` & `practical_astronomy-1.0.0.tar`

### file list

```diff
@@ -1,279 +1,279 @@
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/Makefile
--rwxr-xr-x   0        0        0    26244 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/test_coordinate.py
--rwxr-xr-x   0        0        0      950 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/test_date_of_easter.py
--rwxr-xr-x   0        0        0      631 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/test_day_number.py
--rwxr-xr-x   0        0        0     7283 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/test_eclipses.py
--rwxr-xr-x   0        0        0     2069 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/test_julian.py
--rwxr-xr-x   0        0        0     8880 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/test_moon.py
--rwxr-xr-x   0        0        0     8151 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/test_planet_comet_binary.py
--rwxr-xr-x   0        0        0     8206 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/test_sun.py
--rwxr-xr-x   0        0        0     6694 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/test_time.py
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/README_8md.html
--rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/____init_____8py.html
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/bc_s.png
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/bdwn.png
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/closed.png
--rw-r--r--   0        0        0     8358 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/dir_45978790aec87fba6f3407586a078612.html
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/dir_45978790aec87fba6f3407586a078612.js
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/dir_68267d1309a1af8e8297ef4c3efbcdba.html
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/dir_68267d1309a1af8e8297ef4c3efbcdba.js
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/dir_8ebb4883bd5210c1437544ca4cb0df32.html
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/doc.png
--rw-r--r--   0        0        0    31428 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/doxygen.css
--rw-r--r--   0        0        0    15382 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/doxygen.svg
--rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/dynsections.js
--rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/files.html
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/files_dup.js
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/folderclosed.png
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/folderopen.png
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/glossary_8md.html
--rw-r--r--   0        0        0    13489 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/index.html
--rw-r--r--   0        0        0   175457 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/jquery.js
--rw-r--r--   0        0        0    36700 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/md_src_glossary.html
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/menu.js
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/menudata.js
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers.html
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_b.html
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_c.html
--rw-r--r--   0        0        0     6284 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_d.html
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_dup.js
--rw-r--r--   0        0        0     7873 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_e.html
--rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_f.html
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func.html
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func.js
--rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_b.html
--rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_c.html
--rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_d.html
--rw-r--r--   0        0        0     7757 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_e.html
--rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_f.html
--rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_g.html
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_h.html
--rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_i.html
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_j.html
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_k.html
--rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_l.html
--rw-r--r--   0        0        0     9539 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_m.html
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_n.html
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_o.html
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_p.html
--rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_r.html
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_s.html
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_t.html
--rw-r--r--   0        0        0     7856 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_u.html
--rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_func_v.html
--rw-r--r--   0        0        0     5830 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_g.html
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_h.html
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_i.html
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_j.html
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_k.html
--rw-r--r--   0        0        0     5845 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_l.html
--rw-r--r--   0        0        0     9655 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_m.html
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_n.html
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_o.html
--rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_p.html
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_r.html
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_s.html
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_t.html
--rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_u.html
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_v.html
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacemembers_vars.html
--rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacepractical__astronomy.html
--rw-r--r--   0        0        0    29160 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacepractical__astronomy.js
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__binary.html
--rw-r--r--   0        0        0     7050 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__binary__data.html
--rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__comet.html
--rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__comet__data.html
--rw-r--r--   0        0        0    65567 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__coordinate.html
--rw-r--r--   0        0        0    34005 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__datetime.html
--rw-r--r--   0        0        0    16673 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__eclipses.html
--rw-r--r--   0        0        0   323566 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__macro.html
--rw-r--r--   0        0        0    24903 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__moon.html
--rw-r--r--   0        0        0    15690 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__planet.html
--rw-r--r--   0        0        0     6938 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__planet__data.html
--rw-r--r--   0        0        0    26414 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__sun.html
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__util.html
--rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespaces.html
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/namespaces_dup.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/nav_f.png
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/nav_g.png
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/nav_h.png
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/navtree.css
--rw-r--r--   0        0        0    15609 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/navtree.js
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/navtreedata.js
--rw-r--r--   0        0        0    13764 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/navtreeindex0.js
--rw-r--r--   0        0        0    22404 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/navtreeindex1.js
--rw-r--r--   0        0        0    12247 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/navtreeindex2.js
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/open.png
--rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__binary_8py.html
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__binary_8py.js
--rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__binary__data_8py.html
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__binary__data_8py.js
--rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__comet_8py.html
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__comet_8py.js
--rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__comet__data_8py.html
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__comet__data_8py.js
--rw-r--r--   0        0        0    16991 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__coordinate_8py.html
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__coordinate_8py.js
--rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__datetime_8py.html
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__datetime_8py.js
--rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__eclipses_8py.html
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__eclipses_8py.js
--rw-r--r--   0        0        0    71778 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__macro_8py.html
--rw-r--r--   0        0        0    13320 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__macro_8py.js
--rw-r--r--   0        0        0     8157 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__moon_8py.html
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__moon_8py.js
--rw-r--r--   0        0        0     6623 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__planet_8py.html
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__planet_8py.js
--rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__planet__data_8py.html
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__planet__data_8py.js
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__sun_8py.html
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__sun_8py.js
--rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__util_8py.html
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pa__util_8py.js
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/pages.html
--rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/resize.js
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/splitbar.png
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/sync_off.png
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/sync_on.png
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/tab_a.png
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/tab_b.png
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/tab_h.png
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/tab_s.png
--rw-r--r--   0        0        0     8700 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/tabs.css
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_0.html
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_0.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_1.html
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_1.js
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_10.html
--rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_10.js
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_11.html
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_11.js
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_12.html
--rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_12.js
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_13.html
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_13.js
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_14.html
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_14.js
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_15.html
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_15.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_2.html
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_2.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_3.html
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_3.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_4.html
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_4.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_5.html
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_5.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_6.html
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_6.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_7.html
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_7.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_8.html
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_8.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_9.html
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_9.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_a.html
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_a.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_b.html
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_b.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_c.html
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_c.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_d.html
--rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_d.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_e.html
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_e.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_f.html
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/all_f.js
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/close.svg
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/files_0.html
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/files_0.js
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/files_1.html
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/files_1.js
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/files_2.html
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/files_2.js
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/files_3.html
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/files_3.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_0.html
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_0.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_1.html
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_1.js
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_10.html
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_10.js
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_11.html
--rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_11.js
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_12.html
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_12.js
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_13.html
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_13.js
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_14.html
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_14.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_2.html
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_2.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_3.html
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_3.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_4.html
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_4.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_5.html
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_5.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_6.html
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_6.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_7.html
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_7.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_8.html
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_8.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_9.html
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_9.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_a.html
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_a.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_b.html
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_b.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_c.html
--rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_c.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_d.html
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_d.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_e.html
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_e.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_f.html
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/functions_f.js
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/mag_sel.svg
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/namespaces_0.html
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/namespaces_0.js
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/nomatches.html
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/pages_0.html
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/pages_0.js
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/pages_1.html
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/pages_1.js
--rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/search.css
--rw-r--r--   0        0        0    23521 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/search.js
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/search_l.png
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/search_m.png
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/search_r.png
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/searchdata.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/variables_0.html
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/variables_0.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/variables_1.html
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/variables_1.js
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/variables_2.html
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs/search/variables_2.js
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs-gen/Doxyfile
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs-gen/Makefile
--rw-r--r--   0        0        0    25427 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/docs-gen/src/glossary.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/src/practical_astronomy/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/src/practical_astronomy/__init__.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/src/practical_astronomy/pa_binary.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/src/practical_astronomy/pa_binary_data.py
--rw-r--r--   0        0        0     7666 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/src/practical_astronomy/pa_comet.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/src/practical_astronomy/pa_comet_data.py
--rw-r--r--   0        0        0    28562 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/src/practical_astronomy/pa_coordinate.py
--rw-r--r--   0        0        0     7006 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/src/practical_astronomy/pa_datetime.py
--rw-r--r--   0        0        0    14838 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/src/practical_astronomy/pa_eclipses.py
--rw-r--r--   0        0        0   147348 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/src/practical_astronomy/pa_macro.py
--rw-r--r--   0        0        0    18381 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/src/practical_astronomy/pa_moon.py
--rw-r--r--   0        0        0    11275 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/src/practical_astronomy/pa_planet.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/src/practical_astronomy/pa_planet_data.py
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/src/practical_astronomy/pa_sun.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/src/practical_astronomy/pa_util.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/LICENSE
--rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/README.md
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 practical_astronomy-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/Makefile
+-rwxr-xr-x   0        0        0    26244 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/test_coordinate.py
+-rwxr-xr-x   0        0        0      950 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/test_date_of_easter.py
+-rwxr-xr-x   0        0        0      631 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/test_day_number.py
+-rwxr-xr-x   0        0        0     7283 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/test_eclipses.py
+-rwxr-xr-x   0        0        0     2069 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/test_julian.py
+-rwxr-xr-x   0        0        0     8880 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/test_moon.py
+-rwxr-xr-x   0        0        0     8151 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/test_planet_comet_binary.py
+-rwxr-xr-x   0        0        0     8206 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/test_sun.py
+-rwxr-xr-x   0        0        0     6694 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/test_time.py
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/README_8md.html
+-rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/____init_____8py.html
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/bc_s.png
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/bdwn.png
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/closed.png
+-rw-r--r--   0        0        0     8358 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/dir_45978790aec87fba6f3407586a078612.html
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/dir_45978790aec87fba6f3407586a078612.js
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/dir_68267d1309a1af8e8297ef4c3efbcdba.html
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/dir_68267d1309a1af8e8297ef4c3efbcdba.js
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/dir_8ebb4883bd5210c1437544ca4cb0df32.html
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/doc.png
+-rw-r--r--   0        0        0    31428 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/doxygen.css
+-rw-r--r--   0        0        0    15382 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/doxygen.svg
+-rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/dynsections.js
+-rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/files.html
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/files_dup.js
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/folderclosed.png
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/folderopen.png
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/glossary_8md.html
+-rw-r--r--   0        0        0    14199 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/index.html
+-rw-r--r--   0        0        0   175457 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/jquery.js
+-rw-r--r--   0        0        0    36700 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/md_src_glossary.html
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/menu.js
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/menudata.js
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers.html
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_b.html
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_c.html
+-rw-r--r--   0        0        0     6284 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_d.html
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_dup.js
+-rw-r--r--   0        0        0     7873 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_e.html
+-rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_f.html
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func.html
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func.js
+-rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_b.html
+-rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_c.html
+-rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_d.html
+-rw-r--r--   0        0        0     7757 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_e.html
+-rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_f.html
+-rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_g.html
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_h.html
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_i.html
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_j.html
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_k.html
+-rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_l.html
+-rw-r--r--   0        0        0     9539 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_m.html
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_n.html
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_o.html
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_p.html
+-rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_r.html
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_s.html
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_t.html
+-rw-r--r--   0        0        0     7856 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_u.html
+-rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_func_v.html
+-rw-r--r--   0        0        0     5830 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_g.html
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_h.html
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_i.html
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_j.html
+-rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_k.html
+-rw-r--r--   0        0        0     5845 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_l.html
+-rw-r--r--   0        0        0     9655 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_m.html
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_n.html
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_o.html
+-rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_p.html
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_r.html
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_s.html
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_t.html
+-rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_u.html
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_v.html
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacemembers_vars.html
+-rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacepractical__astronomy.html
+-rw-r--r--   0        0        0    29160 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacepractical__astronomy.js
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__binary.html
+-rw-r--r--   0        0        0     7050 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__binary__data.html
+-rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__comet.html
+-rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__comet__data.html
+-rw-r--r--   0        0        0    65567 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__coordinate.html
+-rw-r--r--   0        0        0    34005 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__datetime.html
+-rw-r--r--   0        0        0    16673 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__eclipses.html
+-rw-r--r--   0        0        0   323566 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__macro.html
+-rw-r--r--   0        0        0    24903 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__moon.html
+-rw-r--r--   0        0        0    15690 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__planet.html
+-rw-r--r--   0        0        0     6938 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__planet__data.html
+-rw-r--r--   0        0        0    26414 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__sun.html
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__util.html
+-rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespaces.html
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/namespaces_dup.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/nav_f.png
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/nav_g.png
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/nav_h.png
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/navtree.css
+-rw-r--r--   0        0        0    15609 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/navtree.js
+-rw-r--r--   0        0        0    11928 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/navtreedata.js
+-rw-r--r--   0        0        0    13734 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/navtreeindex0.js
+-rw-r--r--   0        0        0    22396 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/navtreeindex1.js
+-rw-r--r--   0        0        0    12319 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/navtreeindex2.js
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/open.png
+-rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__binary_8py.html
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__binary_8py.js
+-rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__binary__data_8py.html
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__binary__data_8py.js
+-rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__comet_8py.html
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__comet_8py.js
+-rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__comet__data_8py.html
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__comet__data_8py.js
+-rw-r--r--   0        0        0    16991 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__coordinate_8py.html
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__coordinate_8py.js
+-rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__datetime_8py.html
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__datetime_8py.js
+-rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__eclipses_8py.html
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__eclipses_8py.js
+-rw-r--r--   0        0        0    71778 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__macro_8py.html
+-rw-r--r--   0        0        0    13320 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__macro_8py.js
+-rw-r--r--   0        0        0     8157 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__moon_8py.html
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__moon_8py.js
+-rw-r--r--   0        0        0     6623 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__planet_8py.html
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__planet_8py.js
+-rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__planet__data_8py.html
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__planet__data_8py.js
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__sun_8py.html
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__sun_8py.js
+-rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__util_8py.html
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pa__util_8py.js
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/pages.html
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/resize.js
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/splitbar.png
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/sync_off.png
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/sync_on.png
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/tab_a.png
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/tab_b.png
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/tab_h.png
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/tab_s.png
+-rw-r--r--   0        0        0     8700 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/tabs.css
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_0.html
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_0.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_1.html
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_1.js
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_10.html
+-rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_10.js
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_11.html
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_11.js
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_12.html
+-rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_12.js
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_13.html
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_13.js
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_14.html
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_14.js
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_15.html
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_15.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_2.html
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_2.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_3.html
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_3.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_4.html
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_4.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_5.html
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_5.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_6.html
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_6.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_7.html
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_7.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_8.html
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_8.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_9.html
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_9.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_a.html
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_a.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_b.html
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_b.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_c.html
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_c.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_d.html
+-rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_d.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_e.html
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_e.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_f.html
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/all_f.js
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/close.svg
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/files_0.html
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/files_0.js
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/files_1.html
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/files_1.js
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/files_2.html
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/files_2.js
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/files_3.html
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/files_3.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_0.html
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_0.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_1.html
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_1.js
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_10.html
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_10.js
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_11.html
+-rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_11.js
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_12.html
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_12.js
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_13.html
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_13.js
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_14.html
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_14.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_2.html
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_2.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_3.html
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_3.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_4.html
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_4.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_5.html
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_5.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_6.html
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_6.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_7.html
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_7.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_8.html
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_8.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_9.html
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_9.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_a.html
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_a.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_b.html
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_b.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_c.html
+-rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_c.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_d.html
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_d.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_e.html
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_e.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_f.html
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/functions_f.js
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/mag_sel.svg
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/namespaces_0.html
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/namespaces_0.js
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/nomatches.html
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/pages_0.html
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/pages_0.js
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/pages_1.html
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/pages_1.js
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/search.css
+-rw-r--r--   0        0        0    23521 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/search.js
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/search_l.png
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/search_m.png
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/search_r.png
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/searchdata.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/variables_0.html
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/variables_0.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/variables_1.html
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/variables_1.js
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/variables_2.html
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs/search/variables_2.js
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs-gen/Doxyfile
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs-gen/Makefile
+-rw-r--r--   0        0        0    25427 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/docs-gen/src/glossary.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/src/practical_astronomy/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/src/practical_astronomy/__init__.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/src/practical_astronomy/pa_binary.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/src/practical_astronomy/pa_binary_data.py
+-rw-r--r--   0        0        0     7666 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/src/practical_astronomy/pa_comet.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/src/practical_astronomy/pa_comet_data.py
+-rw-r--r--   0        0        0    28562 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/src/practical_astronomy/pa_coordinate.py
+-rw-r--r--   0        0        0     7006 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/src/practical_astronomy/pa_datetime.py
+-rw-r--r--   0        0        0    14838 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/src/practical_astronomy/pa_eclipses.py
+-rw-r--r--   0        0        0   147348 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/src/practical_astronomy/pa_macro.py
+-rw-r--r--   0        0        0    18381 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/src/practical_astronomy/pa_moon.py
+-rw-r--r--   0        0        0    11275 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/src/practical_astronomy/pa_planet.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/src/practical_astronomy/pa_planet_data.py
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/src/practical_astronomy/pa_sun.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/src/practical_astronomy/pa_util.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/README.md
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 practical_astronomy-1.0.0/PKG-INFO
```

### Comparing `practical_astronomy-0.0.4/Makefile` & `practical_astronomy-1.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/test_coordinate.py` & `practical_astronomy-1.0.0/test_coordinate.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/test_date_of_easter.py` & `practical_astronomy-1.0.0/test_date_of_easter.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/test_day_number.py` & `practical_astronomy-1.0.0/test_day_number.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/test_eclipses.py` & `practical_astronomy-1.0.0/test_eclipses.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/test_julian.py` & `practical_astronomy-1.0.0/test_julian.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/test_moon.py` & `practical_astronomy-1.0.0/test_moon.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/test_planet_comet_binary.py` & `practical_astronomy-1.0.0/test_planet_comet_binary.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/test_sun.py` & `practical_astronomy-1.0.0/test_sun.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/test_time.py` & `practical_astronomy-1.0.0/test_time.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/README_8md.html` & `practical_astronomy-1.0.0/docs/README_8md.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/____init_____8py.html` & `practical_astronomy-1.0.0/docs/____init_____8py.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/bc_s.png` & `practical_astronomy-1.0.0/docs/bc_s.png`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/dir_45978790aec87fba6f3407586a078612.html` & `practical_astronomy-1.0.0/docs/dir_45978790aec87fba6f3407586a078612.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/dir_45978790aec87fba6f3407586a078612.js` & `practical_astronomy-1.0.0/docs/dir_45978790aec87fba6f3407586a078612.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/dir_68267d1309a1af8e8297ef4c3efbcdba.html` & `practical_astronomy-1.0.0/docs/dir_68267d1309a1af8e8297ef4c3efbcdba.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/dir_8ebb4883bd5210c1437544ca4cb0df32.html` & `practical_astronomy-1.0.0/docs/dir_8ebb4883bd5210c1437544ca4cb0df32.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/doc.png` & `practical_astronomy-1.0.0/docs/doc.png`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/doxygen.css` & `practical_astronomy-1.0.0/docs/doxygen.css`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/doxygen.svg` & `practical_astronomy-1.0.0/docs/doxygen.svg`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/dynsections.js` & `practical_astronomy-1.0.0/docs/dynsections.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/files.html` & `practical_astronomy-1.0.0/docs/files.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/folderclosed.png` & `practical_astronomy-1.0.0/docs/folderclosed.png`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/folderopen.png` & `practical_astronomy-1.0.0/docs/folderopen.png`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/glossary_8md.html` & `practical_astronomy-1.0.0/docs/glossary_8md.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/index.html` & `practical_astronomy-1.0.0/docs/index.html`

 * *Files 7% similar despite different names*

```diff
@@ -84,20 +84,33 @@
   <div class="headertitle">
 <div class="title">practical-astronomy-python </div>  </div>
 </div><!--header-->
 <div class="contents">
 <div class="textblock"><p><a class="anchor" id="md__home_jimc_projects_Practical_Astronomy_practical_astronomy_python_venv_practical_astronomy_python_README"></a> Algorithms from <a href="https://www.amazon.com/Practical-Astronomy-your-Calculator-Spreadsheet/dp/1108436072">Practical Astronomy with your Calculator or Spreadsheet</a> by Peter Duffett-Smith, implemented in Python 3. API documentation is published <a href="https://jfcarr.github.io/practical-astronomy-python/">here</a>.</p>
 <p>If you're interested in this topic, please buy the book! It provides far more detail and context.</p>
 <h1><a class="anchor" id="autotoc_md133"></a>
+Quick Start</h1>
+<p>Install:</p>
+<div class="fragment"><div class="line">pip install practical-astronomy</div>
+</div><!-- fragment --><p>Create <code>easter.py</code>:</p>
+<div class="fragment"><div class="line">import practical_astronomy.pa_datetime as pd</div>
+<div class="line"> </div>
+<div class="line">print(pd.get_date_of_easter(2024))</div>
+</div><!-- fragment --><p>Run it:</p>
+<div class="fragment"><div class="line">python easter.py</div>
+</div><!-- fragment --><p>Result:</p>
+<div class="fragment"><div class="line">(3, 31, 2024)</div>
+</div><!-- fragment --><h1><a class="anchor" id="autotoc_md134"></a>
 Unit Tests</h1>
 <p>If you clone the <a href="https://github.com/jfcarr/practical-astronomy-python">repo</a> locally, you can run unit tests with the Make utility:</p>
 <div class="fragment"><div class="line">make all-tests</div>
-</div><!-- fragment --><h1><a class="anchor" id="autotoc_md134"></a>
+</div><!-- fragment --><h1><a class="anchor" id="autotoc_md135"></a>
 Library Functions</h1>
-<h2><a class="anchor" id="autotoc_md135"></a>
+<p>Documentation <a href="https://jfcarr.github.io/practical-astronomy-python/">here</a>.</p>
+<h2><a class="anchor" id="autotoc_md136"></a>
 Date/Time</h2>
 <table class="markdownTable">
 <tr class="markdownTableHead">
 <th class="markdownTableHeadNone">Type   </th><th class="markdownTableHeadNone">Description    </th></tr>
 <tr class="markdownTableRowOdd">
 <td class="markdownTableBodyNone">Calculate   </td><td class="markdownTableBodyNone">Date of Easter    </td></tr>
 <tr class="markdownTableRowEven">
@@ -115,15 +128,15 @@
 <tr class="markdownTableRowEven">
 <td class="markdownTableBodyNone">Convert   </td><td class="markdownTableBodyNone">Local Civil Time &lt;-&gt; Universal Time    </td></tr>
 <tr class="markdownTableRowOdd">
 <td class="markdownTableBodyNone">Convert   </td><td class="markdownTableBodyNone">Universal Time &lt;-&gt; Greenwich Sidereal Time    </td></tr>
 <tr class="markdownTableRowEven">
 <td class="markdownTableBodyNone">Convert   </td><td class="markdownTableBodyNone">Greenwich Sidereal Time &lt;-&gt; Local Sidereal Time   </td></tr>
 </table>
-<h2><a class="anchor" id="autotoc_md136"></a>
+<h2><a class="anchor" id="autotoc_md137"></a>
 Coordinates</h2>
 <table class="markdownTable">
 <tr class="markdownTableHead">
 <th class="markdownTableHeadNone">Type   </th><th class="markdownTableHeadNone">Description    </th></tr>
 <tr class="markdownTableRowOdd">
 <td class="markdownTableBodyNone">Convert   </td><td class="markdownTableBodyNone">Angle &lt;-&gt; Decimal Degrees    </td></tr>
 <tr class="markdownTableRowEven">
@@ -151,15 +164,15 @@
 <tr class="markdownTableRowOdd">
 <td class="markdownTableBodyNone">Calculate   </td><td class="markdownTableBodyNone">Heliographic coordinates    </td></tr>
 <tr class="markdownTableRowEven">
 <td class="markdownTableBodyNone">Calculate   </td><td class="markdownTableBodyNone">Carrington rotation number    </td></tr>
 <tr class="markdownTableRowOdd">
 <td class="markdownTableBodyNone">Calculate   </td><td class="markdownTableBodyNone">Selenographic (lunar) coordinates (sub-Earth and sub-Solar)   </td></tr>
 </table>
-<h2><a class="anchor" id="autotoc_md137"></a>
+<h2><a class="anchor" id="autotoc_md138"></a>
 The Sun</h2>
 <table class="markdownTable">
 <tr class="markdownTableHead">
 <th class="markdownTableHeadNone">Type   </th><th class="markdownTableHeadNone">Description    </th></tr>
 <tr class="markdownTableRowOdd">
 <td class="markdownTableBodyNone">Calculate   </td><td class="markdownTableBodyNone">Approximate and precise positions of the Sun    </td></tr>
 <tr class="markdownTableRowEven">
@@ -169,29 +182,29 @@
 <tr class="markdownTableRowEven">
 <td class="markdownTableBodyNone">Calculate   </td><td class="markdownTableBodyNone">Morning and evening twilight    </td></tr>
 <tr class="markdownTableRowOdd">
 <td class="markdownTableBodyNone">Calculate   </td><td class="markdownTableBodyNone">Equation of time    </td></tr>
 <tr class="markdownTableRowEven">
 <td class="markdownTableBodyNone">Calculate   </td><td class="markdownTableBodyNone">Solar elongation   </td></tr>
 </table>
-<h2><a class="anchor" id="autotoc_md138"></a>
+<h2><a class="anchor" id="autotoc_md139"></a>
 Planets</h2>
 <table class="markdownTable">
 <tr class="markdownTableHead">
 <th class="markdownTableHeadNone">Type   </th><th class="markdownTableHeadNone">Description    </th></tr>
 <tr class="markdownTableRowOdd">
 <td class="markdownTableBodyNone">Calculate   </td><td class="markdownTableBodyNone">Approximate and precise position of planet    </td></tr>
 <tr class="markdownTableRowEven">
 <td class="markdownTableBodyNone">Calculate   </td><td class="markdownTableBodyNone">Visual aspects of planet (distance, angular diameter, phase, light time, position angle of bright limb, and apparent magnitude)    </td></tr>
 <tr class="markdownTableRowOdd">
 <td class="markdownTableBodyNone">Calculate   </td><td class="markdownTableBodyNone">Position of comet (elliptical and parabolic)    </td></tr>
 <tr class="markdownTableRowEven">
 <td class="markdownTableBodyNone">Calculate   </td><td class="markdownTableBodyNone">Binary star orbit data   </td></tr>
 </table>
-<h2><a class="anchor" id="autotoc_md139"></a>
+<h2><a class="anchor" id="autotoc_md140"></a>
 The Moon</h2>
 <table class="markdownTable">
 <tr class="markdownTableHead">
 <th class="markdownTableHeadNone">Type   </th><th class="markdownTableHeadNone">Description    </th></tr>
 <tr class="markdownTableRowOdd">
 <td class="markdownTableBodyNone">Calculate   </td><td class="markdownTableBodyNone">Approximate and precise position of Moon    </td></tr>
 <tr class="markdownTableRowEven">
@@ -199,15 +212,15 @@
 <tr class="markdownTableRowOdd">
 <td class="markdownTableBodyNone">Calculate   </td><td class="markdownTableBodyNone">Times of new Moon and full Moon    </td></tr>
 <tr class="markdownTableRowEven">
 <td class="markdownTableBodyNone">Calculate   </td><td class="markdownTableBodyNone">Moon's distance, angular diameter, and horizontal parallax    </td></tr>
 <tr class="markdownTableRowOdd">
 <td class="markdownTableBodyNone">Calculate   </td><td class="markdownTableBodyNone">Local moonrise and moonset   </td></tr>
 </table>
-<h2><a class="anchor" id="autotoc_md140"></a>
+<h2><a class="anchor" id="autotoc_md141"></a>
 Eclipses</h2>
 <table class="markdownTable">
 <tr class="markdownTableHead">
 <th class="markdownTableHeadNone">Type   </th><th class="markdownTableHeadNone">Description    </th></tr>
 <tr class="markdownTableRowOdd">
 <td class="markdownTableBodyNone">Calculate   </td><td class="markdownTableBodyNone">Lunar eclipse occurrence and circumstances    </td></tr>
 <tr class="markdownTableRowEven">
```

#### html2text {}

```diff
@@ -1,18 +1,29 @@
 Practical Astronomy
 practical-astronomy-python
 Algorithms from _P_r_a_c_t_i_c_a_l_ _A_s_t_r_o_n_o_m_y_ _w_i_t_h_ _y_o_u_r_ _C_a_l_c_u_l_a_t_o_r_ _o_r_ _S_p_r_e_a_d_s_h_e_e_t by
 Peter Duffett-Smith, implemented in Python 3. API documentation is published
 _h_e_r_e.
 If you're interested in this topic, please buy the book! It provides far more
 detail and context.
+QQuuiicckk SSttaarrtt
+Install:
+pip install practical-astronomy
+Create easter.py:
+import practical_astronomy.pa_datetime as pd
+print(pd.get_date_of_easter(2024))
+Run it:
+python easter.py
+Result:
+(3, 31, 2024)
 UUnniitt TTeessttss
 If you clone the _r_e_p_o locally, you can run unit tests with the Make utility:
 make all-tests
 LLiibbrraarryy FFuunnccttiioonnss
+Documentation _h_e_r_e.
 DDaattee//TTiimmee
 TTyyppee      DDeessccrriippttiioonn
 Calculate Date of Easter
 Convert   Civil Date to Day Number
 Convert   Greenwich Date <-> Julian Date
 Convert   Julian Date to Day-of-Week
 Extract   Day, Month, and Year parts of Julian Date
```

### Comparing `practical_astronomy-0.0.4/docs/jquery.js` & `practical_astronomy-1.0.0/docs/jquery.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/md_src_glossary.html` & `practical_astronomy-1.0.0/docs/md_src_glossary.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/menu.js` & `practical_astronomy-1.0.0/docs/menu.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/menudata.js` & `practical_astronomy-1.0.0/docs/menudata.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers.html` & `practical_astronomy-1.0.0/docs/namespacemembers.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_b.html` & `practical_astronomy-1.0.0/docs/namespacemembers_b.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_c.html` & `practical_astronomy-1.0.0/docs/namespacemembers_c.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_d.html` & `practical_astronomy-1.0.0/docs/namespacemembers_d.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_dup.js` & `practical_astronomy-1.0.0/docs/namespacemembers_dup.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_e.html` & `practical_astronomy-1.0.0/docs/namespacemembers_e.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_f.html` & `practical_astronomy-1.0.0/docs/namespacemembers_f.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func.js` & `practical_astronomy-1.0.0/docs/namespacemembers_func.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_b.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_b.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_c.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_c.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_d.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_d.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_e.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_e.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_f.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_f.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_g.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_g.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_h.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_h.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_i.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_i.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_j.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_j.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_k.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_k.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_l.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_l.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_m.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_m.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_n.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_n.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_o.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_o.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_p.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_p.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_r.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_r.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_s.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_s.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_t.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_t.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_u.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_u.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_func_v.html` & `practical_astronomy-1.0.0/docs/namespacemembers_func_v.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_g.html` & `practical_astronomy-1.0.0/docs/namespacemembers_g.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_h.html` & `practical_astronomy-1.0.0/docs/namespacemembers_h.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_i.html` & `practical_astronomy-1.0.0/docs/namespacemembers_i.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_j.html` & `practical_astronomy-1.0.0/docs/namespacemembers_j.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_k.html` & `practical_astronomy-1.0.0/docs/namespacemembers_k.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_l.html` & `practical_astronomy-1.0.0/docs/namespacemembers_l.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_m.html` & `practical_astronomy-1.0.0/docs/namespacemembers_m.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_n.html` & `practical_astronomy-1.0.0/docs/namespacemembers_n.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_o.html` & `practical_astronomy-1.0.0/docs/namespacemembers_o.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_p.html` & `practical_astronomy-1.0.0/docs/namespacemembers_p.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_r.html` & `practical_astronomy-1.0.0/docs/namespacemembers_r.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_s.html` & `practical_astronomy-1.0.0/docs/namespacemembers_s.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_t.html` & `practical_astronomy-1.0.0/docs/namespacemembers_t.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_u.html` & `practical_astronomy-1.0.0/docs/namespacemembers_u.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_v.html` & `practical_astronomy-1.0.0/docs/namespacemembers_v.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacemembers_vars.html` & `practical_astronomy-1.0.0/docs/namespacemembers_vars.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacepractical__astronomy.html` & `practical_astronomy-1.0.0/docs/namespacepractical__astronomy.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacepractical__astronomy.js` & `practical_astronomy-1.0.0/docs/namespacepractical__astronomy.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__binary.html` & `practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__binary.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__binary__data.html` & `practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__binary__data.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__comet.html` & `practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__comet.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__comet__data.html` & `practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__comet__data.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__coordinate.html` & `practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__coordinate.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__datetime.html` & `practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__datetime.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__eclipses.html` & `practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__eclipses.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__macro.html` & `practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__macro.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__moon.html` & `practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__moon.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__planet.html` & `practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__planet.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__planet__data.html` & `practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__planet__data.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__sun.html` & `practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__sun.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespacepractical__astronomy_1_1pa__util.html` & `practical_astronomy-1.0.0/docs/namespacepractical__astronomy_1_1pa__util.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/namespaces.html` & `practical_astronomy-1.0.0/docs/namespaces.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/navtree.css` & `practical_astronomy-1.0.0/docs/navtree.css`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/navtree.js` & `practical_astronomy-1.0.0/docs/navtree.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/navtreedata.js` & `practical_astronomy-1.0.0/docs/navtreedata.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -21,22 +21,23 @@
  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
  @licend  The above is the entire license notice for the JavaScript code in this file
 */
 var NAVTREE = [
     ["Practical Astronomy", "index.html", [
         ["practical-astronomy-python", "index.html", [
-            ["Unit Tests", "index.html#autotoc_md133", null],
-            ["Library Functions", "index.html#autotoc_md134", [
-                ["Date/Time", "index.html#autotoc_md135", null],
-                ["Coordinates", "index.html#autotoc_md136", null],
-                ["The Sun", "index.html#autotoc_md137", null],
-                ["Planets", "index.html#autotoc_md138", null],
-                ["The Moon", "index.html#autotoc_md139", null],
-                ["Eclipses", "index.html#autotoc_md140", null]
+            ["Quick Start", "index.html#autotoc_md133", null],
+            ["Unit Tests", "index.html#autotoc_md134", null],
+            ["Library Functions", "index.html#autotoc_md135", [
+                ["Date/Time", "index.html#autotoc_md136", null],
+                ["Coordinates", "index.html#autotoc_md137", null],
+                ["The Sun", "index.html#autotoc_md138", null],
+                ["Planets", "index.html#autotoc_md139", null],
+                ["The Moon", "index.html#autotoc_md140", null],
+                ["Eclipses", "index.html#autotoc_md141", null]
             ]]
         ]],
         ["Glossary of Terms", "md_src_glossary.html", [
             ["aberration", "md_src_glossary.html#autotoc_md1", null],
             ["age of Moon", "md_src_glossary.html#autotoc_md2", null],
             ["altitude", "md_src_glossary.html#autotoc_md3", null],
             ["annual equation", "md_src_glossary.html#autotoc_md4", null],
@@ -181,13 +182,13 @@
             ["File List", "files.html", "files_dup"]
         ]]
     ]]
 ];
 
 var NAVTREEINDEX = [
     "____init_____8py.html",
-    "namespacepractical__astronomy_1_1pa__eclipses.html#a0ac960734a008556789361349956209c",
-    "pa__macro_8py.html#a0f2f9fa28025bfd0727c883df3ce2ab0"
+    "namespacepractical__astronomy_1_1pa__eclipses.html",
+    "pa__macro_8py.html#a0c65bcdf6c40b6921c80f7df8b7ada4e"
 ];
 
 var SYNCONMSG = 'click to disable panel synchronisation';
 var SYNCOFFMSG = 'click to enable panel synchronisation';
```

### Comparing `practical_astronomy-0.0.4/docs/navtreeindex0.js` & `practical_astronomy-1.0.0/docs/navtreeindex0.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -4,20 +4,21 @@
     "dir_68267d1309a1af8e8297ef4c3efbcdba.html": [3, 0, 1],
     "dir_8ebb4883bd5210c1437544ca4cb0df32.html": [3, 0, 0],
     "files.html": [3, 0],
     "index.html": [],
     "index.html": [0],
     "index.html#autotoc_md133": [0, 0],
     "index.html#autotoc_md134": [0, 1],
-    "index.html#autotoc_md135": [0, 1, 0],
-    "index.html#autotoc_md136": [0, 1, 1],
-    "index.html#autotoc_md137": [0, 1, 2],
-    "index.html#autotoc_md138": [0, 1, 3],
-    "index.html#autotoc_md139": [0, 1, 4],
-    "index.html#autotoc_md140": [0, 1, 5],
+    "index.html#autotoc_md135": [0, 2],
+    "index.html#autotoc_md136": [0, 2, 0],
+    "index.html#autotoc_md137": [0, 2, 1],
+    "index.html#autotoc_md138": [0, 2, 2],
+    "index.html#autotoc_md139": [0, 2, 3],
+    "index.html#autotoc_md140": [0, 2, 4],
+    "index.html#autotoc_md141": [0, 2, 5],
     "md_src_glossary.html": [1],
     "md_src_glossary.html#autotoc_md1": [1, 0],
     "md_src_glossary.html#autotoc_md10": [1, 9],
     "md_src_glossary.html#autotoc_md100": [1, 99],
     "md_src_glossary.html#autotoc_md101": [1, 100],
     "md_src_glossary.html#autotoc_md102": [1, 101],
     "md_src_glossary.html#autotoc_md103": [1, 102],
@@ -243,10 +244,9 @@
     "namespacepractical__astronomy_1_1pa__datetime.html#a7a505017515cdadb479fef83039bbad8": [2, 0, 0, 5, 2],
     "namespacepractical__astronomy_1_1pa__datetime.html#a87c359a968e2ffd19d5c7ee78006762e": [2, 0, 0, 5, 1],
     "namespacepractical__astronomy_1_1pa__datetime.html#aa48dfcf90dce9ac086b0b28bd2dbac7b": [2, 0, 0, 5, 15],
     "namespacepractical__astronomy_1_1pa__datetime.html#ab03052b709178a939ecacd357a9b1730": [2, 0, 0, 5, 9],
     "namespacepractical__astronomy_1_1pa__datetime.html#ab1a46eed14594880e25220f9a9675a37": [2, 0, 0, 5, 13],
     "namespacepractical__astronomy_1_1pa__datetime.html#ad329bcbb2bcaf6b6c3d6c0c918936ecf": [2, 0, 0, 5, 8],
     "namespacepractical__astronomy_1_1pa__datetime.html#af03f0a34f5a3205abfced5fb458b99c8": [2, 0, 0, 5, 3],
-    "namespacepractical__astronomy_1_1pa__datetime.html#af6c7751410aa70a76670b144f50dc619": [2, 0, 0, 5, 11],
-    "namespacepractical__astronomy_1_1pa__eclipses.html": [2, 0, 0, 6]
+    "namespacepractical__astronomy_1_1pa__datetime.html#af6c7751410aa70a76670b144f50dc619": [2, 0, 0, 5, 11]
 };
```

### Comparing `practical_astronomy-0.0.4/docs/navtreeindex1.js` & `practical_astronomy-1.0.0/docs/navtreeindex1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,9 @@
 var NAVTREEINDEX1 = {
+    "namespacepractical__astronomy_1_1pa__eclipses.html": [2, 0, 0, 6],
     "namespacepractical__astronomy_1_1pa__eclipses.html#a0ac960734a008556789361349956209c": [2, 0, 0, 6, 1],
     "namespacepractical__astronomy_1_1pa__eclipses.html#a419c3cdc66fdfadb685e0095404e0beb": [2, 0, 0, 6, 3],
     "namespacepractical__astronomy_1_1pa__eclipses.html#a48d5a9475c1877f1268b4d063dd99f6b": [2, 0, 0, 6, 0],
     "namespacepractical__astronomy_1_1pa__eclipses.html#aa5e0b860a6b90ed84dd91644a7db845e": [2, 0, 0, 6, 2],
     "namespacepractical__astronomy_1_1pa__macro.html": [2, 0, 0, 7],
     "namespacepractical__astronomy_1_1pa__macro.html#a045fb010333f74a3359efd9dc69d626d": [2, 0, 0, 7, 74],
     "namespacepractical__astronomy_1_1pa__macro.html#a06c8bb32b88eb03689ba130e17e5e69b": [2, 0, 0, 7, 38],
@@ -243,10 +244,9 @@
     "pa__eclipses_8py.html#a0ac960734a008556789361349956209c": [3, 0, 1, 0, 7, 1],
     "pa__eclipses_8py.html#a419c3cdc66fdfadb685e0095404e0beb": [3, 0, 1, 0, 7, 3],
     "pa__eclipses_8py.html#a48d5a9475c1877f1268b4d063dd99f6b": [3, 0, 1, 0, 7, 0],
     "pa__eclipses_8py.html#aa5e0b860a6b90ed84dd91644a7db845e": [3, 0, 1, 0, 7, 2],
     "pa__macro_8py.html": [3, 0, 1, 0, 8],
     "pa__macro_8py.html#a045fb010333f74a3359efd9dc69d626d": [3, 0, 1, 0, 8, 74],
     "pa__macro_8py.html#a06c8bb32b88eb03689ba130e17e5e69b": [3, 0, 1, 0, 8, 38],
-    "pa__macro_8py.html#a0aa85cbdf3b976861aa96408228319d3": [3, 0, 1, 0, 8, 92],
-    "pa__macro_8py.html#a0c65bcdf6c40b6921c80f7df8b7ada4e": [3, 0, 1, 0, 8, 146]
+    "pa__macro_8py.html#a0aa85cbdf3b976861aa96408228319d3": [3, 0, 1, 0, 8, 92]
 };
```

### Comparing `practical_astronomy-0.0.4/docs/navtreeindex2.js` & `practical_astronomy-1.0.0/docs/navtreeindex2.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,9 @@
 var NAVTREEINDEX2 = {
+    "pa__macro_8py.html#a0c65bcdf6c40b6921c80f7df8b7ada4e": [3, 0, 1, 0, 8, 146],
     "pa__macro_8py.html#a0f2f9fa28025bfd0727c883df3ce2ab0": [3, 0, 1, 0, 8, 90],
     "pa__macro_8py.html#a0fd38430a2b34a11124d7e58da7812f7": [3, 0, 1, 0, 8, 131],
     "pa__macro_8py.html#a105f28dd78c95603fffb2db1984fbe12": [3, 0, 1, 0, 8, 47],
     "pa__macro_8py.html#a15a292cef81b794f9f4b07fb48fbf471": [3, 0, 1, 0, 8, 150],
     "pa__macro_8py.html#a183688ea9868beb50f0227010d223f4d": [3, 0, 1, 0, 8, 42],
     "pa__macro_8py.html#a1919879b878ae9c8051083293912edc6": [3, 0, 1, 0, 8, 33],
     "pa__macro_8py.html#a1b5eac8af576ccd6282b7b7a63c3e89a": [3, 0, 1, 0, 8, 88],
```

### Comparing `practical_astronomy-0.0.4/docs/pa__binary_8py.html` & `practical_astronomy-1.0.0/docs/pa__binary_8py.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pa__binary__data_8py.html` & `practical_astronomy-1.0.0/docs/pa__binary__data_8py.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pa__comet_8py.html` & `practical_astronomy-1.0.0/docs/pa__comet_8py.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pa__comet__data_8py.html` & `practical_astronomy-1.0.0/docs/pa__comet__data_8py.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pa__coordinate_8py.html` & `practical_astronomy-1.0.0/docs/pa__coordinate_8py.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pa__coordinate_8py.js` & `practical_astronomy-1.0.0/docs/pa__coordinate_8py.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pa__datetime_8py.html` & `practical_astronomy-1.0.0/docs/pa__datetime_8py.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pa__datetime_8py.js` & `practical_astronomy-1.0.0/docs/pa__datetime_8py.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pa__eclipses_8py.html` & `practical_astronomy-1.0.0/docs/pa__eclipses_8py.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pa__macro_8py.html` & `practical_astronomy-1.0.0/docs/pa__macro_8py.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pa__macro_8py.js` & `practical_astronomy-1.0.0/docs/pa__macro_8py.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pa__moon_8py.html` & `practical_astronomy-1.0.0/docs/pa__moon_8py.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pa__moon_8py.js` & `practical_astronomy-1.0.0/docs/pa__moon_8py.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pa__planet_8py.html` & `practical_astronomy-1.0.0/docs/pa__planet_8py.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pa__planet__data_8py.html` & `practical_astronomy-1.0.0/docs/pa__planet__data_8py.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pa__sun_8py.html` & `practical_astronomy-1.0.0/docs/pa__sun_8py.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pa__sun_8py.js` & `practical_astronomy-1.0.0/docs/pa__sun_8py.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pa__util_8py.html` & `practical_astronomy-1.0.0/docs/pa__util_8py.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/pages.html` & `practical_astronomy-1.0.0/docs/pages.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/resize.js` & `practical_astronomy-1.0.0/docs/resize.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/sync_off.png` & `practical_astronomy-1.0.0/docs/sync_off.png`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/sync_on.png` & `practical_astronomy-1.0.0/docs/sync_on.png`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/tabs.css` & `practical_astronomy-1.0.0/docs/tabs.css`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_0.html` & `practical_astronomy-1.0.0/docs/search/all_0.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_1.html` & `practical_astronomy-1.0.0/docs/search/all_1.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_1.js` & `practical_astronomy-1.0.0/docs/search/all_1.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_10.html` & `practical_astronomy-1.0.0/docs/search/all_10.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_10.js` & `practical_astronomy-1.0.0/docs/search/all_10.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_11.html` & `practical_astronomy-1.0.0/docs/search/all_11.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_11.js` & `practical_astronomy-1.0.0/docs/search/all_11.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_12.html` & `practical_astronomy-1.0.0/docs/search/all_12.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_12.js` & `practical_astronomy-1.0.0/docs/search/all_12.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_13.html` & `practical_astronomy-1.0.0/docs/search/all_13.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_13.js` & `practical_astronomy-1.0.0/docs/search/all_13.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_14.html` & `practical_astronomy-1.0.0/docs/search/all_14.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_14.js` & `practical_astronomy-1.0.0/docs/search/all_14.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_15.html` & `practical_astronomy-1.0.0/docs/search/all_15.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_2.html` & `practical_astronomy-1.0.0/docs/search/all_2.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_3.html` & `practical_astronomy-1.0.0/docs/search/all_3.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_3.js` & `practical_astronomy-1.0.0/docs/search/all_3.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_4.html` & `practical_astronomy-1.0.0/docs/search/all_4.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_4.js` & `practical_astronomy-1.0.0/docs/search/all_4.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_5.html` & `practical_astronomy-1.0.0/docs/search/all_5.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_5.js` & `practical_astronomy-1.0.0/docs/search/all_5.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_6.html` & `practical_astronomy-1.0.0/docs/search/all_6.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_6.js` & `practical_astronomy-1.0.0/docs/search/all_6.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_7.html` & `practical_astronomy-1.0.0/docs/search/all_7.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_7.js` & `practical_astronomy-1.0.0/docs/search/all_7.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_8.html` & `practical_astronomy-1.0.0/docs/search/all_8.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_8.js` & `practical_astronomy-1.0.0/docs/search/all_8.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_9.html` & `practical_astronomy-1.0.0/docs/search/all_9.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_a.html` & `practical_astronomy-1.0.0/docs/search/all_a.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_a.js` & `practical_astronomy-1.0.0/docs/search/all_a.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_b.html` & `practical_astronomy-1.0.0/docs/search/all_b.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_c.html` & `practical_astronomy-1.0.0/docs/search/all_c.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_c.js` & `practical_astronomy-1.0.0/docs/search/all_c.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_d.html` & `practical_astronomy-1.0.0/docs/search/all_d.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_d.js` & `practical_astronomy-1.0.0/docs/search/all_d.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_e.html` & `practical_astronomy-1.0.0/docs/search/all_e.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_e.js` & `practical_astronomy-1.0.0/docs/search/all_e.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/all_f.html` & `practical_astronomy-1.0.0/docs/search/all_f.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/close.svg` & `practical_astronomy-1.0.0/docs/search/close.svg`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/files_0.html` & `practical_astronomy-1.0.0/docs/search/files_0.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/files_1.html` & `practical_astronomy-1.0.0/docs/search/files_1.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/files_2.html` & `practical_astronomy-1.0.0/docs/search/files_2.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/files_2.js` & `practical_astronomy-1.0.0/docs/search/files_2.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/files_3.html` & `practical_astronomy-1.0.0/docs/search/files_3.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_0.html` & `practical_astronomy-1.0.0/docs/search/functions_0.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_0.js` & `practical_astronomy-1.0.0/docs/search/functions_0.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_1.html` & `practical_astronomy-1.0.0/docs/search/functions_1.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_10.html` & `practical_astronomy-1.0.0/docs/search/functions_10.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_10.js` & `practical_astronomy-1.0.0/docs/search/functions_10.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_11.html` & `practical_astronomy-1.0.0/docs/search/functions_11.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_11.js` & `practical_astronomy-1.0.0/docs/search/functions_11.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_12.html` & `practical_astronomy-1.0.0/docs/search/functions_12.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_12.js` & `practical_astronomy-1.0.0/docs/search/functions_12.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_13.html` & `practical_astronomy-1.0.0/docs/search/functions_13.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_13.js` & `practical_astronomy-1.0.0/docs/search/functions_13.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_14.html` & `practical_astronomy-1.0.0/docs/search/functions_14.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_2.html` & `practical_astronomy-1.0.0/docs/search/functions_2.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_2.js` & `practical_astronomy-1.0.0/docs/search/functions_2.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_3.html` & `practical_astronomy-1.0.0/docs/search/functions_3.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_3.js` & `practical_astronomy-1.0.0/docs/search/functions_3.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_4.html` & `practical_astronomy-1.0.0/docs/search/functions_4.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_4.js` & `practical_astronomy-1.0.0/docs/search/functions_4.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_5.html` & `practical_astronomy-1.0.0/docs/search/functions_5.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_5.js` & `practical_astronomy-1.0.0/docs/search/functions_5.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_6.html` & `practical_astronomy-1.0.0/docs/search/functions_6.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_6.js` & `practical_astronomy-1.0.0/docs/search/functions_6.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_7.html` & `practical_astronomy-1.0.0/docs/search/functions_7.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_7.js` & `practical_astronomy-1.0.0/docs/search/functions_7.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_8.html` & `practical_astronomy-1.0.0/docs/search/functions_8.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_9.html` & `practical_astronomy-1.0.0/docs/search/functions_9.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_9.js` & `practical_astronomy-1.0.0/docs/search/functions_9.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_a.html` & `practical_astronomy-1.0.0/docs/search/functions_a.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_b.html` & `practical_astronomy-1.0.0/docs/search/functions_b.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_b.js` & `practical_astronomy-1.0.0/docs/search/functions_b.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_c.html` & `practical_astronomy-1.0.0/docs/search/functions_c.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_c.js` & `practical_astronomy-1.0.0/docs/search/functions_c.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_d.html` & `practical_astronomy-1.0.0/docs/search/functions_d.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_d.js` & `practical_astronomy-1.0.0/docs/search/functions_d.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_e.html` & `practical_astronomy-1.0.0/docs/search/functions_e.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_f.html` & `practical_astronomy-1.0.0/docs/search/functions_f.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/functions_f.js` & `practical_astronomy-1.0.0/docs/search/functions_f.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/mag_sel.svg` & `practical_astronomy-1.0.0/docs/search/mag_sel.svg`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/namespaces_0.html` & `practical_astronomy-1.0.0/docs/search/namespaces_0.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/namespaces_0.js` & `practical_astronomy-1.0.0/docs/search/namespaces_0.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/pages_0.html` & `practical_astronomy-1.0.0/docs/search/pages_0.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/pages_1.html` & `practical_astronomy-1.0.0/docs/search/pages_1.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/search.css` & `practical_astronomy-1.0.0/docs/search/search.css`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/search.js` & `practical_astronomy-1.0.0/docs/search/search.js`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/search_l.png` & `practical_astronomy-1.0.0/docs/search/search_l.png`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/search_r.png` & `practical_astronomy-1.0.0/docs/search/search_r.png`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/variables_0.html` & `practical_astronomy-1.0.0/docs/search/variables_0.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/variables_1.html` & `practical_astronomy-1.0.0/docs/search/variables_1.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs/search/variables_2.html` & `practical_astronomy-1.0.0/docs/search/variables_2.html`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs-gen/Doxyfile` & `practical_astronomy-1.0.0/docs-gen/Doxyfile`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/docs-gen/src/glossary.md` & `practical_astronomy-1.0.0/docs-gen/src/glossary.md`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/src/practical_astronomy/pa_binary.py` & `practical_astronomy-1.0.0/src/practical_astronomy/pa_binary.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/src/practical_astronomy/pa_binary_data.py` & `practical_astronomy-1.0.0/src/practical_astronomy/pa_binary_data.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/src/practical_astronomy/pa_comet.py` & `practical_astronomy-1.0.0/src/practical_astronomy/pa_comet.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/src/practical_astronomy/pa_comet_data.py` & `practical_astronomy-1.0.0/src/practical_astronomy/pa_comet_data.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/src/practical_astronomy/pa_coordinate.py` & `practical_astronomy-1.0.0/src/practical_astronomy/pa_coordinate.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/src/practical_astronomy/pa_datetime.py` & `practical_astronomy-1.0.0/src/practical_astronomy/pa_datetime.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/src/practical_astronomy/pa_eclipses.py` & `practical_astronomy-1.0.0/src/practical_astronomy/pa_eclipses.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/src/practical_astronomy/pa_macro.py` & `practical_astronomy-1.0.0/src/practical_astronomy/pa_macro.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/src/practical_astronomy/pa_moon.py` & `practical_astronomy-1.0.0/src/practical_astronomy/pa_moon.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/src/practical_astronomy/pa_planet.py` & `practical_astronomy-1.0.0/src/practical_astronomy/pa_planet.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/src/practical_astronomy/pa_planet_data.py` & `practical_astronomy-1.0.0/src/practical_astronomy/pa_planet_data.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/src/practical_astronomy/pa_sun.py` & `practical_astronomy-1.0.0/src/practical_astronomy/pa_sun.py`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/LICENSE` & `practical_astronomy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/README.md` & `practical_astronomy-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `practical_astronomy-0.0.4/pyproject.toml` & `practical_astronomy-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "practical-astronomy"
-version = "0.0.4"
+version = "1.0.0"
 authors = [{ name = "Jim Carr", email = "jfcarr@gmail.com" }]
 description = "Algorithms from Practical Astronomy, implemented in Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `practical_astronomy-0.0.4/PKG-INFO` & `practical_astronomy-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: practical-astronomy
-Version: 0.0.4
+Version: 1.0.0
 Summary: Algorithms from Practical Astronomy, implemented in Python
 Project-URL: Homepage, https://github.com/jfcarr/practical-astronomy-python
 Project-URL: Issues, https://github.com/jfcarr/practical-astronomy-python/issues
 Project-URL: Documentation, https://jfcarr.github.io/practical-astronomy-python
 Author-email: Jim Carr <jfcarr@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

