# Comparing `tmp/pyxtal-0.6.4.tar.gz` & `tmp/pyxtal-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxtal-0.6.4.tar", last modified: Mon Mar 18 23:59:31 2024, max compression
+gzip compressed data, was "pyxtal-0.6.5.tar", last modified: Sun Apr 21 00:39:52 2024, max compression
```

## Comparing `pyxtal-0.6.4.tar` & `pyxtal-0.6.5.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:31.103556 pyxtal-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-18 23:59:22.000000 pyxtal-0.6.4/LICENSE.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-03-18 23:59:22.000000 pyxtal-0.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-03-18 23:59:31.103556 pyxtal-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-03-18 23:59:22.000000 pyxtal-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:31.067556 pyxtal-0.6.4/pyxtal/
--rw-r--r--   0 runner    (1001) docker     (127)    31243 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/XRD.py
--rw-r--r--   0 runner    (1001) docker     (127)   114637 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/block_crystal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    15342 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/crystal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:31.087556 pyxtal-0.6.4/pyxtal/database/
--rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/HM_Full.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/atomic_scattering_params.json
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/bonds.json
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/bug.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:31.099556 pyxtal-0.6.4/pyxtal/database/cifs/
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/0-G62.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/1-G59.cif
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/191.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/2-G71.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/3-G139.cif
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/4-G225.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/ACBNZA01.cif
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/AXOSOW01.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/BTO-Amm2.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/BTO.cif
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/FAU.cif
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/Fd3.cif
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/Fd3.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/Fd3m.cif
--rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/GUMMUW.cif
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/GeF2.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/HAHCOI.cif
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/I41amd.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/I4_132.cif
--rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/JAPWIH.cif
--rw-r--r--   0 runner    (1001) docker     (127)   441469 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/LAGNAL.cif
--rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/LUFHAW.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/LiCs.cif
--rw-r--r--   0 runner    (1001) docker     (127)    12413 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/MERQIM.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/MPWO.cif
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/NaCl.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/NaSb3F10.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/NbO2.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/NiS-Cm.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/P3_112.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/P4_332.cif
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/P4nmm.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/P6_422.cif
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/PAHYON01.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/PPO.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/PVO.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/Pm3.cif
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/Pmmn.vasp
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/Pn3.vasp
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/Pn3m.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/R-3.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/R-3c.cif
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/R32.cif
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/TMPPIO03.cif
--rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/WEXBOS.cif
--rw-r--r--   0 runner    (1001) docker     (127)   177150 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/YICMOP.cif
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/anthracene.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/aspirin-c.cif
--rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/aspirin.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/benzene.cif
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/bug.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/c_bug.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/c_bug2.vasp
--rw-r--r--   0 runner    (1001) docker     (127)    17895 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/coumarin.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/dist_6_0.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/dist_6_1.cif
--rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/gdh.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/ht_KNbBO.cif
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/ht_cristobalite.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/ht_quartz.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/ice.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/lt_KNbBO.cif
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/lt_cristobalite.cif
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/lt_quartz.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/naphthalene.cif
--rw-r--r--   0 runner    (1001) docker     (127)   317844 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/resorcinol.cif
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/sim-0.vasp
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/sim-1.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/cifs/xxvi.cif
--rw-r--r--   0 runner    (1001) docker     (127)  1103778 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/clusters.json
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    19164 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/element.py
--rw-r--r--   0 runner    (1001) docker     (127) 10480157 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/k_subgroup.json
--rw-r--r--   0 runner    (1001) docker     (127)    20717 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/layer.csv
--rw-r--r--   0 runner    (1001) docker     (127)    25842 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/layer_generators.csv
--rw-r--r--   0 runner    (1001) docker     (127)    58872 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/layer_symmetry.csv
--rw-r--r--   0 runner    (1001) docker     (127)   294912 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/mech.db
--rw-r--r--   0 runner    (1001) docker     (127)    90734 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/molecules.json
--rw-r--r--   0 runner    (1001) docker     (127)   130892 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/point.csv
--rw-r--r--   0 runner    (1001) docker     (127)   146327 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/point_generators.csv
--rw-r--r--   0 runner    (1001) docker     (127)   301944 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/point_symmetry.csv
--rw-r--r--   0 runner    (1001) docker     (127)    18501 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/rod.csv
--rw-r--r--   0 runner    (1001) docker     (127)    21935 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/rod_generators.csv
--rw-r--r--   0 runner    (1001) docker     (127)    44320 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/rod_symmetry.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/symbols.json
--rw-r--r--   0 runner    (1001) docker     (127)  1245398 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/t_subgroup.json
--rw-r--r--   0 runner    (1001) docker     (127)   259897 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/wyckoff_generators.csv
--rw-r--r--   0 runner    (1001) docker     (127)   251719 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/wyckoff_list.csv
--rw-r--r--   0 runner    (1001) docker     (127)   117892 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/wyckoff_sets.json
--rw-r--r--   0 runner    (1001) docker     (127)   627207 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/database/wyckoff_symmetry.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    18755 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)    42644 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/elasticity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:31.099556 pyxtal-0.6.4/pyxtal/interface/
--rw-r--r--   0 runner    (1001) docker     (127)    13515 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/interface/LJ.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27559 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/interface/dftb.py
--rw-r--r--   0 runner    (1001) docker     (127)    14489 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/interface/gulp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19373 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/interface/lammpslib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/interface/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    31490 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/interface/vasprun.py
--rw-r--r--   0 runner    (1001) docker     (127)    23019 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    70535 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)    18102 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/molecular_crystal.py
--rw-r--r--   0 runner    (1001) docker     (127)    64693 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/msg.py
--rw-r--r--   0 runner    (1001) docker     (127)    30341 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:31.099556 pyxtal-0.6.4/pyxtal/optimize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/optimize/fire.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/optimize/fire2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/optimize/myscipy_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/plane.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:31.103556 pyxtal-0.6.4/pyxtal/potentials/
--rw-r--r--   0 runner    (1001) docker     (127)  1820580 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/potentials/CuAg.eam.alloy
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/potentials/LJ_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/potentials/Si.tersoff
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/potentials/SiCGe.tersoff
--rwxr-xr-x   0 runner    (1001) docker     (127)       26 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/potentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17803 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/representation.py
--rw-r--r--   0 runner    (1001) docker     (127)    46126 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/supergroup.py
--rw-r--r--   0 runner    (1001) docker     (127)   133165 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    45953 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/tolerance.py
--rw-r--r--   0 runner    (1001) docker     (127)    19437 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/viz.py
--rw-r--r--   0 runner    (1001) docker     (127)    45507 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/wyckoff_site.py
--rw-r--r--   0 runner    (1001) docker     (127)    21159 2024-03-18 23:59:22.000000 pyxtal-0.6.4/pyxtal/wyckoff_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:31.103556 pyxtal-0.6.4/pyxtal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-03-18 23:59:31.000000 pyxtal-0.6.4/pyxtal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-03-18 23:59:31.000000 pyxtal-0.6.4/pyxtal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 23:59:31.000000 pyxtal-0.6.4/pyxtal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-18 23:59:31.000000 pyxtal-0.6.4/pyxtal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-18 23:59:31.000000 pyxtal-0.6.4/pyxtal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:31.103556 pyxtal-0.6.4/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4251 2024-03-18 23:59:22.000000 pyxtal-0.6.4/scripts/pyxtal_main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      960 2024-03-18 23:59:22.000000 pyxtal-0.6.4/scripts/pyxtal_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-18 23:59:31.103556 pyxtal-0.6.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1850 2024-03-18 23:59:22.000000 pyxtal-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.881802 pyxtal-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-21 00:39:37.000000 pyxtal-0.6.5/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-04-21 00:39:37.000000 pyxtal-0.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-21 00:39:52.881802 pyxtal-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-21 00:39:37.000000 pyxtal-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.845802 pyxtal-0.6.5/pyxtal/
+-rw-r--r--   0 runner    (1001) docker     (127)    31243 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/XRD.py
+-rw-r--r--   0 runner    (1001) docker     (127)   114634 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/block_crystal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15342 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/crystal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.865802 pyxtal-0.6.5/pyxtal/database/
+-rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/HM_Full.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/atomic_scattering_params.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/bonds.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/bug.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.873802 pyxtal-0.6.5/pyxtal/database/cifs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/0-G62.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/1-G59.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/191.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/2-G71.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/3-G139.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/4-G225.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/ACBNZA01.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/AXOSOW01.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/BTO-Amm2.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/BTO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/FAU.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/Fd3.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/Fd3.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/Fd3m.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/GUMMUW.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/GeF2.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/HAHCOI.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/I41amd.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/I4_132.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/JAPWIH.cif
+-rw-r--r--   0 runner    (1001) docker     (127)   441469 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/LAGNAL.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/LUFHAW.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/LiCs.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    12413 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/MERQIM.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/MPWO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/NaCl.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/NaSb3F10.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/NbO2.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/NiS-Cm.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/P3_112.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/P4_332.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/P4nmm.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/P6_422.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/PAHYON01.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/PPO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/PVO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/Pm3.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/Pmmn.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/Pn3.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/Pn3m.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/R-3.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/R-3c.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/R32.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/TMPPIO03.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/WEXBOS.cif
+-rw-r--r--   0 runner    (1001) docker     (127)   177150 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/YICMOP.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/anthracene.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/aspirin-c.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/aspirin.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/benzene.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/bug.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/c_bug.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/c_bug2.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)    17895 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/coumarin.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/dist_6_0.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/dist_6_1.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/gdh.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/ht_KNbBO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/ht_cristobalite.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/ht_quartz.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/ice.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/lt_KNbBO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/lt_cristobalite.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/lt_quartz.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/naphthalene.cif
+-rw-r--r--   0 runner    (1001) docker     (127)   317844 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/resorcinol.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/sim-0.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/sim-1.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/xxvi.cif
+-rw-r--r--   0 runner    (1001) docker     (127)  1103778 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/clusters.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19164 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/element.py
+-rw-r--r--   0 runner    (1001) docker     (127) 10480157 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/k_subgroup.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20717 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/layer.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    25842 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/layer_generators.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    58872 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/layer_symmetry.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   294912 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/mech.db
+-rw-r--r--   0 runner    (1001) docker     (127)    90734 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/molecules.json
+-rw-r--r--   0 runner    (1001) docker     (127)   130892 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/point.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   146327 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/point_generators.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   301944 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/point_symmetry.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18501 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/rod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21935 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/rod_generators.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    44320 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/rod_symmetry.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/symbols.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1245398 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/t_subgroup.json
+-rw-r--r--   0 runner    (1001) docker     (127)   259897 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/wyckoff_generators.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   251719 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/wyckoff_list.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   117892 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/wyckoff_sets.json
+-rw-r--r--   0 runner    (1001) docker     (127)   627207 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/wyckoff_symmetry.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9236 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18755 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42644 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/elasticity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.877802 pyxtal-0.6.5/pyxtal/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)    13515 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/interface/LJ.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27559 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/interface/dftb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14489 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/interface/gulp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19373 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/interface/lammpslib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/interface/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31490 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/interface/vasprun.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23019 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70535 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18102 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/molecular_crystal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66288 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30343 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.877802 pyxtal-0.6.5/pyxtal/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/optimize/fire.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/optimize/fire2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/optimize/myscipy_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/plane.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.877802 pyxtal-0.6.5/pyxtal/potentials/
+-rw-r--r--   0 runner    (1001) docker     (127)  1820580 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/potentials/CuAg.eam.alloy
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/potentials/LJ_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/potentials/Si.tersoff
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/potentials/SiCGe.tersoff
+-rwxr-xr-x   0 runner    (1001) docker     (127)       26 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/potentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18149 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46126 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139385 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46203 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/tolerance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19437 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/viz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45507 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/wyckoff_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21159 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/wyckoff_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.881802 pyxtal-0.6.5/pyxtal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-21 00:39:52.000000 pyxtal-0.6.5/pyxtal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-21 00:39:52.000000 pyxtal-0.6.5/pyxtal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 00:39:52.000000 pyxtal-0.6.5/pyxtal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-21 00:39:52.000000 pyxtal-0.6.5/pyxtal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 00:39:52.000000 pyxtal-0.6.5/pyxtal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.877802 pyxtal-0.6.5/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4251 2024-04-21 00:39:37.000000 pyxtal-0.6.5/scripts/pyxtal_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      960 2024-04-21 00:39:37.000000 pyxtal-0.6.5/scripts/pyxtal_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-21 00:39:52.881802 pyxtal-0.6.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1850 2024-04-21 00:39:37.000000 pyxtal-0.6.5/setup.py
```

### Comparing `pyxtal-0.6.4/LICENSE.txt` & `pyxtal-0.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/PKG-INFO` & `pyxtal-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxtal
-Version: 0.6.4
+Version: 0.6.5
 Summary: Python code for generation of crystal structures based on symmetry constraints.
 Home-page: https://github.com/qzhu2017/PyXtal
 Author: Scott Fredericks, Qiang Zhu
 Author-email: qiang.zhu@unlv.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyxtal-0.6.4/README.md` & `pyxtal-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/XRD.py` & `pyxtal-0.6.5/pyxtal/XRD.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/__init__.py` & `pyxtal-0.6.5/pyxtal/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2842,15 +2842,15 @@
             msg = 'Unknown CSD entry: ' + csd_code
             raise CSDError(msg)
 
         if entry.has_3d_structure:
             smi = entry.molecule.smiles
             if smi is None:
                 raise CSDError("No smile from CSD")
