# Comparing `tmp/phono3py-3.0.0.tar.gz` & `tmp/phono3py-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phono3py-3.0.0.tar", last modified: Fri Apr 19 08:24:44 2024, max compression
+gzip compressed data, was "phono3py-3.0.1.tar", last modified: Sat Apr 20 08:15:34 2024, max compression
```

## Comparing `phono3py-3.0.0.tar` & `phono3py-3.0.1.tar`

### file list

```diff
@@ -1,262 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.540895 phono3py-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-19 08:23:43.000000 phono3py-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-19 08:23:43.000000 phono3py-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-19 08:24:44.540895 phono3py-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-19 08:23:43.000000 phono3py-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 08:24:39.000000 phono3py-3.0.0/__nanoversion__.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.508894 phono3py-3.0.0/c/
--rw-r--r--   0 runner    (1001) docker     (127)    68786 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/_phono3py.c
--rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/_phononcalc.c
--rw-r--r--   0 runner    (1001) docker     (127)    15045 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/bzgrid.c
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/bzgrid.h
--rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/collision_matrix.c
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/collision_matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    29801 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/dynmat.c
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/dynmat.h
--rw-r--r--   0 runner    (1001) docker     (127)    23953 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/fc3.c
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/fc3.h
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/grgrid.c
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/grgrid.h
--rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/gridsys.c
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/gridsys.h
--rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/imag_self_energy_with_g.c
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/imag_self_energy_with_g.h
--rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/interaction.c
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/interaction.h
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/isotope.c
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/isotope.h
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/lagrid.c
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/lagrid.h
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/lapack_wrapper.c
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/lapack_wrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/niggli.c
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/niggli.h
--rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phono3py.c
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phono3py.h
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phonoc_array.h
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phonoc_const.h
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phonoc_utils.c
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phonoc_utils.h
--rw-r--r--   0 runner    (1001) docker     (127)    20519 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phonon.c
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phonon.h
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phononcalc.c
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phononcalc.h
--rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/pp_collision.c
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/pp_collision.h
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/real_self_energy.c
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/real_self_energy.h
--rw-r--r--   0 runner    (1001) docker     (127)    16752 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/real_to_reciprocal.c
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/real_to_reciprocal.h
--rw-r--r--   0 runner    (1001) docker     (127)    11975 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/reciprocal_to_normal.c
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/reciprocal_to_normal.h
--rw-r--r--   0 runner    (1001) docker     (127)    14689 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/snf3x3.c
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/snf3x3.h
--rw-r--r--   0 runner    (1001) docker     (127)    38926 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/tetrahedron_method.c
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/tetrahedron_method.h
--rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/triplet.c
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/triplet.h
--rw-r--r--   0 runner    (1001) docker     (127)    18558 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/triplet_grid.c
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/triplet_grid.h
--rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/triplet_iw.c
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/triplet_iw.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.488894 phono3py-3.0.0/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.512894 phono3py-3.0.0/example/AlN-LDA/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/AlN-LDA/BORN
--rw-r--r--   0 runner    (1001) docker     (127)    86886 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/AlN-LDA/FORCES_FC2
--rw-r--r--   0 runner    (1001) docker     (127)   862253 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/AlN-LDA/FORCES_FC3.lzma
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/AlN-LDA/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/AlN-LDA/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   143873 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/AlN-LDA/phono3py_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   176702 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/AlN-LDA/phono3py_disp_dimfc2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.512894 phono3py-3.0.0/example/NaCl-alm/
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/NaCl-alm/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   303332 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/NaCl-alm/phono3py_params_NaCl222.yaml.xz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.512894 phono3py-3.0.0/example/Si-CRYSTAL/
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-CRYSTAL/FORCES_FC2
--rw-r--r--   0 runner    (1001) docker     (127)    52417 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-CRYSTAL/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-CRYSTAL/README
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-CRYSTAL/TEMPLATE
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-CRYSTAL/TEMPLATE3
--rw-r--r--   0 runner    (1001) docker     (127)    50060 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-CRYSTAL/crystal.o
--rw-r--r--   0 runner    (1001) docker     (127)   801243 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-CRYSTAL/outputs.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.516894 phono3py-3.0.0/example/Si-LDA/
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-LDA/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-LDA/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-LDA/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-LDA/phono3py_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   305364 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-LDA/vasprun_xmls.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.516894 phono3py-3.0.0/example/Si-PBE/
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBE/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBE/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBE/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBE/phono3py_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   314724 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBE/vasprun_xmls.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.520894 phono3py-3.0.0/example/Si-PBEsol/
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    46793 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/Si-band-DOS.png
--rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/Si-kaccum.png
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/Si.py
--rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/phono3py_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    95766 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/phono3py_disp_dimfc2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.488894 phono3py-3.0.0/example/Si-PBEsol/vasprun_xml_fc2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.520894 phono3py-3.0.0/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/INCAR
--rw-r--r--   0 runner    (1001) docker     (127)    31479 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)   291058 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/vasprun.xml
--rw-r--r--   0 runner    (1001) docker     (127)   300636 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/vasprun_xmls.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.520894 phono3py-3.0.0/example/Si-QE/
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-QE/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-QE/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-QE/Si.in
--rw-r--r--   0 runner    (1001) docker     (127)    32833 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-QE/phono3py_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   150928 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-QE/supercell_out.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.524894 phono3py-3.0.0/example/Si-TURBOMOLE/
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-TURBOMOLE/FORCES_FC2
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-TURBOMOLE/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-TURBOMOLE/README
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-TURBOMOLE/control
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-TURBOMOLE/coord
--rw-r--r--   0 runner    (1001) docker     (127)   278495 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-TURBOMOLE/outputs.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.528895 phono3py-3.0.0/example/Wigner_La2Zr2O7/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Wigner_La2Zr2O7/BORN
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Wigner_La2Zr2O7/POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Wigner_La2Zr2O7/command.sh
--rw-r--r--   0 runner    (1001) docker     (127)  1098761 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Wigner_La2Zr2O7/fc2.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)   339529 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Wigner_La2Zr2O7/kappa-m191919.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)   160648 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Wigner_La2Zr2O7/tc_La2Zr2O7.out.xz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.528895 phono3py-3.0.0/example/zb-ZnTe-PBEsol/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/zb-ZnTe-PBEsol/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/zb-ZnTe-PBEsol/launch_phono3py_ZnTe_PBEsol_222.py
--rw-r--r--   0 runner    (1001) docker     (127)   131412 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/zb-ZnTe-PBEsol/phono3py_params_ZnTe.yaml.xz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.492894 phono3py-3.0.0/phono3py/
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/api_isotope.py
--rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/api_jointdos.py
--rw-r--r--   0 runner    (1001) docker     (127)    87780 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/api_phono3py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.492894 phono3py-3.0.0/phono3py/conductivity/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/conductivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31851 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/conductivity/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    71606 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/conductivity/direct_solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/conductivity/kubo.py
--rw-r--r--   0 runner    (1001) docker     (127)    41437 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/conductivity/rta.py
--rw-r--r--   0 runner    (1001) docker     (127)    44752 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/conductivity/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/conductivity/wigner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.496894 phono3py-3.0.0/phono3py/cui/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20611 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/create_force_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/create_supercells.py
--rw-r--r--   0 runner    (1001) docker     (127)    14312 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/kaccum_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    24757 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/load.py
--rw-r--r--   0 runner    (1001) docker     (127)    24731 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/phono3py_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    51088 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/phono3py_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    37210 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/show_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/triplets_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    58029 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/file_IO.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.496894 phono3py-3.0.0/phono3py/interface/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/interface/alm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/interface/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/interface/fc_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22585 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/interface/phono3py_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.496894 phono3py-3.0.0/phono3py/other/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14016 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/other/isotope.py
--rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/other/kaccum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/other/tetrahedron_method.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.496894 phono3py-3.0.0/phono3py/phonon/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon/func.py
--rw-r--r--   0 runner    (1001) docker     (127)    42765 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon/group_velocity_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon/heat_capacity_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon/velocity_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.500894 phono3py-3.0.0/phono3py/phonon3/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/collision_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/displacement_fc3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30148 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/fc3.py
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/gruneisen.py
--rw-r--r--   0 runner    (1001) docker     (127)    38050 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/imag_self_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    37969 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    15753 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/joint_dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    25948 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/real_self_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/real_to_reciprocal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/reciprocal_to_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/spectral_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    14879 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/triplets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.500894 phono3py-3.0.0/phono3py/sscha/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/sscha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19518 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/sscha/sscha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.540895 phono3py-3.0.0/phono3py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-19 08:24:44.000000 phono3py-3.0.0/phono3py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-19 08:24:44.000000 phono3py-3.0.0/phono3py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:24:44.000000 phono3py-3.0.0/phono3py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-19 08:24:44.000000 phono3py-3.0.0/phono3py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 08:24:44.000000 phono3py-3.0.0/phono3py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-19 08:23:43.000000 phono3py-3.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.528895 phono3py-3.0.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1831 2024-04-19 08:23:43.000000 phono3py-3.0.0/scripts/phono3py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3845 2024-04-19 08:23:43.000000 phono3py-3.0.0/scripts/phono3py-coleigplot
--rwxr-xr-x   0 runner    (1001) docker     (127)     1688 2024-04-19 08:23:43.000000 phono3py-3.0.0/scripts/phono3py-kaccum
--rwxr-xr-x   0 runner    (1001) docker     (127)     9488 2024-04-19 08:23:43.000000 phono3py-3.0.0/scripts/phono3py-kdeplot
--rwxr-xr-x   0 runner    (1001) docker     (127)     1797 2024-04-19 08:23:43.000000 phono3py-3.0.0/scripts/phono3py-load
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-19 08:24:44.540895 phono3py-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-04-19 08:23:43.000000 phono3py-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.532895 phono3py-3.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/AgNO2_cell.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/BORN_NaCl
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/FORCES_FC3_si_pbesol
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/FORCE_SETS_NaCl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.532895 phono3py-3.0.0/test/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/api/test_api_phono3py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.536895 phono3py-3.0.0/test/conductivity/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/conductivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/conductivity/test_kappa_LBTE.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/conductivity/test_kappa_LBTE_Wigner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/conductivity/test_kappa_RTA.py
--rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/conductivity/test_kappa_RTA_Wigner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.536895 phono3py-3.0.0/test/cui/
--rw-r--r--   0 runner    (1001) docker     (127)    62552 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/cui/phono3py_params-qe-Si222.yaml.xz
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/cui/test_phono3py_load_script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.536895 phono3py-3.0.0/test/file_IO/
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/file_IO/test_file_IO.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.536895 phono3py-3.0.0/test/interface/
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/interface/test_phono3py_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.536895 phono3py-3.0.0/test/other/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/other/test_isotope.py
--rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/other/test_kaccum.py
--rw-r--r--   0 runner    (1001) docker     (127)   177468 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phono3py_params-Si111-rd.yaml.xz
--rw-r--r--   0 runner    (1001) docker     (127)   943848 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phono3py_params_AlN332.yaml.xz
--rw-r--r--   0 runner    (1001) docker     (127)    26352 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phono3py_params_NaCl111.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    69120 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phono3py_params_NaCl222.yaml.xz
--rw-r--r--   0 runner    (1001) docker     (127)    30693 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phono3py_params_Si-111-222.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    18216 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phono3py_params_Si111.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    32800 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phono3py_si_pbesol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.536895 phono3py-3.0.0/test/phonon/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51828 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    19747 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon/test_velocity_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.540895 phono3py-3.0.0/test/phonon3/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/test_displacements.py
--rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/test_fc3.py
--rw-r--r--   0 runner    (1001) docker     (127)    47987 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/test_imag_self_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/test_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/test_joint_dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    19498 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/test_real_self_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19561 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/test_spectral_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    41126 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/test_triplets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12203 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonopy_disp_NaCl.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   286407 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonopy_params-Si111-iterha.yaml.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonopy_params_Si.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.540895 phono3py-3.0.0/test/sscha/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/sscha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/sscha/test_sscha.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.615732 phono3py-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-20 08:14:40.000000 phono3py-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-20 08:14:40.000000 phono3py-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-20 08:15:34.615732 phono3py-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-20 08:14:40.000000 phono3py-3.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 08:15:29.000000 phono3py-3.0.1/__nanoversion__.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.587732 phono3py-3.0.1/c/
+-rw-r--r--   0 runner    (1001) docker     (127)    68786 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/_phono3py.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/_phononcalc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15045 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/bzgrid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/bzgrid.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/collision_matrix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/collision_matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29801 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/dynmat.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/dynmat.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23953 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/fc3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/fc3.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/grgrid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/grgrid.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/gridsys.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/gridsys.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/imag_self_energy_with_g.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/imag_self_energy_with_g.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/interaction.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/interaction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/isotope.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/isotope.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/lagrid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/lagrid.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/lapack_wrapper.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/lapack_wrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/niggli.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/niggli.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/phono3py.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/phono3py.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/phonoc_array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/phonoc_const.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/phonoc_utils.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/phonoc_utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20519 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/phonon.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/phonon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/phononcalc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/phononcalc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/pp_collision.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/pp_collision.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/real_self_energy.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/real_self_energy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16752 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/real_to_reciprocal.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/real_to_reciprocal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11995 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/reciprocal_to_normal.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/reciprocal_to_normal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14689 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/snf3x3.c
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/snf3x3.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38926 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/tetrahedron_method.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/tetrahedron_method.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/triplet.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/triplet.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18558 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/triplet_grid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/triplet_grid.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/triplet_iw.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-20 08:14:40.000000 phono3py-3.0.1/c/triplet_iw.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.563732 phono3py-3.0.1/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.587732 phono3py-3.0.1/example/AlN-LDA/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/AlN-LDA/BORN
+-rw-r--r--   0 runner    (1001) docker     (127)    86886 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/AlN-LDA/FORCES_FC2
+-rw-r--r--   0 runner    (1001) docker     (127)   862253 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/AlN-LDA/FORCES_FC3.lzma
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/AlN-LDA/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/AlN-LDA/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   143873 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/AlN-LDA/phono3py_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   176702 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/AlN-LDA/phono3py_disp_dimfc2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.587732 phono3py-3.0.1/example/NaCl-alm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/NaCl-alm/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   303332 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/NaCl-alm/phono3py_params_NaCl222.yaml.xz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.591732 phono3py-3.0.1/example/Si-CRYSTAL/
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-CRYSTAL/FORCES_FC2
+-rw-r--r--   0 runner    (1001) docker     (127)    52417 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-CRYSTAL/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-CRYSTAL/README
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-CRYSTAL/TEMPLATE
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-CRYSTAL/TEMPLATE3
+-rw-r--r--   0 runner    (1001) docker     (127)    50060 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-CRYSTAL/crystal.o
+-rw-r--r--   0 runner    (1001) docker     (127)   801243 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-CRYSTAL/outputs.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.591732 phono3py-3.0.1/example/Si-LDA/
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-LDA/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-LDA/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-LDA/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-LDA/phono3py_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   305364 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-LDA/vasprun_xmls.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.595732 phono3py-3.0.1/example/Si-PBE/
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-PBE/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-PBE/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-PBE/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-PBE/phono3py_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   314724 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-PBE/vasprun_xmls.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.595732 phono3py-3.0.1/example/Si-PBEsol/
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-PBEsol/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-PBEsol/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-PBEsol/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    46793 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-PBEsol/Si-band-DOS.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-PBEsol/Si-kaccum.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-PBEsol/Si.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-PBEsol/phono3py_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    95766 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-PBEsol/phono3py_disp_dimfc2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.563732 phono3py-3.0.1/example/Si-PBEsol/vasprun_xml_fc2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.595732 phono3py-3.0.1/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/INCAR
+-rw-r--r--   0 runner    (1001) docker     (127)    31479 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)   291058 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/vasprun.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   300636 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-PBEsol/vasprun_xmls.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.599732 phono3py-3.0.1/example/Si-QE/
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-QE/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-QE/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-QE/Si.in
+-rw-r--r--   0 runner    (1001) docker     (127)    32833 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-QE/phono3py_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   150928 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-QE/supercell_out.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.599732 phono3py-3.0.1/example/Si-TURBOMOLE/
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-TURBOMOLE/FORCES_FC2
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-TURBOMOLE/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-TURBOMOLE/README
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-TURBOMOLE/control
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-TURBOMOLE/coord
+-rw-r--r--   0 runner    (1001) docker     (127)   278495 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Si-TURBOMOLE/outputs.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.603732 phono3py-3.0.1/example/Wigner_La2Zr2O7/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Wigner_La2Zr2O7/BORN
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Wigner_La2Zr2O7/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Wigner_La2Zr2O7/command.sh
+-rw-r--r--   0 runner    (1001) docker     (127)  1098761 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Wigner_La2Zr2O7/fc2.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)   339529 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Wigner_La2Zr2O7/kappa-m191919.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)   160648 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/Wigner_La2Zr2O7/tc_La2Zr2O7.out.xz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.603732 phono3py-3.0.1/example/zb-ZnTe-PBEsol/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/zb-ZnTe-PBEsol/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/zb-ZnTe-PBEsol/launch_phono3py_ZnTe_PBEsol_222.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131412 2024-04-20 08:14:40.000000 phono3py-3.0.1/example/zb-ZnTe-PBEsol/phono3py_params_ZnTe.yaml.xz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.567732 phono3py-3.0.1/phono3py/
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/api_isotope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/api_jointdos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87780 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/api_phono3py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.571732 phono3py-3.0.1/phono3py/conductivity/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/conductivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31851 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/conductivity/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71606 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/conductivity/direct_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/conductivity/kubo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41437 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/conductivity/rta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44752 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/conductivity/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/conductivity/wigner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.571732 phono3py-3.0.1/phono3py/cui/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/cui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20611 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/cui/create_force_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/cui/create_supercells.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14312 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/cui/kaccum_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24757 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/cui/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24731 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/cui/phono3py_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51088 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/cui/phono3py_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37210 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/cui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/cui/show_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/cui/triplets_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58029 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/file_IO.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.571732 phono3py-3.0.1/phono3py/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/interface/alm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/interface/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/interface/fc_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22585 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/interface/phono3py_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.571732 phono3py-3.0.1/phono3py/other/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14016 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/other/isotope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/other/kaccum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/other/tetrahedron_method.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.575732 phono3py-3.0.1/phono3py/phonon/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42765 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon/group_velocity_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon/heat_capacity_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon/velocity_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.575732 phono3py-3.0.1/phono3py/phonon3/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon3/collision_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon3/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon3/displacement_fc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30148 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon3/fc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon3/gruneisen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38050 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon3/imag_self_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37969 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon3/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15753 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon3/joint_dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25948 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon3/real_self_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon3/real_to_reciprocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon3/reciprocal_to_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon3/spectral_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14879 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/phonon3/triplets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.575732 phono3py-3.0.1/phono3py/sscha/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/sscha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19518 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/sscha/sscha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-20 08:14:40.000000 phono3py-3.0.1/phono3py/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.615732 phono3py-3.0.1/phono3py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-20 08:15:34.000000 phono3py-3.0.1/phono3py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-20 08:15:34.000000 phono3py-3.0.1/phono3py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 08:15:34.000000 phono3py-3.0.1/phono3py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-20 08:15:34.000000 phono3py-3.0.1/phono3py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 08:15:34.000000 phono3py-3.0.1/phono3py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-20 08:14:40.000000 phono3py-3.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.607732 phono3py-3.0.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1831 2024-04-20 08:14:40.000000 phono3py-3.0.1/scripts/phono3py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3845 2024-04-20 08:14:40.000000 phono3py-3.0.1/scripts/phono3py-coleigplot
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1688 2024-04-20 08:14:40.000000 phono3py-3.0.1/scripts/phono3py-kaccum
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9488 2024-04-20 08:14:40.000000 phono3py-3.0.1/scripts/phono3py-kdeplot
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1797 2024-04-20 08:14:40.000000 phono3py-3.0.1/scripts/phono3py-load
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-20 08:15:34.615732 phono3py-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-04-20 08:14:40.000000 phono3py-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.611732 phono3py-3.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/AgNO2_cell.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/BORN_NaCl
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/FORCES_FC3_si_pbesol
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/FORCE_SETS_NaCl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.611732 phono3py-3.0.1/test/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/api/test_api_phono3py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.611732 phono3py-3.0.1/test/conductivity/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/conductivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/conductivity/test_kappa_LBTE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/conductivity/test_kappa_LBTE_Wigner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/conductivity/test_kappa_RTA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/conductivity/test_kappa_RTA_Wigner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.611732 phono3py-3.0.1/test/cui/
+-rw-r--r--   0 runner    (1001) docker     (127)    62552 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/cui/phono3py_params-qe-Si222.yaml.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/cui/test_phono3py_load_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.611732 phono3py-3.0.1/test/file_IO/
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/file_IO/test_file_IO.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.611732 phono3py-3.0.1/test/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/interface/test_phono3py_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.611732 phono3py-3.0.1/test/other/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/other/test_isotope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/other/test_kaccum.py
+-rw-r--r--   0 runner    (1001) docker     (127)   177468 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phono3py_params-Si111-rd.yaml.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   943848 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phono3py_params_AlN332.yaml.xz
+-rw-r--r--   0 runner    (1001) docker     (127)    26352 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phono3py_params_NaCl111.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    69120 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phono3py_params_NaCl222.yaml.xz
+-rw-r--r--   0 runner    (1001) docker     (127)    30693 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phono3py_params_Si-111-222.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    18216 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phono3py_params_Si111.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    32800 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phono3py_si_pbesol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.611732 phono3py-3.0.1/test/phonon/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51828 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phonon/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19747 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phonon/test_velocity_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.615732 phono3py-3.0.1/test/phonon3/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phonon3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phonon3/test_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phonon3/test_fc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47987 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phonon3/test_imag_self_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phonon3/test_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phonon3/test_joint_dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19498 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phonon3/test_real_self_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19561 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phonon3/test_spectral_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41126 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phonon3/test_triplets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12203 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phonopy_disp_NaCl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   286407 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phonopy_params-Si111-iterha.yaml.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/phonopy_params_Si.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:15:34.615732 phono3py-3.0.1/test/sscha/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/sscha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-04-20 08:14:40.000000 phono3py-3.0.1/test/sscha/test_sscha.py
```

### Comparing `phono3py-3.0.0/LICENSE` & `phono3py-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/README.md` & `phono3py-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/_phono3py.c` & `phono3py-3.0.1/c/_phono3py.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/_phononcalc.c` & `phono3py-3.0.1/c/_phononcalc.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/bzgrid.c` & `phono3py-3.0.1/c/bzgrid.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/bzgrid.h` & `phono3py-3.0.1/c/bzgrid.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/collision_matrix.c` & `phono3py-3.0.1/c/collision_matrix.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/collision_matrix.h` & `phono3py-3.0.1/c/collision_matrix.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/dynmat.c` & `phono3py-3.0.1/c/dynmat.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/dynmat.h` & `phono3py-3.0.1/c/dynmat.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/fc3.c` & `phono3py-3.0.1/c/fc3.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/fc3.h` & `phono3py-3.0.1/c/fc3.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/grgrid.c` & `phono3py-3.0.1/c/grgrid.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/grgrid.h` & `phono3py-3.0.1/c/grgrid.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/gridsys.c` & `phono3py-3.0.1/c/gridsys.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/gridsys.h` & `phono3py-3.0.1/c/gridsys.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/imag_self_energy_with_g.c` & `phono3py-3.0.1/c/imag_self_energy_with_g.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/imag_self_energy_with_g.h` & `phono3py-3.0.1/c/imag_self_energy_with_g.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/interaction.c` & `phono3py-3.0.1/c/interaction.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/interaction.h` & `phono3py-3.0.1/c/interaction.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/isotope.c` & `phono3py-3.0.1/c/isotope.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/isotope.h` & `phono3py-3.0.1/c/isotope.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/lagrid.c` & `phono3py-3.0.1/c/lagrid.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/lagrid.h` & `phono3py-3.0.1/c/lagrid.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/lapack_wrapper.c` & `phono3py-3.0.1/c/lapack_wrapper.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/lapack_wrapper.h` & `phono3py-3.0.1/c/lapack_wrapper.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/niggli.c` & `phono3py-3.0.1/c/niggli.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/niggli.h` & `phono3py-3.0.1/c/niggli.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/phono3py.c` & `phono3py-3.0.1/c/phono3py.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/phono3py.h` & `phono3py-3.0.1/c/phono3py.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/phonoc_array.h` & `phono3py-3.0.1/c/phonoc_array.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/phonoc_const.h` & `phono3py-3.0.1/c/phonoc_const.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/phonoc_utils.c` & `phono3py-3.0.1/c/phonoc_utils.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/phonoc_utils.h` & `phono3py-3.0.1/c/phonoc_utils.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/phonon.c` & `phono3py-3.0.1/c/phonon.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/phonon.h` & `phono3py-3.0.1/c/phonon.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/phononcalc.c` & `phono3py-3.0.1/c/phononcalc.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/phononcalc.h` & `phono3py-3.0.1/c/phononcalc.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/pp_collision.c` & `phono3py-3.0.1/c/pp_collision.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/pp_collision.h` & `phono3py-3.0.1/c/pp_collision.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/real_self_energy.c` & `phono3py-3.0.1/c/real_self_energy.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/real_self_energy.h` & `phono3py-3.0.1/c/real_self_energy.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/real_to_reciprocal.c` & `phono3py-3.0.1/c/real_to_reciprocal.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/real_to_reciprocal.h` & `phono3py-3.0.1/c/real_to_reciprocal.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/reciprocal_to_normal.c` & `phono3py-3.0.1/c/reciprocal_to_normal.c`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 #if defined(MKL_LAPACKE) || defined(SCIPY_MKL_H)
 #include <mkl_cblas.h>
 #else
 #include <cblas.h>
 #endif
 #include <math.h>
 #include <stdlib.h>
+#include <string.h>
 
 #include "lapack_wrapper.h"
 
 #ifdef MEASURE_R2N
 #include <time.h>
 #include <unistd.h>
 #endif
```