-            elif len(smi) > 250:
+            elif len(smi) > 350:
                 raise CSDError("long smile {:s}".format(smi))
             else:
                 if Chem.MolFromSmiles(smi) is None:
                     raise CSDError("problematic smiles: {:s}".format(smi))
 
             cif = entry.to_string(format='cif')
             smiles = [s+'.smi' for s in smi.split('.')]
@@ -2870,15 +2870,15 @@
                         #'publication': entry.publication,
                        }
 
             cif = process_csd_cif(cif) #, remove_H=True)
             remove_H = False
             #print(cif)
             try:
-                parser = CifParser.from_string(cif, occupancy_tolerance=2.0)
+                parser = CifParser.from_str(cif, occupancy_tolerance=2.0)
                 pmg = get_struc_from__parser(parser)
                 #pmg = Structure.from_str(cif, fmt='cif')
             except:
                 print(cif)
                 msg = "Problem in parsing CSD cif"
                 raise CSDError(msg)
```

### Comparing `pyxtal-0.6.4/pyxtal/block_crystal.py` & `pyxtal-0.6.5/pyxtal/block_crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/constants.py` & `pyxtal-0.6.5/pyxtal/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,14 +21,18 @@
                   "tetragonal", "Tetragonal",
                   "trigonal", "Trigonal",
                   "hexagonal", "Hexagonal",
                   "cubic", "Cubic",
                   "spherical", "Spherical",
                   "ellipsoidal", "Ellipsoidal",
                  ]
+single_smiles = [
+                 "Cl-", "F-", "Br-", "I-", "Li+", "Na+", "Cs+", "Rb+",
+                 "[Cl-]", "[F-]", "[Br-]", "[I-]", "[Li+]", "[Na+]", "[Cs+]", "Rb+",
+                ]
 
 logo = """#############################################################
 #             ______       _    _          _                #
 #            (_____ \     \ \  / /        | |               #
 #             _____) )   _ \ \/ / |_  ____| |               #
 #            |  ____/ | | | )  (|  _)/ _  | |               #
 #            | |    | |_| |/ /\ \ |_( (_| | |___            #
```

### Comparing `pyxtal-0.6.4/pyxtal/crystal.py` & `pyxtal-0.6.5/pyxtal/crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/HM_Full.csv` & `pyxtal-0.6.5/pyxtal/database/HM_Full.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/atomic_scattering_params.json` & `pyxtal-0.6.5/pyxtal/database/atomic_scattering_params.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/bonds.json` & `pyxtal-0.6.5/pyxtal/database/bonds.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/bug.json` & `pyxtal-0.6.5/pyxtal/database/bug.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/0-G62.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/0-G62.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/1-G59.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/1-G59.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/2-G71.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/2-G71.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/3-G139.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/3-G139.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/4-G225.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/4-G225.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/ACBNZA01.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/ACBNZA01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/AXOSOW01.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/AXOSOW01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/BTO-Amm2.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/BTO-Amm2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/BTO.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/BTO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/FAU.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/FAU.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/Fd3.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/Fd3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/Fd3.vasp` & `pyxtal-0.6.5/pyxtal/database/cifs/Fd3.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/Fd3m.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/Fd3m.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/GUMMUW.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/GUMMUW.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/GeF2.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/GeF2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/HAHCOI.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/HAHCOI.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/I4_132.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/I4_132.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/JAPWIH.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/JAPWIH.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/LAGNAL.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/LAGNAL.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/LUFHAW.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/LUFHAW.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/LiCs.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/LiCs.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/MERQIM.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/MERQIM.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/MPWO.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/MPWO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/NaCl.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/NaCl.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/NaSb3F10.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/NaSb3F10.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/NbO2.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/NbO2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/NiS-Cm.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/NiS-Cm.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/P3_112.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/P3_112.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/P4_332.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/P4_332.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/P6_422.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/P6_422.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/PAHYON01.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/PAHYON01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/PPO.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/PPO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/PVO.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/PVO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/Pm3.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/Pm3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/R-3.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/R-3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/R-3c.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/R-3c.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/R32.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/R32.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/TMPPIO03.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/TMPPIO03.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/WEXBOS.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/WEXBOS.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/YICMOP.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/YICMOP.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/anthracene.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/anthracene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/aspirin-c.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/aspirin-c.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/aspirin.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/aspirin.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/benzene.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/benzene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/bug.vasp` & `pyxtal-0.6.5/pyxtal/database/cifs/bug.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/c_bug.vasp` & `pyxtal-0.6.5/pyxtal/database/cifs/c_bug.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/c_bug2.vasp` & `pyxtal-0.6.5/pyxtal/database/cifs/c_bug2.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/coumarin.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/coumarin.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/dist_6_0.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/dist_6_0.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/dist_6_1.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/dist_6_1.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/gdh.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/gdh.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/ht_KNbBO.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/ht_KNbBO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/ht_cristobalite.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/ht_cristobalite.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/ht_quartz.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/ht_quartz.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/ice.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/ice.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/lt_KNbBO.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/lt_KNbBO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/lt_cristobalite.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/lt_cristobalite.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/lt_quartz.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/lt_quartz.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/naphthalene.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/naphthalene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/resorcinol.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/resorcinol.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/cifs/xxvi.cif` & `pyxtal-0.6.5/pyxtal/database/cifs/xxvi.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/clusters.json` & `pyxtal-0.6.5/pyxtal/database/clusters.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/collection.py` & `pyxtal-0.6.5/pyxtal/database/collection.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/element.py` & `pyxtal-0.6.5/pyxtal/database/element.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/k_subgroup.json` & `pyxtal-0.6.5/pyxtal/database/k_subgroup.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/layer.csv` & `pyxtal-0.6.5/pyxtal/database/layer.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/layer_generators.csv` & `pyxtal-0.6.5/pyxtal/database/layer_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/layer_symmetry.csv` & `pyxtal-0.6.5/pyxtal/database/layer_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/mech.db` & `pyxtal-0.6.5/pyxtal/database/mech.db`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/molecules.json` & `pyxtal-0.6.5/pyxtal/database/molecules.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/point.csv` & `pyxtal-0.6.5/pyxtal/database/point.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/point_generators.csv` & `pyxtal-0.6.5/pyxtal/database/point_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/point_symmetry.csv` & `pyxtal-0.6.5/pyxtal/database/point_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/rod.csv` & `pyxtal-0.6.5/pyxtal/database/rod.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/rod_generators.csv` & `pyxtal-0.6.5/pyxtal/database/rod_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/rod_symmetry.csv` & `pyxtal-0.6.5/pyxtal/database/rod_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/symbols.json` & `pyxtal-0.6.5/pyxtal/database/symbols.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/t_subgroup.json` & `pyxtal-0.6.5/pyxtal/database/t_subgroup.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/wyckoff_generators.csv` & `pyxtal-0.6.5/pyxtal/database/wyckoff_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/wyckoff_list.csv` & `pyxtal-0.6.5/pyxtal/database/wyckoff_list.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/wyckoff_sets.json` & `pyxtal-0.6.5/pyxtal/database/wyckoff_sets.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/database/wyckoff_symmetry.csv` & `pyxtal-0.6.5/pyxtal/database/wyckoff_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/db.py` & `pyxtal-0.6.5/pyxtal/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 
     # add structure
     for i, code in enumerate(codes):
         entry = make_entry_from_CSD(code)
         if entry is not None:
             db.add(entry)
             print(i, code)
+    return db
 
 class database():
     """
     This is a database class to process crystal data
 
     Args:
         db_name: *.db format from ase database
```

### Comparing `pyxtal-0.6.4/pyxtal/descriptor.py` & `pyxtal-0.6.5/pyxtal/descriptor.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/elasticity.py` & `pyxtal-0.6.5/pyxtal/elasticity.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/interface/LJ.py` & `pyxtal-0.6.5/pyxtal/interface/LJ.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/interface/dftb.py` & `pyxtal-0.6.5/pyxtal/interface/dftb.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/interface/gulp.py` & `pyxtal-0.6.5/pyxtal/interface/gulp.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/interface/lammpslib.py` & `pyxtal-0.6.5/pyxtal/interface/lammpslib.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/interface/vasp.py` & `pyxtal-0.6.5/pyxtal/interface/vasp.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/interface/vasprun.py` & `pyxtal-0.6.5/pyxtal/interface/vasprun.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/io.py` & `pyxtal-0.6.5/pyxtal/io.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/lattice.py` & `pyxtal-0.6.5/pyxtal/lattice.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/molecular_crystal.py` & `pyxtal-0.6.5/pyxtal/molecular_crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/molecule.py` & `pyxtal-0.6.5/pyxtal/molecule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Module for handling molecules.
 """
-import os
+import os, re
 from pkg_resources import resource_filename
 from copy import deepcopy
 from operator import itemgetter
 from random import choice, random
 import numpy as np
 from scipy.spatial.transform import Rotation
 import networkx as nx
@@ -18,19 +18,23 @@
 # PyXtal imports
 from pyxtal.symmetry import Group
 from pyxtal.tolerance import Tol_matrix
 from pyxtal.database.element import Element
 from pyxtal.operations import SymmOp, OperationAnalyzer, rotate_vector, angle
 from pyxtal.database.collection import Collection
 from pyxtal.msg import ConformerError, AtomTypeError
+from pyxtal.constants import single_smiles
 
 # Define functions
 bonds = loadfn(resource_filename("pyxtal", "database/bonds.json"))
 molecule_collection = Collection("molecules")
-
+#single_smiles = [
+#                 "Cl-", "F-", "Br-", "I-", "Li+", "Na+", "Cs+", "Rb+",
+#                 "[Cl-]", "[F-]", "[Br-]", "[I-]", "[Li+]", "[Na+]", "[Cs+]", "Rb+",
+#                ]
 def find_rotor_from_smile(smile):
     """
     Find the positions of rotatable bonds in the molecule.
     """
     def cleaner(list_to_clean, neighbors):
         """
         Remove duplicate torsion from a list of atom index tuples.
@@ -87,15 +91,44 @@
             (i, j, k, l) = t
             b = mol.GetBondBetweenAtoms(j,k)
             if not b.IsInRing():
                 torsions.append(t)
         #if len(torsions) > 6: torsions[1] = (4, 7, 10, 15)
         return torsions #+ [(6, 7, 8, 3), (6, 5, 4, 3)]
 
-def generate_molecules(smile, wps=None, N_iter=4, N_conf=10, tol=0.5):
+def has_non_aromatic_ring(smiles):
+    """
+    Determine if a molecule has a non-aromatic ring.
+    Mainly used to check if a cyclic ring exists.
+
+    Args:
+        smiles: smiles string
+
+    Returns:
+        True or False
+    """
+    from rdkit import Chem
+    # Convert the SMILES string to an RDKit molecule object
+    mol = Chem.MolFromSmiles(smiles)
+
+    # Check if the molecule has rings at all
+    if not mol.HasSubstructMatch(Chem.MolFromSmarts('[R]')):
+        return False  # No rings present
+
+    # Get information about the rings in the molecule
+    ring_info = mol.GetRingInfo()
+
+    # Check each ring to see if it is aromatic; return True if a non-aromatic ring is found
+    for ring in ring_info.BondRings():
+        if not all(mol.GetBondWithIdx(idx).GetIsAromatic() for idx in ring):
+            return True  # Found a non-aromatic ring
+    return False  # No non-aromatic rings found
+
+
+def generate_molecules(smile, wps=None, N_iter=5, N_conf=10, tol=0.5):
     """
     generate pyxtal_molecules from smiles codes.
 
     Args:
         smile: smiles code
         wps: list of wps
         N_iter: rdkit parameter
@@ -106,22 +139,27 @@
         a list of pyxtal molecules
     """
 
     from rdkit import Chem
     from rdkit.Chem import AllChem
 
     torsionlist = find_rotor_from_smile(smile)
+    if len(torsionlist) == 0:
+        if has_non_aromatic_ring(smile):
+            Num = 10
+    else:
+        Num = len(tor)
 
     def get_conformers(smile, seed):
         mol = Chem.MolFromSmiles(smile)
         mol = Chem.AddHs(mol)
         ps = AllChem.ETKDGv3()
         ps.randomSeed = seed
         ps.runeRmsThresh = tol
-        AllChem.EmbedMultipleConfs(mol, max([4, 4*len(torsionlist)]), ps)
+        AllChem.EmbedMultipleConfs(mol, max([4, Num]), ps)
         return mol
 
     m0 = pyxtal_molecule(smile+'.smi', fix=True)
     _, valid = m0.get_orientations_in_wps(wps)
     if valid:
         #print('torsion', m0.get_torsion_angles())
         mols = [m0]
@@ -251,15 +289,17 @@
         self.box = self.get_box()
         self.volume = self.box.volume
         self.get_symbols()
         self.get_radius()
         self.tols_matrix = self.get_tols_matrix()
         xyz = self.mol.cart_coords
         self.reset_positions(xyz-self.get_center(xyz))
-        if self.smile is not None: ori, _, self.reflect = self.get_orientation(xyz)
+        if self.smile is not None and self.smile not in single_smiles:
+            #print(self.smile)
+            ori, _, self.reflect = self.get_orientation(xyz)
 
     def __str__(self):
         return '[' + self.name + ']'
 
     def save_str(self):
         """
         save the object as a dictionary
@@ -733,15 +773,15 @@
             fix: whether or not fix the seed
             torsions: None or list
         """
         from rdkit import Chem
         from rdkit.Chem import AllChem
         from rdkit.Chem import rdMolTransforms as rdmt
 
-        if smile not in ["Cl-", "F-", "Br-", "I-", "Li+", "Na+"]:
+        if smile not in single_smiles: #["Cl-", "F-", "Br-", "I-", "Li+", "Na+"]:
             torsionlist = find_rotor_from_smile(smile)
             mol = Chem.MolFromSmiles(smile)
             mol = Chem.AddHs(mol)
             symbols = []
             for id in range(mol.GetNumAtoms()):
                 symbols.append(mol.GetAtomWithIdx(id).GetSymbol())
             if len(smile) > 100: #a tmp fix for KEKULN10
@@ -780,15 +820,20 @@
             if torsions is not None:
                 xyz = self.set_torsion_angles(conf, torsions, torsionlist=torsionlist)
             else:
                 xyz = conf.GetPositions()
                 xyz -= self.get_center(xyz)
         else:
             #single atom cation or anions