### Comparing `phono3py-3.0.0/c/reciprocal_to_normal.h` & `phono3py-3.0.1/c/reciprocal_to_normal.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/snf3x3.c` & `phono3py-3.0.1/c/snf3x3.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/tetrahedron_method.c` & `phono3py-3.0.1/c/tetrahedron_method.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/tetrahedron_method.h` & `phono3py-3.0.1/c/tetrahedron_method.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/triplet.c` & `phono3py-3.0.1/c/triplet.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/triplet.h` & `phono3py-3.0.1/c/triplet.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/triplet_grid.c` & `phono3py-3.0.1/c/triplet_grid.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/triplet_grid.h` & `phono3py-3.0.1/c/triplet_grid.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/triplet_iw.c` & `phono3py-3.0.1/c/triplet_iw.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/c/triplet_iw.h` & `phono3py-3.0.1/c/triplet_iw.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/AlN-LDA/FORCES_FC2` & `phono3py-3.0.1/example/AlN-LDA/FORCES_FC2`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/AlN-LDA/FORCES_FC3.lzma` & `phono3py-3.0.1/example/AlN-LDA/FORCES_FC3.lzma`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/AlN-LDA/README.md` & `phono3py-3.0.1/example/AlN-LDA/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/AlN-LDA/phono3py_disp.yaml` & `phono3py-3.0.1/example/AlN-LDA/phono3py_disp.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/AlN-LDA/phono3py_disp_dimfc2.yaml` & `phono3py-3.0.1/example/AlN-LDA/phono3py_disp_dimfc2.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/NaCl-alm/README.md` & `phono3py-3.0.1/example/NaCl-alm/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/NaCl-alm/phono3py_params_NaCl222.yaml.xz` & `phono3py-3.0.1/example/NaCl-alm/phono3py_params_NaCl222.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-CRYSTAL/FORCES_FC2` & `phono3py-3.0.1/example/Si-CRYSTAL/FORCES_FC2`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-CRYSTAL/FORCES_FC3` & `phono3py-3.0.1/example/Si-CRYSTAL/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-CRYSTAL/README` & `phono3py-3.0.1/example/Si-CRYSTAL/README`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-CRYSTAL/TEMPLATE` & `phono3py-3.0.1/example/Si-CRYSTAL/TEMPLATE`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-CRYSTAL/TEMPLATE3` & `phono3py-3.0.1/example/Si-CRYSTAL/TEMPLATE3`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-CRYSTAL/crystal.o` & `phono3py-3.0.1/example/Si-CRYSTAL/crystal.o`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-CRYSTAL/outputs.tar.gz` & `phono3py-3.0.1/example/Si-CRYSTAL/outputs.tar.gz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-LDA/FORCES_FC3` & `phono3py-3.0.1/example/Si-LDA/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-LDA/POSCAR-unitcell` & `phono3py-3.0.1/example/Si-LDA/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-LDA/README.md` & `phono3py-3.0.1/example/Si-LDA/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-LDA/phono3py_disp.yaml` & `phono3py-3.0.1/example/Si-LDA/phono3py_disp.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-LDA/vasprun_xmls.tar.lzma` & `phono3py-3.0.1/example/Si-LDA/vasprun_xmls.tar.lzma`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-PBE/FORCES_FC3` & `phono3py-3.0.1/example/Si-PBE/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-PBE/POSCAR-unitcell` & `phono3py-3.0.1/example/Si-PBE/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-PBE/README.md` & `phono3py-3.0.1/example/Si-PBE/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-PBE/phono3py_disp.yaml` & `phono3py-3.0.1/example/Si-PBE/phono3py_disp.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-PBE/vasprun_xmls.tar.lzma` & `phono3py-3.0.1/example/Si-PBE/vasprun_xmls.tar.lzma`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-PBEsol/FORCES_FC3` & `phono3py-3.0.1/example/Si-PBEsol/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-PBEsol/POSCAR-unitcell` & `phono3py-3.0.1/example/Si-PBEsol/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-PBEsol/README.md` & `phono3py-3.0.1/example/Si-PBEsol/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-PBEsol/Si-band-DOS.png` & `phono3py-3.0.1/example/Si-PBEsol/Si-band-DOS.png`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-PBEsol/Si-kaccum.png` & `phono3py-3.0.1/example/Si-PBEsol/Si-kaccum.png`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-PBEsol/Si.py` & `phono3py-3.0.1/example/Si-PBEsol/Si.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-PBEsol/phono3py_disp.yaml` & `phono3py-3.0.1/example/Si-PBEsol/phono3py_disp.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-PBEsol/phono3py_disp_dimfc2.yaml` & `phono3py-3.0.1/example/Si-PBEsol/phono3py_disp_dimfc2.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/POSCAR` & `phono3py-3.0.1/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/POSCAR`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/vasprun.xml` & `phono3py-3.0.1/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/vasprun.xml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-PBEsol/vasprun_xmls.tar.lzma` & `phono3py-3.0.1/example/Si-PBEsol/vasprun_xmls.tar.lzma`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-QE/FORCES_FC3` & `phono3py-3.0.1/example/Si-QE/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-QE/README.md` & `phono3py-3.0.1/example/Si-QE/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-QE/Si.in` & `phono3py-3.0.1/example/Si-QE/Si.in`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-QE/phono3py_disp.yaml` & `phono3py-3.0.1/example/Si-QE/phono3py_disp.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-QE/supercell_out.tar.lzma` & `phono3py-3.0.1/example/Si-QE/supercell_out.tar.lzma`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-TURBOMOLE/FORCES_FC2` & `phono3py-3.0.1/example/Si-TURBOMOLE/FORCES_FC2`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-TURBOMOLE/FORCES_FC3` & `phono3py-3.0.1/example/Si-TURBOMOLE/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-TURBOMOLE/README` & `phono3py-3.0.1/example/Si-TURBOMOLE/README`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Si-TURBOMOLE/outputs.tar.gz` & `phono3py-3.0.1/example/Si-TURBOMOLE/outputs.tar.gz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Wigner_La2Zr2O7/BORN` & `phono3py-3.0.1/example/Wigner_La2Zr2O7/BORN`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Wigner_La2Zr2O7/POSCAR` & `phono3py-3.0.1/example/Wigner_La2Zr2O7/POSCAR`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Wigner_La2Zr2O7/fc2.hdf5` & `phono3py-3.0.1/example/Wigner_La2Zr2O7/fc2.hdf5`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Wigner_La2Zr2O7/kappa-m191919.hdf5` & `phono3py-3.0.1/example/Wigner_La2Zr2O7/kappa-m191919.hdf5`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/Wigner_La2Zr2O7/tc_La2Zr2O7.out.xz` & `phono3py-3.0.1/example/Wigner_La2Zr2O7/tc_La2Zr2O7.out.xz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/zb-ZnTe-PBEsol/README.md` & `phono3py-3.0.1/example/zb-ZnTe-PBEsol/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/zb-ZnTe-PBEsol/launch_phono3py_ZnTe_PBEsol_222.py` & `phono3py-3.0.1/example/zb-ZnTe-PBEsol/launch_phono3py_ZnTe_PBEsol_222.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/example/zb-ZnTe-PBEsol/phono3py_params_ZnTe.yaml.xz` & `phono3py-3.0.1/example/zb-ZnTe-PBEsol/phono3py_params_ZnTe.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/__init__.py` & `phono3py-3.0.1/phono3py/__init__.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/api_isotope.py` & `phono3py-3.0.1/phono3py/api_isotope.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/api_jointdos.py` & `phono3py-3.0.1/phono3py/api_jointdos.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/api_phono3py.py` & `phono3py-3.0.1/phono3py/api_phono3py.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/conductivity/base.py` & `phono3py-3.0.1/phono3py/conductivity/base.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/conductivity/direct_solution.py` & `phono3py-3.0.1/phono3py/conductivity/direct_solution.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/conductivity/kubo.py` & `phono3py-3.0.1/phono3py/conductivity/kubo.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/conductivity/rta.py` & `phono3py-3.0.1/phono3py/conductivity/rta.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/conductivity/utils.py` & `phono3py-3.0.1/phono3py/conductivity/utils.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/conductivity/wigner.py` & `phono3py-3.0.1/phono3py/conductivity/wigner.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/cui/create_force_constants.py` & `phono3py-3.0.1/phono3py/cui/create_force_constants.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/cui/create_supercells.py` & `phono3py-3.0.1/phono3py/cui/create_supercells.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/cui/kaccum_script.py` & `phono3py-3.0.1/phono3py/cui/kaccum_script.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/cui/load.py` & `phono3py-3.0.1/phono3py/cui/load.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/cui/phono3py_argparse.py` & `phono3py-3.0.1/phono3py/cui/phono3py_argparse.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/cui/phono3py_script.py` & `phono3py-3.0.1/phono3py/cui/phono3py_script.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/cui/settings.py` & `phono3py-3.0.1/phono3py/cui/settings.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/cui/show_log.py` & `phono3py-3.0.1/phono3py/cui/show_log.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/cui/triplets_info.py` & `phono3py-3.0.1/phono3py/cui/triplets_info.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/file_IO.py` & `phono3py-3.0.1/phono3py/file_IO.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/interface/alm.py` & `phono3py-3.0.1/phono3py/interface/alm.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/interface/calculator.py` & `phono3py-3.0.1/phono3py/interface/calculator.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/interface/fc_calculator.py` & `phono3py-3.0.1/phono3py/interface/fc_calculator.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/interface/phono3py_yaml.py` & `phono3py-3.0.1/phono3py/interface/phono3py_yaml.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/other/isotope.py` & `phono3py-3.0.1/phono3py/other/isotope.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/other/kaccum.py` & `phono3py-3.0.1/phono3py/other/kaccum.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/other/tetrahedron_method.py` & `phono3py-3.0.1/phono3py/other/tetrahedron_method.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon/func.py` & `phono3py-3.0.1/phono3py/phonon/func.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon/grid.py` & `phono3py-3.0.1/phono3py/phonon/grid.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon/group_velocity_matrix.py` & `phono3py-3.0.1/phono3py/phonon/group_velocity_matrix.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon/heat_capacity_matrix.py` & `phono3py-3.0.1/phono3py/phonon/heat_capacity_matrix.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon/solver.py` & `phono3py-3.0.1/phono3py/phonon/solver.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon/velocity_operator.py` & `phono3py-3.0.1/phono3py/phonon/velocity_operator.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon3/collision_matrix.py` & `phono3py-3.0.1/phono3py/phonon3/collision_matrix.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon3/dataset.py` & `phono3py-3.0.1/phono3py/phonon3/dataset.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon3/displacement_fc3.py` & `phono3py-3.0.1/phono3py/phonon3/displacement_fc3.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon3/fc3.py` & `phono3py-3.0.1/phono3py/phonon3/fc3.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon3/gruneisen.py` & `phono3py-3.0.1/phono3py/phonon3/gruneisen.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon3/imag_self_energy.py` & `phono3py-3.0.1/phono3py/phonon3/imag_self_energy.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon3/interaction.py` & `phono3py-3.0.1/phono3py/phonon3/interaction.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon3/joint_dos.py` & `phono3py-3.0.1/phono3py/phonon3/joint_dos.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon3/real_self_energy.py` & `phono3py-3.0.1/phono3py/phonon3/real_self_energy.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon3/real_to_reciprocal.py` & `phono3py-3.0.1/phono3py/phonon3/real_to_reciprocal.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon3/reciprocal_to_normal.py` & `phono3py-3.0.1/phono3py/phonon3/reciprocal_to_normal.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon3/spectral_function.py` & `phono3py-3.0.1/phono3py/phonon3/spectral_function.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/phonon3/triplets.py` & `phono3py-3.0.1/phono3py/phonon3/triplets.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/sscha/sscha.py` & `phono3py-3.0.1/phono3py/sscha/sscha.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/phono3py/version.py` & `phono3py-3.0.1/phono3py/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 # BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 # LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
 # ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "3.0.0"