-            symbols = ["Cl"]
+            pattern = r'[A-Za-z]+(?=[+\-]?[^A-Za-z]|$)'
+            matches = re.findall(pattern, smile)
+            if matches:
+                symbols = [matches[0]] #["Cl"]
+            else:
+                raise ValueError("the input smiles cannot be analyzed", smile)
             xyz = np.zeros([1,3])
             torsionlist = []
         return symbols, xyz, torsionlist
 
     def perturb_torsion(self, xyz):
         """
         slightly perturb the torsion
```

### Comparing `pyxtal-0.6.4/pyxtal/msg.py` & `pyxtal-0.6.5/pyxtal/msg.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/operations.py` & `pyxtal-0.6.5/pyxtal/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -645,21 +645,21 @@
             x = (n * angle) / (2.0 * np.pi)
             y = x - np.round(x)
             if abs(y) <= tol:
                 found = True
                 break
         if found:
             # Double order of odd-rotation rotoinversions
-            if rotoinversion:
-                if n % 2 == 1:
-                    return int(n * 2)
-                else:
-                    return int(n)
-            else:
-                return int(n)
+            #if rotoinversion:
+            #    if n % 2 == 1:
+            #        return int(n * 2)
+            #    else:
+            #        return int(n)
+            #else:
+            return int(n)
         if not found:
             return "irrational"
 
     def __init__(self, op):
         if type(op) == deepcopy(SymmOp):
             self.op = op
             """The original SymmOp object being analyzed"""
```

### Comparing `pyxtal-0.6.4/pyxtal/optimize/fire.py` & `pyxtal-0.6.5/pyxtal/optimize/fire.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/optimize/fire2.py` & `pyxtal-0.6.5/pyxtal/optimize/fire2.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/optimize/myscipy_optimize.py` & `pyxtal-0.6.5/pyxtal/optimize/myscipy_optimize.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/plane.py` & `pyxtal-0.6.5/pyxtal/plane.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/potentials/CuAg.eam.alloy` & `pyxtal-0.6.5/pyxtal/potentials/CuAg.eam.alloy`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/potentials/LJ_cluster.py` & `pyxtal-0.6.5/pyxtal/potentials/LJ_cluster.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/potentials/Si.tersoff` & `pyxtal-0.6.5/pyxtal/potentials/Si.tersoff`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/potentials/SiCGe.tersoff` & `pyxtal-0.6.5/pyxtal/potentials/SiCGe.tersoff`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/representation.py` & `pyxtal-0.6.5/pyxtal/representation.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,37 +76,40 @@
         try:
             struc.lattice = Lattice.from_para(a, b, c, alpha, beta, gamma, ltype=ltype)
         except:
             print(a, b, c, alpha, beta, gamma, ltype)
             raise ValueError("Problem in Lattice")
 
         # sites
-        struc.numIons = [0] * len(smiles)
+        struc.numIons = []
         struc.atom_sites = []
+        species = []
 
-        count = 1
-        for i, comp in enumerate(composition):
-            for j in range(comp):
-                v = self.x[count]
-                dicts = {}
-                dicts['type'] = i
-                dicts['dim'] = 3
-                dicts['PBC'] = [1, 1, 1]
-                dicts['hn'] = struc.group.hall_number
-                dicts['index'] = 0
-                dicts['lattice'] = struc.lattice.matrix
-                dicts['lattice_type'] = ltype
-                site = atom_site.from_1D_dicts(dicts)
-                site.type = i
-                struc.atom_sites.append(site)
-                struc.numIons[i] += site.wp.multiplicity
-                #move to next rep
-                count += 1
-            struc.species.append(site.specie)
+        for _x in self.x[1:]:
+            dicts = {}
+            specie, index, pos = _x[0], _x[1], _x[2:]
+            dicts['specie'] = specie
+            dicts['index'] = index
+            dicts['dim'] = 3
+            dicts['PBC'] = [1, 1, 1]
+            dicts['hn'] = struc.group.hall_number
+            wp = struc.group[index]
+            dicts['position'] = wp.get_position_from_free_xyzs(pos)
+            site = atom_site.load_dict(dicts)
+            struc.atom_sites.append(site)
+
+            if specie not in species:
+                species.append(specie)
+                struc.numIons.append(wp.multiplicity)
+            else:
+                for i, _specie in enumerate(species):
+                    if _specie == specie:
+                        struc.numIons[i] += site.wp.multiplicity
 
+        struc.species = species
         struc._get_formula()
         struc.source = '1D rep.'
         struc.valid = True
         struc.standard_setting = site.wp.is_standard_setting()
 
         return struc
 
@@ -146,15 +149,15 @@
 
         # data for atoms
         strs += "{:d} ".format(len(x)-1)  # Number of sites
         for i in range(1, len(x)):
             strs += "{:s} ".format(x[i][0])
             strs += "{:d} ".format(x[i][1])
             for v in x[i][2:]:
-                strs += "{:4.2f} ".format(v)
+                strs += "{:6.4f} ".format(v)
 
         if time is not None:
             strs += "{:5.2f}".format(time)
 
         if eng is not None:
             strs += "{:11.3f}".format(eng)
 
@@ -502,14 +505,22 @@
     smiles = ['CC1=CC=C(C=C1)S(=O)(=O)C2=C(N=C(S2)C3=CC=C(C=C3)NC(=O)OCC4=CC=CC=C4)C']
     rep4 = representation.from_string(string1, smiles)
     rep5 = representation.from_string(string2, smiles)
     print(string1)
     print(string2)
     print(rep4.get_dist(rep5))
 
+    from pyxtal import pyxtal
+    xtal = pyxtal()
+    xtal.from_seed('pyxtal/database/cifs/Fd3.cif')
+    xtal.from_seed('pyxtal/database/cifs/NaSb3F10.cif')
+    rep = representation_atom.from_pyxtal(xtal)
+    print(rep)
+    print(xtal)
+    print(rep.to_pyxtal())
     #strings = [
     #"83 14.08  6.36 25.31  83.9 1 0.72 0.40 0.27  131.6  -17.0 -120.0  -83.8 -134.1 -174.5 -175.7 -168.8  173.9  178.0 -157.4 0",
     #"81 14.08  6.36 25.31  83.9 1 0.59 0.81 0.39 -117.8  -50.1  -95.3  -25.8  -80.6  164.7  155.9 -124.9 -159.2  178.6 -154.7 0",
     #"81 14.08  6.36 25.31  83.9 1 0.75 0.09 0.01  133.8  -19.5  -55.1  -86.7  -91.7 -175.0 -170.4 -176.8  173.3 -164.8  -58.4 0",
     #"81 14.08  6.36 25.31  83.9 1 0.72 0.44 0.01  135.2   27.5   97.2 -101.1 -105.1  -29.7 -169.7  -50.1  172.2 -173.1  131.6 0",
     #"82 14.00  6.34 25.26  83.6 1 0.21 0.08 0.54  146.0  -12.0   50.2  108.0  112.3 -166.3 -158.7  -35.5  172.3 -168.7  133.0 0",
     #"81 14.08  6.36 25.31  83.9 1 0.05 0.30 0.89  -68.2   41.2  148.8  -66.9  -85.0 -167.4  172.3 -166.2 -178.3  166.4  -45.9 0",
```

### Comparing `pyxtal-0.6.4/pyxtal/supergroup.py` & `pyxtal-0.6.5/pyxtal/supergroup.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/symmetry.py` & `pyxtal-0.6.5/pyxtal/symmetry.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,16 @@
     - Group class
     - Wyckoff_Position class.
     - Hall class
 """
 # Imports ------------------------------
 # Standard Libraries
 import numpy as np
-from pkg_resources import resource_filename as rf
+#from pkg_resources import resource_filename as rf
+
 from copy import deepcopy
 import random
 import itertools
 import re
 
 # External Libraries
 from pymatgen.symmetry.analyzer import generate_full_symmops
@@ -28,14 +29,20 @@
     distance,
     distance_matrix,
     create_matrix,
     OperationAnalyzer,
     check_images,
 )
 from pyxtal.constants import letters
+import importlib.util
+import os
+
+def rf(package_name, resource_path):
+    package_path = importlib.util.find_spec(package_name).submodule_search_locations[0]
+    return os.path.join(package_path, resource_path)
 # ------------------------------ Constants ---------------------------------------
 
 wyckoff_df = read_csv(rf("pyxtal", "database/wyckoff_list.csv"))
 wyckoff_symmetry_df = read_csv(rf("pyxtal", "database/wyckoff_symmetry.csv"))
 wyckoff_generators_df = read_csv(rf("pyxtal", "database/wyckoff_generators.csv"))
 layer_df = read_csv(rf("pyxtal", "database/layer.csv"))
 layer_symmetry_df = read_csv(rf("pyxtal", "database/layer_symmetry.csv"))
@@ -48,14 +55,18 @@
 point_generators_df = read_csv(rf("pyxtal", "database/point_generators.csv"))
 symbols = loadfn(rf("pyxtal", "database/symbols.json"))
 t_subgroup = loadfn(rf("pyxtal",'database/t_subgroup.json'))
 k_subgroup = loadfn(rf("pyxtal",'database/k_subgroup.json'))
 wyc_sets = loadfn(rf("pyxtal",'database/wyckoff_sets.json'))
 hex_cell = np.array([[1, -0.5, 0], [0, np.sqrt(3) / 2, 0], [0, 0, 1]])
 hall_table = read_csv(rf("pyxtal", "database/HM_Full.csv"), sep=',')
+all_directions = [(1, 0, 0), (0, 1, 0), (0, 0, 1), (1, 1, 1),
+                  (1, -1, -1), (-1, 1, -1), (-1, -1, 1), (1, -1, 0),
+                  (1, 1, 0), (0, 1, -1), (0, 1, 1), (-1, 0, 1),
+                  (1, 0, 1), (1, 2, 0), (2, 1, 0)]
 
 #The map between spglib default space group and hall numbers
 spglib_hall_numbers = [
 1,   2,   3,   6,   9,   18,  21,  30,  39,  57,  60,  63,  72,  81,  90,
 108, 109, 112, 115, 116, 119, 122, 123, 124, 125, 128, 134, 137, 143, 149,
 155, 161, 164, 170, 173, 176, 182, 185, 191, 197, 203, 209, 212, 215, 218,
 221, 227, 228, 230, 233, 239, 245, 251, 257, 263, 266, 269, 275, 278, 284,
@@ -278,14 +289,16 @@
                     "PBC": self.PBC,
                     "dim": self.dim,
                     "number": self.number,
                     "symbol": self.symbol,
                     "P": self.P,
                     "P1": self.P1,
                     "hall_number": self.hall_number,
+                    "directions": self.get_symmetry_directions(),
+                    "lattice_type": self.lattice_type,
                 }
                 for i in range(len(self.wyckoffs))
             ]
 
             # A list of Wyckoff_positions sorted by descending multiplicity
             self.Wyckoff_positions = []
             for wpdict in wpdicts:
@@ -1308,14 +1321,27 @@
         return len(self) - letters.index(letter) - 1
 
     def get_wp_by_letter(self, letter):
         """
         get the wp object by the letter
         """
         return self[self.get_index_by_letter(letter)]
+
+    def get_symmetry_directions(self):
+        """
+        Table 2.1.3.1 from International Tables for Crystallography (2016).
+        Vol. A, Chapter 2.1, pp. 142–174.
+        including Primary, secondary and Tertiary
+        """
+        #if self.dim == 3:
+        return get_symmetry_directions(self.lattice_type, self.symbol[0])
+        #else:
+        #    print("Cannot handle dimension other than 3")
+        #    pass
+
 #
 # ----------------------- Wyckoff Position class  ------------------------
 
 class Wyckoff_position:
     """
     Class for a single Wyckoff position within a symmetry group
 
@@ -1385,32 +1411,37 @@
         """
         number, hall_number, P, P1 = group, None, None, None
         if not use_hall:
             symbol, number = get_symbol_and_number(group, dim)
         else:
             symbol = hall_table['Symbol'][group-1]
             number = hall_table['Spg_num'][group-1]
+        pbc, lattice_type = get_pbc_and_lattice(number, dim)
 
         if dim == 3:
             PBC = [1, 1, 1]
             if not use_hall:
                 if style == 'pyxtal':
                     hall_number = pyxtal_hall_numbers[number-1]
                 else:
                     hall_number = spglib_hall_numbers[number-1]
                     P = abc2matrix(hall_table['P'][hall_number-1])
                     P1 = abc2matrix(hall_table['P^-1'][hall_number-1])
             else:
                 hall_number = group
                 P = abc2matrix(hall_table['P'][hall_number-1])
                 P1 = abc2matrix(hall_table['P^-1'][hall_number-1])
+            directions = get_symmetry_directions(lattice_type, symbol[0])
+
         elif dim == 2:
             PBC = [1, 1, 0]
+            directions = None
         elif dim == 1:
             PBC = [0, 0, 1]
+            directions = None
 
         if wyckoffs is None:
             wyckoffs = get_wyckoffs(number, dim=dim)
 
         wpdict = {
                   "index": index,
                   "letter": letter_from_index(index, wyckoffs, dim=dim),
@@ -1421,15 +1452,18 @@
                   "PBC": PBC,
                   "dim": dim,
                   "number": number,
                   "P": P,
                   "P1": P1,
                   "hall_number": hall_number,
                   "symbol": symbol,
+                  "directions": directions,
+                  "lattice_type": lattice_type,
                  }
+
         return Wyckoff_position.from_dict(wpdict)
 
     def from_symops_wo_group(ops):
         """
         search Wyckoff Position by symmetry operations
         Now only supports space group symmetry
         Assuming general position only
@@ -1763,20 +1797,28 @@
     def get_site_symm_wo_translation(self):
         ops = []
         for op in self.symmetry[0]:
             op = SymmOp.from_rotation_and_translation(op.rotation_matrix, [0, 0, 0])
             ops.append(op)
         return ops
 
+    def get_site_symmetry_object(self):
+        ops = self.get_site_symm_ops()
+        return site_symmetry(ops, self.lattice_type, self.symbol[0])
+
     def get_site_symmetry(self):
+        ss = self.get_site_symmetry_object()
+        self.site_symm = ss.name #ss_string_from_ops(ops, self.number, dim=self.dim)
+
+    def get_site_symm_ops(self):
         if self.euclidean:
             ops = self.get_euclidean_symmetries()
         else:
             ops = self.symmetry[0]
-        self.site_symm = ss_string_from_ops(ops, self.number, dim=self.dim)
+        return ops
 
     def get_hm_number(tol=1e-5):
         if self.index == 0:
             return get_symmetry_from_ops(self.ops, tol)[0]
         else:
             print(self)
             raise ValueError("input must be general position")
@@ -2508,15 +2550,15 @@
     Args:
         ops: SymmOp object
         permutation: list, e.g. [0, 1, 2]
 
     Returns:
         the new xyz string after transformation
     """
-    if permutation == [0,1,2]:
+    if permutation == [0, 1, 2]:
         return ops
     else:
         new = []
         for op in ops:
             m = op.affine_matrix.copy()
             m[:3,:] = m[permutation, :]
             for row in range(3):
@@ -2642,357 +2684,359 @@
         for k, b in enumerate(a):
             num += 1
             if num == i:
                 return [j, k]
     return None
 
 
-def i_from_jk(j, k, olist):
+class site_symmetry:
     """
-    Inverse operation of jk_from_i: gives one list index from 2
+    Derive the site symmetry group from symmetry operations
+    site-symmetry group is indicated by an oriented symbol,
+    which is a variation of the Hermann–Mauguin point-group
+    symbol that provides information about the orientation
+    of the symmetry elements. The constituents of the oriented
+    symbol are ordered according to the symmetry directions of
+    the corresponding crystal lattice (primary, secondary and tertiary)
 
     Args:
-        j, k: indices corresponding to the location of an element in the
-            organized list
-        olist: the organized list of Wyckoff positions or molecular orientations
+        ops: a list of SymmOp objects representing the site symmetry
+        lattice_type (str): e.g., 'cubic'
+        hm_symbol (str): hm_symbol for lattice 'P', 'R'
 
     Returns:
-        i: one index corresponding to the item's location in the
-            unorganized list
+        a string representing the site symmetry (e.g., `2mm`)
     """
-    num = -1
-    for x, a in enumerate(olist):
-        for y, b in enumerate(a):
-            num += 1
-            if x == j and y == k:
-                return num
-    return None
+    def __init__(self, ops, lattice_type, hm_symbol):
 
+        #self.G = G
+        self.opas = [OperationAnalyzer(op) for op in ops]
+        self.lattice_type = lattice_type
+        self.directions = get_symmetry_directions(lattice_type, hm_symbol)
+        tables = self.to_table()
+        self.set_full_hm_symbols(tables)
+        self.set_short_symbols()
+
+    def to_matrix_representation(self):
+        """
+        To create a 15 * 14 binary matrix to represent the
+        symmetry elements on each axes
+        #[1, -1, 2, m, 3, 2/m, 4, -3, 6, 4/m, -6, 6/m]
+        [1, -1, 2, m, 3, 4, -3, 6, -6]
+        """
+        symbols = ['1', '-1', '2', 'm', '3', '4', '-4', '-3', '6', '-6']
+        matrix = np.zeros([len(all_directions), len(symbols)], dtype=int)
+        # every direction must has identity symmetry
+        matrix[:, 0] = 1
+        self.inversion = False
+
+        for opa in self.opas:
+            if opa.type == 'inversion':
+                self.inversion = True
+            elif opa.type != 'identity':
+                for i, ax in enumerate(all_directions):
+                    store = False
+                    if self.lattice_type in ['hexagonal', 'trigonal']:
+                        ax0 = np.dot(ax, hex_cell.T)
+                        ax0 /= np.linalg.norm(ax0)
+                    else:
+                        ax0 = ax / np.linalg.norm(ax)
+                    if np.isclose(abs(np.dot(opa.axis, ax0)), 1):
+                        store = True
+                        break
+                if store:
+                    # Pure rotation
+                    #print('add symmetry', i, ax, opa.type, opa.order)
+                    if opa.type == 'rotation':
+                        if opa.order == 2:
+                            matrix[i, 2] = 1
+                        elif opa.order == 3:
+                            matrix[i, 4] = 1
+                        elif opa.order == 4:
+                            matrix[i, 5] = 1
+                        elif opa.order == 6:
+                            matrix[i, 8] = 1
+                        else:
+                            raise RuntimeError("Unexpected rotation order", opa.order)
+                    elif opa.type == 'rotoinversion':
+                        if opa.order == 2:
+                            matrix[i, 3] = 1 # -2 is m
+                        elif opa.order == 3:
+                            matrix[i, 7] = 1 # -2 is m
+                        elif opa.order == 4:
+                            matrix[i, 6] = 1 # -4
+                        elif opa.order == 6:
+                            matrix[i, 9] = 1
+                        else:
+                            raise RuntimeError("Unexpected rotinversion order", opa.order)
+            if self.inversion:
+                matrix[:, 1] = 1 # if inversion is present
+        return matrix
 
-def ss_string_from_ops(ops, number, dim=3, complete=True):
-    """
-    Print the Hermann-Mauguin symbol for a site symmetry group, using a list of
-    SymmOps as input. Note that the symbol does not necessarily refer to the
-    x,y,z axes. For information on reading these symbols, see:
-    http://en.wikipedia.org/wiki/Hermann-Mauguin_notation#Point_groups
+    def to_table(self, skip=False):
+        """
+        Get the complete table representation.
 
-    Args:
-        ops: a list of SymmOp objects representing the site symmetry
-        number: International number of the symmetry group. Used to determine which
-            axes to show. For example, a 3-fold rotation in a cubic system is
-            written as ".3.", whereas a 3-fold rotation in a trigonal system is
-            written as "3.."
-        dim: the dimension of the crystal. Also used to determine notation type
-        complete: whether or not all symmetry operations in the group
-            are present. If False, we generate the rest
+        Args:
+            skip (bool): whether or not skip 1 or -1 symmetry
 