+__version__ = "3.0.1"
```

### Comparing `phono3py-3.0.0/phono3py.egg-info/SOURCES.txt` & `phono3py-3.0.1/phono3py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/scripts/phono3py` & `phono3py-3.0.1/scripts/phono3py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/scripts/phono3py-coleigplot` & `phono3py-3.0.1/scripts/phono3py-coleigplot`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/scripts/phono3py-kaccum` & `phono3py-3.0.1/scripts/phono3py-kaccum`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/scripts/phono3py-kdeplot` & `phono3py-3.0.1/scripts/phono3py-kdeplot`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/scripts/phono3py-load` & `phono3py-3.0.1/scripts/phono3py-load`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/setup.py` & `phono3py-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/AgNO2_cell.yaml` & `phono3py-3.0.1/test/AgNO2_cell.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/FORCES_FC3_si_pbesol` & `phono3py-3.0.1/test/FORCES_FC3_si_pbesol`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/FORCE_SETS_NaCl` & `phono3py-3.0.1/test/FORCE_SETS_NaCl`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/api/test_api_phono3py.py` & `phono3py-3.0.1/test/api/test_api_phono3py.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/conductivity/test_kappa_LBTE.py` & `phono3py-3.0.1/test/conductivity/test_kappa_LBTE.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/conductivity/test_kappa_LBTE_Wigner.py` & `phono3py-3.0.1/test/conductivity/test_kappa_LBTE_Wigner.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/conductivity/test_kappa_RTA.py` & `phono3py-3.0.1/test/conductivity/test_kappa_RTA.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/conductivity/test_kappa_RTA_Wigner.py` & `phono3py-3.0.1/test/conductivity/test_kappa_RTA_Wigner.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/conftest.py` & `phono3py-3.0.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/cui/phono3py_params-qe-Si222.yaml.xz` & `phono3py-3.0.1/test/cui/phono3py_params-qe-Si222.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/cui/test_phono3py_load_script.py` & `phono3py-3.0.1/test/cui/test_phono3py_load_script.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/file_IO/test_file_IO.py` & `phono3py-3.0.1/test/file_IO/test_file_IO.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/interface/test_phono3py_yaml.py` & `phono3py-3.0.1/test/interface/test_phono3py_yaml.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/other/test_isotope.py` & `phono3py-3.0.1/test/other/test_isotope.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/other/test_kaccum.py` & `phono3py-3.0.1/test/other/test_kaccum.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phono3py_params-Si111-rd.yaml.xz` & `phono3py-3.0.1/test/phono3py_params-Si111-rd.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phono3py_params_AlN332.yaml.xz` & `phono3py-3.0.1/test/phono3py_params_AlN332.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phono3py_params_NaCl111.yaml` & `phono3py-3.0.1/test/phono3py_params_NaCl111.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phono3py_params_NaCl222.yaml.xz` & `phono3py-3.0.1/test/phono3py_params_NaCl222.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phono3py_params_Si-111-222.yaml` & `phono3py-3.0.1/test/phono3py_params_Si-111-222.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phono3py_params_Si111.yaml` & `phono3py-3.0.1/test/phono3py_params_Si111.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phono3py_si_pbesol.yaml` & `phono3py-3.0.1/test/phono3py_si_pbesol.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phonon/test_grid.py` & `phono3py-3.0.1/test/phonon/test_grid.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phonon/test_velocity_operator.py` & `phono3py-3.0.1/test/phonon/test_velocity_operator.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phonon3/test_displacements.py` & `phono3py-3.0.1/test/phonon3/test_displacements.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phonon3/test_fc3.py` & `phono3py-3.0.1/test/phonon3/test_fc3.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phonon3/test_imag_self_energy.py` & `phono3py-3.0.1/test/phonon3/test_imag_self_energy.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phonon3/test_interaction.py` & `phono3py-3.0.1/test/phonon3/test_interaction.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phonon3/test_joint_dos.py` & `phono3py-3.0.1/test/phonon3/test_joint_dos.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phonon3/test_real_self_energy.py` & `phono3py-3.0.1/test/phonon3/test_real_self_energy.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phonon3/test_spectral_function.py` & `phono3py-3.0.1/test/phonon3/test_spectral_function.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phonon3/test_triplets.py` & `phono3py-3.0.1/test/phonon3/test_triplets.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phonopy_disp_NaCl.yaml` & `phono3py-3.0.1/test/phonopy_disp_NaCl.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phonopy_params-Si111-iterha.yaml.gz` & `phono3py-3.0.1/test/phonopy_params-Si111-iterha.yaml.gz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/phonopy_params_Si.yaml` & `phono3py-3.0.1/test/phonopy_params_Si.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.0/test/sscha/test_sscha.py` & `phono3py-3.0.1/test/sscha/test_sscha.py`

 * *Files identical despite different names*