-    Returns:
-        a string representing the site symmetry (e.g., `2mm`)
-    """
-    # TODO: Automatically detect which symm_type to use based on ops
-    # Determine which notation to use
-    symm_type = "high"
-    if dim == 3:
-        if number >= 1 and number <= 74:
-            # Triclinic, monoclinic, orthorhombic
-            symm_type = "low"
-        elif number >= 75 and number <= 194:
-            # Trigonal, Hexagonal, Tetragonal
-            symm_type = "medium"
-        elif number >= 195 and number <= 230:
-            # cubic
-            symm_type = "high"
-    if dim == 2:
-        if number >= 1 and number <= 48:
-            # Triclinic, monoclinic, orthorhombic
-            symm_type = "low"
-        elif number >= 49 and number <= 80:
-            # Trigonal, Hexagonal, Tetragonal
-            symm_type = "medium"
-    if dim == 1:
-        if number >= 1 and number <= 22:
-            # Triclinic, monoclinic, orthorhombic
-            symm_type = "low"
-        elif number >= 23 and number <= 75:
-            # Trigonal, Hexagonal, Tetragonal
-            symm_type = "medium"
-
-    # TODO: replace sg with number, add dim variable
-    # Return the symbol for a single axis
-    # Will be called later in the function
-    def get_symbol(opas, order, has_reflection):
-        # ops: a list of Symmetry operations about the axis
-        # order: highest order of any symmetry operation about the axis
-        # has_reflection: whether or not the axis has mirror symmetry
-        if has_reflection:
-            # rotations have priority
-            for opa in opas:
-                if opa.order == order and opa.type == "rotation":
-                    return str(opa.rotation_order) + "/m"
-            for opa in opas:
-                if (
-                    opa.order == order
-                    and opa.type == "rotoinversion"
-                    and opa.order != 2
-                ):
-                    return "-" + str(opa.rotation_order)
-            return "m"
-        elif has_reflection is False:
-            # rotoinversion has priority
-            for opa in opas:
-                if opa.order == order and opa.type == "rotoinversion":
-                    return "-" + str(opa.rotation_order)
-            for opa in opas:
-                if opa.order == order and opa.type == "rotation":
-                    return str(opa.rotation_order)
-            return "."
-
-    # Given a list of single-axis symbols, return the one with highest symmetry
-    # Will be called later in the function
-    def get_highest_symbol(symbols):
-        symbol_list = [
-            ".",
-            "2",
-            "m",
-            "-2",
-            "2/m",
-            "3",
-            "4",
-            "-4",
-            "4/m",
-            "-3",
-            "6",
-            "-6",
-            "6/m",
-        ]
-        max_index = 0
-        use_list = True
-        for j, symbol in enumerate(symbols):
-            if symbol in symbol_list:
-                i = symbol_list.index(symbol)
-            else:
-                use_list = False
-                num_str = "".join(c for c in symbol if c.isdigit())
-                i1 = int(num_str)
-                if "m" in symbol or "-" in symbol:
-                    if i1 % 2 == 0:
-                        i = i1
-                    elif i1 % 2 == 1:
-                        i = i1 * 2
+        Returns:
+            sorted table with (list of symmetry elements, symbols, order)
+        """
+        # Complete list of symmetry for one given axis
+        # symbols = ['1', '-1', '2', 'm', '3', '4', '-4', '-3', '6', '-6']
+        if self.lattice_type == 'triclinic': skip = False
+
+        matrix = self.to_matrix_representation()
+        tables = []
+        for i, axis in enumerate(all_directions):
+            direction_id = find_axis_order(axis, self.directions)
+            if direction_id is not None:
+                if skip:
+                    num_symmetries = matrix[i, 2:].sum()
                 else:
-                    i = i1
-            if i > max_index:
-                max_j = j
-                max_index = i
-        if use_list is True:
-            return symbol_list[max_index]
-        else:
-            return symbols[max_j]
-
-    def are_symmetrically_equivalent(index1, index2):
-        """
-        Return whether or not two axes are symmetrically equivalent
-        It is assumed that both axes possess the same symbol
-        Will be called within combine_axes
-        """
-
-        axis1 = axes[index1]
-        axis2 = axes[index2]
-        condition1 = False
-        condition2 = False
-        # Check for an operation mapping one axis onto the other
-        for op in ops:
-            if condition1 is False or condition2 is False:
-                new1 = op.operate(axis1)
-                new2 = op.operate(axis2)
-                if np.isclose(abs(np.dot(new1, axis2)), 1):
-                    condition1 = True
-                if np.isclose(abs(np.dot(new2, axis1)), 1):
-                    condition2 = True
-        if condition1 is True and condition2 is True:
-            return True
-        else:
-            return False
+                    num_symmetries = matrix[i].sum()
+                if num_symmetries > 0:
+                    strs = '{:4d} ({:2d} {:2d} {:2d}): '.format(direction_id, *axis)
+                    strs += "{:4d}{:4d}{:4d}{:4d}{:4d}{:4d}{:4d}{:4d}{:4d}{:4d}".format(*matrix[i])
+                    symbol = self.get_highest_symmetry(matrix[i])
+                    strs += "{:>6s}".format(symbol)
+                    tables.append((strs, symbol, direction_id))
+            #else:
+            #    raise ValueError('Wrong input axis', axis, 'lattice_type', self.lattice_type)
+        sorted_tables = sorted(tables, key=lambda x: x[-1])
+        return sorted_tables
 
-    def combine_axes(indices):
+    def set_full_hm_symbols(self, tables):
         """
-        Given a list of axis indices, return the combined symbol
-        Axes may or may not be symmetrically equivalent, but must be of the same
-        type (x/y/z, face-diagonal, body-diagonal)
-        Will be called for mid- and high-symmetry crystallographic point groups
-        """
-
-        symbols = {}
-        for index in deepcopy(indices):
-            symbol = get_symbol(params[index], orders[index], reflections[index])
-            if symbol == ".":
-                indices.remove(index)
-            else:
-                symbols[index] = symbol
-
-        if len(indices) == 0:
-            return "."
-
-        # Remove redundant axes
-        for i in deepcopy(indices):
-            for j in deepcopy(indices):
-                if j > i:
-                    if symbols[i] == symbols[j]:
-                        if are_symmetrically_equivalent(i, j):
-                            if j in indices:
-                                indices.remove(j)
-
-        # Combine symbols for non-equivalent axes
-        new_symbols = []
-        for i in indices:
-            new_symbols.append(symbols[i])
-
-        symbol = ""
-        while new_symbols != []:
-            highest = get_highest_symbol(new_symbols)
-            symbol += highest
-            new_symbols.remove(highest)
-        if symbol == "":
-            printx("Error: could not combine site symmetry axes.", priority=1)
-            return
-        else:
-            return symbol
-
-    # Generate needed ops
-    if not complete:
-        ops = generate_full_symmops(ops, 1e-3)
-
-    # Get OperationAnalyzer object for all ops
-    opas = []
-    for op in ops:
-        opas.append(OperationAnalyzer(op))
-
-    # Store the symmetry of each axis
-    params = [[], [], [], [], [], [], [], [], [], [], [], [], []]
-    has_inversion = False
-    # Store possible symmetry axes for crystallographic point groups
-    axes = [
-        [1, 0, 0],
-        [0, 1, 0],
-        [0, 0, 1],
-        [1, 1, 0],
-        [0, 1, 1],
-        [1, 0, 1],
-        [1, -1, 0],
-        [0, 1, -1],
-        [1, 0, -1],
-        [1, 1, 1],
-        [-1, 1, 1],
-        [1, -1, 1],
-        [1, 1, -1],
-    ]
-
-    for i, axis in enumerate(axes):
-        axes[i] = axis / np.linalg.norm(axis)
-
-    for opa in opas:
-
-        # Search for the primary rotation axis
-        if opa.type != "identity" and opa.type != "inversion":
-            found = False
-            for i, axis in enumerate(axes):
-                if np.isclose(abs(np.dot(opa.axis, axis)), 1):
-                    found = True
-                    params[i].append(opa)
-
-            # Store uncommon axes for trigonal and hexagonal lattices
-            if not found: #is False:
-                axes.append(opa.axis)
-                # Check that new axis is not symmetrically equivalent to others
-                unique = True
-                for i, axis in enumerate(axes):
-                    if i != len(axes) - 1:
-                        if are_symmetrically_equivalent(i, len(axes) - 1):
-                            unique = False
-                if unique: # is True:
-                    params.append([opa])
-                else: #if unique is False:
-                    axes.pop()
-
-        elif opa.type == "inversion":
-            has_inversion = True
-
-    # Determine how many high-symmetry axes are present
-    n_axes = 0
-    # Store the order of each axis
-    orders = []
-    # Store whether or not each axis has reflection symmetry
-    reflections = []
-    for axis in params:
-        order = 1
-        high_symm = False
-        has_reflection = False
-        for opa in axis:
-            if opa.order >= 3:
-                high_symm = True
-            if opa.order > order:
-                order = opa.order
-            if opa.order == 2 and opa.type == "rotoinversion":
-                has_reflection = True
-        orders.append(order)
-
-        if high_symm: #== True:
-            n_axes += 1
-        reflections.append(has_reflection)
-    # Triclinic, monoclinic, orthorhombic
-    # Positions in symbol refer to x,y,z axes respectively
-    if symm_type == "low":
-        symbol = (
-            get_symbol(params[0], orders[0], reflections[0])
-            + get_symbol(params[1], orders[1], reflections[1])
-            + get_symbol(params[2], orders[2], reflections[2])
-        )
-        if symbol != "...":
-            return symbol
-        elif symbol == "...":
-            if has_inversion: #is True:
-                return "-1"
-            else:
-                return "1"
-    # Trigonal, Hexagonal, Tetragonal
-    elif symm_type == "medium":
-        # 1st symbol: z axis
-        s1 = get_symbol(params[2], orders[2], reflections[2])
-        # 2nd symbol: x or y axes (whichever have higher symmetry)
-        s2 = combine_axes([0, 1])
-        # 3rd symbol: face-diagonal axes (whichever have highest symmetry)
-        s3 = combine_axes(list(range(3, len(axes))))
-        symbol = s1 + " " + s2 + " " + s3
-        if symbol != ". . .":
-            return symbol
-        elif symbol == ". . .":
-            if has_inversion: #is True:
-                return "-1"
-            else:
-                return "1"
-    # Cubic
-    elif symm_type == "high":
-        pass
-        # 1st symbol: x, y, and/or z axes (whichever have highest symmetry)
-        s1 = combine_axes([0, 1, 2])
-        # 2nd symbol: body-diagonal axes (whichever has highest symmetry)
-        s2 = combine_axes([9, 10, 11, 12])
-        # 3rd symbol: face-diagonal axes (whichever have highest symmetry)
-        s3 = combine_axes([3, 4, 5, 6, 7, 8])
-        symbol = s1 + " " + s2 + " " + s3
-        if symbol != ". . .":
-            return symbol
-        elif symbol == ". . .":
-            if has_inversion: #is True:
-                return "-1"
-            else:
-                return "1"
-    else:
-        printx("Error: invalid spacegroup number", priority=1)
-        return
+        Set the full hm symbols for each axis
+
+        Args:
+            tables: sorted table with (list of symmetry elements, symbols, order)
+
+        Returns:
+            a list of symmetry elements on {primary, secondary, tertiery} directions
+        """
+        hm_symbols = [[] for _ in range(len(self.directions))]
+        #for row in tables: print(row)
+        for row in tables:
+            (_, symbol, direction_id) = row
+            if symbol not in ['1', '-1']:
+                hm_symbols[direction_id].append(symbol)
+            #print(hm_symbols, direction_id)
+
+        for i, hm_symbol in enumerate(hm_symbols):
+            if len(hm_symbol) == 0:
+                hm_symbols[i] = ['.']
+            #elif hm_symbol == ['1']:
+            #    hm_symbols[i] = ['.']
+        self.hm_symbols  = hm_symbols
+
+    def unique_symmetry(self, symbols, symmetry):
+        for symbol in symbols:
+            if symbol not in ['.', symmetry]:
+                return False
+        return True
+
+    def ref_symmetry(self, symbols, reference):
+        for symbol in symbols:
+            if symbol in reference:
+                return True
+        return False
+
+
+    def set_short_symbols(self):
+        """
+        Set short symbols from the Full symbols
+        """
+        #if hasattr(self, 'hm_symbols'):
+        #    self.set_full_hm_symbols()
+
+        self.symbols = []
+        #print(self.hm_symbols)
+        for hm_symbol in self.hm_symbols:
+            if len(hm_symbol) == 1:
+                #print('single', hm_symbol)
+                self.symbols.append(hm_symbol[0])
+            else:
+                symbol = ''
+                for hm in hm_symbol:
+                    symbol += hm
+                self.symbols.append(symbol)
+                #print('multi', hm_symbol)
+
+        # Some simplifications
+        if self.lattice_type == 'orthorhombic':
+            if self.symbols == ['2/m', '2/m', '2/m']:
+                self.symbols = ['m', 'm', 'm']
+
+        elif self.lattice_type == 'tetragonal':
+            for i, symbol in enumerate(self.symbols):
+                if symbol == '2/m2/m':
+                    self.symbols[i] = 'mm'
+                elif symbol == '2/m':
+                    if not self.unique_symmetry(self.symbols, '2/m'):
+                        self.symbols[i] = 'm'
+                elif symbol == 'm2':
+                    self.symbols[i] = '2m'
+            if self.symbols == ['4', '22', '22']:
+                self.symbols = ['4', '2', '2']
+            elif self.symbols == ['4', 'mm', 'mm']:
+                self.symbols = ['4', 'm', 'm']
+            elif self.symbols == ['-4', '22', 'mm']:
+                self.symbols = ['-4', '2', 'm']
+            elif self.symbols == ['-4', 'mm', '22']:
+                self.symbols = ['-4', 'm', '2']
+            elif self.symbols == ['2/m', '2/m', '2/m']:
+                self.symbols = ['m', 'm', 'm']
+            elif self.symbols == ['4/m', 'mm', 'mm']:
+                self.symbols = ['4/m', 'm', 'm']
+
+        elif self.lattice_type in ['trigonal', 'hexagonal']:
+            for i, symbol in enumerate(self.symbols):
+                if symbol in ['2/m2/m', '2/m2/m2/m', 'mm', 'mmm']:
+                    if not self.unique_symmetry(self.symbols, symbol):
+                        self.symbols[i] = 'm'
+                elif symbol in ['22', '222']:
+                    if not self.unique_symmetry(self.symbols, symbol):
+                        self.symbols[i] = '2'
+            if self.symbols == ['2/m', '2/m', '2/m']:
+                self.symbols = ['m', 'm', 'm']
+
+        elif self.lattice_type == 'cubic':
+            for i, symbol in enumerate(self.symbols):
+                if symbol in ['2/m2/m2/m']:
+                    if not self.unique_symmetry(self.symbols, symbol):
+                        self.symbols[i] = 'm'
+                    else:
+                        self.symbols[i] = 'mmm'
+                elif symbol == 'mmm':
+                    if not self.unique_symmetry(self.symbols, symbol):
+                        self.symbols[i] = 'm'
+                elif symbol == '222':
+                    #print(symbol, self.unique_symmetry(self.symbols, symbol))
+                    if not self.unique_symmetry(self.symbols, symbol):
+                        self.symbols[i] = '2'
+                elif symbol in ['2222', '222222']:
+                    self.symbols[i] = '2'
+                elif symbol in ['333', '3333']:
+                    self.symbols[i] = '3'
+                elif symbol in ['-3-3-3-3']:
+                    self.symbols[i] = '-3'
+                elif symbol == '444':
+                    self.symbols[i] = '4'
+                elif symbol == '-4-4-4':
+                    self.symbols[i] = '-4'
+                elif symbol == '422':
+                    self.symbols[i] = '42'
+                elif symbol == '-422':
+                    self.symbols[i] = '-42'
+                elif symbol == '2mm':
+                    self.symbols[i] = 'mm2'
+                elif symbol in ['mmmm', 'mmmmmm']:
+                    self.symbols[i] = 'm'
+                elif symbol in ['2m']:
+                    self.symbols[i] = 'm2'
+                elif symbol in ['4mm']:
+                    self.symbols[i] = '4m'
+                elif symbol in ['-4mm']:
+                    self.symbols[i] = '-4m'
+                elif symbol == '4/m2/m2/m':
+                    self.symbols[i] = '4/mm'
+                elif symbol in ['4/m4/m4/m', '2/m2/m2/m2/m2/m2/m']:
+                    self.symbols[i] = 'm'
+                elif symbol == '2/m2/m':
+                    if self.ref_symmetry(self.symbols, ['4/mm']):
+                        self.symbols[i] = 'm'
+                    else:
+                        self.symbols[i] = 'mm'
+                elif symbol == '2/m':
+                    if not self.unique_symmetry(self.symbols, symbol):
+                        self.symbols[i] = 'm'
+
+            for i, symbol in enumerate(self.symbols):
+                if symbol == 'mm':
+                    if self.ref_symmetry(self.symbols, ['-42', '4m']):
+                        self.symbols[i] = 'm'
+                if symbol == '22':
+                    if self.ref_symmetry(self.symbols, ['42', '-4m']):
+                        self.symbols[i] = '2'
+
+
+        #    #if self.symbols in [['4', '-3', '2'], ['-4', '-3', 'm']]:
+        #    #    self.symbols = ['m', '-3', 'm']
+        #    #if '222' in self.symbols:
+        #    #    if len(self.opas) > 4:
+        #    #        for i in range(len(self.symbols)):
+        #    #            if self.symbols[i] == '222':
+        #    #                self.symbols[i] = '2'#; print('Find ===')
+
+        self.get_name()
+
+    def get_name(self):
+        if self.symbols in [['.', '.', '.'], ['.', '.'], ['.']]:
+            if self.inversion:
+                self.name = '-1'
+            else:
+                self.name = '1'
+        else:
+            self.name = ''
+            for symbol in self.symbols:
+                #self.name += ' '
+                for s in symbol:
+                    self.name += s
+
+    def to_beautiful_matrix_representation(self, skip=True):
+        """
+        A shortcut to check the representation
+
+        Args:
+            skip (bool): whether or not skip 1 or -1 symmetry
+        """
+        print('Order    Axis       1  -1   2   m   3   4  -4  -3   6  -6   Group')
+        sorted_tables = self.to_table(skip)
+        for row in sorted_tables:
+            print(row[0])
+
+    def get_highest_symmetry(self, row):
+        #['1']
+        #['1', '-1']
+        #['1', '2']
+        #['1', 'm']
+        #['1', '3']
+        #['1', '2', 'm', '2/m']
+        #['1', '2', '4']
+        #['1', '2', '-4']
+        #['1', '-1', '3', '-3']
+        #['1', '2', '3', '6']
+        #['1', 'm', '3', '-6']
+        #['1', '-1', '2', 'm', '4', '-4', '4/m']
+        #['1', '-1', '2', 'm', '3', '-3', '6', '-6', '6/m']
+        ref_arrays = [
+            (np.array([1, 0, 0, 0, 0, 0, 0, 0, 0, 0], dtype=int), '1'),
+            (np.array([1, 1, 0, 0, 0, 0, 0, 0, 0, 0], dtype=int), '-1'),
+            (np.array([1, 0, 1, 0, 0, 0, 0, 0, 0, 0], dtype=int), '2'),
+            (np.array([1, 0, 0, 1, 0, 0, 0, 0, 0, 0], dtype=int), 'm'),
+            (np.array([1, 0, 0, 0, 1, 0, 0, 0, 0, 0], dtype=int), '3'),
+            (np.array([1, 1, 1, 1, 0, 0, 0, 0, 0, 0], dtype=int), '2/m'),
+            (np.array([1, 0, 1, 0, 0, 1, 0, 0, 0, 0], dtype=int), '4'),
+            (np.array([1, 0, 1, 0, 0, 0, 1, 0, 0, 0], dtype=int), '-4'),
+            (np.array([1, 1, 0, 0, 1, 0, 0, 1, 0, 0], dtype=int), '-3'),
+            (np.array([1, 0, 1, 0, 1, 0, 0, 0, 1, 0], dtype=int), '6'),
+            (np.array([1, 0, 0, 1, 1, 0, 0, 0, 0, 1], dtype=int), '-6'),
+            (np.array([1, 1, 1, 1, 0, 1, 1, 0, 0, 0], dtype=int), '4/m'),
+            (np.array([1, 1, 1, 1, 1, 0, 0, 1, 1, 1], dtype=int), '6/m')]
+
+        for ref_array in ref_arrays:
+            if np.array_equal(row, ref_array[0]):
+                return ref_array[1]
+        else:
+            symbols = ['1', '-1', '2', 'm', '3', '4', '-4', '-3', '6', '-6']
+            strs = [symbols[i] for i, x in enumerate(row) if x == 1]
+            raise ValueError("Incompatible symmetry list", strs)
 
 
 def organized_wyckoffs(group):
     """
     Takes a Group object or unorganized list of Wyckoff positions and returns
     a 2D list of Wyckoff positions organized by multiplicity.
 
@@ -3403,14 +3447,16 @@
             lattice_type = "triclinic"
         elif number <= 15:
             lattice_type = "monoclinic"
         elif number <= 74:
             lattice_type = "orthorhombic"
         elif number <= 142:
             lattice_type = "tetragonal"
+        elif number <= 167:
+            lattice_type = "trigonal"
         elif number <= 194:
             lattice_type = "hexagonal"
         elif number <= 230:
             lattice_type = "cubic"
     elif dim == 2:
         PBC = [1, 1, 0]
         if number <= 2:
@@ -3862,12 +3908,73 @@
                         if abs(b[j]) > 0:
                             coef = tmp[j]/b[j]
                             break
                     tran[i] -= coef*b[3]
         ops1.append(SymmOp.from_rotation_and_translation(rot, tran))
 
     return ops
-#op = SymmOp.from_xyz_str('y+1/8, -y+1/8, 0')
-#op = SymmOp.from_xyz_str('1/8, y+1/8, -y+1/8')
-#op = SymmOp.from_xyz_str(['x+1/8,x+1/8,z+1/8', '')
-#print(trim_op(op).as_xyz_str())
-#from_symops(ops, group=None, permutation=True)
+
+def find_axis_order(axis, directions):
+    for i, axes in enumerate(directions):
+        for ax in axes:
+            if ax == axis:
+                return i
+
+
+def get_symmetry_directions(lattice_type, symbol='P', unique_axis='b'):
+    """
+    Get the symmetry directions
+    """
+    if lattice_type == 'monoclinic':
+        if unique_axis == 'b':
+            return [[(0, 1, 0)]]
+        elif unique_axis == 'c':
+            return [[(0, 0, 1)]]
+        else:
+            return [[(1, 0, 0)]]
+    elif lattice_type == 'orthorhombic':
+        return [[(1, 0, 0)],
+                [(0, 1, 0)],
+                [(0, 0, 1)]]
+    elif lattice_type == 'tetragonal':
+        return [[(0, 0, 1)],
+                [(1, 0, 0), (0, 1, 0)],
+                [(1, -1, 0), (1, 1, 0)]]
+    elif lattice_type == 'hexagonal' or (lattice_type == 'trigonal' and symbol=='P'):
+        return [[(0, 0, 1)],
+                [(1, 0, 0), (0, 1, 0), (1, 1, 0)],
+                [(1, -1, 0), (1, 2, 0), (2, 1, 0)]]
+    elif lattice_type == 'trigonal' and symbol=='R':
+        return [[(0, 0, 1)],
+                [(1, 0, 0), (0, 1, 0), (1, 1, 0)]]
+    #elif lattice_type == 'rhombohedral':
+    #    return [[(0, 0, 1)],
+    #            [(1, 0, 0), (0, 1, 0), (-1, -1, 0)]]
+    elif lattice_type == 'cubic':
+        return [[(1, 0, 0), (0, 1, 0), (0, 0, 1)],
+                [(1, 1, 1), (1, -1, -1), (-1, 1, -1), (-1, -1, 1)],
+                [(1, -1, 0), (1, 1, 0), (0, 1, -1),
+                 (0, 1, 1), (-1, 0, 1), (1, 0, 1)]]
+    else:
+        return [[(0, 1, 0)]]
+
+
+if __name__ == "__main__":
+    print("Test of pyxtal.wp.site symmetry")
+    for i in [14, 36, 62, 99, 143, 160, 182, 191, 225, 230]:
+        g = Group(i)
+        for wp in g:
+            wp.get_site_symmetry()
+            print("{:4d} {:10s} {:10s}".format(wp.number, wp.get_label(), wp.site_symm))
+
+    print("Test of pyxtal.wp.site symmetry representation")
+    for i in [14, 36, 62, 99, 143, 160, 182, 191, 225, 230]:
+        g = Group(i)
+        for wp in g:
+            #ss = site_symmetry(wp.get_site_symm_ops(), g.lattice_type, g.symbol[0])
+            if wp.index > 0:
+                ss = wp.get_site_symmetry_object()
+                print('\n{:4d} {:10s} {:10s}'.format(wp.number, wp.get_label(), ss.name), ss.hm_symbols)
+                ss.to_beautiful_matrix_representation(skip=True)
+                #print(ss.to_matrix_representation())
+                #if ss.name == '1':
+                #    print("Problem eixt")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyxtal-0.6.4/pyxtal/test_all.py` & `pyxtal-0.6.5/pyxtal/test_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # python -m unittest pyxtal/test_all.py
 import unittest
 import os
+import importlib.util
 
 from random import choice, shuffle
 import numpy as np
-from pkg_resources import resource_filename
 from pymatgen.core import Structure
 from pymatgen.core import Lattice as pmg_Lattice
 from pymatgen.core.structure import Molecule
 import pymatgen.analysis.structure_matcher as sm
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 from pymatgen.core.operations import SymmOp
 
@@ -17,14 +17,19 @@
 from pyxtal.molecule import pyxtal_molecule
 from pyxtal.symmetry import Group, Wyckoff_position, get_wyckoffs, Hall
 from pyxtal.XRD import Similarity
 from pyxtal.operations import get_inverse
 from pyxtal.supergroup import supergroups, supergroup
 from pyxtal.util import generate_wp_lib
 
+
+def resource_filename(package_name, resource_path):
+    package_path = importlib.util.find_spec(package_name).submodule_search_locations[0]
+    return os.path.join(package_path, resource_path)
+
 cif_path = resource_filename("pyxtal", "database/cifs/")
 l01 = Lattice.from_matrix([[4.08, 0, 0], [0, 9.13, 0], [0, 0, 5.50]])
 l02 = Lattice.from_para(4.08, 9.13, 5.50, 90, 90, 90)
 wp1 = Wyckoff_position.from_group_and_index(36, 0)
 wp2 = Wyckoff_position.from_group_and_letter(36, "4a")
 
 class TestGroup(unittest.TestCase):
@@ -483,22 +488,24 @@
 
 class TestWP(unittest.TestCase):
 
     def test_wp_check_translation(self):
         pass
 
     def test_wp_site_symm(self):
-        data = [(143, 1, '3 . .'),
-                (230, 6, '. 3 2'),
-                (160, 1, '. . m'),
-                (160, 2, '3 m .')]
+        data = [(143, 1, '3..'),
+                (160, 1, '.m'),
+                (160, 2, '3m'),
+                (230, 6, '.32'),
+               ]
         for d in data:
             (sg, i, symbol) = d
             wp = Group(sg)[i]
             wp.get_site_symmetry()
+            print("\n========", wp.site_symm, symbol, "==========\n")
             self.assertTrue(wp.site_symm == symbol)
 
     def test_wp_dof(self):
         for sg in range(1, 231):
             g = Group(sg)
             for wp in g:
                 axs = wp.get_frozen_axis()
```

### Comparing `pyxtal-0.6.4/pyxtal/tolerance.py` & `pyxtal-0.6.5/pyxtal/tolerance.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/util.py` & `pyxtal-0.6.5/pyxtal/util.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/viz.py` & `pyxtal-0.6.5/pyxtal/viz.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/wyckoff_site.py` & `pyxtal-0.6.5/pyxtal/wyckoff_site.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal/wyckoff_split.py` & `pyxtal-0.6.5/pyxtal/wyckoff_split.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/pyxtal.egg-info/PKG-INFO` & `pyxtal-0.6.5/pyxtal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxtal
-Version: 0.6.4
+Version: 0.6.5
 Summary: Python code for generation of crystal structures based on symmetry constraints.
 Home-page: https://github.com/qzhu2017/PyXtal
 Author: Scott Fredericks, Qiang Zhu
 Author-email: qiang.zhu@unlv.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyxtal-0.6.4/pyxtal.egg-info/SOURCES.txt` & `pyxtal-0.6.5/pyxtal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/scripts/pyxtal_main.py` & `pyxtal-0.6.5/scripts/pyxtal_main.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/scripts/pyxtal_symmetry.py` & `pyxtal-0.6.5/scripts/pyxtal_symmetry.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.4/setup.py` & `pyxtal-0.6.5/setup.py`

 * *Files identical despite different names*

