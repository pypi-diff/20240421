# Comparing `tmp/func_adl_servicex_xaodr21-2.0.0.21.2.231a11.tar.gz` & `tmp/func_adl_servicex_xaodr21-2.0.0.21.2.231a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_adl_servicex_xaodr21-2.0.0.21.2.231a11.tar", max compression
+gzip compressed data, was "func_adl_servicex_xaodr21-2.0.0.21.2.231a9.tar", max compression
```

## Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11.tar` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9.tar`

### file list

```diff
@@ -1,132 +1,127 @@
--rw-r--r--   0        0        0      571 2024-04-21 08:51:19.540310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/README.md
--rw-r--r--   0        0        0     1168 2024-04-21 08:51:19.712309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/Muon/__init__.py
--rw-r--r--   0        0        0     7861 2024-04-21 08:51:19.660309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/Muon/muonstationindex.py
--rw-r--r--   0        0        0     1166 2024-04-21 08:51:19.712309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Detail/TSchemaRuleSet/__init__.py
--rw-r--r--   0        0        0     1421 2024-04-21 08:51:19.660309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Detail/TSchemaRuleSet/tmatches.py
--rw-r--r--   0        0        0     1198 2024-04-21 08:51:19.712309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Detail/__init__.py
--rw-r--r--   0        0        0     2070 2024-04-21 08:51:19.660309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Detail/tschemaruleset.py
--rw-r--r--   0        0        0     1668 2024-04-21 08:51:19.712309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Fit/__init__.py
--rw-r--r--   0        0        0     8181 2024-04-21 08:51:19.660309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Fit/bindata.py
--rw-r--r--   0        0        0     1856 2024-04-21 08:51:19.660309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Fit/datarange.py
--rw-r--r--   0        0        0     5519 2024-04-21 08:51:19.660309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Fit/fitconfig.py
--rw-r--r--   0        0        0     2464 2024-04-21 08:51:19.660309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Fit/fitdata.py
--rw-r--r--   0        0        0    11642 2024-04-21 08:51:19.660309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Fit/fitresult.py
--rw-r--r--   0        0        0     3600 2024-04-21 08:51:19.660309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Fit/parametersettings.py
--rw-r--r--   0        0        0     1479 2024-04-21 08:51:19.712309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Math/__init__.py
--rw-r--r--   0        0        0     1748 2024-04-21 08:51:19.660309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Math/ibaseparam.py
--rw-r--r--   0        0        0     1142 2024-04-21 08:51:19.664309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Math/ioptions.py
--rw-r--r--   0        0        0    15120 2024-04-21 08:51:19.664309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Math/minimizer.py
--rw-r--r--   0        0        0     7091 2024-04-21 08:51:19.664309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Math/minimizeroptions.py
--rw-r--r--   0        0        0     1211 2024-04-21 08:51:19.712309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/__init__.py
--rw-r--r--   0        0        0     1650 2024-04-21 08:51:19.664309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/tschemarule.py
--rw-r--r--   0        0        0     9273 2024-04-21 08:51:19.712309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/__init__.py
--rw-r--r--   0        0        0     1786 2024-04-21 08:51:19.624310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/calibration_event_config.py
--rw-r--r--   0        0        0    11099 2024-04-21 08:51:19.624310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/calibration_support.py
--rw-r--r--   0        0        0     4967 2024-04-21 08:51:19.636309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/calosampling.py
--rw-r--r--   0        0        0     1975 2024-04-21 08:51:19.624310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/default_calibration_config.py
--rw-r--r--   0        0        0    17855 2024-04-21 08:51:19.640310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_btagging_v1__.py
--rw-r--r--   0        0        0    23243 2024-04-21 08:51:19.640310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_calocluster_v1__.py
--rw-r--r--   0        0        0    17874 2024-04-21 08:51:19.644310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_eventinfo_v1__.py
--rw-r--r--   0        0        0     6179 2024-04-21 08:51:19.644310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_iparticle__.py
--rw-r--r--   0        0        0    11161 2024-04-21 08:51:19.644310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_jet_v1__.py
--rw-r--r--   0        0        0    17262 2024-04-21 08:51:19.648310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_muon_v1__.py
--rw-r--r--   0        0        0     9438 2024-04-21 08:51:19.648310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_muonsegment_v1__.py
--rw-r--r--   0        0        0     9163 2024-04-21 08:51:19.648310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_neutralparticle_v1__.py
--rw-r--r--   0        0        0    13320 2024-04-21 08:51:19.652310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_pfo_v1__.py
--rw-r--r--   0        0        0    10002 2024-04-21 08:51:19.652310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_tautrack_v1__.py
--rw-r--r--   0        0        0    14399 2024-04-21 08:51:19.652310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_trackparticle_v1__.py
--rw-r--r--   0        0        0    26625 2024-04-21 08:51:19.656309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_truthparticle_v1__.py
--rw-r--r--   0        0        0     9846 2024-04-21 08:51:19.656309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_truthvertex_v1__.py
--rw-r--r--   0        0        0    10155 2024-04-21 08:51:19.656309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_vertex_v1__.py
--rw-r--r--   0        0        0    28940 2024-04-21 08:51:19.620310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/event_collection.py
--rw-r--r--   0        0        0     1034 2024-04-21 08:51:19.620310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/func_adl_iterable.py
--rw-r--r--   0        0        0     2792 2024-04-21 08:51:19.624310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/metadata_for_collections.py
--rw-r--r--   0        0        0     1067 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/mutex.py
--rw-r--r--   0        0        0     1260 2024-04-21 08:51:19.712309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/std/__init__.py
--rw-r--r--   0        0        0     1092 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/std/vector_float_.py
--rw-r--r--   0        0        0     1085 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/std/vector_int_.py
--rw-r--r--   0        0        0     2025 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/str.py
--rw-r--r--   0        0        0     2979 2024-04-21 08:51:19.624310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/sx_dataset.py
--rw-r--r--   0        0        0     8948 2024-04-21 08:51:19.664309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/tcomplex.py
--rw-r--r--   0        0        0       65 2024-04-21 08:51:19.624310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/add_calibration_to_job.py
--rw-r--r--   0        0        0      849 2024-04-21 08:51:19.624310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/corrections_electron.py
--rw-r--r--   0        0        0     1319 2024-04-21 08:51:19.624310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/corrections_jet.py
--rw-r--r--   0        0        0      619 2024-04-21 08:51:19.624310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/corrections_met.py
--rw-r--r--   0        0        0      799 2024-04-21 08:51:19.624310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/corrections_muon.py
--rw-r--r--   0        0        0     1465 2024-04-21 08:51:19.624310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/corrections_overlap.py
--rw-r--r--   0        0        0     1081 2024-04-21 08:51:19.624310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/corrections_photon.py
--rw-r--r--   0        0        0      632 2024-04-21 08:51:19.624310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/corrections_tau.py
--rw-r--r--   0        0        0      517 2024-04-21 08:51:19.624310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/pileup_tool.py
--rw-r--r--   0        0        0      502 2024-04-21 08:51:19.624310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/sys_error_tool.py
--rw-r--r--   0        0        0     2885 2024-04-21 08:51:19.664309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/tlorentzvector.py
--rw-r--r--   0        0        0     4876 2024-04-21 08:51:19.624310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/trigger.py
--rw-r--r--   0        0        0     4256 2024-04-21 08:51:19.664309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/trotation.py
--rw-r--r--   0        0        0     2400 2024-04-21 08:51:19.664309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/tsqlresult.py
--rw-r--r--   0        0        0     1616 2024-04-21 08:51:19.664309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/tsqlrow.py
--rw-r--r--   0        0        0     5960 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/tthread.py
--rw-r--r--   0        0        0     2723 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/tvector2.py
--rw-r--r--   0        0        0     3393 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/tvector3.py
--rw-r--r--   0        0        0     2572 2024-04-21 08:51:19.624310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/type_support.py
--rw-r--r--   0        0        0     1275 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_calocluster_v1___.py
--rw-r--r--   0        0        0     1255 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_iparticle___.py
--rw-r--r--   0        0        0     1275 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_muonsegment_v1___.py
--rw-r--r--   0        0        0     1291 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_neutralparticle_v1___.py
--rw-r--r--   0        0        0     1243 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_pfo_v1___.py
--rw-r--r--   0        0        0     1263 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_tautrack_v1___.py
--rw-r--r--   0        0        0     1283 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_trackparticle_v1___.py
--rw-r--r--   0        0        0     1283 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_truthparticle_v1___.py
--rw-r--r--   0        0        0     1275 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_truthvertex_v1___.py
--rw-r--r--   0        0        0     1255 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_vertex_v1___.py
--rw-r--r--   0        0        0     1086 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_float_.py
--rw-r--r--   0        0        0     1080 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_int_.py
--rw-r--r--   0        0        0     1095 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_pair_float_float__.py
--rw-r--r--   0        0        0     1091 2024-04-21 08:51:19.672309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_pair_str_str__.py
--rw-r--r--   0        0        0     1195 2024-04-21 08:51:19.668309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_root_fit_parametersettings_.py
--rw-r--r--   0        0        0     1113 2024-04-21 08:51:19.672309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_str_.py
--rw-r--r--   0        0        0     1150 2024-04-21 08:51:19.672309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_vector_float__.py
--rw-r--r--   0        0        0     1226 2024-04-21 08:51:19.672309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_xaod_caloclusterbadchanneldata_v1_.py
--rw-r--r--   0        0        0     1190 2024-04-21 08:51:19.672309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_xaod_eventinfo_v1_streamtag_.py
--rw-r--r--   0        0        0     1186 2024-04-21 08:51:19.672309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_xaod_eventinfo_v1_subevent_.py
--rw-r--r--   0        0        0     1170 2024-04-21 08:51:19.672309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_xaod_jetconstituent_.py
--rw-r--r--   0        0        0     1267 2024-04-21 08:51:19.712309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/EventInfo_v1/__init__.py
--rw-r--r--   0        0        0     1859 2024-04-21 08:51:19.684309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/EventInfo_v1/streamtag.py
--rw-r--r--   0        0        0     2270 2024-04-21 08:51:19.684309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/EventInfo_v1/subevent.py
--rw-r--r--   0        0        0     1155 2024-04-21 08:51:19.712309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/TruthEvent_v1/__init__.py
--rw-r--r--   0        0        0     1304 2024-04-21 08:51:19.708309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/TruthEvent_v1/pdfinfo.py
--rw-r--r--   0        0        0     1173 2024-04-21 08:51:19.712309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/TruthParticle_v1/__init__.py
--rw-r--r--   0        0        0     1323 2024-04-21 08:51:19.708309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/TruthParticle_v1/polarization.py
--rw-r--r--   0        0        0     4609 2024-04-21 08:51:19.712309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/__init__.py
--rw-r--r--   0        0        0    15528 2024-04-21 08:51:19.672309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/btagging_v1.py
--rw-r--r--   0        0        0     7229 2024-04-21 08:51:19.672309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/btagvertex_v1.py
--rw-r--r--   0        0        0    41009 2024-04-21 08:51:19.676309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/calocluster_v1.py
--rw-r--r--   0        0        0     2229 2024-04-21 08:51:19.676309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/caloclusterbadchanneldata_v1.py
--rw-r--r--   0        0        0     5406 2024-04-21 08:51:19.676309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/calotower_v1.py
--rw-r--r--   0        0        0    11722 2024-04-21 08:51:19.680309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/ditaujet_v1.py
--rw-r--r--   0        0        0     8079 2024-04-21 08:51:19.680309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/egamma_v1.py
--rw-r--r--   0        0        0    10012 2024-04-21 08:51:19.680309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/electron_v1.py
--rw-r--r--   0        0        0    17020 2024-04-21 08:51:19.684309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/eventinfo_v1.py
--rw-r--r--   0        0        0     5324 2024-04-21 08:51:19.684309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/iparticle.py
--rw-r--r--   0        0        0     9669 2024-04-21 08:51:19.688309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/jet_v1.py
--rw-r--r--   0        0        0     2007 2024-04-21 08:51:19.684309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/jetalgorithmtype.py
--rw-r--r--   0        0        0     3124 2024-04-21 08:51:19.684309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/jetconstituent.py
--rw-r--r--   0        0        0     3052 2024-04-21 08:51:19.684309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/jetconstituentvector.py
--rw-r--r--   0        0        0     3142 2024-04-21 08:51:19.684309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/jetinput.py
--rw-r--r--   0        0        0     5486 2024-04-21 08:51:19.688309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/missinget_v1.py
--rw-r--r--   0        0        0    16978 2024-04-21 08:51:19.692309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/muon_v1.py
--rw-r--r--   0        0        0     8106 2024-04-21 08:51:19.688309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/muonsegment_v1.py
--rw-r--r--   0        0        0     7893 2024-04-21 08:51:19.692309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/neutralparticle_v1.py
--rw-r--r--   0        0        0    11482 2024-04-21 08:51:19.696309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/pfo_v1.py
--rw-r--r--   0        0        0     9829 2024-04-21 08:51:19.696309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/photon_v1.py
--rw-r--r--   0        0        0     9107 2024-04-21 08:51:19.696309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/slowmuon_v1.py
--rw-r--r--   0        0        0    32775 2024-04-21 08:51:19.700309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/taujet_v3.py
--rw-r--r--   0        0        0     8665 2024-04-21 08:51:19.700309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/tautrack_v1.py
--rw-r--r--   0        0        0     7184 2024-04-21 08:51:19.700309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/trackcalocluster_v1.py
--rw-r--r--   0        0        0    12327 2024-04-21 08:51:19.704309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/trackparticle_v1.py
--rw-r--r--   0        0        0    11988 2024-04-21 08:51:19.704309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/truthevent_v1.py
--rw-r--r--   0        0        0     7014 2024-04-21 08:51:19.704309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/trutheventbase_v1.py
--rw-r--r--   0        0        0     6676 2024-04-21 08:51:19.708309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/truthmetadata_v1.py
--rw-r--r--   0        0        0    22732 2024-04-21 08:51:19.708309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/truthparticle_v1.py
--rw-r--r--   0        0        0     8566 2024-04-21 08:51:19.712309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/truthvertex_v1.py
--rw-r--r--   0        0        0     8876 2024-04-21 08:51:19.712309 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/vertex_v1.py
--rw-r--r--   0        0        0      388 2024-04-21 08:51:19.544310 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/pyproject.toml
--rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 func_adl_servicex_xaodr21-2.0.0.21.2.231a11/PKG-INFO
+-rw-r--r--   0        0        0      340 2023-11-10 10:14:07.856776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/README.md
+-rw-r--r--   0        0        0     1166 2023-11-10 10:14:07.960776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Detail/TSchemaRuleSet/__init__.py
+-rw-r--r--   0        0        0     1281 2023-11-10 10:14:07.912776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Detail/TSchemaRuleSet/tmatches.py
+-rw-r--r--   0        0        0     1198 2023-11-10 10:14:07.960776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Detail/__init__.py
+-rw-r--r--   0        0        0     1824 2023-11-10 10:14:07.912776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Detail/tschemaruleset.py
+-rw-r--r--   0        0        0     1668 2023-11-10 10:14:07.960776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Fit/__init__.py
+-rw-r--r--   0        0        0     7579 2023-11-10 10:14:07.912776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Fit/bindata.py
+-rw-r--r--   0        0        0     1716 2023-11-10 10:14:07.912776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Fit/datarange.py
+-rw-r--r--   0        0        0     5379 2023-11-10 10:14:07.912776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Fit/fitconfig.py
+-rw-r--r--   0        0        0     2324 2023-11-10 10:14:07.916776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Fit/fitdata.py
+-rw-r--r--   0        0        0    11472 2023-11-10 10:14:07.916776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Fit/fitresult.py
+-rw-r--r--   0        0        0     3460 2023-11-10 10:14:07.916776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Fit/parametersettings.py
+-rw-r--r--   0        0        0     1479 2023-11-10 10:14:07.964776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Math/__init__.py
+-rw-r--r--   0        0        0     1608 2023-11-10 10:14:07.916776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Math/ibaseparam.py
+-rw-r--r--   0        0        0     1002 2023-11-10 10:14:07.916776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Math/ioptions.py
+-rw-r--r--   0        0        0    14747 2023-11-10 10:14:07.916776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Math/minimizer.py
+-rw-r--r--   0        0        0     6951 2023-11-10 10:14:07.916776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Math/minimizeroptions.py
+-rw-r--r--   0        0        0     1211 2023-11-10 10:14:07.964776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/__init__.py
+-rw-r--r--   0        0        0     1510 2023-11-10 10:14:07.916776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/tschemarule.py
+-rw-r--r--   0        0        0     8888 2023-11-10 10:14:07.964776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/__init__.py
+-rw-r--r--   0        0        0     1786 2023-11-10 10:14:07.884776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/calibration_event_config.py
+-rw-r--r--   0        0        0    11099 2023-11-10 10:14:07.884776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/calibration_support.py
+-rw-r--r--   0        0        0     1975 2023-11-10 10:14:07.884776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/default_calibration_config.py
+-rw-r--r--   0        0        0    17445 2023-11-10 10:14:07.896776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_btagging_v1__.py
+-rw-r--r--   0        0        0    10138 2023-11-10 10:14:07.896776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_calocluster_v1__.py
+-rw-r--r--   0        0        0    14680 2023-11-10 10:14:07.896776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_eventinfo_v1__.py
+-rw-r--r--   0        0        0     5979 2023-11-10 10:14:07.900776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_iparticle__.py
+-rw-r--r--   0        0        0    10159 2023-11-10 10:14:07.900776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_jet_v1__.py
+-rw-r--r--   0        0        0    13078 2023-11-10 10:14:07.904776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_muon_v1__.py
+-rw-r--r--   0        0        0     8412 2023-11-10 10:14:07.900776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_muonsegment_v1__.py
+-rw-r--r--   0        0        0     8963 2023-11-10 10:14:07.904776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_neutralparticle_v1__.py
+-rw-r--r--   0        0        0    12337 2023-11-10 10:14:07.904776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_pfo_v1__.py
+-rw-r--r--   0        0        0     9638 2023-11-10 10:14:07.908776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_tautrack_v1__.py
+-rw-r--r--   0        0        0    14199 2023-11-10 10:14:07.908776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_trackparticle_v1__.py
+-rw-r--r--   0        0        0    25532 2023-11-10 10:14:07.908776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_truthparticle_v1__.py
+-rw-r--r--   0        0        0     9646 2023-11-10 10:14:07.912776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_truthvertex_v1__.py
+-rw-r--r--   0        0        0     9955 2023-11-10 10:14:07.912776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_vertex_v1__.py
+-rw-r--r--   0        0        0    28940 2023-11-10 10:14:07.880777 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/event_collection.py
+-rw-r--r--   0        0        0     1034 2023-11-10 10:14:07.880777 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/func_adl_iterable.py
+-rw-r--r--   0        0        0     2792 2023-11-10 10:14:07.884776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/metadata_for_collections.py
+-rw-r--r--   0        0        0      927 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/mutex.py
+-rw-r--r--   0        0        0     1260 2023-11-10 10:14:07.960776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/std/__init__.py
+-rw-r--r--   0        0        0      952 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/std/vector_float_.py
+-rw-r--r--   0        0        0      945 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/std/vector_int_.py
+-rw-r--r--   0        0        0     1885 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/str.py
+-rw-r--r--   0        0        0     1018 2023-11-10 10:14:07.884776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/sx_dataset.py
+-rw-r--r--   0        0        0     8808 2023-11-10 10:14:07.916776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/tcomplex.py
+-rw-r--r--   0        0        0       65 2023-11-10 10:14:07.884776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/add_calibration_to_job.py
+-rw-r--r--   0        0        0      849 2023-11-10 10:14:07.884776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/corrections_electron.py
+-rw-r--r--   0        0        0     1319 2023-11-10 10:14:07.884776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/corrections_jet.py
+-rw-r--r--   0        0        0      619 2023-11-10 10:14:07.884776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/corrections_met.py
+-rw-r--r--   0        0        0      799 2023-11-10 10:14:07.884776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/corrections_muon.py
+-rw-r--r--   0        0        0     1465 2023-11-10 10:14:07.884776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/corrections_overlap.py
+-rw-r--r--   0        0        0     1081 2023-11-10 10:14:07.884776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/corrections_photon.py
+-rw-r--r--   0        0        0      632 2023-11-10 10:14:07.884776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/corrections_tau.py
+-rw-r--r--   0        0        0      517 2023-11-10 10:14:07.884776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/pileup_tool.py
+-rw-r--r--   0        0        0      502 2023-11-10 10:14:07.884776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/sys_error_tool.py
+-rw-r--r--   0        0        0     2709 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/tlorentzvector.py
+-rw-r--r--   0        0        0     4876 2023-11-10 10:14:07.884776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/trigger.py
+-rw-r--r--   0        0        0     3906 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/trotation.py
+-rw-r--r--   0        0        0     2260 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/tsqlresult.py
+-rw-r--r--   0        0        0     1476 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/tsqlrow.py
+-rw-r--r--   0        0        0     4875 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/tthread.py
+-rw-r--r--   0        0        0     2583 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/tvector2.py
+-rw-r--r--   0        0        0     3217 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/tvector3.py
+-rw-r--r--   0        0        0     2572 2023-11-10 10:14:07.884776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/type_support.py
+-rw-r--r--   0        0        0     1135 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_calocluster_v1___.py
+-rw-r--r--   0        0        0     1115 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_iparticle___.py
+-rw-r--r--   0        0        0     1135 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_muonsegment_v1___.py
+-rw-r--r--   0        0        0     1151 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_neutralparticle_v1___.py
+-rw-r--r--   0        0        0     1103 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_pfo_v1___.py
+-rw-r--r--   0        0        0     1123 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_tautrack_v1___.py
+-rw-r--r--   0        0        0     1143 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_trackparticle_v1___.py
+-rw-r--r--   0        0        0     1143 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_truthparticle_v1___.py
+-rw-r--r--   0        0        0     1135 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_truthvertex_v1___.py
+-rw-r--r--   0        0        0     1115 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_vertex_v1___.py
+-rw-r--r--   0        0        0      946 2023-11-10 10:14:07.924776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_float_.py
+-rw-r--r--   0        0        0      940 2023-11-10 10:14:07.924776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_int_.py
+-rw-r--r--   0        0        0      955 2023-11-10 10:14:07.924776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_pair_float_float__.py
+-rw-r--r--   0        0        0      951 2023-11-10 10:14:07.924776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_pair_str_str__.py
+-rw-r--r--   0        0        0     1055 2023-11-10 10:14:07.920776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_root_fit_parametersettings_.py
+-rw-r--r--   0        0        0      973 2023-11-10 10:14:07.924776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_str_.py
+-rw-r--r--   0        0        0     1010 2023-11-10 10:14:07.924776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_vector_float__.py
+-rw-r--r--   0        0        0     1086 2023-11-10 10:14:07.924776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_xaod_caloclusterbadchanneldata_v1_.py
+-rw-r--r--   0        0        0     1050 2023-11-10 10:14:07.924776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_xaod_eventinfo_v1_streamtag_.py
+-rw-r--r--   0        0        0     1046 2023-11-10 10:14:07.924776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_xaod_eventinfo_v1_subevent_.py
+-rw-r--r--   0        0        0     1030 2023-11-10 10:14:07.924776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_xaod_jetconstituent_.py
+-rw-r--r--   0        0        0     1267 2023-11-10 10:14:07.960776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/EventInfo_v1/__init__.py
+-rw-r--r--   0        0        0     1719 2023-11-10 10:14:07.936776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/EventInfo_v1/streamtag.py
+-rw-r--r--   0        0        0     1794 2023-11-10 10:14:07.936776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/EventInfo_v1/subevent.py
+-rw-r--r--   0        0        0     1155 2023-11-10 10:14:07.960776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/TruthEvent_v1/__init__.py
+-rw-r--r--   0        0        0     1164 2023-11-10 10:14:07.956776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/TruthEvent_v1/pdfinfo.py
+-rw-r--r--   0        0        0     1173 2023-11-10 10:14:07.964776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/TruthParticle_v1/__init__.py
+-rw-r--r--   0        0        0     1183 2023-11-10 10:14:07.960776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/TruthParticle_v1/polarization.py
+-rw-r--r--   0        0        0     4397 2023-11-10 10:14:07.960776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/__init__.py
+-rw-r--r--   0        0        0    15118 2023-11-10 10:14:07.928776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/btagging_v1.py
+-rw-r--r--   0        0        0     7029 2023-11-10 10:14:07.924776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/btagvertex_v1.py
+-rw-r--r--   0        0        0     8716 2023-11-10 10:14:07.928776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/calocluster_v1.py
+-rw-r--r--   0        0        0     1755 2023-11-10 10:14:07.928776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/caloclusterbadchanneldata_v1.py
+-rw-r--r--   0        0        0     5206 2023-11-10 10:14:07.928776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/calotower_v1.py
+-rw-r--r--   0        0        0    11522 2023-11-10 10:14:07.932776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/ditaujet_v1.py
+-rw-r--r--   0        0        0     7849 2023-11-10 10:14:07.932776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/egamma_v1.py
+-rw-r--r--   0        0        0     9782 2023-11-10 10:14:07.932776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/electron_v1.py
+-rw-r--r--   0        0        0    12606 2023-11-10 10:14:07.936776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/eventinfo_v1.py
+-rw-r--r--   0        0        0     5124 2023-11-10 10:14:07.936776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/iparticle.py
+-rw-r--r--   0        0        0     8767 2023-11-10 10:14:07.940776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/jet_v1.py
+-rw-r--r--   0        0        0     2984 2023-11-10 10:14:07.936776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/jetconstituent.py
+-rw-r--r--   0        0        0     2912 2023-11-10 10:14:07.936776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/jetconstituentvector.py
+-rw-r--r--   0        0        0     5286 2023-11-10 10:14:07.940776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/missinget_v1.py
+-rw-r--r--   0        0        0    11439 2023-11-10 10:14:07.940776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/muon_v1.py
+-rw-r--r--   0        0        0     7180 2023-11-10 10:14:07.940776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/muonsegment_v1.py
+-rw-r--r--   0        0        0     7693 2023-11-10 10:14:07.944776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/neutralparticle_v1.py
+-rw-r--r--   0        0        0    10549 2023-11-10 10:14:07.944776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/pfo_v1.py
+-rw-r--r--   0        0        0     9599 2023-11-10 10:14:07.944776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/photon_v1.py
+-rw-r--r--   0        0        0     8907 2023-11-10 10:14:07.948776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/slowmuon_v1.py
+-rw-r--r--   0        0        0    32158 2023-11-10 10:14:07.948776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/taujet_v3.py
+-rw-r--r--   0        0        0     8301 2023-11-10 10:14:07.952776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/tautrack_v1.py
+-rw-r--r--   0        0        0     6899 2023-11-10 10:14:07.952776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/trackcalocluster_v1.py
+-rw-r--r--   0        0        0    12127 2023-11-10 10:14:07.952776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/trackparticle_v1.py
+-rw-r--r--   0        0        0     9667 2023-11-10 10:14:07.956776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/truthevent_v1.py
+-rw-r--r--   0        0        0     6814 2023-11-10 10:14:07.956776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/trutheventbase_v1.py
+-rw-r--r--   0        0        0     6476 2023-11-10 10:14:07.956776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/truthmetadata_v1.py
+-rw-r--r--   0        0        0    21654 2023-11-10 10:14:07.960776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/truthparticle_v1.py
+-rw-r--r--   0        0        0     8366 2023-11-10 10:14:07.960776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/truthvertex_v1.py
+-rw-r--r--   0        0        0     8676 2023-11-10 10:14:07.960776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/vertex_v1.py
+-rw-r--r--   0        0        0      464 2023-11-10 10:14:07.856776 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/pyproject.toml
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 func_adl_servicex_xaodr21-2.0.0.21.2.231a9/PKG-INFO
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/Muon/__init__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,12 +22,15 @@
             self._loaded = importlib.import_module(self._name)
         return getattr(self._loaded, __name)
 
 
 # Class loads. We do this to both enable type checking and also
 # get around potential circular references in the C++ data model.
 if not TYPE_CHECKING:
-    muonstationindex = _load_me("func_adl_servicex_xaodr21.Muon.muonstationindex")
+    tschemarule = _load_me("func_adl_servicex_xaodr21.ROOT.tschemarule")
 else:
-    from . import muonstationindex
+    from . import tschemarule
 
-# Include sub-namespace items
+# Include sub-namespace items
+from . import Math
+from . import Fit
+from . import Detail
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Detail/TSchemaRuleSet/__init__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Detail/TSchemaRuleSet/__init__.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Detail/TSchemaRuleSet/tmatches.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Detail/TSchemaRuleSet/tmatches.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'empty': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::Detail::TSchemaRuleSet::TMatches',
         'method_name': 'empty',
@@ -16,38 +15,33 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::Detail::TSchemaRuleSet::TMatches',
         'method_name': 'data',
         'return_type': 'const ROOT::TSchemaRule*',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class TMatches:
     "A class"
 
-
     def empty(self) -> bool:
         "A method"
         ...
 
     def data(self) -> func_adl_servicex_xaodr21.ROOT.tschemarule.TSchemaRule:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Detail/__init__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Detail/__init__.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Detail/tschemaruleset.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/tsqlrow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,53 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
-    'GetClassVersion': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ROOT::Detail::TSchemaRuleSet',
-        'method_name': 'GetClassVersion',
-        'return_type': 'int',
-    },
     'ImplFileLine': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ROOT::Detail::TSchemaRuleSet',
+        'type_string': 'TSQLRow',
         'method_name': 'ImplFileLine',
         'return_type': 'int',
     },
     'DeclFileLine': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ROOT::Detail::TSchemaRuleSet',
+        'type_string': 'TSQLRow',
         'method_name': 'DeclFileLine',
         'return_type': 'int',
     },
     'DistancetoPrimitive': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ROOT::Detail::TSchemaRuleSet',
+        'type_string': 'TSQLRow',
         'method_name': 'DistancetoPrimitive',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class TSchemaRuleSet:
+class TSQLRow:
     "A class"
 
-    class EConsistencyCheck(Enum):
-        kNoCheck = 0
-        kCheckAll = 1
-        kCheckConflict = 2
-
-
-    def GetClassVersion(self) -> int:
-        "A method"
-        ...
-
     def ImplFileLine(self) -> int:
         "A method"
         ...
 
     def DeclFileLine(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Fit/__init__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Fit/__init__.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Fit/bindata.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Fit/bindata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'HaveCoordErrors': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::Fit::BinData',
         'method_name': 'HaveCoordErrors',
@@ -98,20 +97,14 @@
     },
     'RefVolume': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::Fit::BinData',
         'method_name': 'RefVolume',
         'return_type': 'double',
     },
-    'GetErrorType': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ROOT::Fit::BinData',
-        'method_name': 'GetErrorType',
-        'return_type': 'ROOT::Fit::BinData::ErrorType',
-    },
     'SumOfContent': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::Fit::BinData',
         'method_name': 'SumOfContent',
         'return_type': 'double',
     },
     'SumOfError2': {
@@ -160,44 +153,33 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::Fit::BinData',
         'method_name': 'Range',
         'return_type': 'const ROOT::Fit::DataRange',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class BinData:
     "A class"
 
-    class ErrorType(Enum):
-        kNoError = 0
-        kValueError = 1
-        kCoordError = 2
-        kAsymError = 3
-
-
     def HaveCoordErrors(self) -> bool:
         "A method"
         ...
 
     def HaveAsymErrors(self) -> bool:
         "A method"
         ...
@@ -254,18 +236,14 @@
         "A method"
         ...
 
     def RefVolume(self) -> float:
         "A method"
         ...
 
-    def GetErrorType(self) -> func_adl_servicex_xaodr21.ROOT.Fit.bindata.BinData.ErrorType:
-        "A method"
-        ...
-
     def SumOfContent(self) -> float:
         "A method"
         ...
 
     def SumOfError2(self) -> float:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Fit/datarange.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_trackparticle_v1___.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
-    'NDim': {
+    'size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ROOT::Fit::DataRange',
-        'method_name': 'NDim',
-        'return_type': 'unsigned int',
-    },
-    'Size': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ROOT::Fit::DataRange',
-        'method_name': 'Size',
-        'return_type': 'unsigned int',
-    },
-    'IsSet': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ROOT::Fit::DataRange',
-        'method_name': 'IsSet',
-        'return_type': 'bool',
-    },
-    'IsInside': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ROOT::Fit::DataRange',
-        'method_name': 'IsInside',
-        'return_type': 'bool',
+        'type_string': 'vector<ElementLink<DataVector<xAOD::TrackParticle_v1>>>',
+        'method_name': 'size',
+        'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class DataRange:
+class vector_ElementLink_DataVector_xAOD_TrackParticle_v1___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_trackparticle_v1__.ElementLink_DataVector_xAOD_TrackParticle_v1__]):
     "A class"
 
-
-    def NDim(self) -> int:
-        "A method"
-        ...
-
-    def Size(self, icoord: int) -> int:
-        "A method"
-        ...
-
-    def IsSet(self) -> bool:
-        "A method"
-        ...
-
-    def IsInside(self, x: float, icoord: int) -> bool:
+    def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Fit/fitconfig.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Fit/fitconfig.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'ParSettings': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::Fit::FitConfig',
         'method_name': 'ParSettings',
@@ -93,38 +92,33 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::Fit::FitConfig',
         'method_name': 'UseWeightCorrection',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class FitConfig:
     "A class"
 
-
     def ParSettings(self, i: int) -> func_adl_servicex_xaodr21.ROOT.Fit.parametersettings.ParameterSettings:
         "A method"
         ...
 
     def ParamsSettings(self) -> func_adl_servicex_xaodr21.vector_root_fit_parametersettings_.vector_ROOT_Fit_ParameterSettings_:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Fit/fitdata.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Fit/fitdata.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'GetCoordComponent': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::Fit::FitData',
         'method_name': 'GetCoordComponent',
@@ -40,38 +39,33 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::Fit::FitData',
         'method_name': 'Range',
         'return_type': 'const ROOT::Fit::DataRange',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class FitData:
     "A class"
 
-
     def GetCoordComponent(self, ipoint: int, icoord: int) -> float:
         "A method"
         ...
 
     def Coords(self, ipoint: int) -> float:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Fit/fitresult.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Fit/fitresult.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'MinimizerType': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::Fit::FitResult',
         'method_name': 'MinimizerType',
@@ -237,38 +236,33 @@
         'type_string': 'ROOT::Fit::FitResult',
         'method_name': 'GetParameterName',
         'return_type_element': '__gnu_cxx::__normal_iterator<char*,string>',
         'return_type_collection': 'string',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class FitResult:
     "A class"
 
-
     def MinimizerType(self) -> func_adl_servicex_xaodr21.str.str:
         "A method"
         ...
 
     def IsValid(self) -> bool:
         "A method"
         ...
@@ -389,15 +383,15 @@
         "A method"
         ...
 
     def Contour(self, ipar: int, jpar: int, npoints: int, pntsx: float, pntsy: float, confLevel: float) -> bool:
         "A method"
         ...
 
-    def Index(self, name: func_adl_servicex_xaodr21.str.str) -> int:
+    def Index(self, name: str) -> int:
         "A method"
         ...
 
     def NormalizedErrors(self) -> bool:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Fit/parametersettings.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Fit/parametersettings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'Value': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::Fit::ParameterSettings',
         'method_name': 'Value',
@@ -65,38 +64,33 @@
         'type_string': 'ROOT::Fit::ParameterSettings',
         'method_name': 'Name',
         'return_type_element': '__gnu_cxx::__normal_iterator<char*,string>',
         'return_type_collection': 'const string',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class ParameterSettings:
     "A class"
 
-
     def Value(self) -> float:
         "A method"
         ...
 
     def StepSize(self) -> float:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Math/__init__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Math/__init__.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Math/ibaseparam.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Math/ibaseparam.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'Parameters': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::Math::IBaseParam',
         'method_name': 'Parameters',
@@ -23,38 +22,33 @@
         'type_string': 'ROOT::Math::IBaseParam',
         'method_name': 'ParameterName',
         'return_type_element': '__gnu_cxx::__normal_iterator<char*,string>',
         'return_type_collection': 'string',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class IBaseParam:
     "A class"
 
-
     def Parameters(self) -> float:
         "A method"
         ...
 
     def NPar(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Math/ioptions.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Math/ioptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'Clone': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::Math::IOptions',
         'method_name': 'Clone',
         'return_type': 'ROOT::Math::IOptions*',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class IOptions:
     "A class"
 
-
     def Clone(self) -> func_adl_servicex_xaodr21.ROOT.Math.ioptions.IOptions:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Math/minimizer.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Math/minimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'SetVariable': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::Math::Minimizer',
         'method_name': 'SetVariable',
@@ -299,55 +298,50 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::Math::Minimizer',
         'method_name': 'Options',
         'return_type': 'ROOT::Math::MinimizerOptions',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class Minimizer:
     "A class"
 
-
-    def SetVariable(self, ivar: int, name: func_adl_servicex_xaodr21.str.str, val: float, step: float) -> bool:
+    def SetVariable(self, ivar: int, name: str, val: float, step: float) -> bool:
         "A method"
         ...
 
-    def SetLowerLimitedVariable(self, ivar: int, name: func_adl_servicex_xaodr21.str.str, val: float, step: float, lower: float) -> bool:
+    def SetLowerLimitedVariable(self, ivar: int, name: str, val: float, step: float, lower: float) -> bool:
         "A method"
         ...
 
-    def SetUpperLimitedVariable(self, ivar: int, name: func_adl_servicex_xaodr21.str.str, val: float, step: float, upper: float) -> bool:
+    def SetUpperLimitedVariable(self, ivar: int, name: str, val: float, step: float, upper: float) -> bool:
         "A method"
         ...
 
-    def SetLimitedVariable(self, ivar: int, name: func_adl_servicex_xaodr21.str.str, val: float, step: float, lower: float, upper: float) -> bool:
+    def SetLimitedVariable(self, ivar: int, name: str, val: float, step: float, lower: float, upper: float) -> bool:
         "A method"
         ...
 
-    def SetFixedVariable(self, ivar: int, name: func_adl_servicex_xaodr21.str.str, val: float) -> bool:
+    def SetFixedVariable(self, ivar: int, name: str, val: float) -> bool:
         "A method"
         ...
 
     def SetVariableValue(self, ivar: int, value: float) -> bool:
         "A method"
         ...
 
@@ -379,15 +373,15 @@
         "A method"
         ...
 
     def IsFixedVariable(self, ivar: int) -> bool:
         "A method"
         ...
 
-    def GetVariableSettings(self, ivar: int, pars: func_adl_servicex_xaodr21.ROOT.Fit.parametersettings.ParameterSettings) -> bool:
+    def GetVariableSettings(self, ivar: int, pars: ParameterSettings) -> bool:
         "A method"
         ...
 
     def SetVariableInitialRange(self, noname_arg: int, noname_arg_1: float, noname_arg_2: float) -> bool:
         "A method"
         ...
 
@@ -475,15 +469,15 @@
         "A method"
         ...
 
     def VariableName(self, ivar: int) -> func_adl_servicex_xaodr21.str.str:
         "A method"
         ...
 
-    def VariableIndex(self, name: func_adl_servicex_xaodr21.str.str) -> int:
+    def VariableIndex(self, name: str) -> int:
         "A method"
         ...
 
     def PrintLevel(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/Math/minimizeroptions.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Math/minimizeroptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'DefaultMinimizerType': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::Math::MinimizerOptions',
         'method_name': 'DefaultMinimizerType',
@@ -128,38 +127,33 @@
         'type_string': 'ROOT::Math::MinimizerOptions',
         'method_name': 'MinimizerAlgorithm',
         'return_type_element': '__gnu_cxx::__normal_iterator<char*,string>',
         'return_type_collection': 'const string',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class MinimizerOptions:
     "A class"
 
-
     def DefaultMinimizerType(self) -> func_adl_servicex_xaodr21.str.str:
         "A method"
         ...
 
     def DefaultMinimizerAlgo(self) -> func_adl_servicex_xaodr21.str.str:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/__init__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/std/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,15 +22,14 @@
             self._loaded = importlib.import_module(self._name)
         return getattr(self._loaded, __name)
 
 
 # Class loads. We do this to both enable type checking and also
 # get around potential circular references in the C++ data model.
 if not TYPE_CHECKING:
-    tschemarule = _load_me("func_adl_servicex_xaodr21.ROOT.tschemarule")
+    vector_float_ = _load_me("func_adl_servicex_xaodr21.std.vector_float_")
+    vector_int_ = _load_me("func_adl_servicex_xaodr21.std.vector_int_")
 else:
-    from . import tschemarule
+    from . import vector_float_
+    from . import vector_int_
 
-# Include sub-namespace items
-from . import Math
-from . import Detail
-from . import Fit
+# Include sub-namespace items
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/ROOT/tschemarule.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/tschemarule.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'ImplFileLine': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::TSchemaRule',
         'method_name': 'ImplFileLine',
@@ -22,38 +21,33 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'ROOT::TSchemaRule',
         'method_name': 'DistancetoPrimitive',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class TSchemaRule:
     "A class"
 
-
     def ImplFileLine(self) -> int:
         "A method"
         ...
 
     def DeclFileLine(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/__init__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,12 @@
 from typing import Any, TYPE_CHECKING
 try:
     from .sx_dataset import SXDSAtlasxAODR21
-    from .sx_dataset import SXDSAtlasxAODR21PHYS
 except ImportError:
-    # Servicex frontend client 2.X not loaded.
     pass
-
-try:
-    from .sx_dataset import FuncADLQuery
-    from .sx_dataset import FuncADLQueryPHYS
-except ImportError:
-    # Servicex frontend client 3.X not loaded.
-    pass
-
 from .func_adl_iterable import FADLStream
 from .trigger import tdt_chain_fired
 from .trigger import tmt_match_object
 from .type_support import cpp_float, cpp_double, cpp_vfloat, cpp_string, cpp_int
 from . import type_support
 from .calibration_support import CalibrationEventConfig, calib_tools
 atlas_release = "21.2.231"
@@ -44,15 +34,14 @@
             self._loaded = importlib.import_module(self._name)
         return getattr(self._loaded, __name)
 
 
 # Class loads. We do this to both enable type checking and also
 # get around potential circular references in the C++ data model.
 if not TYPE_CHECKING:
-    calosampling = _load_me("func_adl_servicex_xaodr21.calosampling")
     elementlink_datavector_xaod_btagging_v1__ = _load_me("func_adl_servicex_xaodr21.elementlink_datavector_xaod_btagging_v1__")
     elementlink_datavector_xaod_calocluster_v1__ = _load_me("func_adl_servicex_xaodr21.elementlink_datavector_xaod_calocluster_v1__")
     elementlink_datavector_xaod_eventinfo_v1__ = _load_me("func_adl_servicex_xaodr21.elementlink_datavector_xaod_eventinfo_v1__")
     elementlink_datavector_xaod_iparticle__ = _load_me("func_adl_servicex_xaodr21.elementlink_datavector_xaod_iparticle__")
     elementlink_datavector_xaod_jet_v1__ = _load_me("func_adl_servicex_xaodr21.elementlink_datavector_xaod_jet_v1__")
     elementlink_datavector_xaod_muonsegment_v1__ = _load_me("func_adl_servicex_xaodr21.elementlink_datavector_xaod_muonsegment_v1__")
     elementlink_datavector_xaod_muon_v1__ = _load_me("func_adl_servicex_xaodr21.elementlink_datavector_xaod_muon_v1__")
@@ -92,15 +81,14 @@
     vector_str_ = _load_me("func_adl_servicex_xaodr21.vector_str_")
     vector_vector_float__ = _load_me("func_adl_servicex_xaodr21.vector_vector_float__")
     vector_xaod_caloclusterbadchanneldata_v1_ = _load_me("func_adl_servicex_xaodr21.vector_xaod_caloclusterbadchanneldata_v1_")
     vector_xaod_eventinfo_v1_streamtag_ = _load_me("func_adl_servicex_xaodr21.vector_xaod_eventinfo_v1_streamtag_")
     vector_xaod_eventinfo_v1_subevent_ = _load_me("func_adl_servicex_xaodr21.vector_xaod_eventinfo_v1_subevent_")
     vector_xaod_jetconstituent_ = _load_me("func_adl_servicex_xaodr21.vector_xaod_jetconstituent_")
 else:
-    from . import calosampling
     from . import elementlink_datavector_xaod_btagging_v1__
     from . import elementlink_datavector_xaod_calocluster_v1__
     from . import elementlink_datavector_xaod_eventinfo_v1__
     from . import elementlink_datavector_xaod_iparticle__
     from . import elementlink_datavector_xaod_jet_v1__
     from . import elementlink_datavector_xaod_muonsegment_v1__
     from . import elementlink_datavector_xaod_muon_v1__
@@ -141,11 +129,10 @@
     from . import vector_vector_float__
     from . import vector_xaod_caloclusterbadchanneldata_v1_
     from . import vector_xaod_eventinfo_v1_streamtag_
     from . import vector_xaod_eventinfo_v1_subevent_
     from . import vector_xaod_jetconstituent_
 
 # Include sub-namespace items
-from . import xAOD
 from . import ROOT
-from . import Muon
+from . import xAOD
 from . import std
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/calibration_event_config.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/calibration_event_config.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/calibration_support.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/calibration_support.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/default_calibration_config.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/default_calibration_config.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_btagging_v1__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_btagging_v1__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'isValid': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::BTagging_v1>>',
         'method_name': 'isValid',
@@ -329,38 +328,33 @@
         'type_string': 'ElementLink<DataVector<xAOD::BTagging_v1>>',
         'method_name': 'isAvailable',
         'return_type': 'bool',
         'deref_count': 2
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class ElementLink_DataVector_xAOD_BTagging_v1__:
     "A class"
 
-
     def isValid(self) -> bool:
         "A method"
         ...
 
     def SV0_significance3D(self) -> float:
         "A method"
         ...
@@ -481,31 +475,31 @@
         "A method"
         ...
 
     def MV1_discriminant(self) -> float:
         "A method"
         ...
 
-    def loglikelihoodratio(self, taggername: func_adl_servicex_xaodr21.str.str, value: float, signal: func_adl_servicex_xaodr21.str.str, bckgd: func_adl_servicex_xaodr21.str.str) -> bool:
+    def loglikelihoodratio(self, taggername: str, value: float, signal: str, bckgd: str) -> bool:
         "A method"
         ...
 
-    def MVx_discriminant(self, taggername: func_adl_servicex_xaodr21.str.str, value: float) -> bool:
+    def MVx_discriminant(self, taggername: str, value: float) -> bool:
         "A method"
         ...
 
-    def pu(self, taggername: func_adl_servicex_xaodr21.str.str, value: float) -> bool:
+    def pu(self, taggername: str, value: float) -> bool:
         "A method"
         ...
 
-    def pb(self, taggername: func_adl_servicex_xaodr21.str.str, value: float) -> bool:
+    def pb(self, taggername: str, value: float) -> bool:
         "A method"
         ...
 
-    def pc(self, taggername: func_adl_servicex_xaodr21.str.str, value: float) -> bool:
+    def pc(self, taggername: str, value: float) -> bool:
         "A method"
         ...
 
     def calcLLR(self, num: float, den: float) -> float:
         "A method"
         ...
 
@@ -531,16 +525,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_calocluster_v1__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_truthparticle_v1__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,500 +1,633 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'isValid': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
         'method_name': 'isValid',
         'return_type': 'bool',
     },
+    'pdgId': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'pdgId',
+        'return_type': 'int',
+        'deref_count': 2
+    },
+    'absPdgId': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'absPdgId',
+        'return_type': 'int',
+        'deref_count': 2
+    },
+    'barcode': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'barcode',
+        'return_type': 'int',
+        'deref_count': 2
+    },
+    'status': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'status',
+        'return_type': 'int',
+        'deref_count': 2
+    },
+    'hasProdVtx': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'hasProdVtx',
+        'return_type': 'bool',
+        'deref_count': 2
+    },
+    'prodVtx': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'prodVtx',
+        'return_type': 'const xAOD::TruthVertex_v1*',
+        'deref_count': 2
+    },
+    'prodVtxLink': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'prodVtxLink',
+        'return_type': 'const ElementLink<DataVector<xAOD::TruthVertex_v1>>',
+        'deref_count': 2
+    },
+    'hasDecayVtx': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'hasDecayVtx',
+        'return_type': 'bool',
+        'deref_count': 2
+    },
+    'decayVtx': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'decayVtx',
+        'return_type': 'const xAOD::TruthVertex_v1*',
+        'deref_count': 2
+    },
+    'decayVtxLink': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'decayVtxLink',
+        'return_type': 'const ElementLink<DataVector<xAOD::TruthVertex_v1>>',
+        'deref_count': 2
+    },
+    'nParents': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'nParents',
+        'return_type': 'int',
+        'deref_count': 2
+    },
+    'parent': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'parent',
+        'return_type': 'const xAOD::TruthParticle_v1*',
+        'deref_count': 2
+    },
+    'nChildren': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'nChildren',
+        'return_type': 'int',
+        'deref_count': 2
+    },
+    'child': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'child',
+        'return_type': 'const xAOD::TruthParticle_v1*',
+        'deref_count': 2
+    },
     'pt': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
         'method_name': 'pt',
         'return_type': 'double',
         'deref_count': 2
     },
     'eta': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
         'method_name': 'eta',
         'return_type': 'double',
         'deref_count': 2
     },
     'phi': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
         'method_name': 'phi',
         'return_type': 'double',
         'deref_count': 2
     },
     'm': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
         'method_name': 'm',
         'return_type': 'double',
         'deref_count': 2
     },
     'e': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
         'method_name': 'e',
         'return_type': 'double',
         'deref_count': 2
     },
     'rapidity': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
         'method_name': 'rapidity',
         'return_type': 'double',
         'deref_count': 2
     },
     'p4': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
         'method_name': 'p4',
         'return_type': 'const TLorentzVector',
         'deref_count': 2
     },
-    'et': {
+    'abseta': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'et',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'abseta',
         'return_type': 'double',
         'deref_count': 2
     },
-    'eSample': {
+    'absrapidity': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'eSample',
-        'return_type': 'float',
-        'deref_count': 2
-    },
-    'etaSample': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'etaSample',
-        'return_type': 'float',
-        'deref_count': 2
-    },
-    'phiSample': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'phiSample',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'absrapidity',
+        'return_type': 'double',
         'deref_count': 2
     },
-    'energy_max': {
+    'px': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'energy_max',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'px',
         'return_type': 'float',
         'deref_count': 2
     },
-    'etamax': {
+    'py': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'etamax',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'py',
         'return_type': 'float',
         'deref_count': 2
     },
-    'phimax': {
+    'pz': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'phimax',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'pz',
         'return_type': 'float',
         'deref_count': 2
     },
-    'etasize': {
+    'charge': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'etasize',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'charge',
+        'return_type': 'double',
         'deref_count': 2
     },
-    'phisize': {
+    'threeCharge': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'phisize',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'threeCharge',
+        'return_type': 'int',
         'deref_count': 2
     },
-    'energyBE': {
+    'isCharged': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'energyBE',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isCharged',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'etaBE': {
+    'isNeutral': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'etaBE',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isNeutral',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'phiBE': {
+    'isPhoton': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'phiBE',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isPhoton',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'setEnergy': {
+    'isLepton': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'setEnergy',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isLepton',
         'return_type': 'bool',
         'deref_count': 2
     },
-    'setEta': {
+    'isChLepton': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'setEta',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isChLepton',
         'return_type': 'bool',
         'deref_count': 2
     },
-    'setPhi': {
+    'isElectron': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'setPhi',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isElectron',
         'return_type': 'bool',
         'deref_count': 2
     },
-    'setEmax': {
+    'isMuon': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'setEmax',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isMuon',
         'return_type': 'bool',
         'deref_count': 2
     },
-    'setEtamax': {
+    'isTau': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'setEtamax',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isTau',
         'return_type': 'bool',
         'deref_count': 2
     },
-    'setPhimax': {
+    'isNeutrino': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'setPhimax',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isNeutrino',
         'return_type': 'bool',
         'deref_count': 2
     },
-    'setEtasize': {
+    'isHadron': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'setEtasize',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isHadron',
         'return_type': 'bool',
         'deref_count': 2
     },
-    'setPhisize': {
+    'isMeson': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'setPhisize',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isMeson',
         'return_type': 'bool',
         'deref_count': 2
     },
-    'retrieveMoment': {
+    'isBaryon': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'retrieveMoment',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isBaryon',
         'return_type': 'bool',
         'deref_count': 2
     },
-    'getMomentValue': {
+    'hasStrange': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'getMomentValue',
-        'return_type': 'double',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'hasStrange',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'eta0': {
+    'hasCharm': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'eta0',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'hasCharm',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'phi0': {
+    'hasBottom': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'phi0',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'hasBottom',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'time': {
+    'isLightMeson': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'time',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isLightMeson',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'samplingPattern': {
+    'isLightBaryon': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'samplingPattern',
-        'return_type': 'unsigned int',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isLightBaryon',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'nSamples': {
+    'isLightHadron': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'nSamples',
-        'return_type': 'unsigned int',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isLightHadron',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'hasSampling': {
+    'isHeavyMeson': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'hasSampling',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isHeavyMeson',
         'return_type': 'bool',
         'deref_count': 2
     },
-    'clusterSize': {
+    'isHeavyBaryon': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'clusterSize',
-        'return_type': 'xAOD::CaloCluster_v1::ClusterSize',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isHeavyBaryon',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'inBarrel': {
+    'isHeavyHadron': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'inBarrel',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isHeavyHadron',
         'return_type': 'bool',
         'deref_count': 2
     },
-    'inEndcap': {
+    'isBottomMeson': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'inEndcap',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isBottomMeson',
         'return_type': 'bool',
         'deref_count': 2
     },
-    'rawE': {
+    'isBottomBaryon': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'rawE',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isBottomBaryon',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'rawEta': {
+    'isBottomHadron': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'rawEta',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isBottomHadron',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'rawPhi': {
+    'isCharmMeson': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'rawPhi',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isCharmMeson',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'rawM': {
+    'isCharmBaryon': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'rawM',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isCharmBaryon',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'altE': {
+    'isCharmHadron': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'altE',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isCharmHadron',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'altEta': {
+    'isStrangeMeson': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'altEta',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isStrangeMeson',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'altPhi': {
+    'isStrangeBaryon': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'altPhi',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isStrangeBaryon',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'altM': {
+    'isStrangeHadron': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'altM',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isStrangeHadron',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'calE': {
+    'isQuark': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'calE',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isQuark',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'calEta': {
+    'isParton': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'calEta',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isParton',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'calPhi': {
+    'isTop': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'calPhi',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isTop',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'calM': {
+    'isW': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'calM',
-        'return_type': 'float',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isW',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'setSignalState': {
+    'isZ': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'setSignalState',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isZ',
         'return_type': 'bool',
         'deref_count': 2
     },
-    'signalState': {
+    'isHiggs': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'signalState',
-        'return_type': 'xAOD::CaloCluster_v1::State',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isHiggs',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'getClusterEtaSize': {
+    'isResonance': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'getClusterEtaSize',
-        'return_type': 'unsigned int',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isResonance',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'getClusterPhiSize': {
+    'isGenSpecific': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'getClusterPhiSize',
-        'return_type': 'unsigned int',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isGenSpecific',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'badChannelList': {
+    'isBSM': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'badChannelList',
-        'return_type_element': 'xAOD::CaloClusterBadChannelData_v1',
-        'return_type_collection': 'const vector<xAOD::CaloClusterBadChannelData_v1>',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'isBSM',
+        'return_type': 'bool',
         'deref_count': 2
     },
-    'getSisterCluster': {
+    'polarization': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
-        'method_name': 'getSisterCluster',
-        'return_type': 'const xAOD::CaloCluster_v1*',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
+        'method_name': 'polarization',
+        'return_type': 'xAOD::TruthParticle_v1::Polarization',
         'deref_count': 2
     },
     'index': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
         'method_name': 'index',
         'return_type': 'int',
         'deref_count': 2
     },
     'usingPrivateStore': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
         'method_name': 'usingPrivateStore',
         'return_type': 'bool',
         'deref_count': 2
     },
     'usingStandaloneStore': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
         'method_name': 'usingStandaloneStore',
         'return_type': 'bool',
         'deref_count': 2
     },
     'hasStore': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
         'method_name': 'hasStore',
         'return_type': 'bool',
         'deref_count': 2
     },
     'hasNonConstStore': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
         'method_name': 'hasNonConstStore',
         'return_type': 'bool',
         'deref_count': 2
     },
     'clearDecorations': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
         'method_name': 'clearDecorations',
         'return_type': 'bool',
         'deref_count': 2
     },
     'auxdataConst': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
         'method_name': 'auxdataConst',
         'return_type': 'U',
         'deref_count': 2
     },
     'isAvailable': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::CaloCluster_v1>>',
+        'type_string': 'ElementLink<DataVector<xAOD::TruthParticle_v1>>',
         'method_name': 'isAvailable',
         'return_type': 'bool',
         'deref_count': 2
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class ElementLink_DataVector_xAOD_CaloCluster_v1__:
+class ElementLink_DataVector_xAOD_TruthParticle_v1__:
     "A class"
 
-
     def isValid(self) -> bool:
         "A method"
         ...
 
+    def pdgId(self) -> int:
+        "A method"
+        ...
+
+    def absPdgId(self) -> int:
+        "A method"
+        ...
+
+    def barcode(self) -> int:
+        "A method"
+        ...
+
+    def status(self) -> int:
+        "A method"
+        ...
+
+    def hasProdVtx(self) -> bool:
+        "A method"
+        ...
+
+    def prodVtx(self) -> func_adl_servicex_xaodr21.xAOD.truthvertex_v1.TruthVertex_v1:
+        "A method"
+        ...
+
+    def prodVtxLink(self) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_truthvertex_v1__.ElementLink_DataVector_xAOD_TruthVertex_v1__:
+        "A method"
+        ...
+
+    def hasDecayVtx(self) -> bool:
+        "A method"
+        ...
+
+    def decayVtx(self) -> func_adl_servicex_xaodr21.xAOD.truthvertex_v1.TruthVertex_v1:
+        "A method"
+        ...
+
+    def decayVtxLink(self) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_truthvertex_v1__.ElementLink_DataVector_xAOD_TruthVertex_v1__:
+        "A method"
+        ...
+
+    def nParents(self) -> int:
+        "A method"
+        ...
+
+    def parent(self, i: int) -> func_adl_servicex_xaodr21.xAOD.truthparticle_v1.TruthParticle_v1:
+        "A method"
+        ...
+
+    def nChildren(self) -> int:
+        "A method"
+        ...
+
+    def child(self, i: int) -> func_adl_servicex_xaodr21.xAOD.truthparticle_v1.TruthParticle_v1:
+        "A method"
+        ...
+
     def pt(self) -> float:
         "A method"
         ...
 
     def eta(self) -> float:
         "A method"
         ...
@@ -515,207 +648,199 @@
         "A method"
         ...
 
     def p4(self) -> func_adl_servicex_xaodr21.tlorentzvector.TLorentzVector:
         "A method"
         ...
 
-    def et(self) -> float:
-        "A method"
-        ...
-
-    def eSample(self, sampling: func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample) -> float:
-        "A method"
-        ...
-
-    def etaSample(self, sampling: func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample) -> float:
+    def abseta(self) -> float:
         "A method"
         ...
 
-    def phiSample(self, sampling: func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample) -> float:
+    def absrapidity(self) -> float:
         "A method"
         ...
 
-    def energy_max(self, sampling: func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample) -> float:
+    def px(self) -> float:
         "A method"
         ...
 
-    def etamax(self, sampling: func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample) -> float:
+    def py(self) -> float:
         "A method"
         ...
 
-    def phimax(self, sampling: func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample) -> float:
+    def pz(self) -> float:
         "A method"
         ...
 
-    def etasize(self, sampling: func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample) -> float:
+    def charge(self) -> float:
         "A method"
         ...
 
-    def phisize(self, sampling: func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample) -> float:
+    def threeCharge(self) -> int:
         "A method"
         ...
 
-    def energyBE(self, layer: int) -> float:
+    def isCharged(self) -> bool:
         "A method"
         ...
 
-    def etaBE(self, layer: int) -> float:
+    def isNeutral(self) -> bool:
         "A method"
         ...
 
-    def phiBE(self, layer: int) -> float:
+    def isPhoton(self) -> bool:
         "A method"
         ...
 
-    def setEnergy(self, sampling: func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample, e: float) -> bool:
+    def isLepton(self) -> bool:
         "A method"
         ...
 
-    def setEta(self, sampling: func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample, eta: float) -> bool:
+    def isChLepton(self) -> bool:
         "A method"
         ...
 
-    def setPhi(self, sampling: func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample, phi: float) -> bool:
+    def isElectron(self) -> bool:
         "A method"
         ...
 
-    def setEmax(self, sampling: func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample, eMax: float) -> bool:
+    def isMuon(self) -> bool:
         "A method"
         ...
 
-    def setEtamax(self, sampling: func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample, etaMax: float) -> bool:
+    def isTau(self) -> bool:
         "A method"
         ...
 
-    def setPhimax(self, sampling: func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample, phiMax: float) -> bool:
+    def isNeutrino(self) -> bool:
         "A method"
         ...
 
-    def setEtasize(self, sampling: func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample, etaSize: float) -> bool:
+    def isHadron(self) -> bool:
         "A method"
         ...
 
-    def setPhisize(self, sampling: func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample, phiSize: float) -> bool:
+    def isMeson(self) -> bool:
         "A method"
         ...
 
-    def retrieveMoment(self, type: func_adl_servicex_xaodr21.xAOD.calocluster_v1.CaloCluster_v1.MomentType, value: float) -> bool:
+    def isBaryon(self) -> bool:
         "A method"
         ...
 
-    def getMomentValue(self, type: func_adl_servicex_xaodr21.xAOD.calocluster_v1.CaloCluster_v1.MomentType) -> float:
+    def hasStrange(self) -> bool:
         "A method"
         ...
 
-    def eta0(self) -> float:
+    def hasCharm(self) -> bool:
         "A method"
         ...
 
-    def phi0(self) -> float:
+    def hasBottom(self) -> bool:
         "A method"
         ...
 
-    def time(self) -> float:
+    def isLightMeson(self) -> bool:
         "A method"
         ...
 
-    def samplingPattern(self) -> int:
+    def isLightBaryon(self) -> bool:
         "A method"
         ...
 
-    def nSamples(self) -> int:
+    def isLightHadron(self) -> bool:
         "A method"
         ...
 
-    def hasSampling(self, s: func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample) -> bool:
+    def isHeavyMeson(self) -> bool:
         "A method"
         ...
 
-    def clusterSize(self) -> func_adl_servicex_xaodr21.xAOD.calocluster_v1.CaloCluster_v1.ClusterSize:
+    def isHeavyBaryon(self) -> bool:
         "A method"
         ...
 
-    def inBarrel(self) -> bool:
+    def isHeavyHadron(self) -> bool:
         "A method"
         ...
 
-    def inEndcap(self) -> bool:
+    def isBottomMeson(self) -> bool:
         "A method"
         ...
 
-    def rawE(self) -> float:
+    def isBottomBaryon(self) -> bool:
         "A method"
         ...
 
-    def rawEta(self) -> float:
+    def isBottomHadron(self) -> bool:
         "A method"
         ...
 
-    def rawPhi(self) -> float:
+    def isCharmMeson(self) -> bool:
         "A method"
         ...
 
-    def rawM(self) -> float:
+    def isCharmBaryon(self) -> bool:
         "A method"
         ...
 
-    def altE(self) -> float:
+    def isCharmHadron(self) -> bool:
         "A method"
         ...
 
-    def altEta(self) -> float:
+    def isStrangeMeson(self) -> bool:
         "A method"
         ...
 
-    def altPhi(self) -> float:
+    def isStrangeBaryon(self) -> bool:
         "A method"
         ...
 
-    def altM(self) -> float:
+    def isStrangeHadron(self) -> bool:
         "A method"
         ...
 
-    def calE(self) -> float:
+    def isQuark(self) -> bool:
         "A method"
         ...
 
-    def calEta(self) -> float:
+    def isParton(self) -> bool:
         "A method"
         ...
 
-    def calPhi(self) -> float:
+    def isTop(self) -> bool:
         "A method"
         ...
 
-    def calM(self) -> float:
+    def isW(self) -> bool:
         "A method"
         ...
 
-    def setSignalState(self, s: func_adl_servicex_xaodr21.xAOD.calocluster_v1.CaloCluster_v1.State) -> bool:
+    def isZ(self) -> bool:
         "A method"
         ...
 
-    def signalState(self) -> func_adl_servicex_xaodr21.xAOD.calocluster_v1.CaloCluster_v1.State:
+    def isHiggs(self) -> bool:
         "A method"
         ...
 
-    def getClusterEtaSize(self) -> int:
+    def isResonance(self) -> bool:
         "A method"
         ...
 
-    def getClusterPhiSize(self) -> int:
+    def isGenSpecific(self) -> bool:
         "A method"
         ...
 
-    def badChannelList(self) -> func_adl_servicex_xaodr21.vector_xaod_caloclusterbadchanneldata_v1_.vector_xAOD_CaloClusterBadChannelData_v1_:
+    def isBSM(self) -> bool:
         "A method"
         ...
 
-    def getSisterCluster(self) -> func_adl_servicex_xaodr21.xAOD.calocluster_v1.CaloCluster_v1:
+    def polarization(self) -> func_adl_servicex_xaodr21.xAOD.TruthParticle_v1.polarization.Polarization:
         "A method"
         ...
 
     def index(self) -> int:
         "A method"
         ...
 
@@ -737,16 +862,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_eventinfo_v1__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_eventinfo_v1__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'isValid': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::EventInfo_v1>>',
         'method_name': 'isValid',
@@ -121,21 +120,14 @@
     'eventTypeBitmask': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::EventInfo_v1>>',
         'method_name': 'eventTypeBitmask',
         'return_type': 'unsigned int',
         'deref_count': 2
     },
-    'eventType': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::EventInfo_v1>>',
-        'method_name': 'eventType',
-        'return_type': 'bool',
-        'deref_count': 2
-    },
     'statusElement': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::EventInfo_v1>>',
         'method_name': 'statusElement',
         'return_type': 'unsigned int',
         'deref_count': 2
     },
@@ -172,56 +164,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::EventInfo_v1>>',
         'method_name': 'subEvents',
         'return_type_element': 'xAOD::EventInfo_v1::SubEvent',
         'return_type_collection': 'const vector<xAOD::EventInfo_v1::SubEvent>',
         'deref_count': 2
     },
-    'eventFlags': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::EventInfo_v1>>',
-        'method_name': 'eventFlags',
-        'return_type': 'unsigned int',
-        'deref_count': 2
-    },
-    'isEventFlagBitSet': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::EventInfo_v1>>',
-        'method_name': 'isEventFlagBitSet',
-        'return_type': 'bool',
-        'deref_count': 2
-    },
-    'setEventFlags': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::EventInfo_v1>>',
-        'method_name': 'setEventFlags',
-        'return_type': 'bool',
-        'deref_count': 2
-    },
-    'setEventFlagBit': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::EventInfo_v1>>',
-        'method_name': 'setEventFlagBit',
-        'return_type': 'bool',
-        'deref_count': 2
-    },
-    'errorState': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::EventInfo_v1>>',
-        'method_name': 'errorState',
-        'return_type': 'xAOD::EventInfo_v1::EventFlagErrorState',
-        'deref_count': 2
-    },
-    'setErrorState': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::EventInfo_v1>>',
-        'method_name': 'setErrorState',
-        'return_type': 'bool',
-        'deref_count': 2
-    },
     'beamPosX': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::EventInfo_v1>>',
         'method_name': 'beamPosX',
         'return_type': 'float',
         'deref_count': 2
     },
@@ -342,38 +292,33 @@
         'type_string': 'ElementLink<DataVector<xAOD::EventInfo_v1>>',
         'method_name': 'isAvailable',
         'return_type': 'bool',
         'deref_count': 2
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class ElementLink_DataVector_xAOD_EventInfo_v1__:
     "A class"
 
-
     def isValid(self) -> bool:
         "A method"
         ...
 
     def runNumber(self) -> int:
         "A method"
         ...
@@ -434,18 +379,14 @@
         "A method"
         ...
 
     def eventTypeBitmask(self) -> int:
         "A method"
         ...
 
-    def eventType(self, type: func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventType) -> bool:
-        "A method"
-        ...
-
     def statusElement(self) -> int:
         "A method"
         ...
 
     def extendedLevel1ID(self) -> int:
         "A method"
         ...
@@ -462,38 +403,14 @@
         "A method"
         ...
 
     def subEvents(self) -> func_adl_servicex_xaodr21.vector_xaod_eventinfo_v1_subevent_.vector_xAOD_EventInfo_v1_SubEvent_:
         "A method"
         ...
 
-    def eventFlags(self, subDet: func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventFlagSubDet) -> int:
-        "A method"
-        ...
-
-    def isEventFlagBitSet(self, subDet: func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventFlagSubDet, bit: int) -> bool:
-        "A method"
-        ...
-
-    def setEventFlags(self, subDet: func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventFlagSubDet, flags: int) -> bool:
-        "A method"
-        ...
-
-    def setEventFlagBit(self, subDet: func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventFlagSubDet, bit: int, set: bool) -> bool:
-        "A method"
-        ...
-
-    def errorState(self, subDet: func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventFlagSubDet) -> func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventFlagErrorState:
-        "A method"
-        ...
-
-    def setErrorState(self, subDet: func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventFlagSubDet, state: func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventFlagErrorState) -> bool:
-        "A method"
-        ...
-
     def beamPosX(self) -> float:
         "A method"
         ...
 
     def beamPosY(self) -> float:
         "A method"
         ...
@@ -552,16 +469,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_iparticle__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_iparticle__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'isValid': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::IParticle>>',
         'method_name': 'isValid',
@@ -115,38 +114,33 @@
         'type_string': 'ElementLink<DataVector<xAOD::IParticle>>',
         'method_name': 'isAvailable',
         'return_type': 'bool',
         'deref_count': 2
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class ElementLink_DataVector_xAOD_IParticle__:
     "A class"
 
-
     def isValid(self) -> bool:
         "A method"
         ...
 
     def pt(self) -> float:
         "A method"
         ...
@@ -197,16 +191,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_jet_v1__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_jet_v1__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'isValid': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::Jet_v1>>',
         'method_name': 'isValid',
@@ -129,28 +128,14 @@
     'getSizeParameter': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::Jet_v1>>',
         'method_name': 'getSizeParameter',
         'return_type': 'float',
         'deref_count': 2
     },
-    'getAlgorithmType': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::Jet_v1>>',
-        'method_name': 'getAlgorithmType',
-        'return_type': 'xAOD::JetAlgorithmType::ID',
-        'deref_count': 2
-    },
-    'getInputType': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::Jet_v1>>',
-        'method_name': 'getInputType',
-        'return_type': 'xAOD::JetInput::Type',
-        'deref_count': 2
-    },
     'index': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::Jet_v1>>',
         'method_name': 'index',
         'return_type': 'int',
         'deref_count': 2
     },
@@ -208,38 +193,33 @@
         'type_string': 'ElementLink<DataVector<xAOD::Jet_v1>>',
         'method_name': 'isAvailable',
         'return_type': 'bool',
         'deref_count': 2
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class ElementLink_DataVector_xAOD_Jet_v1__:
     "A class"
 
-
     def isValid(self) -> bool:
         "A method"
         ...
 
     def pt(self) -> float:
         "A method"
         ...
@@ -304,22 +284,14 @@
         "A method"
         ...
 
     def getSizeParameter(self) -> float:
         "A method"
         ...
 
-    def getAlgorithmType(self) -> func_adl_servicex_xaodr21.xAOD.jetalgorithmtype.JetAlgorithmType.ID:
-        "A method"
-        ...
-
-    def getInputType(self) -> func_adl_servicex_xaodr21.xAOD.jetinput.JetInput.Type:
-        "A method"
-        ...
-
     def index(self) -> int:
         "A method"
         ...
 
     def usingPrivateStore(self) -> bool:
         "A method"
         ...
@@ -338,22 +310,22 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('getAttribute', s, a, param_1))
     @property
-    def getAttribute(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def getAttribute(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_muon_v1__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_muon_v1__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'isValid': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
         'method_name': 'isValid',
@@ -64,63 +63,14 @@
     'charge': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
         'method_name': 'charge',
         'return_type': 'float',
         'deref_count': 2
     },
-    'author': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
-        'method_name': 'author',
-        'return_type': 'xAOD::Muon_v1::Author',
-        'deref_count': 2
-    },
-    'isAuthor': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
-        'method_name': 'isAuthor',
-        'return_type': 'bool',
-        'deref_count': 2
-    },
-    'muonType': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
-        'method_name': 'muonType',
-        'return_type': 'xAOD::Muon_v1::MuonType',
-        'deref_count': 2
-    },
-    'parameter': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
-        'method_name': 'parameter',
-        'return_type': 'bool',
-        'deref_count': 2
-    },
-    'floatParameter': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
-        'method_name': 'floatParameter',
-        'return_type': 'float',
-        'deref_count': 2
-    },
-    'intParameter': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
-        'method_name': 'intParameter',
-        'return_type': 'int',
-        'deref_count': 2
-    },
-    'quality': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
-        'method_name': 'quality',
-        'return_type': 'xAOD::Muon_v1::Quality',
-        'deref_count': 2
-    },
     'passesIDCuts': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
         'method_name': 'passesIDCuts',
         'return_type': 'bool',
         'deref_count': 2
     },
@@ -176,49 +126,28 @@
     'msOnlyExtrapolatedMuonSpectrometerTrackParticleLink': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
         'method_name': 'msOnlyExtrapolatedMuonSpectrometerTrackParticleLink',
         'return_type': 'const ElementLink<DataVector<xAOD::TrackParticle_v1>>',
         'deref_count': 2
     },
-    'trackParticleLink': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
-        'method_name': 'trackParticleLink',
-        'return_type': 'const ElementLink<DataVector<xAOD::TrackParticle_v1>>',
-        'deref_count': 2
-    },
-    'trackParticle': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
-        'method_name': 'trackParticle',
-        'return_type': 'const xAOD::TrackParticle_v1*',
-        'deref_count': 2
-    },
     'clusterLink': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
         'method_name': 'clusterLink',
         'return_type': 'const ElementLink<DataVector<xAOD::CaloCluster_v1>>',
         'deref_count': 2
     },
     'cluster': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
         'method_name': 'cluster',
         'return_type': 'const xAOD::CaloCluster_v1*',
         'deref_count': 2
     },
-    'energyLossType': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
-        'method_name': 'energyLossType',
-        'return_type': 'xAOD::Muon_v1::EnergyLossType',
-        'deref_count': 2
-    },
     'muonSegmentLinks': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
         'method_name': 'muonSegmentLinks',
         'return_type_element': 'ElementLink<DataVector<xAOD::MuonSegment_v1>>',
         'return_type_collection': 'const vector<ElementLink<DataVector<xAOD::MuonSegment_v1>>>',
         'deref_count': 2
@@ -298,38 +227,33 @@
         'type_string': 'ElementLink<DataVector<xAOD::Muon_v1>>',
         'method_name': 'isAvailable',
         'return_type': 'bool',
         'deref_count': 2
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class ElementLink_DataVector_xAOD_Muon_v1__:
     "A class"
 
-
     def isValid(self) -> bool:
         "A method"
         ...
 
     def pt(self) -> float:
         "A method"
         ...
@@ -358,42 +282,14 @@
         "A method"
         ...
 
     def charge(self) -> float:
         "A method"
         ...
 
-    def author(self) -> func_adl_servicex_xaodr21.xAOD.muon_v1.Muon_v1.Author:
-        "A method"
-        ...
-
-    def isAuthor(self, author: func_adl_servicex_xaodr21.xAOD.muon_v1.Muon_v1.Author) -> bool:
-        "A method"
-        ...
-
-    def muonType(self) -> func_adl_servicex_xaodr21.xAOD.muon_v1.Muon_v1.MuonType:
-        "A method"
-        ...
-
-    def parameter(self, value: float, parameter: func_adl_servicex_xaodr21.xAOD.muon_v1.Muon_v1.ParamDef) -> bool:
-        "A method"
-        ...
-
-    def floatParameter(self, parameter: func_adl_servicex_xaodr21.xAOD.muon_v1.Muon_v1.ParamDef) -> float:
-        "A method"
-        ...
-
-    def intParameter(self, parameter: func_adl_servicex_xaodr21.xAOD.muon_v1.Muon_v1.ParamDef) -> int:
-        "A method"
-        ...
-
-    def quality(self) -> func_adl_servicex_xaodr21.xAOD.muon_v1.Muon_v1.Quality:
-        "A method"
-        ...
-
     def passesIDCuts(self) -> bool:
         "A method"
         ...
 
     def passesHighPtCuts(self) -> bool:
         "A method"
         ...
@@ -422,34 +318,22 @@
         "A method"
         ...
 
     def msOnlyExtrapolatedMuonSpectrometerTrackParticleLink(self) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_trackparticle_v1__.ElementLink_DataVector_xAOD_TrackParticle_v1__:
         "A method"
         ...
 
-    def trackParticleLink(self, type: func_adl_servicex_xaodr21.xAOD.muon_v1.Muon_v1.TrackParticleType) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_trackparticle_v1__.ElementLink_DataVector_xAOD_TrackParticle_v1__:
-        "A method"
-        ...
-
-    def trackParticle(self, type: func_adl_servicex_xaodr21.xAOD.muon_v1.Muon_v1.TrackParticleType) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
-        "A method"
-        ...
-
     def clusterLink(self) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_calocluster_v1__.ElementLink_DataVector_xAOD_CaloCluster_v1__:
         "A method"
         ...
 
     def cluster(self) -> func_adl_servicex_xaodr21.xAOD.calocluster_v1.CaloCluster_v1:
         "A method"
         ...
 
-    def energyLossType(self) -> func_adl_servicex_xaodr21.xAOD.muon_v1.Muon_v1.EnergyLossType:
-        "A method"
-        ...
-
     def muonSegmentLinks(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_muonsegment_v1___.vector_ElementLink_DataVector_xAOD_MuonSegment_v1___:
         "A method"
         ...
 
     def nMuonSegments(self) -> int:
         "A method"
         ...
@@ -484,16 +368,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_muonsegment_v1__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_muonsegment_v1__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'isValid': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::MuonSegment_v1>>',
         'method_name': 'isValid',
@@ -85,35 +84,21 @@
     'sector': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::MuonSegment_v1>>',
         'method_name': 'sector',
         'return_type': 'int',
         'deref_count': 2
     },
-    'chamberIndex': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::MuonSegment_v1>>',
-        'method_name': 'chamberIndex',
-        'return_type': 'Muon::MuonStationIndex::ChIndex',
-        'deref_count': 2
-    },
     'etaIndex': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::MuonSegment_v1>>',
         'method_name': 'etaIndex',
         'return_type': 'int',
         'deref_count': 2
     },
-    'technology': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::MuonSegment_v1>>',
-        'method_name': 'technology',
-        'return_type': 'Muon::MuonStationIndex::TechnologyIndex',
-        'deref_count': 2
-    },
     'nPrecisionHits': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::MuonSegment_v1>>',
         'method_name': 'nPrecisionHits',
         'return_type': 'int',
         'deref_count': 2
     },
@@ -185,38 +170,33 @@
         'type_string': 'ElementLink<DataVector<xAOD::MuonSegment_v1>>',
         'method_name': 'isAvailable',
         'return_type': 'bool',
         'deref_count': 2
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class ElementLink_DataVector_xAOD_MuonSegment_v1__:
     "A class"
 
-
     def isValid(self) -> bool:
         "A method"
         ...
 
     def x(self) -> float:
         "A method"
         ...
@@ -257,26 +237,18 @@
         "A method"
         ...
 
     def sector(self) -> int:
         "A method"
         ...
 
-    def chamberIndex(self) -> func_adl_servicex_xaodr21.Muon.muonstationindex.MuonStationIndex.ChIndex:
-        "A method"
-        ...
-
     def etaIndex(self) -> int:
         "A method"
         ...
 
-    def technology(self) -> func_adl_servicex_xaodr21.Muon.muonstationindex.MuonStationIndex.TechnologyIndex:
-        "A method"
-        ...
-
     def nPrecisionHits(self) -> int:
         "A method"
         ...
 
     def nPhiLayers(self) -> int:
         "A method"
         ...
@@ -307,16 +279,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_neutralparticle_v1__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_neutralparticle_v1__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'isValid': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::NeutralParticle_v1>>',
         'method_name': 'isValid',
@@ -179,38 +178,33 @@
         'type_string': 'ElementLink<DataVector<xAOD::NeutralParticle_v1>>',
         'method_name': 'isAvailable',
         'return_type': 'bool',
         'deref_count': 2
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class ElementLink_DataVector_xAOD_NeutralParticle_v1__:
     "A class"
 
-
     def isValid(self) -> bool:
         "A method"
         ...
 
     def pt(self) -> float:
         "A method"
         ...
@@ -297,16 +291,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_pfo_v1__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/btagging_v1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,401 +1,459 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
-    'isValid': {
+    'SV0_significance3D': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'isValid',
-        'return_type': 'bool',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'SV0_significance3D',
+        'return_type': 'double',
     },
-    'pt': {
+    'SV0_TrackParticleLinks': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'pt',
-        'return_type': 'double',
-        'deref_count': 2
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'SV0_TrackParticleLinks',
+        'return_type_element': 'ElementLink<DataVector<xAOD::TrackParticle_v1>>',
+        'return_type_collection': 'const vector<ElementLink<DataVector<xAOD::TrackParticle_v1>>>',
+    },
+    'SV0_TrackParticle': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'SV0_TrackParticle',
+        'return_type': 'const xAOD::TrackParticle_v1*',
+    },
+    'nSV0_TrackParticles': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'nSV0_TrackParticles',
+        'return_type': 'int',
     },
-    'eta': {
+    'SV1_pb': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'eta',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'SV1_pb',
         'return_type': 'double',
-        'deref_count': 2
     },
-    'phi': {
+    'SV1_pc': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'phi',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'SV1_pc',
         'return_type': 'double',
-        'deref_count': 2
     },
-    'm': {
+    'SV1_pu': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'm',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'SV1_pu',
         'return_type': 'double',
-        'deref_count': 2
     },
-    'e': {
+    'SV1_loglikelihoodratio': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'e',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'SV1_loglikelihoodratio',
         'return_type': 'double',
-        'deref_count': 2
     },
-    'rapidity': {
+    'SV1_TrackParticleLinks': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'rapidity',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'SV1_TrackParticleLinks',
+        'return_type_element': 'ElementLink<DataVector<xAOD::TrackParticle_v1>>',
+        'return_type_collection': 'const vector<ElementLink<DataVector<xAOD::TrackParticle_v1>>>',
+    },
+    'SV1_TrackParticle': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'SV1_TrackParticle',
+        'return_type': 'const xAOD::TrackParticle_v1*',
+    },
+    'nSV1_TrackParticles': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'nSV1_TrackParticles',
+        'return_type': 'int',
+    },
+    'IP2D_pb': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'IP2D_pb',
         'return_type': 'double',
-        'deref_count': 2
     },
-    'p4': {
+    'IP2D_pc': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'p4',
-        'return_type': 'const TLorentzVector',
-        'deref_count': 2
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'IP2D_pc',
+        'return_type': 'double',
     },
-    'p4EM': {
+    'IP2D_pu': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'p4EM',
-        'return_type': 'const TLorentzVector',
-        'deref_count': 2
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'IP2D_pu',
+        'return_type': 'double',
     },
-    'ptEM': {
+    'IP2D_loglikelihoodratio': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'ptEM',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'IP2D_loglikelihoodratio',
         'return_type': 'double',
-        'deref_count': 2
     },
-    'etaEM': {
+    'IP2D_TrackParticleLinks': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'IP2D_TrackParticleLinks',
+        'return_type_element': 'ElementLink<DataVector<xAOD::TrackParticle_v1>>',
+        'return_type_collection': 'const vector<ElementLink<DataVector<xAOD::TrackParticle_v1>>>',
+    },
+    'IP2D_TrackParticle': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'IP2D_TrackParticle',
+        'return_type': 'const xAOD::TrackParticle_v1*',
+    },
+    'nIP2D_TrackParticles': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'nIP2D_TrackParticles',
+        'return_type': 'int',
+    },
+    'IP3D_pb': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'etaEM',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'IP3D_pb',
         'return_type': 'double',
-        'deref_count': 2
     },
-    'phiEM': {
+    'IP3D_pc': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'phiEM',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'IP3D_pc',
         'return_type': 'double',
-        'deref_count': 2
     },
-    'mEM': {
+    'IP3D_pu': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'mEM',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'IP3D_pu',
         'return_type': 'double',
-        'deref_count': 2
     },
-    'eEM': {
+    'IP3D_loglikelihoodratio': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'eEM',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'IP3D_loglikelihoodratio',
         'return_type': 'double',
-        'deref_count': 2
     },
-    'bdtPi0Score': {
+    'IP3D_TrackParticleLinks': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'bdtPi0Score',
-        'return_type': 'float',
-        'deref_count': 2
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'IP3D_TrackParticleLinks',
+        'return_type_element': 'ElementLink<DataVector<xAOD::TrackParticle_v1>>',
+        'return_type_collection': 'const vector<ElementLink<DataVector<xAOD::TrackParticle_v1>>>',
     },
-    'centerMag': {
+    'IP3D_TrackParticle': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'centerMag',
-        'return_type': 'float',
-        'deref_count': 2
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'IP3D_TrackParticle',
+        'return_type': 'const xAOD::TrackParticle_v1*',
     },
-    'isCharged': {
+    'nIP3D_TrackParticles': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'isCharged',
-        'return_type': 'bool',
-        'deref_count': 2
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'nIP3D_TrackParticles',
+        'return_type': 'int',
     },
-    'charge': {
+    'SV1plusIP3D_discriminant': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'charge',
-        'return_type': 'float',
-        'deref_count': 2
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'SV1plusIP3D_discriminant',
+        'return_type': 'double',
     },
-    'getClusterMoment': {
+    'JetFitter_pb': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'getClusterMoment',
-        'return_type': 'bool',
-        'deref_count': 2
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'JetFitter_pb',
+        'return_type': 'double',
     },
-    'cluster': {
+    'JetFitter_pc': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'cluster',
-        'return_type': 'const xAOD::CaloCluster_v1*',
-        'deref_count': 2
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'JetFitter_pc',
+        'return_type': 'double',
     },
-    'track': {
+    'JetFitter_pu': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'track',
-        'return_type': 'const xAOD::TrackParticle_v1*',
-        'deref_count': 2
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'JetFitter_pu',
+        'return_type': 'double',
     },
-    'vertex': {
+    'JetFitter_loglikelihoodratio': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'vertex',
-        'return_type': 'const xAOD::Vertex_v1*',
-        'deref_count': 2
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'JetFitter_loglikelihoodratio',
+        'return_type': 'double',
+    },
+    'MV1_discriminant': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'MV1_discriminant',
+        'return_type': 'double',
     },
-    'setVertexLink': {
+    'loglikelihoodratio': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'setVertexLink',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'loglikelihoodratio',
         'return_type': 'bool',
-        'deref_count': 2
     },
-    'setTrackLink': {
+    'MVx_discriminant': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'setTrackLink',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'MVx_discriminant',
         'return_type': 'bool',
-        'deref_count': 2
     },
-    'setClusterLink': {
+    'pu': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'setClusterLink',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'pu',
         'return_type': 'bool',
-        'deref_count': 2
     },
-    'addClusterLink': {
+    'pb': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'addClusterLink',
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'pb',
         'return_type': 'bool',
-        'deref_count': 2
     },
-    'GetVertexCorrectedFourVec': {
+    'pc': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'GetVertexCorrectedFourVec',
-        'return_type': 'TLorentzVector',
-        'deref_count': 2
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'pc',
+        'return_type': 'bool',
     },
-    'GetVertexCorrectedEMFourVec': {
+    'calcLLR': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
-        'method_name': 'GetVertexCorrectedEMFourVec',
-        'return_type': 'TLorentzVector',
-        'deref_count': 2
+        'type_string': 'xAOD::BTagging_v1',
+        'method_name': 'calcLLR',
+        'return_type': 'double',
     },
     'index': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
+        'type_string': 'xAOD::BTagging_v1',
         'method_name': 'index',
         'return_type': 'int',
-        'deref_count': 2
     },
     'usingPrivateStore': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
+        'type_string': 'xAOD::BTagging_v1',
         'method_name': 'usingPrivateStore',
         'return_type': 'bool',
-        'deref_count': 2
     },
     'usingStandaloneStore': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
+        'type_string': 'xAOD::BTagging_v1',
         'method_name': 'usingStandaloneStore',
         'return_type': 'bool',
-        'deref_count': 2
     },
     'hasStore': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
+        'type_string': 'xAOD::BTagging_v1',
         'method_name': 'hasStore',
         'return_type': 'bool',
-        'deref_count': 2
     },
     'hasNonConstStore': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
+        'type_string': 'xAOD::BTagging_v1',
         'method_name': 'hasNonConstStore',
         'return_type': 'bool',
-        'deref_count': 2
     },
     'clearDecorations': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
+        'type_string': 'xAOD::BTagging_v1',
         'method_name': 'clearDecorations',
         'return_type': 'bool',
-        'deref_count': 2
     },
     'auxdataConst': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
+        'type_string': 'xAOD::BTagging_v1',
         'method_name': 'auxdataConst',
         'return_type': 'U',
-        'deref_count': 2
     },
     'isAvailable': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'ElementLink<DataVector<xAOD::PFO_v1>>',
+        'type_string': 'xAOD::BTagging_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
-        'deref_count': 2
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
+        s_update = s_update.MetaData({
+            'metadata_type': 'inject_code',
+            'name': 'xAODBTagging/versions/BTagging_v1.h',
+            'body_includes': ["xAODBTagging/versions/BTagging_v1.h"],
+        })
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class ElementLink_DataVector_xAOD_PFO_v1__:
+class BTagging_v1:
     "A class"
 
+    def SV0_significance3D(self) -> float:
+        "A method"
+        ...
+
+    def SV0_TrackParticleLinks(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_trackparticle_v1___.vector_ElementLink_DataVector_xAOD_TrackParticle_v1___:
+        "A method"
+        ...
+
+    def SV0_TrackParticle(self, i: int) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
+        "A method"
+        ...
+
+    def nSV0_TrackParticles(self) -> int:
+        "A method"
+        ...
+
+    def SV1_pb(self) -> float:
+        "A method"
+        ...
+
+    def SV1_pc(self) -> float:
+        "A method"
+        ...
+
+    def SV1_pu(self) -> float:
+        "A method"
+        ...
+
+    def SV1_loglikelihoodratio(self) -> float:
+        "A method"
+        ...
+
+    def SV1_TrackParticleLinks(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_trackparticle_v1___.vector_ElementLink_DataVector_xAOD_TrackParticle_v1___:
+        "A method"
+        ...
 
-    def isValid(self) -> bool:
+    def SV1_TrackParticle(self, i: int) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
         "A method"
         ...
 
-    def pt(self) -> float:
+    def nSV1_TrackParticles(self) -> int:
         "A method"
         ...
 
-    def eta(self) -> float:
+    def IP2D_pb(self) -> float:
         "A method"
         ...
 
-    def phi(self) -> float:
+    def IP2D_pc(self) -> float:
         "A method"
         ...
 
-    def m(self) -> float:
+    def IP2D_pu(self) -> float:
         "A method"
         ...
 
-    def e(self) -> float:
+    def IP2D_loglikelihoodratio(self) -> float:
         "A method"
         ...
 
-    def rapidity(self) -> float:
+    def IP2D_TrackParticleLinks(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_trackparticle_v1___.vector_ElementLink_DataVector_xAOD_TrackParticle_v1___:
         "A method"
         ...
 
-    def p4(self) -> func_adl_servicex_xaodr21.tlorentzvector.TLorentzVector:
+    def IP2D_TrackParticle(self, i: int) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
         "A method"
         ...
 
-    def p4EM(self) -> func_adl_servicex_xaodr21.tlorentzvector.TLorentzVector:
+    def nIP2D_TrackParticles(self) -> int:
         "A method"
         ...
 
-    def ptEM(self) -> float:
+    def IP3D_pb(self) -> float:
         "A method"
         ...
 
-    def etaEM(self) -> float:
+    def IP3D_pc(self) -> float:
         "A method"
         ...
 
-    def phiEM(self) -> float:
+    def IP3D_pu(self) -> float:
         "A method"
         ...
 
-    def mEM(self) -> float:
+    def IP3D_loglikelihoodratio(self) -> float:
         "A method"
         ...
 
-    def eEM(self) -> float:
+    def IP3D_TrackParticleLinks(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_trackparticle_v1___.vector_ElementLink_DataVector_xAOD_TrackParticle_v1___:
         "A method"
         ...
 
-    def bdtPi0Score(self) -> float:
+    def IP3D_TrackParticle(self, i: int) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
         "A method"
         ...
 
-    def centerMag(self) -> float:
+    def nIP3D_TrackParticles(self) -> int:
         "A method"
         ...
 
-    def isCharged(self) -> bool:
+    def SV1plusIP3D_discriminant(self) -> float:
         "A method"
         ...
 
-    def charge(self) -> float:
+    def JetFitter_pb(self) -> float:
         "A method"
         ...
 
-    def getClusterMoment(self, theMoment: float, momentType: func_adl_servicex_xaodr21.xAOD.calocluster_v1.CaloCluster_v1.MomentType) -> bool:
+    def JetFitter_pc(self) -> float:
         "A method"
         ...
 
-    def cluster(self, index: int) -> func_adl_servicex_xaodr21.xAOD.calocluster_v1.CaloCluster_v1:
+    def JetFitter_pu(self) -> float:
         "A method"
         ...
 
-    def track(self, index: int) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
+    def JetFitter_loglikelihoodratio(self) -> float:
         "A method"
         ...
 
-    def vertex(self) -> func_adl_servicex_xaodr21.xAOD.vertex_v1.Vertex_v1:
+    def MV1_discriminant(self) -> float:
         "A method"
         ...
 
-    def setVertexLink(self, theVertexLink: func_adl_servicex_xaodr21.elementlink_datavector_xaod_vertex_v1__.ElementLink_DataVector_xAOD_Vertex_v1__) -> bool:
+    def loglikelihoodratio(self, taggername: str, value: float, signal: str, bckgd: str) -> bool:
         "A method"
         ...
 
-    def setTrackLink(self, theTrack: func_adl_servicex_xaodr21.elementlink_datavector_xaod_trackparticle_v1__.ElementLink_DataVector_xAOD_TrackParticle_v1__) -> bool:
+    def MVx_discriminant(self, taggername: str, value: float) -> bool:
         "A method"
         ...
 
-    def setClusterLink(self, theCluster: func_adl_servicex_xaodr21.elementlink_datavector_xaod_calocluster_v1__.ElementLink_DataVector_xAOD_CaloCluster_v1__) -> bool:
+    def pu(self, taggername: str, value: float) -> bool:
         "A method"
         ...
 
-    def addClusterLink(self, theCluster: func_adl_servicex_xaodr21.elementlink_datavector_xaod_calocluster_v1__.ElementLink_DataVector_xAOD_CaloCluster_v1__) -> bool:
+    def pb(self, taggername: str, value: float) -> bool:
         "A method"
         ...
 
-    def GetVertexCorrectedFourVec(self, vertexToCorrectTo: func_adl_servicex_xaodr21.xAOD.vertex_v1.Vertex_v1) -> func_adl_servicex_xaodr21.tlorentzvector.TLorentzVector:
+    def pc(self, taggername: str, value: float) -> bool:
         "A method"
         ...
 
-    def GetVertexCorrectedEMFourVec(self, vertexToCorrectTo: func_adl_servicex_xaodr21.xAOD.vertex_v1.Vertex_v1) -> func_adl_servicex_xaodr21.tlorentzvector.TLorentzVector:
+    def calcLLR(self, num: float, den: float) -> float:
         "A method"
         ...
 
     def index(self) -> int:
         "A method"
         ...
 
@@ -417,16 +475,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_tautrack_v1__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_tautrack_v1__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'isValid': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::TauTrack_v1>>',
         'method_name': 'isValid',
@@ -187,38 +186,33 @@
         'type_string': 'ElementLink<DataVector<xAOD::TauTrack_v1>>',
         'method_name': 'isAvailable',
         'return_type': 'bool',
         'deref_count': 2
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class ElementLink_DataVector_xAOD_TauTrack_v1__:
     "A class"
 
-
     def isValid(self) -> bool:
         "A method"
         ...
 
     def pt(self) -> float:
         "A method"
         ...
@@ -247,27 +241,27 @@
         "A method"
         ...
 
     def flagWithMask(self, noname_arg: int) -> bool:
         "A method"
         ...
 
-    def z0sinThetaTJVA(self, noname_arg: func_adl_servicex_xaodr21.xAOD.iparticle.IParticle) -> float:
+    def z0sinThetaTJVA(self, noname_arg: IParticle) -> float:
         "A method"
         ...
 
-    def rConv(self, noname_arg: func_adl_servicex_xaodr21.xAOD.iparticle.IParticle) -> float:
+    def rConv(self, noname_arg: IParticle) -> float:
         "A method"
         ...
 
-    def rConvII(self, noname_arg: func_adl_servicex_xaodr21.xAOD.iparticle.IParticle) -> float:
+    def rConvII(self, noname_arg: IParticle) -> float:
         "A method"
         ...
 
-    def dRJetSeedAxis(self, noname_arg: func_adl_servicex_xaodr21.xAOD.iparticle.IParticle) -> float:
+    def dRJetSeedAxis(self, noname_arg: IParticle) -> float:
         "A method"
         ...
 
     def bdtScores(self) -> func_adl_servicex_xaodr21.vector_float_.vector_float_:
         "A method"
         ...
 
@@ -309,16 +303,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_trackparticle_v1__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_trackparticle_v1__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'isValid': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::TrackParticle_v1>>',
         'method_name': 'isValid',
@@ -291,38 +290,33 @@
         'type_string': 'ElementLink<DataVector<xAOD::TrackParticle_v1>>',
         'method_name': 'isAvailable',
         'return_type': 'bool',
         'deref_count': 2
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class ElementLink_DataVector_xAOD_TrackParticle_v1__:
     "A class"
 
-
     def isValid(self) -> bool:
         "A method"
         ...
 
     def pt(self) -> float:
         "A method"
         ...
@@ -473,16 +467,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_truthvertex_v1__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_truthvertex_v1__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'isValid': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::TruthVertex_v1>>',
         'method_name': 'isValid',
@@ -180,38 +179,33 @@
         'type_string': 'ElementLink<DataVector<xAOD::TruthVertex_v1>>',
         'method_name': 'isAvailable',
         'return_type': 'bool',
         'deref_count': 2
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class ElementLink_DataVector_xAOD_TruthVertex_v1__:
     "A class"
 
-
     def isValid(self) -> bool:
         "A method"
         ...
 
     def id(self) -> int:
         "A method"
         ...
@@ -298,16 +292,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/elementlink_datavector_xaod_vertex_v1__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/elementlink_datavector_xaod_vertex_v1__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'isValid': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'ElementLink<DataVector<xAOD::Vertex_v1>>',
         'method_name': 'isValid',
@@ -183,38 +182,33 @@
         'type_string': 'ElementLink<DataVector<xAOD::Vertex_v1>>',
         'method_name': 'isAvailable',
         'return_type': 'bool',
         'deref_count': 2
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class ElementLink_DataVector_xAOD_Vertex_v1__:
     "A class"
 
-
     def isValid(self) -> bool:
         "A method"
         ...
 
     def x(self) -> float:
         "A method"
         ...
@@ -301,16 +295,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/event_collection.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/event_collection.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,58 +3,40 @@
 from func_adl import ObjectStream, func_adl_callback
 import ast
 import copy
 import func_adl_servicex_xaodr21
 
 # The map for collection definitions in ATLAS
 _collection_map = {
-    'CaloTowers': {
-        'metadata_type': 'add_atlas_event_collection_info',
-        'name': 'CaloTowers',
-        'include_files': ['xAODCaloEvent/CaloTowerContainer.h',],
-        'container_type': 'xAOD::CaloTowerContainer_v1',
-        'element_type': 'xAOD::CaloTower_v1',
-        'contains_collection': True,
-        'link_libraries': ['xAODCaloEvent'],
-    },
-    'CaloClusters': {
+    'BTaggings': {
         'metadata_type': 'add_atlas_event_collection_info',
-        'name': 'CaloClusters',
-        'include_files': ['xAODCaloEvent/CaloClusterContainer.h',],
-        'container_type': 'DataVector<xAOD::CaloCluster_v1>',
-        'element_type': 'xAOD::CaloCluster_v1',
+        'name': 'BTaggings',
+        'include_files': ['xAODBTagging/BTaggingContainer.h',],
+        'container_type': 'DataVector<xAOD::BTagging_v1>',
+        'element_type': 'xAOD::BTagging_v1',
         'contains_collection': True,
-        'link_libraries': ['xAODCaloEvent'],
+        'link_libraries': ['xAODBTagging'],
     },
     'BTagVertices': {
         'metadata_type': 'add_atlas_event_collection_info',
         'name': 'BTagVertices',
         'include_files': ['xAODBTagging/BTagVertexContainer.h',],
         'container_type': 'DataVector<xAOD::BTagVertex_v1>',
         'element_type': 'xAOD::BTagVertex_v1',
         'contains_collection': True,
         'link_libraries': ['xAODBTagging'],
     },
-    'BTaggings': {
-        'metadata_type': 'add_atlas_event_collection_info',
-        'name': 'BTaggings',
-        'include_files': ['xAODBTagging/BTaggingContainer.h',],
-        'container_type': 'DataVector<xAOD::BTagging_v1>',
-        'element_type': 'xAOD::BTagging_v1',
-        'contains_collection': True,
-        'link_libraries': ['xAODBTagging'],
-    },
-    'Photons': {
+    'Jets': {
         'metadata_type': 'add_atlas_event_collection_info',
-        'name': 'Photons',
-        'include_files': ['xAODEgamma/PhotonContainer.h',],
-        'container_type': 'DataVector<xAOD::Photon_v1>',
-        'element_type': 'xAOD::Photon_v1',
+        'name': 'Jets',
+        'include_files': ['xAODJet/JetContainer.h',],
+        'container_type': 'DataVector<xAOD::Jet_v1>',
+        'element_type': 'xAOD::Jet_v1',
         'contains_collection': True,
-        'link_libraries': ['xAODEgamma'],
+        'link_libraries': ['xAODJet'],
     },
     'Egammas': {
         'metadata_type': 'add_atlas_event_collection_info',
         'name': 'Egammas',
         'include_files': ['xAODEgamma/EgammaContainer.h',],
         'container_type': 'DataVector<xAOD::Egamma_v1>',
         'element_type': 'xAOD::Egamma_v1',
@@ -66,14 +48,59 @@
         'name': 'Electrons',
         'include_files': ['xAODEgamma/ElectronContainer.h',],
         'container_type': 'DataVector<xAOD::Electron_v1>',
         'element_type': 'xAOD::Electron_v1',
         'contains_collection': True,
         'link_libraries': ['xAODEgamma'],
     },
+    'Photons': {
+        'metadata_type': 'add_atlas_event_collection_info',
+        'name': 'Photons',
+        'include_files': ['xAODEgamma/PhotonContainer.h',],
+        'container_type': 'DataVector<xAOD::Photon_v1>',
+        'element_type': 'xAOD::Photon_v1',
+        'contains_collection': True,
+        'link_libraries': ['xAODEgamma'],
+    },
+    'TauJets': {
+        'metadata_type': 'add_atlas_event_collection_info',
+        'name': 'TauJets',
+        'include_files': ['xAODTau/TauJetContainer.h',],
+        'container_type': 'DataVector<xAOD::TauJet_v3>',
+        'element_type': 'xAOD::TauJet_v3',
+        'contains_collection': True,
+        'link_libraries': ['xAODTau'],
+    },
+    'DiTauJets': {
+        'metadata_type': 'add_atlas_event_collection_info',
+        'name': 'DiTauJets',
+        'include_files': ['xAODTau/DiTauJetContainer.h',],
+        'container_type': 'DataVector<xAOD::DiTauJet_v1>',
+        'element_type': 'xAOD::DiTauJet_v1',
+        'contains_collection': True,
+        'link_libraries': ['xAODTau'],
+    },
+    'TauTracks': {
+        'metadata_type': 'add_atlas_event_collection_info',
+        'name': 'TauTracks',
+        'include_files': ['xAODTau/TauTrackContainer.h',],
+        'container_type': 'DataVector<xAOD::TauTrack_v1>',
+        'element_type': 'xAOD::TauTrack_v1',
+        'contains_collection': True,
+        'link_libraries': ['xAODTau'],
+    },
+    'TruthVertices': {
+        'metadata_type': 'add_atlas_event_collection_info',
+        'name': 'TruthVertices',
+        'include_files': ['xAODTruth/TruthVertexContainer.h',],
+        'container_type': 'DataVector<xAOD::TruthVertex_v1>',
+        'element_type': 'xAOD::TruthVertex_v1',
+        'contains_collection': True,
+        'link_libraries': ['xAODTruth'],
+    },
     'TruthEvents': {
         'metadata_type': 'add_atlas_event_collection_info',
         'name': 'TruthEvents',
         'include_files': ['xAODTruth/TruthEventContainer.h',],
         'container_type': 'DataVector<xAOD::TruthEvent_v1>',
         'element_type': 'xAOD::TruthEvent_v1',
         'contains_collection': True,
@@ -93,23 +120,14 @@
         'name': 'TruthMetaDatas',
         'include_files': ['xAODTruth/TruthMetaDataContainer.h',],
         'container_type': 'DataVector<xAOD::TruthMetaData_v1>',
         'element_type': 'xAOD::TruthMetaData_v1',
         'contains_collection': True,
         'link_libraries': ['xAODTruth'],
     },
-    'TruthVertices': {
-        'metadata_type': 'add_atlas_event_collection_info',
-        'name': 'TruthVertices',
-        'include_files': ['xAODTruth/TruthVertexContainer.h',],
-        'container_type': 'DataVector<xAOD::TruthVertex_v1>',
-        'element_type': 'xAOD::TruthVertex_v1',
-        'contains_collection': True,
-        'link_libraries': ['xAODTruth'],
-    },
     'MissingET': {
         'metadata_type': 'add_atlas_event_collection_info',
         'name': 'MissingET',
         'include_files': ['xAODMissingET/MissingETContainer.h',],
         'container_type': 'xAOD::MissingETContainer_v1',
         'element_type': 'xAOD::MissingET_v1',
         'contains_collection': True,
@@ -120,50 +138,14 @@
         'name': 'EventInfos',
         'include_files': ['xAODEventInfo/EventInfoContainer.h',],
         'container_type': 'DataVector<xAOD::EventInfo_v1>',
         'element_type': 'xAOD::EventInfo_v1',
         'contains_collection': True,
         'link_libraries': ['xAODEventInfo'],
     },
-    'TauJets': {
-        'metadata_type': 'add_atlas_event_collection_info',
-        'name': 'TauJets',
-        'include_files': ['xAODTau/TauJetContainer.h',],
-        'container_type': 'DataVector<xAOD::TauJet_v3>',
-        'element_type': 'xAOD::TauJet_v3',
-        'contains_collection': True,
-        'link_libraries': ['xAODTau'],
-    },
-    'DiTauJets': {
-        'metadata_type': 'add_atlas_event_collection_info',
-        'name': 'DiTauJets',
-        'include_files': ['xAODTau/DiTauJetContainer.h',],
-        'container_type': 'DataVector<xAOD::DiTauJet_v1>',
-        'element_type': 'xAOD::DiTauJet_v1',
-        'contains_collection': True,
-        'link_libraries': ['xAODTau'],
-    },
-    'TauTracks': {
-        'metadata_type': 'add_atlas_event_collection_info',
-        'name': 'TauTracks',
-        'include_files': ['xAODTau/TauTrackContainer.h',],
-        'container_type': 'DataVector<xAOD::TauTrack_v1>',
-        'element_type': 'xAOD::TauTrack_v1',
-        'contains_collection': True,
-        'link_libraries': ['xAODTau'],
-    },
-    'Muons': {
-        'metadata_type': 'add_atlas_event_collection_info',
-        'name': 'Muons',
-        'include_files': ['xAODMuon/MuonContainer.h',],
-        'container_type': 'DataVector<xAOD::Muon_v1>',
-        'element_type': 'xAOD::Muon_v1',
-        'contains_collection': True,
-        'link_libraries': ['xAODMuon'],
-    },
     'MuonSegments': {
         'metadata_type': 'add_atlas_event_collection_info',
         'name': 'MuonSegments',
         'include_files': ['xAODMuon/MuonSegmentContainer.h',],
         'container_type': 'DataVector<xAOD::MuonSegment_v1>',
         'element_type': 'xAOD::MuonSegment_v1',
         'contains_collection': True,
@@ -174,49 +156,40 @@
         'name': 'SlowMuons',
         'include_files': ['xAODMuon/SlowMuonContainer.h',],
         'container_type': 'DataVector<xAOD::SlowMuon_v1>',
         'element_type': 'xAOD::SlowMuon_v1',
         'contains_collection': True,
         'link_libraries': ['xAODMuon'],
     },
+    'Muons': {
+        'metadata_type': 'add_atlas_event_collection_info',
+        'name': 'Muons',
+        'include_files': ['xAODMuon/MuonContainer.h',],
+        'container_type': 'DataVector<xAOD::Muon_v1>',
+        'element_type': 'xAOD::Muon_v1',
+        'contains_collection': True,
+        'link_libraries': ['xAODMuon'],
+    },
     'IParticles': {
         'metadata_type': 'add_atlas_event_collection_info',
         'name': 'IParticles',
         'include_files': ['xAODBase/IParticleContainer.h',],
         'container_type': 'DataVector<xAOD::IParticle>',
         'element_type': 'xAOD::IParticle',
         'contains_collection': True,
         'link_libraries': ['xAODBase'],
     },
-    'TrackCaloClusters': {
-        'metadata_type': 'add_atlas_event_collection_info',
-        'name': 'TrackCaloClusters',
-        'include_files': ['xAODPFlow/TrackCaloClusterContainer.h',],
-        'container_type': 'DataVector<xAOD::TrackCaloCluster_v1>',
-        'element_type': 'xAOD::TrackCaloCluster_v1',
-        'contains_collection': True,
-        'link_libraries': ['xAODPFlow'],
-    },
-    'PFOs': {
-        'metadata_type': 'add_atlas_event_collection_info',
-        'name': 'PFOs',
-        'include_files': ['xAODPFlow/PFOContainer.h',],
-        'container_type': 'DataVector<xAOD::PFO_v1>',
-        'element_type': 'xAOD::PFO_v1',
-        'contains_collection': True,
-        'link_libraries': ['xAODPFlow'],
-    },
-    'Jets': {
+    'Vertices': {
         'metadata_type': 'add_atlas_event_collection_info',
-        'name': 'Jets',
-        'include_files': ['xAODJet/JetContainer.h',],
-        'container_type': 'DataVector<xAOD::Jet_v1>',
-        'element_type': 'xAOD::Jet_v1',
+        'name': 'Vertices',
+        'include_files': ['xAODTracking/VertexContainer.h',],
+        'container_type': 'DataVector<xAOD::Vertex_v1>',
+        'element_type': 'xAOD::Vertex_v1',
         'contains_collection': True,
-        'link_libraries': ['xAODJet'],
+        'link_libraries': ['xAODTracking'],
     },
     'NeutralParticles': {
         'metadata_type': 'add_atlas_event_collection_info',
         'name': 'NeutralParticles',
         'include_files': ['xAODTracking/NeutralParticleContainer.h',],
         'container_type': 'DataVector<xAOD::NeutralParticle_v1>',
         'element_type': 'xAOD::NeutralParticle_v1',
@@ -228,22 +201,49 @@
         'name': 'TrackParticles',
         'include_files': ['xAODTracking/TrackParticleContainer.h',],
         'container_type': 'DataVector<xAOD::TrackParticle_v1>',
         'element_type': 'xAOD::TrackParticle_v1',
         'contains_collection': True,
         'link_libraries': ['xAODTracking'],
     },
-    'Vertices': {
+    'PFOs': {
         'metadata_type': 'add_atlas_event_collection_info',
-        'name': 'Vertices',
-        'include_files': ['xAODTracking/VertexContainer.h',],
-        'container_type': 'DataVector<xAOD::Vertex_v1>',
-        'element_type': 'xAOD::Vertex_v1',
+        'name': 'PFOs',
+        'include_files': ['xAODPFlow/PFOContainer.h',],
+        'container_type': 'DataVector<xAOD::PFO_v1>',
+        'element_type': 'xAOD::PFO_v1',
         'contains_collection': True,
-        'link_libraries': ['xAODTracking'],
+        'link_libraries': ['xAODPFlow'],
+    },
+    'TrackCaloClusters': {
+        'metadata_type': 'add_atlas_event_collection_info',
+        'name': 'TrackCaloClusters',
+        'include_files': ['xAODPFlow/TrackCaloClusterContainer.h',],
+        'container_type': 'DataVector<xAOD::TrackCaloCluster_v1>',
+        'element_type': 'xAOD::TrackCaloCluster_v1',
+        'contains_collection': True,
+        'link_libraries': ['xAODPFlow'],
+    },
+    'CaloTowers': {
+        'metadata_type': 'add_atlas_event_collection_info',
+        'name': 'CaloTowers',
+        'include_files': ['xAODCaloEvent/CaloTowerContainer.h',],
+        'container_type': 'xAOD::CaloTowerContainer_v1',
+        'element_type': 'xAOD::CaloTower_v1',
+        'contains_collection': True,
+        'link_libraries': ['xAODCaloEvent'],
+    },
+    'CaloClusters': {
+        'metadata_type': 'add_atlas_event_collection_info',
+        'name': 'CaloClusters',
+        'include_files': ['xAODCaloEvent/CaloClusterContainer.h',],
+        'container_type': 'DataVector<xAOD::CaloCluster_v1>',
+        'element_type': 'xAOD::CaloCluster_v1',
+        'contains_collection': True,
+        'link_libraries': ['xAODCaloEvent'],
     },
     'EventInfo': {
         'metadata_type': 'add_atlas_event_collection_info',
         'name': 'EventInfo',
         'include_files': ['xAODEventInfo/versions/EventInfo_v1.h',],
         'container_type': 'xAOD::EventInfo_v1',
         'contains_collection': False,
@@ -537,93 +537,93 @@
 @func_adl_callback(_add_collection_metadata)
 class Event:
     '''The top level event class. All data in the event is accessed from here
     '''
 
 
 
-    def CaloTowers(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.calotower_v1.CaloTower_v1]:
+    def BTaggings(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.btagging_v1.BTagging_v1]:
         ...
 
-    def CaloClusters(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.calocluster_v1.CaloCluster_v1]:
+    def BTagVertices(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.btagvertex_v1.BTagVertex_v1]:
         ...
 
-    def BTagVertices(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.btagvertex_v1.BTagVertex_v1]:
+    @func_adl_callback(lambda s, a: func_adl_servicex_xaodr21.calibration_support.fixup_collection_call(s, a, 'jet_collection'))
+    def Jets(self, collection: Optional[str] = None, calibrate: Optional[bool] = True) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.jet_v1.Jet_v1]:
         ...
 
-    def BTaggings(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.btagging_v1.BTagging_v1]:
+    def Egammas(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.egamma_v1.Egamma_v1]:
+        ...
+
+    @func_adl_callback(lambda s, a: func_adl_servicex_xaodr21.calibration_support.fixup_collection_call(s, a, 'electron_collection'))
+    def Electrons(self, collection: Optional[str] = None, calibrate: Optional[bool] = True) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.electron_v1.Electron_v1]:
         ...
 
     @func_adl_callback(lambda s, a: func_adl_servicex_xaodr21.calibration_support.fixup_collection_call(s, a, 'photon_collection'))
     def Photons(self, collection: Optional[str] = None, calibrate: Optional[bool] = True) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.photon_v1.Photon_v1]:
         ...
 
-    def Egammas(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.egamma_v1.Egamma_v1]:
+    @func_adl_callback(lambda s, a: func_adl_servicex_xaodr21.calibration_support.fixup_collection_call(s, a, 'tau_collection'))
+    def TauJets(self, collection: Optional[str] = None, calibrate: Optional[bool] = True) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.taujet_v3.TauJet_v3]:
         ...
 
-    @func_adl_callback(lambda s, a: func_adl_servicex_xaodr21.calibration_support.fixup_collection_call(s, a, 'electron_collection'))
-    def Electrons(self, collection: Optional[str] = None, calibrate: Optional[bool] = True) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.electron_v1.Electron_v1]:
+    def DiTauJets(self, calibration: str = 'NOSYS', working_point: str = 'Tight') -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.ditaujet_v1.DiTauJet_v1]:
+        ...
+
+    def TauTracks(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.tautrack_v1.TauTrack_v1]:
+        ...
+
+    def TruthVertices(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.truthvertex_v1.TruthVertex_v1]:
         ...
 
     def TruthEvents(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.truthevent_v1.TruthEvent_v1]:
         ...
 
     def TruthParticles(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.truthparticle_v1.TruthParticle_v1]:
         ...
 
     def TruthMetaDatas(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.truthmetadata_v1.TruthMetaData_v1]:
         ...
 
-    def TruthVertices(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.truthvertex_v1.TruthVertex_v1]:
-        ...
-
     @func_adl_callback(lambda s, a: func_adl_servicex_xaodr21.calibration_support.fixup_collection_call(s, a, 'met_collection'))
     def MissingET(self, collection: Optional[str] = None, calibrate: Optional[bool] = True) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.missinget_v1.MissingET_v1]:
         ...
 
     def EventInfos(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1]:
         ...
 
-    @func_adl_callback(lambda s, a: func_adl_servicex_xaodr21.calibration_support.fixup_collection_call(s, a, 'tau_collection'))
-    def TauJets(self, collection: Optional[str] = None, calibrate: Optional[bool] = True) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.taujet_v3.TauJet_v3]:
-        ...
-
-    def DiTauJets(self, calibration: str = 'NOSYS', working_point: str = 'Tight') -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.ditaujet_v1.DiTauJet_v1]:
+    def MuonSegments(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.muonsegment_v1.MuonSegment_v1]:
         ...
 
-    def TauTracks(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.tautrack_v1.TauTrack_v1]:
+    def SlowMuons(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.slowmuon_v1.SlowMuon_v1]:
         ...
 
     @func_adl_callback(lambda s, a: func_adl_servicex_xaodr21.calibration_support.fixup_collection_call(s, a, 'muon_collection'))
     def Muons(self, collection: Optional[str] = None, calibrate: Optional[bool] = True) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.muon_v1.Muon_v1]:
         ...
 
-    def MuonSegments(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.muonsegment_v1.MuonSegment_v1]:
+    def IParticles(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.iparticle.IParticle]:
         ...
 
-    def SlowMuons(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.slowmuon_v1.SlowMuon_v1]:
+    def Vertices(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.vertex_v1.Vertex_v1]:
         ...
 
-    def IParticles(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.iparticle.IParticle]:
+    def NeutralParticles(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.neutralparticle_v1.NeutralParticle_v1]:
         ...
 
-    def TrackCaloClusters(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.trackcalocluster_v1.TrackCaloCluster_v1]:
+    def TrackParticles(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1]:
         ...
 
     def PFOs(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.pfo_v1.PFO_v1]:
         ...
 
-    @func_adl_callback(lambda s, a: func_adl_servicex_xaodr21.calibration_support.fixup_collection_call(s, a, 'jet_collection'))
-    def Jets(self, collection: Optional[str] = None, calibrate: Optional[bool] = True) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.jet_v1.Jet_v1]:
-        ...
-
-    def NeutralParticles(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.neutralparticle_v1.NeutralParticle_v1]:
+    def TrackCaloClusters(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.trackcalocluster_v1.TrackCaloCluster_v1]:
         ...
 
-    def TrackParticles(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1]:
+    def CaloTowers(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.calotower_v1.CaloTower_v1]:
         ...
 
-    def Vertices(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.vertex_v1.Vertex_v1]:
+    def CaloClusters(self, name: str) -> func_adl_servicex_xaodr21.FADLStream[func_adl_servicex_xaodr21.xAOD.calocluster_v1.CaloCluster_v1]:
         ...
 
     def EventInfo(self, name: str) -> func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1:
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/func_adl_iterable.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/func_adl_iterable.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/metadata_for_collections.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/metadata_for_collections.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/mutex.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/mutex.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'try_lock': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'mutex',
         'method_name': 'try_lock',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class mutex:
     "A class"
 
-
     def try_lock(self) -> bool:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/std/__init__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/TruthEvent_v1/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,12 @@
             self._loaded = importlib.import_module(self._name)
         return getattr(self._loaded, __name)
 
 
 # Class loads. We do this to both enable type checking and also
 # get around potential circular references in the C++ data model.
 if not TYPE_CHECKING:
-    vector_float_ = _load_me("func_adl_servicex_xaodr21.std.vector_float_")
-    vector_int_ = _load_me("func_adl_servicex_xaodr21.std.vector_int_")
+    pdfinfo = _load_me("func_adl_servicex_xaodr21.xAOD.TruthEvent_v1.pdfinfo")
 else:
-    from . import vector_float_
-    from . import vector_int_
+    from . import pdfinfo
 
 # Include sub-namespace items
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/std/vector_float_.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_int_.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'std::vector<double>',
+        'type_string': 'vector<int>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class vector_float_(Iterable[float]):
+class vector_int_(Iterable[int]):
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/std/vector_int_.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_xaod_eventinfo_v1_subevent_.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'std::vector<int>',
+        'type_string': 'vector<xAOD::EventInfo_v1::SubEvent>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class vector_int_(Iterable[int]):
+class vector_xAOD_EventInfo_v1_SubEvent_(Iterable[func_adl_servicex_xaodr21.xAOD.EventInfo_v1.subevent.SubEvent]):
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/str.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/str.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'empty': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'string',
         'method_name': 'empty',
@@ -30,38 +29,33 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'string',
         'method_name': 'compare',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class str:
     "A class"
 
-
     def empty(self) -> bool:
         "A method"
         ...
 
     def append(self, __str: str) -> func_adl_servicex_xaodr21.str.str:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/tcomplex.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/tcomplex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'I': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'TComplex',
         'method_name': 'I',
@@ -178,38 +177,33 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'TComplex',
         'method_name': 'DeclFileLine',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class TComplex:
     "A class"
 
-
     def I(self) -> func_adl_servicex_xaodr21.tcomplex.TComplex:
         "A method"
         ...
 
     def One(self) -> func_adl_servicex_xaodr21.tcomplex.TComplex:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/corrections_electron.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/corrections_electron.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/corrections_jet.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/corrections_jet.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/corrections_met.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/corrections_met.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/corrections_muon.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/corrections_muon.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/corrections_overlap.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/corrections_overlap.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/corrections_photon.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/corrections_photon.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/corrections_tau.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/corrections_tau.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/templates/pileup_tool.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/templates/pileup_tool.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/tlorentzvector.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/tlorentzvector.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'Vect': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'TLorentzVector',
         'method_name': 'Vect',
@@ -46,51 +45,46 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'TLorentzVector',
         'method_name': 'DistancetoPrimitive',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class TLorentzVector:
     "A class"
 
-
     def Vect(self) -> func_adl_servicex_xaodr21.tvector3.TVector3:
         "A method"
         ...
 
     def EtaPhiVector(self) -> func_adl_servicex_xaodr21.tvector2.TVector2:
         "A method"
         ...
 
     def BoostVector(self) -> func_adl_servicex_xaodr21.tvector3.TVector3:
         "A method"
         ...
 
-    def Transform(self, noname_arg: func_adl_servicex_xaodr21.trotation.TRotation) -> func_adl_servicex_xaodr21.tlorentzvector.TLorentzVector:
+    def Transform(self, noname_arg: TRotation) -> func_adl_servicex_xaodr21.tlorentzvector.TLorentzVector:
         "A method"
         ...
 
     def ImplFileLine(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/trigger.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/trigger.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/trotation.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/trotation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'Transform': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'TRotation',
         'method_name': 'Transform',
@@ -70,67 +69,62 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'TRotation',
         'method_name': 'DistancetoPrimitive',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class TRotation:
     "A class"
 
-
     def Transform(self, noname_arg: TRotation) -> func_adl_servicex_xaodr21.trotation.TRotation:
         "A method"
         ...
 
     def Inverse(self) -> func_adl_servicex_xaodr21.trotation.TRotation:
         "A method"
         ...
 
     def Invert(self) -> func_adl_servicex_xaodr21.trotation.TRotation:
         "A method"
         ...
 
-    def RotateAxes(self, newX: func_adl_servicex_xaodr21.tvector3.TVector3, newY: func_adl_servicex_xaodr21.tvector3.TVector3, newZ: func_adl_servicex_xaodr21.tvector3.TVector3) -> func_adl_servicex_xaodr21.trotation.TRotation:
+    def RotateAxes(self, newX: TVector3, newY: TVector3, newZ: TVector3) -> func_adl_servicex_xaodr21.trotation.TRotation:
         "A method"
         ...
 
     def SetToIdentity(self) -> func_adl_servicex_xaodr21.trotation.TRotation:
         "A method"
         ...
 
-    def SetXAxis(self, axis: func_adl_servicex_xaodr21.tvector3.TVector3) -> func_adl_servicex_xaodr21.trotation.TRotation:
+    def SetXAxis(self, axis: TVector3) -> func_adl_servicex_xaodr21.trotation.TRotation:
         "A method"
         ...
 
-    def SetYAxis(self, axis: func_adl_servicex_xaodr21.tvector3.TVector3) -> func_adl_servicex_xaodr21.trotation.TRotation:
+    def SetYAxis(self, axis: TVector3) -> func_adl_servicex_xaodr21.trotation.TRotation:
         "A method"
         ...
 
-    def SetZAxis(self, axis: func_adl_servicex_xaodr21.tvector3.TVector3) -> func_adl_servicex_xaodr21.trotation.TRotation:
+    def SetZAxis(self, axis: TVector3) -> func_adl_servicex_xaodr21.trotation.TRotation:
         "A method"
         ...
 
     def ImplFileLine(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/tsqlresult.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Detail/tschemaruleset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,60 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
-    'GetFieldCount': {
+    'GetClassVersion': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'TSQLResult',
-        'method_name': 'GetFieldCount',
+        'type_string': 'ROOT::Detail::TSchemaRuleSet',
+        'method_name': 'GetClassVersion',
         'return_type': 'int',
     },
-    'GetRowCount': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'TSQLResult',
-        'method_name': 'GetRowCount',
-        'return_type': 'int',
-    },
-    'Next': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'TSQLResult',
-        'method_name': 'Next',
-        'return_type': 'TSQLRow*',
-    },
     'ImplFileLine': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'TSQLResult',
+        'type_string': 'ROOT::Detail::TSchemaRuleSet',
         'method_name': 'ImplFileLine',
         'return_type': 'int',
     },
     'DeclFileLine': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'TSQLResult',
+        'type_string': 'ROOT::Detail::TSchemaRuleSet',
         'method_name': 'DeclFileLine',
         'return_type': 'int',
     },
     'DistancetoPrimitive': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'TSQLResult',
+        'type_string': 'ROOT::Detail::TSchemaRuleSet',
         'method_name': 'DistancetoPrimitive',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class TSQLResult:
+class TSchemaRuleSet:
     "A class"
 
-
-    def GetFieldCount(self) -> int:
-        "A method"
-        ...
-
-    def GetRowCount(self) -> int:
-        "A method"
-        ...
-
-    def Next(self) -> func_adl_servicex_xaodr21.tsqlrow.TSQLRow:
+    def GetClassVersion(self) -> int:
         "A method"
         ...
 
     def ImplFileLine(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/tsqlrow.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_truthvertex_v1___.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
-    'ImplFileLine': {
+    'size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'TSQLRow',
-        'method_name': 'ImplFileLine',
-        'return_type': 'int',
-    },
-    'DeclFileLine': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'TSQLRow',
-        'method_name': 'DeclFileLine',
-        'return_type': 'int',
-    },
-    'DistancetoPrimitive': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'TSQLRow',
-        'method_name': 'DistancetoPrimitive',
+        'type_string': 'vector<ElementLink<DataVector<xAOD::TruthVertex_v1>>>',
+        'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class TSQLRow:
+class vector_ElementLink_DataVector_xAOD_TruthVertex_v1___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_truthvertex_v1__.ElementLink_DataVector_xAOD_TruthVertex_v1__]):
     "A class"
 
-
-    def ImplFileLine(self) -> int:
-        "A method"
-        ...
-
-    def DeclFileLine(self) -> int:
-        "A method"
-        ...
-
-    def DistancetoPrimitive(self, px: int, py: int) -> int:
+    def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/tthread.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/tthread.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,20 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'Kill': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'TThread',
         'method_name': 'Kill',
         'return_type': 'int',
     },
-    'GetPriority': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'TThread',
-        'method_name': 'GetPriority',
-        'return_type': 'TThread::EPriority',
-    },
-    'GetState': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'TThread',
-        'method_name': 'GetState',
-        'return_type': 'TThread::EState',
-    },
     'Exists': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'TThread',
         'method_name': 'Exists',
         'return_type': 'int',
     },
     'Lock': {
@@ -118,65 +105,37 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'TThread',
         'method_name': 'DistancetoPrimitive',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class TThread:
     "A class"
 
-    class EPriority(Enum):
-        kLowPriority = 0
-        kNormalPriority = 1
-        kHighPriority = 2
-
-    class EState(Enum):
-        kInvalidState = 0
-        kNewState = 1
-        kRunningState = 2
-        kTerminatedState = 3
-        kFinishedState = 4
-        kCancelingState = 5
-        kCanceledState = 6
-        kDeletingState = 7
-
-
     def Kill(self) -> int:
         "A method"
         ...
 
-    def GetPriority(self) -> func_adl_servicex_xaodr21.tthread.TThread.EPriority:
-        "A method"
-        ...
-
-    def GetState(self) -> func_adl_servicex_xaodr21.tthread.TThread.EState:
-        "A method"
-        ...
-
     def Exists(self) -> int:
         "A method"
         ...
 
     def Lock(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/tvector2.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/tvector2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'Unit': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'TVector2',
         'method_name': 'Unit',
@@ -46,38 +45,33 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'TVector2',
         'method_name': 'DistancetoPrimitive',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class TVector2:
     "A class"
 
-
     def Unit(self) -> func_adl_servicex_xaodr21.tvector2.TVector2:
         "A method"
         ...
 
     def Ort(self) -> func_adl_servicex_xaodr21.tvector2.TVector2:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/tvector3.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/tvector3.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'EtaPhiVector': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'TVector3',
         'method_name': 'EtaPhiVector',
@@ -58,38 +57,33 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'TVector3',
         'method_name': 'DistancetoPrimitive',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class TVector3:
     "A class"
 
-
     def EtaPhiVector(self) -> func_adl_servicex_xaodr21.tvector2.TVector2:
         "A method"
         ...
 
     def Unit(self) -> func_adl_servicex_xaodr21.tvector3.TVector3:
         "A method"
         ...
@@ -98,15 +92,15 @@
         "A method"
         ...
 
     def Cross(self, noname_arg: TVector3) -> func_adl_servicex_xaodr21.tvector3.TVector3:
         "A method"
         ...
 
-    def Transform(self, noname_arg: func_adl_servicex_xaodr21.trotation.TRotation) -> func_adl_servicex_xaodr21.tvector3.TVector3:
+    def Transform(self, noname_arg: TRotation) -> func_adl_servicex_xaodr21.tvector3.TVector3:
         "A method"
         ...
 
     def XYvector(self) -> func_adl_servicex_xaodr21.tvector2.TVector2:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/type_support.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/type_support.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_calocluster_v1___.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_vertex_v1___.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'vector<ElementLink<DataVector<xAOD::CaloCluster_v1>>>',
+        'type_string': 'vector<ElementLink<DataVector<xAOD::Vertex_v1>>>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class vector_ElementLink_DataVector_xAOD_CaloCluster_v1___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_calocluster_v1__.ElementLink_DataVector_xAOD_CaloCluster_v1__]):
+class vector_ElementLink_DataVector_xAOD_Vertex_v1___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_vertex_v1__.ElementLink_DataVector_xAOD_Vertex_v1__]):
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_iparticle___.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_neutralparticle_v1___.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'vector<ElementLink<DataVector<xAOD::IParticle>>>',
+        'type_string': 'vector<ElementLink<DataVector<xAOD::NeutralParticle_v1>>>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class vector_ElementLink_DataVector_xAOD_IParticle___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_iparticle__.ElementLink_DataVector_xAOD_IParticle__]):
+class vector_ElementLink_DataVector_xAOD_NeutralParticle_v1___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_neutralparticle_v1__.ElementLink_DataVector_xAOD_NeutralParticle_v1__]):
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_muonsegment_v1___.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_iparticle___.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'vector<ElementLink<DataVector<xAOD::MuonSegment_v1>>>',
+        'type_string': 'vector<ElementLink<DataVector<xAOD::IParticle>>>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class vector_ElementLink_DataVector_xAOD_MuonSegment_v1___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_muonsegment_v1__.ElementLink_DataVector_xAOD_MuonSegment_v1__]):
+class vector_ElementLink_DataVector_xAOD_IParticle___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_iparticle__.ElementLink_DataVector_xAOD_IParticle__]):
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_neutralparticle_v1___.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_vector_float__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'vector<ElementLink<DataVector<xAOD::NeutralParticle_v1>>>',
+        'type_string': 'vector<vector<float>>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class vector_ElementLink_DataVector_xAOD_NeutralParticle_v1___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_neutralparticle_v1__.ElementLink_DataVector_xAOD_NeutralParticle_v1__]):
+class vector_vector_float__(Iterable[func_adl_servicex_xaodr21.vector_float_.vector_float_]):
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_pfo_v1___.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_pfo_v1___.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'vector<ElementLink<DataVector<xAOD::PFO_v1>>>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class vector_ElementLink_DataVector_xAOD_PFO_v1___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_pfo_v1__.ElementLink_DataVector_xAOD_PFO_v1__]):
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_tautrack_v1___.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_tautrack_v1___.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'vector<ElementLink<DataVector<xAOD::TauTrack_v1>>>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class vector_ElementLink_DataVector_xAOD_TauTrack_v1___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_tautrack_v1__.ElementLink_DataVector_xAOD_TauTrack_v1__]):
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_trackparticle_v1___.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_root_fit_parametersettings_.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'vector<ElementLink<DataVector<xAOD::TrackParticle_v1>>>',
+        'type_string': 'vector<ROOT::Fit::ParameterSettings>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class vector_ElementLink_DataVector_xAOD_TrackParticle_v1___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_trackparticle_v1__.ElementLink_DataVector_xAOD_TrackParticle_v1__]):
+class vector_ROOT_Fit_ParameterSettings_(Iterable[func_adl_servicex_xaodr21.ROOT.Fit.parametersettings.ParameterSettings]):
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_truthparticle_v1___.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_calocluster_v1___.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'vector<ElementLink<DataVector<xAOD::TruthParticle_v1>>>',
+        'type_string': 'vector<ElementLink<DataVector<xAOD::CaloCluster_v1>>>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class vector_ElementLink_DataVector_xAOD_TruthParticle_v1___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_truthparticle_v1__.ElementLink_DataVector_xAOD_TruthParticle_v1__]):
+class vector_ElementLink_DataVector_xAOD_CaloCluster_v1___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_calocluster_v1__.ElementLink_DataVector_xAOD_CaloCluster_v1__]):
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_truthvertex_v1___.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_muonsegment_v1___.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'vector<ElementLink<DataVector<xAOD::TruthVertex_v1>>>',
+        'type_string': 'vector<ElementLink<DataVector<xAOD::MuonSegment_v1>>>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class vector_ElementLink_DataVector_xAOD_TruthVertex_v1___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_truthvertex_v1__.ElementLink_DataVector_xAOD_TruthVertex_v1__]):
+class vector_ElementLink_DataVector_xAOD_MuonSegment_v1___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_muonsegment_v1__.ElementLink_DataVector_xAOD_MuonSegment_v1__]):
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_vertex_v1___.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/TruthParticle_v1/polarization.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
-    'size': {
+    'valid': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'vector<ElementLink<DataVector<xAOD::Vertex_v1>>>',
-        'method_name': 'size',
-        'return_type': 'int',
+        'type_string': 'xAOD::TruthParticle_v1::Polarization',
+        'method_name': 'valid',
+        'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
+        s_update = s_update.MetaData({
+            'metadata_type': 'inject_code',
+            'name': 'xAODTruth/versions/TruthParticle_v1.h',
+            'body_includes': ["xAODTruth/versions/TruthParticle_v1.h"],
+        })
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class vector_ElementLink_DataVector_xAOD_Vertex_v1___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_vertex_v1__.ElementLink_DataVector_xAOD_Vertex_v1__]):
+class Polarization:
     "A class"
 
-
-    def size(self) -> int:
+    def valid(self) -> bool:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_float_.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_xaod_caloclusterbadchanneldata_v1_.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'vector<float>',
+        'type_string': 'vector<xAOD::CaloClusterBadChannelData_v1>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class vector_float_(Iterable[float]):
+class vector_xAOD_CaloClusterBadChannelData_v1_(Iterable[func_adl_servicex_xaodr21.xAOD.caloclusterbadchanneldata_v1.CaloClusterBadChannelData_v1]):
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_int_.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/TruthEvent_v1/pdfinfo.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
-    'size': {
+    'valid': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'vector<int>',
-        'method_name': 'size',
-        'return_type': 'int',
+        'type_string': 'xAOD::TruthEvent_v1::PdfInfo',
+        'method_name': 'valid',
+        'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
+        s_update = s_update.MetaData({
+            'metadata_type': 'inject_code',
+            'name': 'xAODTruth/versions/TruthEvent_v1.h',
+            'body_includes': ["xAODTruth/versions/TruthEvent_v1.h"],
+        })
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class vector_int_(Iterable[int]):
+class PdfInfo:
     "A class"
 
-
-    def size(self) -> int:
+    def valid(self) -> bool:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_pair_float_float__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_float_.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'vector<pair<double,double>>',
+        'type_string': 'vector<float>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class vector_pair_float_float__:
+class vector_float_(Iterable[float]):
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_pair_str_str__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_pair_str_str__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'vector<pair<string,string>>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class vector_pair_str_str__:
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_str_.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_elementlink_datavector_xaod_truthparticle_v1___.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'vector<string>',
+        'type_string': 'vector<ElementLink<DataVector<xAOD::TruthParticle_v1>>>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class vector_str_(Iterable[func_adl_servicex_xaodr21.str.str]):
+class vector_ElementLink_DataVector_xAOD_TruthParticle_v1___(Iterable[func_adl_servicex_xaodr21.elementlink_datavector_xaod_truthparticle_v1__.ElementLink_DataVector_xAOD_TruthParticle_v1__]):
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_xaod_caloclusterbadchanneldata_v1_.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_str_.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'vector<xAOD::CaloClusterBadChannelData_v1>',
+        'type_string': 'vector<string>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class vector_xAOD_CaloClusterBadChannelData_v1_(Iterable[func_adl_servicex_xaodr21.xAOD.caloclusterbadchanneldata_v1.CaloClusterBadChannelData_v1]):
+class vector_str_(Iterable[func_adl_servicex_xaodr21.str.str]):
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_xaod_eventinfo_v1_streamtag_.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_xaod_eventinfo_v1_streamtag_.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'vector<xAOD::EventInfo_v1::StreamTag>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class vector_xAOD_EventInfo_v1_StreamTag_(Iterable[func_adl_servicex_xaodr21.xAOD.EventInfo_v1.streamtag.StreamTag]):
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/vector_xaod_jetconstituent_.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/vector_xaod_jetconstituent_.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'size': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'vector<xAOD::JetConstituent>',
         'method_name': 'size',
         'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class vector_xAOD_JetConstituent_(Iterable[func_adl_servicex_xaodr21.xAOD.jetconstituent.JetConstituent]):
     "A class"
 
-
     def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/EventInfo_v1/__init__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/EventInfo_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/EventInfo_v1/streamtag.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/EventInfo_v1/streamtag.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'name': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::EventInfo_v1::StreamTag',
         'method_name': 'name',
@@ -24,38 +23,33 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::EventInfo_v1::StreamTag',
         'method_name': 'obeysLumiblock',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class StreamTag:
     "A class"
 
-
     def name(self) -> func_adl_servicex_xaodr21.str.str:
         "A method"
         ...
 
     def type(self) -> func_adl_servicex_xaodr21.str.str:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/EventInfo_v1/subevent.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/EventInfo_v1/subevent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
-    'type': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::EventInfo_v1::SubEvent',
-        'method_name': 'type',
-        'return_type': 'xAOD::EventInfo_v1::PileUpType',
-    },
     'typeName': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::EventInfo_v1::SubEvent',
         'method_name': 'typeName',
         'return_type_element': '__gnu_cxx::__normal_iterator<char*,string>',
         'return_type_collection': 'const string',
     },
@@ -29,42 +22,33 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::EventInfo_v1::SubEvent',
         'method_name': 'ptr',
         'return_type': 'const xAOD::EventInfo_v1*',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class SubEvent:
     "A class"
 
-
-    def type(self) -> func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.PileUpType:
-        "A method"
-        ...
-
     def typeName(self) -> func_adl_servicex_xaodr21.str.str:
         "A method"
         ...
 
     def link(self) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_eventinfo_v1__.ElementLink_DataVector_xAOD_EventInfo_v1__:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/TruthEvent_v1/__init__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/TruthParticle_v1/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,12 +22,12 @@
             self._loaded = importlib.import_module(self._name)
         return getattr(self._loaded, __name)
 
 
 # Class loads. We do this to both enable type checking and also
 # get around potential circular references in the C++ data model.
 if not TYPE_CHECKING:
-    pdfinfo = _load_me("func_adl_servicex_xaodr21.xAOD.TruthEvent_v1.pdfinfo")
+    polarization = _load_me("func_adl_servicex_xaodr21.xAOD.TruthParticle_v1.polarization")
 else:
-    from . import pdfinfo
+    from . import polarization
 
 # Include sub-namespace items
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/TruthEvent_v1/pdfinfo.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/std/vector_float_.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
-    'valid': {
+    'size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::TruthEvent_v1::PdfInfo',
-        'method_name': 'valid',
-        'return_type': 'bool',
+        'type_string': 'std::vector<double>',
+        'method_name': 'size',
+        'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        s_update = s_update.MetaData({
-            'metadata_type': 'inject_code',
-            'name': 'xAODTruth/versions/TruthEvent_v1.h',
-            'body_includes': ["xAODTruth/versions/TruthEvent_v1.h"],
-        })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class PdfInfo:
+class vector_float_(Iterable[float]):
     "A class"
 
-
-    def valid(self) -> bool:
+    def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/TruthParticle_v1/polarization.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/std/vector_int_.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,37 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
-    'valid': {
+    'size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::TruthParticle_v1::Polarization',
-        'method_name': 'valid',
-        'return_type': 'bool',
+        'type_string': 'std::vector<int>',
+        'method_name': 'size',
+        'return_type': 'int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        s_update = s_update.MetaData({
-            'metadata_type': 'inject_code',
-            'name': 'xAODTruth/versions/TruthParticle_v1.h',
-            'body_includes': ["xAODTruth/versions/TruthParticle_v1.h"],
-        })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class Polarization:
+class vector_int_(Iterable[int]):
     "A class"
 
-
-    def valid(self) -> bool:
+    def size(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/__init__.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,16 @@
     calocluster_v1 = _load_me("func_adl_servicex_xaodr21.xAOD.calocluster_v1")
     calotower_v1 = _load_me("func_adl_servicex_xaodr21.xAOD.calotower_v1")
     ditaujet_v1 = _load_me("func_adl_servicex_xaodr21.xAOD.ditaujet_v1")
     egamma_v1 = _load_me("func_adl_servicex_xaodr21.xAOD.egamma_v1")
     electron_v1 = _load_me("func_adl_servicex_xaodr21.xAOD.electron_v1")
     eventinfo_v1 = _load_me("func_adl_servicex_xaodr21.xAOD.eventinfo_v1")
     iparticle = _load_me("func_adl_servicex_xaodr21.xAOD.iparticle")
-    jetalgorithmtype = _load_me("func_adl_servicex_xaodr21.xAOD.jetalgorithmtype")
     jetconstituent = _load_me("func_adl_servicex_xaodr21.xAOD.jetconstituent")
     jetconstituentvector = _load_me("func_adl_servicex_xaodr21.xAOD.jetconstituentvector")
-    jetinput = _load_me("func_adl_servicex_xaodr21.xAOD.jetinput")
     jet_v1 = _load_me("func_adl_servicex_xaodr21.xAOD.jet_v1")
     missinget_v1 = _load_me("func_adl_servicex_xaodr21.xAOD.missinget_v1")
     muonsegment_v1 = _load_me("func_adl_servicex_xaodr21.xAOD.muonsegment_v1")
     muon_v1 = _load_me("func_adl_servicex_xaodr21.xAOD.muon_v1")
     neutralparticle_v1 = _load_me("func_adl_servicex_xaodr21.xAOD.neutralparticle_v1")
     pfo_v1 = _load_me("func_adl_servicex_xaodr21.xAOD.pfo_v1")
     photon_v1 = _load_me("func_adl_servicex_xaodr21.xAOD.photon_v1")
@@ -65,18 +63,16 @@
     from . import calocluster_v1
     from . import calotower_v1
     from . import ditaujet_v1
     from . import egamma_v1
     from . import electron_v1
     from . import eventinfo_v1
     from . import iparticle
-    from . import jetalgorithmtype
     from . import jetconstituent
     from . import jetconstituentvector
-    from . import jetinput
     from . import jet_v1
     from . import missinget_v1
     from . import muonsegment_v1
     from . import muon_v1
     from . import neutralparticle_v1
     from . import pfo_v1
     from . import photon_v1
@@ -89,10 +85,10 @@
     from . import truthevent_v1
     from . import truthmetadata_v1
     from . import truthparticle_v1
     from . import truthvertex_v1
     from . import vertex_v1
 
 # Include sub-namespace items
-from . import EventInfo_v1
 from . import TruthParticle_v1
+from . import EventInfo_v1
 from . import TruthEvent_v1
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/btagging_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/ditaujet_v1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,465 +1,348 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
-    'SV0_significance3D': {
+    'pt': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'SV0_significance3D',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'pt',
         'return_type': 'double',
     },
-    'SV0_TrackParticleLinks': {
+    'eta': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'SV0_TrackParticleLinks',
-        'return_type_element': 'ElementLink<DataVector<xAOD::TrackParticle_v1>>',
-        'return_type_collection': 'const vector<ElementLink<DataVector<xAOD::TrackParticle_v1>>>',
-    },
-    'SV0_TrackParticle': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'SV0_TrackParticle',
-        'return_type': 'const xAOD::TrackParticle_v1*',
-    },
-    'nSV0_TrackParticles': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'nSV0_TrackParticles',
-        'return_type': 'int',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'eta',
+        'return_type': 'double',
     },
-    'SV1_pb': {
+    'phi': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'SV1_pb',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'phi',
         'return_type': 'double',
     },
-    'SV1_pc': {
+    'e': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'SV1_pc',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'e',
         'return_type': 'double',
     },
-    'SV1_pu': {
+    'm': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'SV1_pu',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'm',
         'return_type': 'double',
     },
-    'SV1_loglikelihoodratio': {
+    'rapidity': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'SV1_loglikelihoodratio',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'rapidity',
         'return_type': 'double',
     },
-    'SV1_TrackParticleLinks': {
+    'p4': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'SV1_TrackParticleLinks',
-        'return_type_element': 'ElementLink<DataVector<xAOD::TrackParticle_v1>>',
-        'return_type_collection': 'const vector<ElementLink<DataVector<xAOD::TrackParticle_v1>>>',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'p4',
+        'return_type': 'const TLorentzVector',
     },
-    'SV1_TrackParticle': {
+    'jetLink': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'SV1_TrackParticle',
-        'return_type': 'const xAOD::TrackParticle_v1*',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'jetLink',
+        'return_type': 'const ElementLink<DataVector<xAOD::Jet_v1>>',
     },
-    'nSV1_TrackParticles': {
+    'jet': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'nSV1_TrackParticles',
-        'return_type': 'int',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'jet',
+        'return_type': 'const xAOD::Jet_v1*',
     },
-    'IP2D_pb': {
+    'subjetPt': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'IP2D_pb',
-        'return_type': 'double',
-    },
-    'IP2D_pc': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'IP2D_pc',
-        'return_type': 'double',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'subjetPt',
+        'return_type': 'float',
     },
-    'IP2D_pu': {
+    'subjetEta': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'IP2D_pu',
-        'return_type': 'double',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'subjetEta',
+        'return_type': 'float',
     },
-    'IP2D_loglikelihoodratio': {
+    'subjetPhi': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'IP2D_loglikelihoodratio',
-        'return_type': 'double',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'subjetPhi',
+        'return_type': 'float',
     },
-    'IP2D_TrackParticleLinks': {
+    'subjetE': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'IP2D_TrackParticleLinks',
-        'return_type_element': 'ElementLink<DataVector<xAOD::TrackParticle_v1>>',
-        'return_type_collection': 'const vector<ElementLink<DataVector<xAOD::TrackParticle_v1>>>',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'subjetE',
+        'return_type': 'float',
     },
-    'IP2D_TrackParticle': {
+    'nSubjets': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'IP2D_TrackParticle',
-        'return_type': 'const xAOD::TrackParticle_v1*',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'nSubjets',
+        'return_type': 'float',
     },
-    'nIP2D_TrackParticles': {
+    'fCore': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'nIP2D_TrackParticles',
-        'return_type': 'int',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'fCore',
+        'return_type': 'float',
     },
-    'IP3D_pb': {
+    'vertexLink': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'IP3D_pb',
-        'return_type': 'double',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'vertexLink',
+        'return_type': 'const ElementLink<DataVector<xAOD::Vertex_v1>>',
     },
-    'IP3D_pc': {
+    'vertex': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'IP3D_pc',
-        'return_type': 'double',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'vertex',
+        'return_type': 'const xAOD::Vertex_v1*',
     },
-    'IP3D_pu': {
+    'trackLinks': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'IP3D_pu',
-        'return_type': 'double',
-    },
-    'IP3D_loglikelihoodratio': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'IP3D_loglikelihoodratio',
-        'return_type': 'double',
-    },
-    'IP3D_TrackParticleLinks': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'IP3D_TrackParticleLinks',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'trackLinks',
         'return_type_element': 'ElementLink<DataVector<xAOD::TrackParticle_v1>>',
         'return_type_collection': 'const vector<ElementLink<DataVector<xAOD::TrackParticle_v1>>>',
     },
-    'IP3D_TrackParticle': {
+    'track': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'IP3D_TrackParticle',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'track',
         'return_type': 'const xAOD::TrackParticle_v1*',
     },
-    'nIP3D_TrackParticles': {
+    'nTracks': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'nIP3D_TrackParticles',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'nTracks',
         'return_type': 'int',
     },
-    'SV1plusIP3D_discriminant': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'SV1plusIP3D_discriminant',
-        'return_type': 'double',
-    },
-    'JetFitter_pb': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'JetFitter_pb',
-        'return_type': 'double',
-    },
-    'JetFitter_pc': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'JetFitter_pc',
-        'return_type': 'double',
-    },
-    'JetFitter_pu': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'JetFitter_pu',
-        'return_type': 'double',
-    },
-    'JetFitter_loglikelihoodratio': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'JetFitter_loglikelihoodratio',
-        'return_type': 'double',
-    },
-    'MV1_discriminant': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'MV1_discriminant',
-        'return_type': 'double',
-    },
-    'loglikelihoodratio': {
+    'otherTrackLinks': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'loglikelihoodratio',
-        'return_type': 'bool',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'otherTrackLinks',
+        'return_type_element': 'ElementLink<DataVector<xAOD::TrackParticle_v1>>',
+        'return_type_collection': 'const vector<ElementLink<DataVector<xAOD::TrackParticle_v1>>>',
     },
-    'MVx_discriminant': {
+    'otherTrack': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'MVx_discriminant',
-        'return_type': 'bool',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'otherTrack',
+        'return_type': 'const xAOD::TrackParticle_v1*',
     },
-    'pu': {
+    'nOtherTracks': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'pu',
-        'return_type': 'bool',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'nOtherTracks',
+        'return_type': 'int',
     },
-    'pb': {
+    'isoTrackLinks': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'pb',
-        'return_type': 'bool',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'isoTrackLinks',
+        'return_type_element': 'ElementLink<DataVector<xAOD::TrackParticle_v1>>',
+        'return_type_collection': 'const vector<ElementLink<DataVector<xAOD::TrackParticle_v1>>>',
     },
-    'pc': {
+    'isoTrack': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'pc',
-        'return_type': 'bool',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'isoTrack',
+        'return_type': 'const xAOD::TrackParticle_v1*',
     },
-    'calcLLR': {
+    'nIsoTracks': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
-        'method_name': 'calcLLR',
-        'return_type': 'double',
+        'type_string': 'xAOD::DiTauJet_v1',
+        'method_name': 'nIsoTracks',
+        'return_type': 'int',
     },
     'index': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
+        'type_string': 'xAOD::DiTauJet_v1',
         'method_name': 'index',
         'return_type': 'int',
     },
     'usingPrivateStore': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
+        'type_string': 'xAOD::DiTauJet_v1',
         'method_name': 'usingPrivateStore',
         'return_type': 'bool',
     },
     'usingStandaloneStore': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
+        'type_string': 'xAOD::DiTauJet_v1',
         'method_name': 'usingStandaloneStore',
         'return_type': 'bool',
     },
     'hasStore': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
+        'type_string': 'xAOD::DiTauJet_v1',
         'method_name': 'hasStore',
         'return_type': 'bool',
     },
     'hasNonConstStore': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
+        'type_string': 'xAOD::DiTauJet_v1',
         'method_name': 'hasNonConstStore',
         'return_type': 'bool',
     },
     'clearDecorations': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
+        'type_string': 'xAOD::DiTauJet_v1',
         'method_name': 'clearDecorations',
         'return_type': 'bool',
     },
     'auxdataConst': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
+        'type_string': 'xAOD::DiTauJet_v1',
         'method_name': 'auxdataConst',
         'return_type': 'U',
     },
     'isAvailable': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::BTagging_v1',
+        'type_string': 'xAOD::DiTauJet_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
-            'name': 'xAODBTagging/versions/BTagging_v1.h',
-            'body_includes': ["xAODBTagging/versions/BTagging_v1.h"],
+            'name': 'xAODTau/versions/DiTauJet_v1.h',
+            'body_includes': ["xAODTau/versions/DiTauJet_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class BTagging_v1:
+class DiTauJet_v1:
     "A class"
 
-
-    def SV0_significance3D(self) -> float:
-        "A method"
-        ...
-
-    def SV0_TrackParticleLinks(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_trackparticle_v1___.vector_ElementLink_DataVector_xAOD_TrackParticle_v1___:
-        "A method"
-        ...
-
-    def SV0_TrackParticle(self, i: int) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
-        "A method"
-        ...
-
-    def nSV0_TrackParticles(self) -> int:
-        "A method"
-        ...
-
-    def SV1_pb(self) -> float:
-        "A method"
-        ...
-
-    def SV1_pc(self) -> float:
-        "A method"
-        ...
-
-    def SV1_pu(self) -> float:
-        "A method"
-        ...
-
-    def SV1_loglikelihoodratio(self) -> float:
-        "A method"
-        ...
-
-    def SV1_TrackParticleLinks(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_trackparticle_v1___.vector_ElementLink_DataVector_xAOD_TrackParticle_v1___:
-        "A method"
-        ...
-
-    def SV1_TrackParticle(self, i: int) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
-        "A method"
-        ...
-
-    def nSV1_TrackParticles(self) -> int:
-        "A method"
-        ...
-
-    def IP2D_pb(self) -> float:
+    def pt(self) -> float:
         "A method"
         ...
 
-    def IP2D_pc(self) -> float:
+    def eta(self) -> float:
         "A method"
         ...
 
-    def IP2D_pu(self) -> float:
+    def phi(self) -> float:
         "A method"
         ...
 
-    def IP2D_loglikelihoodratio(self) -> float:
+    def e(self) -> float:
         "A method"
         ...
 
-    def IP2D_TrackParticleLinks(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_trackparticle_v1___.vector_ElementLink_DataVector_xAOD_TrackParticle_v1___:
+    def m(self) -> float:
         "A method"
         ...
 
-    def IP2D_TrackParticle(self, i: int) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
+    def rapidity(self) -> float:
         "A method"
         ...
 
-    def nIP2D_TrackParticles(self) -> int:
+    def p4(self) -> func_adl_servicex_xaodr21.tlorentzvector.TLorentzVector:
         "A method"
         ...
 
-    def IP3D_pb(self) -> float:
+    def jetLink(self) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_jet_v1__.ElementLink_DataVector_xAOD_Jet_v1__:
         "A method"
         ...
 
-    def IP3D_pc(self) -> float:
+    def jet(self) -> func_adl_servicex_xaodr21.xAOD.jet_v1.Jet_v1:
         "A method"
         ...
 
-    def IP3D_pu(self) -> float:
+    def subjetPt(self, numSubjet: int) -> float:
         "A method"
         ...
 
-    def IP3D_loglikelihoodratio(self) -> float:
+    def subjetEta(self, numSubjet: int) -> float:
         "A method"
         ...
 
-    def IP3D_TrackParticleLinks(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_trackparticle_v1___.vector_ElementLink_DataVector_xAOD_TrackParticle_v1___:
+    def subjetPhi(self, numSubjet: int) -> float:
         "A method"
         ...
 
-    def IP3D_TrackParticle(self, i: int) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
+    def subjetE(self, numSubjet: int) -> float:
         "A method"
         ...
 
-    def nIP3D_TrackParticles(self) -> int:
+    def nSubjets(self) -> float:
         "A method"
         ...
 
-    def SV1plusIP3D_discriminant(self) -> float:
+    def fCore(self, numSubjet: int) -> float:
         "A method"
         ...
 
-    def JetFitter_pb(self) -> float:
+    def vertexLink(self) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_vertex_v1__.ElementLink_DataVector_xAOD_Vertex_v1__:
         "A method"
         ...
 
-    def JetFitter_pc(self) -> float:
+    def vertex(self) -> func_adl_servicex_xaodr21.xAOD.vertex_v1.Vertex_v1:
         "A method"
         ...
 
-    def JetFitter_pu(self) -> float:
+    def trackLinks(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_trackparticle_v1___.vector_ElementLink_DataVector_xAOD_TrackParticle_v1___:
         "A method"
         ...
 
-    def JetFitter_loglikelihoodratio(self) -> float:
+    def track(self, i: int) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
         "A method"
         ...
 
-    def MV1_discriminant(self) -> float:
+    def nTracks(self) -> int:
         "A method"
         ...
 
-    def loglikelihoodratio(self, taggername: func_adl_servicex_xaodr21.str.str, value: float, signal: func_adl_servicex_xaodr21.str.str, bckgd: func_adl_servicex_xaodr21.str.str) -> bool:
+    def otherTrackLinks(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_trackparticle_v1___.vector_ElementLink_DataVector_xAOD_TrackParticle_v1___:
         "A method"
         ...
 
-    def MVx_discriminant(self, taggername: func_adl_servicex_xaodr21.str.str, value: float) -> bool:
+    def otherTrack(self, i: int) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
         "A method"
         ...
 
-    def pu(self, taggername: func_adl_servicex_xaodr21.str.str, value: float) -> bool:
+    def nOtherTracks(self) -> int:
         "A method"
         ...
 
-    def pb(self, taggername: func_adl_servicex_xaodr21.str.str, value: float) -> bool:
+    def isoTrackLinks(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_trackparticle_v1___.vector_ElementLink_DataVector_xAOD_TrackParticle_v1___:
         "A method"
         ...
 
-    def pc(self, taggername: func_adl_servicex_xaodr21.str.str, value: float) -> bool:
+    def isoTrack(self, i: int) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
         "A method"
         ...
 
-    def calcLLR(self, num: float, den: float) -> float:
+    def nIsoTracks(self) -> int:
         "A method"
         ...
 
     def index(self) -> int:
         "A method"
         ...
 
@@ -481,16 +364,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/btagvertex_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/btagvertex_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'chi2': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::BTagVertex_v1',
         'method_name': 'chi2',
@@ -119,16 +118,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::BTagVertex_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -136,26 +133,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODBTagging/versions/BTagVertex_v1.h',
             'body_includes': ["xAODBTagging/versions/BTagVertex_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class BTagVertex_v1:
     "A class"
 
-
     def chi2(self) -> float:
         "A method"
         ...
 
     def NDF(self) -> float:
         "A method"
         ...
@@ -214,16 +208,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/caloclusterbadchanneldata_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/caloclusterbadchanneldata_v1.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'eta': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::CaloClusterBadChannelData_v1',
         'method_name': 'eta',
@@ -14,30 +13,22 @@
     },
     'phi': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::CaloClusterBadChannelData_v1',
         'method_name': 'phi',
         'return_type': 'float',
     },
-    'layer': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::CaloClusterBadChannelData_v1',
-        'method_name': 'layer',
-        'return_type': 'CaloSampling::CaloSample',
-    },
     'badChannel': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::CaloClusterBadChannelData_v1',
         'method_name': 'badChannel',
         'return_type': 'unsigned int',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -45,34 +36,27 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODCaloEvent/versions/CaloClusterBadChannelData_v1.h',
             'body_includes': ["xAODCaloEvent/versions/CaloClusterBadChannelData_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class CaloClusterBadChannelData_v1:
     "A class"
 
-
     def eta(self) -> float:
         "A method"
         ...
 
     def phi(self) -> float:
         "A method"
         ...
 
-    def layer(self) -> func_adl_servicex_xaodr21.calosampling.CaloSampling.CaloSample:
-        "A method"
-        ...
-
     def badChannel(self) -> int:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/calotower_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/calotower_v1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'pt': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::CaloTower_v1',
         'method_name': 'pt',
@@ -94,16 +93,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::CaloTower_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -111,26 +108,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODCaloEvent/versions/CaloTower_v1.h',
             'body_includes': ["xAODCaloEvent/versions/CaloTower_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class CaloTower_v1:
     "A class"
 
-
     def pt(self) -> float:
         "A method"
         ...
 
     def eta(self) -> float:
         "A method"
         ...
@@ -177,16 +171,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/ditaujet_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/muon_v1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,354 +1,316 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'pt': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
+        'type_string': 'xAOD::Muon_v1',
         'method_name': 'pt',
         'return_type': 'double',
     },
     'eta': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
+        'type_string': 'xAOD::Muon_v1',
         'method_name': 'eta',
         'return_type': 'double',
     },
     'phi': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
+        'type_string': 'xAOD::Muon_v1',
         'method_name': 'phi',
         'return_type': 'double',
     },
-    'e': {
+    'm': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'e',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'm',
         'return_type': 'double',
     },
-    'm': {
+    'e': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'm',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'e',
         'return_type': 'double',
     },
     'rapidity': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
+        'type_string': 'xAOD::Muon_v1',
         'method_name': 'rapidity',
         'return_type': 'double',
     },
     'p4': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
+        'type_string': 'xAOD::Muon_v1',
         'method_name': 'p4',
         'return_type': 'const TLorentzVector',
     },
-    'jetLink': {
+    'charge': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'jetLink',
-        'return_type': 'const ElementLink<DataVector<xAOD::Jet_v1>>',
-    },
-    'jet': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'jet',
-        'return_type': 'const xAOD::Jet_v1*',
-    },
-    'subjetPt': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'subjetPt',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'charge',
         'return_type': 'float',
     },
-    'subjetEta': {
+    'passesIDCuts': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'subjetEta',
-        'return_type': 'float',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'passesIDCuts',
+        'return_type': 'bool',
     },
-    'subjetPhi': {
+    'passesHighPtCuts': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'subjetPhi',
-        'return_type': 'float',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'passesHighPtCuts',
+        'return_type': 'bool',
     },
-    'subjetE': {
+    'primaryTrackParticleLink': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'subjetE',
-        'return_type': 'float',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'primaryTrackParticleLink',
+        'return_type': 'const ElementLink<DataVector<xAOD::TrackParticle_v1>>',
     },
-    'nSubjets': {
+    'primaryTrackParticle': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'nSubjets',
-        'return_type': 'float',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'primaryTrackParticle',
+        'return_type': 'const xAOD::TrackParticle_v1*',
     },
-    'fCore': {
+    'inDetTrackParticleLink': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'fCore',
-        'return_type': 'float',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'inDetTrackParticleLink',
+        'return_type': 'const ElementLink<DataVector<xAOD::TrackParticle_v1>>',
     },
-    'vertexLink': {
+    'muonSpectrometerTrackParticleLink': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'vertexLink',
-        'return_type': 'const ElementLink<DataVector<xAOD::Vertex_v1>>',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'muonSpectrometerTrackParticleLink',
+        'return_type': 'const ElementLink<DataVector<xAOD::TrackParticle_v1>>',
     },
-    'vertex': {
+    'combinedTrackParticleLink': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'vertex',
-        'return_type': 'const xAOD::Vertex_v1*',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'combinedTrackParticleLink',
+        'return_type': 'const ElementLink<DataVector<xAOD::TrackParticle_v1>>',
     },
-    'trackLinks': {
+    'extrapolatedMuonSpectrometerTrackParticleLink': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'trackLinks',
-        'return_type_element': 'ElementLink<DataVector<xAOD::TrackParticle_v1>>',
-        'return_type_collection': 'const vector<ElementLink<DataVector<xAOD::TrackParticle_v1>>>',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'extrapolatedMuonSpectrometerTrackParticleLink',
+        'return_type': 'const ElementLink<DataVector<xAOD::TrackParticle_v1>>',
     },
-    'track': {
+    'msOnlyExtrapolatedMuonSpectrometerTrackParticleLink': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'track',
-        'return_type': 'const xAOD::TrackParticle_v1*',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'msOnlyExtrapolatedMuonSpectrometerTrackParticleLink',
+        'return_type': 'const ElementLink<DataVector<xAOD::TrackParticle_v1>>',
     },
-    'nTracks': {
+    'clusterLink': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'nTracks',
-        'return_type': 'int',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'clusterLink',
+        'return_type': 'const ElementLink<DataVector<xAOD::CaloCluster_v1>>',
     },
-    'otherTrackLinks': {
+    'cluster': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'otherTrackLinks',
-        'return_type_element': 'ElementLink<DataVector<xAOD::TrackParticle_v1>>',
-        'return_type_collection': 'const vector<ElementLink<DataVector<xAOD::TrackParticle_v1>>>',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'cluster',
+        'return_type': 'const xAOD::CaloCluster_v1*',
     },
-    'otherTrack': {
+    'muonSegmentLinks': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'otherTrack',
-        'return_type': 'const xAOD::TrackParticle_v1*',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'muonSegmentLinks',
+        'return_type_element': 'ElementLink<DataVector<xAOD::MuonSegment_v1>>',
+        'return_type_collection': 'const vector<ElementLink<DataVector<xAOD::MuonSegment_v1>>>',
     },
-    'nOtherTracks': {
+    'nMuonSegments': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'nOtherTracks',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'nMuonSegments',
         'return_type': 'int',
     },
-    'isoTrackLinks': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'isoTrackLinks',
-        'return_type_element': 'ElementLink<DataVector<xAOD::TrackParticle_v1>>',
-        'return_type_collection': 'const vector<ElementLink<DataVector<xAOD::TrackParticle_v1>>>',
-    },
-    'isoTrack': {
+    'muonSegment': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'isoTrack',
-        'return_type': 'const xAOD::TrackParticle_v1*',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'muonSegment',
+        'return_type': 'const xAOD::MuonSegment_v1*',
     },
-    'nIsoTracks': {
+    'muonSegmentLink': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
-        'method_name': 'nIsoTracks',
-        'return_type': 'int',
+        'type_string': 'xAOD::Muon_v1',
+        'method_name': 'muonSegmentLink',
+        'return_type': 'const ElementLink<DataVector<xAOD::MuonSegment_v1>>',
     },
     'index': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
+        'type_string': 'xAOD::Muon_v1',
         'method_name': 'index',
         'return_type': 'int',
     },
     'usingPrivateStore': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
+        'type_string': 'xAOD::Muon_v1',
         'method_name': 'usingPrivateStore',
         'return_type': 'bool',
     },
     'usingStandaloneStore': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
+        'type_string': 'xAOD::Muon_v1',
         'method_name': 'usingStandaloneStore',
         'return_type': 'bool',
     },
     'hasStore': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
+        'type_string': 'xAOD::Muon_v1',
         'method_name': 'hasStore',
         'return_type': 'bool',
     },
     'hasNonConstStore': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
+        'type_string': 'xAOD::Muon_v1',
         'method_name': 'hasNonConstStore',
         'return_type': 'bool',
     },
     'clearDecorations': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
+        'type_string': 'xAOD::Muon_v1',
         'method_name': 'clearDecorations',
         'return_type': 'bool',
     },
     'auxdataConst': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
+        'type_string': 'xAOD::Muon_v1',
         'method_name': 'auxdataConst',
         'return_type': 'U',
     },
     'isAvailable': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::DiTauJet_v1',
+        'type_string': 'xAOD::Muon_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
-            'name': 'xAODTau/versions/DiTauJet_v1.h',
-            'body_includes': ["xAODTau/versions/DiTauJet_v1.h"],
+            'name': 'xAODMuon/versions/Muon_v1.h',
+            'body_includes': ["xAODMuon/versions/Muon_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class DiTauJet_v1:
+class Muon_v1:
     "A class"
 
-
     def pt(self) -> float:
         "A method"
         ...
 
     def eta(self) -> float:
         "A method"
         ...
 
     def phi(self) -> float:
         "A method"
         ...
 
-    def e(self) -> float:
+    def m(self) -> float:
         "A method"
         ...
 
-    def m(self) -> float:
+    def e(self) -> float:
         "A method"
         ...
 
     def rapidity(self) -> float:
         "A method"
         ...
 
     def p4(self) -> func_adl_servicex_xaodr21.tlorentzvector.TLorentzVector:
         "A method"
         ...
 
-    def jetLink(self) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_jet_v1__.ElementLink_DataVector_xAOD_Jet_v1__:
-        "A method"
-        ...
-
-    def jet(self) -> func_adl_servicex_xaodr21.xAOD.jet_v1.Jet_v1:
-        "A method"
-        ...
-
-    def subjetPt(self, numSubjet: int) -> float:
-        "A method"
-        ...
-
-    def subjetEta(self, numSubjet: int) -> float:
+    def charge(self) -> float:
         "A method"
         ...
 
-    def subjetPhi(self, numSubjet: int) -> float:
+    def passesIDCuts(self) -> bool:
         "A method"
         ...
 
-    def subjetE(self, numSubjet: int) -> float:
+    def passesHighPtCuts(self) -> bool:
         "A method"
         ...
 
-    def nSubjets(self) -> float:
+    def primaryTrackParticleLink(self) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_trackparticle_v1__.ElementLink_DataVector_xAOD_TrackParticle_v1__:
         "A method"
         ...
 
-    def fCore(self, numSubjet: int) -> float:
+    def primaryTrackParticle(self) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
         "A method"
         ...
 
-    def vertexLink(self) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_vertex_v1__.ElementLink_DataVector_xAOD_Vertex_v1__:
+    def inDetTrackParticleLink(self) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_trackparticle_v1__.ElementLink_DataVector_xAOD_TrackParticle_v1__:
         "A method"
         ...
 
-    def vertex(self) -> func_adl_servicex_xaodr21.xAOD.vertex_v1.Vertex_v1:
+    def muonSpectrometerTrackParticleLink(self) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_trackparticle_v1__.ElementLink_DataVector_xAOD_TrackParticle_v1__:
         "A method"
         ...
 
-    def trackLinks(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_trackparticle_v1___.vector_ElementLink_DataVector_xAOD_TrackParticle_v1___:
+    def combinedTrackParticleLink(self) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_trackparticle_v1__.ElementLink_DataVector_xAOD_TrackParticle_v1__:
         "A method"
         ...
 
-    def track(self, i: int) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
+    def extrapolatedMuonSpectrometerTrackParticleLink(self) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_trackparticle_v1__.ElementLink_DataVector_xAOD_TrackParticle_v1__:
         "A method"
         ...
 
-    def nTracks(self) -> int:
+    def msOnlyExtrapolatedMuonSpectrometerTrackParticleLink(self) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_trackparticle_v1__.ElementLink_DataVector_xAOD_TrackParticle_v1__:
         "A method"
         ...
 
-    def otherTrackLinks(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_trackparticle_v1___.vector_ElementLink_DataVector_xAOD_TrackParticle_v1___:
+    def clusterLink(self) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_calocluster_v1__.ElementLink_DataVector_xAOD_CaloCluster_v1__:
         "A method"
         ...
 
-    def otherTrack(self, i: int) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
+    def cluster(self) -> func_adl_servicex_xaodr21.xAOD.calocluster_v1.CaloCluster_v1:
         "A method"
         ...
 
-    def nOtherTracks(self) -> int:
+    def muonSegmentLinks(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_muonsegment_v1___.vector_ElementLink_DataVector_xAOD_MuonSegment_v1___:
         "A method"
         ...
 
-    def isoTrackLinks(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_trackparticle_v1___.vector_ElementLink_DataVector_xAOD_TrackParticle_v1___:
+    def nMuonSegments(self) -> int:
         "A method"
         ...
 
-    def isoTrack(self, i: int) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
+    def muonSegment(self, i: int) -> func_adl_servicex_xaodr21.xAOD.muonsegment_v1.MuonSegment_v1:
         "A method"
         ...
 
-    def nIsoTracks(self) -> int:
+    def muonSegmentLink(self, i: int) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_muonsegment_v1__.ElementLink_DataVector_xAOD_MuonSegment_v1__:
         "A method"
         ...
 
     def index(self) -> int:
         "A method"
         ...
 
@@ -370,16 +332,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/egamma_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/egamma_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'pt': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::Egamma_v1',
         'method_name': 'pt',
@@ -143,16 +142,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::Egamma_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -160,26 +157,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODEgamma/versions/Egamma_v1.h',
             'body_includes': ["xAODEgamma/versions/Egamma_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class Egamma_v1:
     "A class"
 
-
     def pt(self) -> float:
         "A method"
         ...
 
     def eta(self) -> float:
         "A method"
         ...
@@ -228,15 +222,15 @@
         "A method"
         ...
 
     def OQ(self) -> int:
         "A method"
         ...
 
-    def likelihoodValue(self, value: float, LHValue: func_adl_servicex_xaodr21.str.str) -> bool:
+    def likelihoodValue(self, value: float, LHValue: str) -> bool:
         "A method"
         ...
 
     def index(self) -> int:
         "A method"
         ...
 
@@ -258,16 +252,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/electron_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/electron_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'charge': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::Electron_v1',
         'method_name': 'charge',
@@ -174,16 +173,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::Electron_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -191,26 +188,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODEgamma/versions/Electron_v1.h',
             'body_includes': ["xAODEgamma/versions/Electron_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class Electron_v1:
     "A class"
 
-
     def charge(self) -> float:
         "A method"
         ...
 
     def nTrackParticles(self) -> int:
         "A method"
         ...
@@ -279,15 +273,15 @@
         "A method"
         ...
 
     def OQ(self) -> int:
         "A method"
         ...
 
-    def likelihoodValue(self, value: float, LHValue: func_adl_servicex_xaodr21.str.str) -> bool:
+    def likelihoodValue(self, value: float, LHValue: str) -> bool:
         "A method"
         ...
 
     def index(self) -> int:
         "A method"
         ...
 
@@ -309,16 +303,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/eventinfo_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/eventinfo_v1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'runNumber': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::EventInfo_v1',
         'method_name': 'runNumber',
@@ -99,20 +98,14 @@
     },
     'eventTypeBitmask': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::EventInfo_v1',
         'method_name': 'eventTypeBitmask',
         'return_type': 'unsigned int',
     },
-    'eventType': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::EventInfo_v1',
-        'method_name': 'eventType',
-        'return_type': 'bool',
-    },
     'statusElement': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::EventInfo_v1',
         'method_name': 'statusElement',
         'return_type': 'unsigned int',
     },
     'extendedLevel1ID': {
@@ -143,50 +136,14 @@
     'subEvents': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::EventInfo_v1',
         'method_name': 'subEvents',
         'return_type_element': 'xAOD::EventInfo_v1::SubEvent',
         'return_type_collection': 'const vector<xAOD::EventInfo_v1::SubEvent>',
     },
-    'eventFlags': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::EventInfo_v1',
-        'method_name': 'eventFlags',
-        'return_type': 'unsigned int',
-    },
-    'isEventFlagBitSet': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::EventInfo_v1',
-        'method_name': 'isEventFlagBitSet',
-        'return_type': 'bool',
-    },
-    'setEventFlags': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::EventInfo_v1',
-        'method_name': 'setEventFlags',
-        'return_type': 'bool',
-    },
-    'setEventFlagBit': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::EventInfo_v1',
-        'method_name': 'setEventFlagBit',
-        'return_type': 'bool',
-    },
-    'errorState': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::EventInfo_v1',
-        'method_name': 'errorState',
-        'return_type': 'xAOD::EventInfo_v1::EventFlagErrorState',
-    },
-    'setErrorState': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::EventInfo_v1',
-        'method_name': 'setErrorState',
-        'return_type': 'bool',
-    },
     'beamPosX': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::EventInfo_v1',
         'method_name': 'beamPosX',
         'return_type': 'float',
     },
     'beamPosY': {
@@ -289,16 +246,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::EventInfo_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -306,92 +261,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODEventInfo/versions/EventInfo_v1.h',
             'body_includes': ["xAODEventInfo/versions/EventInfo_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class EventInfo_v1:
     "A class"
 
-    class EventType(Enum):
-        IS_SIMULATION = 1
-        IS_TESTBEAM = 2
-        IS_CALIBRATION = 4
-
-    class PileUpType(Enum):
-        Unknown = 99
-        Signal = 0
-        MinimumBias = 1
-        Cavern = 2
-        HaloGas = 3
-        ZeroBias = 4
-
-    class EventFlagSubDet(Enum):
-        Pixel = 0
-        SCT = 1
-        TRT = 2
-        LAr = 3
-        Tile = 4
-        Muon = 5
-        ForwardDet = 6
-        Core = 7
-        Background = 8
-        Lumi = 9
-        nDets = 10
-
-    class EventFlagErrorState(Enum):
-        NotSet = 0
-        Warning = 1
-        Error = 2
-
-    class BackgroundEventFlag(Enum):
-        MBTSTimeDiffHalo = 0
-        MBTSTimeDiffCol = 1
-        LArECTimeDiffHalo = 2
-        LArECTimeDiffCol = 3
-        PixMultiplicityHuge = 4
-        PixSPNonEmpty = 5
-        SCTMultiplicityHuge = 6
-        SCTSPNonEmpty = 7
-        CSCTimeDiffHalo = 8
-        CSCTimeDiffCol = 9
-        BCMTimeDiffHalo = 10
-        BCMTimeDiffCol = 11
-        MuonTimingCol = 12
-        MuonTimingCosmic = 13
-        MBTSBeamVeto = 14
-        BCMBeamVeto = 15
-        LUCIDBeamVeto = 16
-        HaloMuonSegment = 17
-        HaloClusterShape = 18
-        HaloMuonOneSided = 19
-        HaloMuonTwoSided = 20
-        HaloTileClusterPattern = 21
-        BeamGasPixel = 22
-        CosmicStandAlone = 23
-        CosmicStandAloneTight = 24
-        CosmicCombined = 25
-        CosmicCombinedTight = 26
-        BkgdResvBit1 = 27
-        BkgdResvBit2 = 28
-        BkgdResvBit3 = 29
-        BkgdResvBit4 = 30
-        BkgdResvBit5 = 31
-        NBackgroundWords = 32
-
-
     def runNumber(self) -> int:
         "A method"
         ...
 
     def eventNumber(self) -> int:
         "A method"
         ...
@@ -448,18 +334,14 @@
         "A method"
         ...
 
     def eventTypeBitmask(self) -> int:
         "A method"
         ...
 
-    def eventType(self, type: func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventType) -> bool:
-        "A method"
-        ...
-
     def statusElement(self) -> int:
         "A method"
         ...
 
     def extendedLevel1ID(self) -> int:
         "A method"
         ...
@@ -476,38 +358,14 @@
         "A method"
         ...
 
     def subEvents(self) -> func_adl_servicex_xaodr21.vector_xaod_eventinfo_v1_subevent_.vector_xAOD_EventInfo_v1_SubEvent_:
         "A method"
         ...
 
-    def eventFlags(self, subDet: func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventFlagSubDet) -> int:
-        "A method"
-        ...
-
-    def isEventFlagBitSet(self, subDet: func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventFlagSubDet, bit: int) -> bool:
-        "A method"
-        ...
-
-    def setEventFlags(self, subDet: func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventFlagSubDet, flags: int) -> bool:
-        "A method"
-        ...
-
-    def setEventFlagBit(self, subDet: func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventFlagSubDet, bit: int, set: bool) -> bool:
-        "A method"
-        ...
-
-    def errorState(self, subDet: func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventFlagSubDet) -> func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventFlagErrorState:
-        "A method"
-        ...
-
-    def setErrorState(self, subDet: func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventFlagSubDet, state: func_adl_servicex_xaodr21.xAOD.eventinfo_v1.EventInfo_v1.EventFlagErrorState) -> bool:
-        "A method"
-        ...
-
     def beamPosX(self) -> float:
         "A method"
         ...
 
     def beamPosY(self) -> float:
         "A method"
         ...
@@ -566,16 +424,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/iparticle.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/iparticle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'pt': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::IParticle',
         'method_name': 'pt',
@@ -94,16 +93,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::IParticle',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -111,26 +108,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODBase/IParticle.h',
             'body_includes': ["xAODBase/IParticle.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class IParticle:
     "A class"
 
-
     def pt(self) -> float:
         "A method"
         ...
 
     def eta(self) -> float:
         "A method"
         ...
@@ -177,16 +171,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/jet_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/jet_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'pt': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::Jet_v1',
         'method_name': 'pt',
@@ -106,26 +105,14 @@
     },
     'getSizeParameter': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::Jet_v1',
         'method_name': 'getSizeParameter',
         'return_type': 'float',
     },
-    'getAlgorithmType': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::Jet_v1',
-        'method_name': 'getAlgorithmType',
-        'return_type': 'xAOD::JetAlgorithmType::ID',
-    },
-    'getInputType': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::Jet_v1',
-        'method_name': 'getInputType',
-        'return_type': 'xAOD::JetInput::Type',
-    },
     'index': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::Jet_v1',
         'method_name': 'index',
         'return_type': 'int',
     },
     'usingPrivateStore': {
@@ -174,16 +161,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::Jet_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -191,26 +176,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODJet/versions/Jet_v1.h',
             'body_includes': ["xAODJet/versions/Jet_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class Jet_v1:
     "A class"
 
-
     def pt(self) -> float:
         "A method"
         ...
 
     def eta(self) -> float:
         "A method"
         ...
@@ -271,22 +253,14 @@
         "A method"
         ...
 
     def getSizeParameter(self) -> float:
         "A method"
         ...
 
-    def getAlgorithmType(self) -> func_adl_servicex_xaodr21.xAOD.jetalgorithmtype.JetAlgorithmType.ID:
-        "A method"
-        ...
-
-    def getInputType(self) -> func_adl_servicex_xaodr21.xAOD.jetinput.JetInput.Type:
-        "A method"
-        ...
-
     def index(self) -> int:
         "A method"
         ...
 
     def usingPrivateStore(self) -> bool:
         "A method"
         ...
@@ -305,22 +279,22 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('getAttribute', s, a, param_1))
     @property
-    def getAttribute(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def getAttribute(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/jetalgorithmtype.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/ROOT/Fit/datarange.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
-    'algName': {
+    'NDim': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::JetAlgorithmType',
-        'method_name': 'algName',
-        'return_type_element': '__gnu_cxx::__normal_iterator<char*,string>',
-        'return_type_collection': 'const string',
+        'type_string': 'ROOT::Fit::DataRange',
+        'method_name': 'NDim',
+        'return_type': 'unsigned int',
     },
-    'algId': {
+    'Size': {
         'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::JetAlgorithmType',
-        'method_name': 'algId',
-        'return_type': 'xAOD::JetAlgorithmType::ID',
+        'type_string': 'ROOT::Fit::DataRange',
+        'method_name': 'Size',
+        'return_type': 'unsigned int',
+    },
+    'IsSet': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'ROOT::Fit::DataRange',
+        'method_name': 'IsSet',
+        'return_type': 'bool',
+    },
+    'IsInside': {
+        'metadata_type': 'add_method_type_info',
+        'type_string': 'ROOT::Fit::DataRange',
+        'method_name': 'IsInside',
+        'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
-class JetAlgorithmType:
+class DataRange:
     "A class"
 
-    class ID(Enum):
-        kt_algorithm = 0
-        cambridge_algorithm = 1
-        antikt_algorithm = 2
-        genkt_algorithm = 3
-        cambridge_for_passive_algorithm = 11
-        genkt_for_passive_algorithm = 13
-        ee_kt_algorithm = 50
-        ee_genkt_algorithm = 53
-        plugin_algorithm = 99
-        undefined_jet_algorithm = 999
+    def NDim(self) -> int:
+        "A method"
+        ...
 
+    def Size(self, icoord: int) -> int:
+        "A method"
+        ...
 
-    def algName(self, id: func_adl_servicex_xaodr21.xAOD.jetalgorithmtype.JetAlgorithmType.ID) -> func_adl_servicex_xaodr21.str.str:
+    def IsSet(self) -> bool:
         "A method"
         ...
 
-    def algId(self, n: func_adl_servicex_xaodr21.str.str) -> func_adl_servicex_xaodr21.xAOD.jetalgorithmtype.JetAlgorithmType.ID:
+    def IsInside(self, x: float, icoord: int) -> bool:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/jetconstituent.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/jetconstituent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'pt': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::JetConstituent',
         'method_name': 'pt',
@@ -58,38 +57,33 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::JetConstituent',
         'method_name': 'isSpacelike',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class JetConstituent:
     "A class"
 
-
     def pt(self) -> float:
         "A method"
         ...
 
     def eta(self) -> float:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/jetconstituentvector.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/jetconstituentvector.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'isValid': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::JetConstituentVector',
         'method_name': 'isValid',
@@ -47,38 +46,33 @@
         'type_string': 'xAOD::JetConstituentVector',
         'method_name': 'asSTLVector',
         'return_type_element': 'xAOD::JetConstituent',
         'return_type_collection': 'vector<xAOD::JetConstituent>',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class JetConstituentVector(Iterable[func_adl_servicex_xaodr21.xAOD.jetconstituent.JetConstituent]):
     "A class"
 
-
     def isValid(self) -> bool:
         "A method"
         ...
 
     def empty(self) -> bool:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/missinget_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/missinget_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'mpx': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::MissingET_v1',
         'method_name': 'mpx',
@@ -95,16 +94,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::MissingET_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -112,26 +109,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODMissingET/versions/MissingET_v1.h',
             'body_includes': ["xAODMissingET/versions/MissingET_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class MissingET_v1:
     "A class"
 
-
     def mpx(self) -> float:
         "A method"
         ...
 
     def mpy(self) -> float:
         "A method"
         ...
@@ -178,16 +172,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/muonsegment_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/muonsegment_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'x': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::MuonSegment_v1',
         'method_name': 'x',
@@ -68,32 +67,20 @@
     },
     'sector': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::MuonSegment_v1',
         'method_name': 'sector',
         'return_type': 'int',
     },
-    'chamberIndex': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::MuonSegment_v1',
-        'method_name': 'chamberIndex',
-        'return_type': 'Muon::MuonStationIndex::ChIndex',
-    },
     'etaIndex': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::MuonSegment_v1',
         'method_name': 'etaIndex',
         'return_type': 'int',
     },
-    'technology': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::MuonSegment_v1',
-        'method_name': 'technology',
-        'return_type': 'Muon::MuonStationIndex::TechnologyIndex',
-    },
     'nPrecisionHits': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::MuonSegment_v1',
         'method_name': 'nPrecisionHits',
         'return_type': 'int',
     },
     'nPhiLayers': {
@@ -154,16 +141,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::MuonSegment_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -171,26 +156,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODMuon/versions/MuonSegment_v1.h',
             'body_includes': ["xAODMuon/versions/MuonSegment_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class MuonSegment_v1:
     "A class"
 
-
     def x(self) -> float:
         "A method"
         ...
 
     def y(self) -> float:
         "A method"
         ...
@@ -227,26 +209,18 @@
         "A method"
         ...
 
     def sector(self) -> int:
         "A method"
         ...
 
-    def chamberIndex(self) -> func_adl_servicex_xaodr21.Muon.muonstationindex.MuonStationIndex.ChIndex:
-        "A method"
-        ...
-
     def etaIndex(self) -> int:
         "A method"
         ...
 
-    def technology(self) -> func_adl_servicex_xaodr21.Muon.muonstationindex.MuonStationIndex.TechnologyIndex:
-        "A method"
-        ...
-
     def nPrecisionHits(self) -> int:
         "A method"
         ...
 
     def nPhiLayers(self) -> int:
         "A method"
         ...
@@ -277,16 +251,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/neutralparticle_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/neutralparticle_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'pt': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::NeutralParticle_v1',
         'method_name': 'pt',
@@ -149,16 +148,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::NeutralParticle_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -166,26 +163,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODTracking/versions/NeutralParticle_v1.h',
             'body_includes': ["xAODTracking/versions/NeutralParticle_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class NeutralParticle_v1:
     "A class"
 
-
     def pt(self) -> float:
         "A method"
         ...
 
     def eta(self) -> float:
         "A method"
         ...
@@ -268,16 +262,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/pfo_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/pfo_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'pt': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::PFO_v1',
         'method_name': 'pt',
@@ -104,20 +103,14 @@
     },
     'charge': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::PFO_v1',
         'method_name': 'charge',
         'return_type': 'float',
     },
-    'getClusterMoment': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::PFO_v1',
-        'method_name': 'getClusterMoment',
-        'return_type': 'bool',
-    },
     'cluster': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::PFO_v1',
         'method_name': 'cluster',
         'return_type': 'const xAOD::CaloCluster_v1*',
     },
     'track': {
@@ -214,16 +207,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::PFO_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -231,26 +222,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODPFlow/versions/PFO_v1.h',
             'body_includes': ["xAODPFlow/versions/PFO_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class PFO_v1:
     "A class"
 
-
     def pt(self) -> float:
         "A method"
         ...
 
     def eta(self) -> float:
         "A method"
         ...
@@ -311,51 +299,47 @@
         "A method"
         ...
 
     def charge(self) -> float:
         "A method"
         ...
 
-    def getClusterMoment(self, theMoment: float, momentType: func_adl_servicex_xaodr21.xAOD.calocluster_v1.CaloCluster_v1.MomentType) -> bool:
-        "A method"
-        ...
-
     def cluster(self, index: int) -> func_adl_servicex_xaodr21.xAOD.calocluster_v1.CaloCluster_v1:
         "A method"
         ...
 
     def track(self, index: int) -> func_adl_servicex_xaodr21.xAOD.trackparticle_v1.TrackParticle_v1:
         "A method"
         ...
 
     def vertex(self) -> func_adl_servicex_xaodr21.xAOD.vertex_v1.Vertex_v1:
         "A method"
         ...
 
-    def setVertexLink(self, theVertexLink: func_adl_servicex_xaodr21.elementlink_datavector_xaod_vertex_v1__.ElementLink_DataVector_xAOD_Vertex_v1__) -> bool:
+    def setVertexLink(self, theVertexLink: ElementLink_DataVector_xAOD_Vertex_v1__) -> bool:
         "A method"
         ...
 
-    def setTrackLink(self, theTrack: func_adl_servicex_xaodr21.elementlink_datavector_xaod_trackparticle_v1__.ElementLink_DataVector_xAOD_TrackParticle_v1__) -> bool:
+    def setTrackLink(self, theTrack: ElementLink_DataVector_xAOD_TrackParticle_v1__) -> bool:
         "A method"
         ...
 
-    def setClusterLink(self, theCluster: func_adl_servicex_xaodr21.elementlink_datavector_xaod_calocluster_v1__.ElementLink_DataVector_xAOD_CaloCluster_v1__) -> bool:
+    def setClusterLink(self, theCluster: ElementLink_DataVector_xAOD_CaloCluster_v1__) -> bool:
         "A method"
         ...
 
-    def addClusterLink(self, theCluster: func_adl_servicex_xaodr21.elementlink_datavector_xaod_calocluster_v1__.ElementLink_DataVector_xAOD_CaloCluster_v1__) -> bool:
+    def addClusterLink(self, theCluster: ElementLink_DataVector_xAOD_CaloCluster_v1__) -> bool:
         "A method"
         ...
 
-    def GetVertexCorrectedFourVec(self, vertexToCorrectTo: func_adl_servicex_xaodr21.xAOD.vertex_v1.Vertex_v1) -> func_adl_servicex_xaodr21.tlorentzvector.TLorentzVector:
+    def GetVertexCorrectedFourVec(self, vertexToCorrectTo: Vertex_v1) -> func_adl_servicex_xaodr21.tlorentzvector.TLorentzVector:
         "A method"
         ...
 
-    def GetVertexCorrectedEMFourVec(self, vertexToCorrectTo: func_adl_servicex_xaodr21.xAOD.vertex_v1.Vertex_v1) -> func_adl_servicex_xaodr21.tlorentzvector.TLorentzVector:
+    def GetVertexCorrectedEMFourVec(self, vertexToCorrectTo: Vertex_v1) -> func_adl_servicex_xaodr21.tlorentzvector.TLorentzVector:
         "A method"
         ...
 
     def index(self) -> int:
         "A method"
         ...
 
@@ -377,16 +361,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/photon_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/photon_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'vertex': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::Photon_v1',
         'method_name': 'vertex',
@@ -174,16 +173,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::Photon_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -191,26 +188,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODEgamma/versions/Photon_v1.h',
             'body_includes': ["xAODEgamma/versions/Photon_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class Photon_v1:
     "A class"
 
-
     def vertex(self, index: int) -> func_adl_servicex_xaodr21.xAOD.vertex_v1.Vertex_v1:
         "A method"
         ...
 
     def vertexLink(self, index: int) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_vertex_v1__.ElementLink_DataVector_xAOD_Vertex_v1__:
         "A method"
         ...
@@ -279,15 +273,15 @@
         "A method"
         ...
 
     def OQ(self) -> int:
         "A method"
         ...
 
-    def likelihoodValue(self, value: float, LHValue: func_adl_servicex_xaodr21.str.str) -> bool:
+    def likelihoodValue(self, value: float, LHValue: str) -> bool:
         "A method"
         ...
 
     def index(self) -> int:
         "A method"
         ...
 
@@ -309,16 +303,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/slowmuon_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/slowmuon_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'beta': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::SlowMuon_v1',
         'method_name': 'beta',
@@ -178,16 +177,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::SlowMuon_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -195,26 +192,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODMuon/versions/SlowMuon_v1.h',
             'body_includes': ["xAODMuon/versions/SlowMuon_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class SlowMuon_v1:
     "A class"
 
-
     def beta(self) -> float:
         "A method"
         ...
 
     def betaT(self) -> float:
         "A method"
         ...
@@ -317,16 +311,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/taujet_v3.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/taujet_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'pt': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TauJet_v3',
         'method_name': 'pt',
@@ -372,20 +371,14 @@
     },
     'cluster': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TauJet_v3',
         'method_name': 'cluster',
         'return_type': 'const xAOD::IParticle*',
     },
-    'calibratedCluster': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::TauJet_v3',
-        'method_name': 'calibratedCluster',
-        'return_type': 'TLorentzVector',
-    },
     'nClusters': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TauJet_v3',
         'method_name': 'nClusters',
         'return_type': 'int',
     },
     'pi0Links': {
@@ -623,16 +616,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TauJet_v3',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -640,26 +631,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODTau/versions/TauJet_v3.h',
             'body_includes': ["xAODTau/versions/TauJet_v3.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class TauJet_v3:
     "A class"
 
-
     def pt(self) -> float:
         "A method"
         ...
 
     def eta(self) -> float:
         "A method"
         ...
@@ -896,18 +884,14 @@
         "A method"
         ...
 
     def cluster(self, i: int) -> func_adl_servicex_xaodr21.xAOD.iparticle.IParticle:
         "A method"
         ...
 
-    def calibratedCluster(self, i: int, state: func_adl_servicex_xaodr21.xAOD.calocluster_v1.CaloCluster_v1.State) -> func_adl_servicex_xaodr21.tlorentzvector.TLorentzVector:
-        "A method"
-        ...
-
     def nClusters(self) -> int:
         "A method"
         ...
 
     def pi0Links(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_iparticle___.vector_ElementLink_DataVector_xAOD_IParticle___:
         "A method"
         ...
@@ -1050,16 +1034,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/tautrack_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/tautrack_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'pt': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TauTrack_v1',
         'method_name': 'pt',
@@ -156,16 +155,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TauTrack_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -173,26 +170,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODTau/versions/TauTrack_v1.h',
             'body_includes': ["xAODTau/versions/TauTrack_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class TauTrack_v1:
     "A class"
 
-
     def pt(self) -> float:
         "A method"
         ...
 
     def eta(self) -> float:
         "A method"
         ...
@@ -217,27 +211,27 @@
         "A method"
         ...
 
     def flagWithMask(self, noname_arg: int) -> bool:
         "A method"
         ...
 
-    def z0sinThetaTJVA(self, noname_arg: func_adl_servicex_xaodr21.xAOD.iparticle.IParticle) -> float:
+    def z0sinThetaTJVA(self, noname_arg: IParticle) -> float:
         "A method"
         ...
 
-    def rConv(self, noname_arg: func_adl_servicex_xaodr21.xAOD.iparticle.IParticle) -> float:
+    def rConv(self, noname_arg: IParticle) -> float:
         "A method"
         ...
 
-    def rConvII(self, noname_arg: func_adl_servicex_xaodr21.xAOD.iparticle.IParticle) -> float:
+    def rConvII(self, noname_arg: IParticle) -> float:
         "A method"
         ...
 
-    def dRJetSeedAxis(self, noname_arg: func_adl_servicex_xaodr21.xAOD.iparticle.IParticle) -> float:
+    def dRJetSeedAxis(self, noname_arg: IParticle) -> float:
         "A method"
         ...
 
     def bdtScores(self) -> func_adl_servicex_xaodr21.vector_float_.vector_float_:
         "A method"
         ...
 
@@ -279,16 +273,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/trackcalocluster_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/trackcalocluster_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'pt': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TrackCaloCluster_v1',
         'method_name': 'pt',
@@ -119,16 +118,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TrackCaloCluster_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -136,31 +133,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODPFlow/versions/TrackCaloCluster_v1.h',
             'body_includes': ["xAODPFlow/versions/TrackCaloCluster_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class TrackCaloCluster_v1:
     "A class"
 
-    class Taste(Enum):
-        Charged = 0
-        Neutral = 1
-        Combined = 2
-
-
     def pt(self) -> float:
         "A method"
         ...
 
     def eta(self) -> float:
         "A method"
         ...
@@ -223,16 +212,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/trackparticle_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/trackparticle_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'pt': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TrackParticle_v1',
         'method_name': 'pt',
@@ -245,16 +244,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TrackParticle_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -262,26 +259,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODTracking/versions/TrackParticle_v1.h',
             'body_includes': ["xAODTracking/versions/TrackParticle_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class TrackParticle_v1:
     "A class"
 
-
     def pt(self) -> float:
         "A method"
         ...
 
     def eta(self) -> float:
         "A method"
         ...
@@ -428,16 +422,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/truthevent_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/truthevent_v1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'weights': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TruthEvent_v1',
         'method_name': 'weights',
@@ -21,44 +20,20 @@
     },
     'crossSectionError': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TruthEvent_v1',
         'method_name': 'crossSectionError',
         'return_type': 'float',
     },
-    'pdfInfoParameter': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::TruthEvent_v1',
-        'method_name': 'pdfInfoParameter',
-        'return_type': 'bool',
-    },
-    'setPdfInfoParameter': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::TruthEvent_v1',
-        'method_name': 'setPdfInfoParameter',
-        'return_type': 'bool',
-    },
     'pdfInfo': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TruthEvent_v1',
         'method_name': 'pdfInfo',
         'return_type': 'xAOD::TruthEvent_v1::PdfInfo',
     },
-    'heavyIonParameter': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::TruthEvent_v1',
-        'method_name': 'heavyIonParameter',
-        'return_type': 'bool',
-    },
-    'setHeavyIonParameter': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::TruthEvent_v1',
-        'method_name': 'setHeavyIonParameter',
-        'return_type': 'bool',
-    },
     'signalProcessVertex': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TruthEvent_v1',
         'method_name': 'signalProcessVertex',
         'return_type': 'const xAOD::TruthVertex_v1*',
     },
     'signalProcessVertexLink': {
@@ -175,16 +150,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TruthEvent_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -192,88 +165,39 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODTruth/versions/TruthEvent_v1.h',
             'body_includes': ["xAODTruth/versions/TruthEvent_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class TruthEvent_v1:
     "A class"
 
-    class PdfParam(Enum):
-        PDGID1 = 0
-        PDGID2 = 1
-        PDFID1 = 2
-        PDFID2 = 3
-        X1 = 4
-        X2 = 5
-        SCALE = 6
-        Q = 6
-        PDF1 = 7
-        PDF2 = 8
-        XF1 = 7
-        XF2 = 8
-
-    class HIParam(Enum):
-        NCOLLHARD = 0
-        NPARTPROJ = 1
-        NPARTTARG = 2
-        NCOLL = 3
-        SPECTATORNEUTRONS = 4
-        SPECTATORPROTONS = 5
-        NNWOUNDEDCOLLISIONS = 6
-        NWOUNDEDNCOLLISIONS = 7
-        NWOUNDEDNWOUNDEDCOLLISIONS = 8
-        IMPACTPARAMETER = 9
-        EVENTPLANEANGLE = 10
-        ECCENTRICITY = 11
-        SIGMAINELNN = 12
-        CENTRALITY = 13
-
-
     def weights(self) -> func_adl_servicex_xaodr21.vector_float_.vector_float_:
         "A method"
         ...
 
     def crossSection(self) -> float:
         "A method"
         ...
 
     def crossSectionError(self) -> float:
         "A method"
         ...
 
-    def pdfInfoParameter(self, value: int, parameter: func_adl_servicex_xaodr21.xAOD.truthevent_v1.TruthEvent_v1.PdfParam) -> bool:
-        "A method"
-        ...
-
-    def setPdfInfoParameter(self, value: int, parameter: func_adl_servicex_xaodr21.xAOD.truthevent_v1.TruthEvent_v1.PdfParam) -> bool:
-        "A method"
-        ...
-
     def pdfInfo(self) -> func_adl_servicex_xaodr21.xAOD.TruthEvent_v1.pdfinfo.PdfInfo:
         "A method"
         ...
 
-    def heavyIonParameter(self, value: int, parameter: func_adl_servicex_xaodr21.xAOD.truthevent_v1.TruthEvent_v1.HIParam) -> bool:
-        "A method"
-        ...
-
-    def setHeavyIonParameter(self, value: int, parameter: func_adl_servicex_xaodr21.xAOD.truthevent_v1.TruthEvent_v1.HIParam) -> bool:
-        "A method"
-        ...
-
     def signalProcessVertex(self) -> func_adl_servicex_xaodr21.xAOD.truthvertex_v1.TruthVertex_v1:
         "A method"
         ...
 
     def signalProcessVertexLink(self) -> func_adl_servicex_xaodr21.elementlink_datavector_xaod_truthvertex_v1__.ElementLink_DataVector_xAOD_TruthVertex_v1__:
         "A method"
         ...
@@ -340,16 +264,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/trutheventbase_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/trutheventbase_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'truthParticleLinks': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TruthEventBase_v1',
         'method_name': 'truthParticleLinks',
@@ -102,16 +101,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TruthEventBase_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -119,26 +116,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODTruth/versions/TruthEventBase_v1.h',
             'body_includes': ["xAODTruth/versions/TruthEventBase_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class TruthEventBase_v1:
     "A class"
 
-
     def truthParticleLinks(self) -> func_adl_servicex_xaodr21.vector_elementlink_datavector_xaod_truthparticle_v1___.vector_ElementLink_DataVector_xAOD_TruthParticle_v1___:
         "A method"
         ...
 
     def nTruthParticles(self) -> int:
         "A method"
         ...
@@ -189,16 +183,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/truthmetadata_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/truthmetadata_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'mcChannelNumber': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TruthMetaData_v1',
         'method_name': 'mcChannelNumber',
@@ -107,16 +106,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TruthMetaData_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -124,26 +121,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODTruth/versions/TruthMetaData_v1.h',
             'body_includes': ["xAODTruth/versions/TruthMetaData_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class TruthMetaData_v1:
     "A class"
 
-
     def mcChannelNumber(self) -> int:
         "A method"
         ...
 
     def weightNames(self) -> func_adl_servicex_xaodr21.vector_str_.vector_str_:
         "A method"
         ...
@@ -194,16 +188,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/truthparticle_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/truthparticle_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'pdgId': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TruthParticle_v1',
         'method_name': 'pdgId',
@@ -404,26 +403,14 @@
     },
     'isBSM': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TruthParticle_v1',
         'method_name': 'isBSM',
         'return_type': 'bool',
     },
-    'polarizationParameter': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::TruthParticle_v1',
-        'method_name': 'polarizationParameter',
-        'return_type': 'bool',
-    },
-    'setPolarizationParameter': {
-        'metadata_type': 'add_method_type_info',
-        'type_string': 'xAOD::TruthParticle_v1',
-        'method_name': 'setPolarizationParameter',
-        'return_type': 'bool',
-    },
     'polarization': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TruthParticle_v1',
         'method_name': 'polarization',
         'return_type': 'xAOD::TruthParticle_v1::Polarization',
     },
     'index': {
@@ -472,16 +459,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TruthParticle_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -489,30 +474,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODTruth/versions/TruthParticle_v1.h',
             'body_includes': ["xAODTruth/versions/TruthParticle_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class TruthParticle_v1:
     "A class"
 
-    class PolParam(Enum):
-        polarizationPhi = 0
-        polarizationTheta = 1
-
-
     def pdgId(self) -> int:
         "A method"
         ...
 
     def absPdgId(self) -> int:
         "A method"
         ...
@@ -773,22 +751,14 @@
         "A method"
         ...
 
     def isBSM(self) -> bool:
         "A method"
         ...
 
-    def polarizationParameter(self, value: float, parameter: func_adl_servicex_xaodr21.xAOD.truthparticle_v1.TruthParticle_v1.PolParam) -> bool:
-        "A method"
-        ...
-
-    def setPolarizationParameter(self, value: float, parameter: func_adl_servicex_xaodr21.xAOD.truthparticle_v1.TruthParticle_v1.PolParam) -> bool:
-        "A method"
-        ...
-
     def polarization(self) -> func_adl_servicex_xaodr21.xAOD.TruthParticle_v1.polarization.Polarization:
         "A method"
         ...
 
     def index(self) -> int:
         "A method"
         ...
@@ -811,16 +781,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/truthvertex_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/truthvertex_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'id': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TruthVertex_v1',
         'method_name': 'id',
@@ -150,16 +149,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::TruthVertex_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -167,26 +164,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODTruth/versions/TruthVertex_v1.h',
             'body_includes': ["xAODTruth/versions/TruthVertex_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class TruthVertex_v1:
     "A class"
 
-
     def id(self) -> int:
         "A method"
         ...
 
     def barcode(self) -> int:
         "A method"
         ...
@@ -269,16 +263,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/func_adl_servicex_xaodr21/xAOD/vertex_v1.py` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/func_adl_servicex_xaodr21/xAOD/vertex_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import ast
 from typing import Tuple, TypeVar, Iterable
 from func_adl import ObjectStream, func_adl_callback, func_adl_parameterized_call
-from enum import Enum
 import func_adl_servicex_xaodr21
 
 _method_map = {
     'x': {
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::Vertex_v1',
         'method_name': 'x',
@@ -153,16 +152,14 @@
         'metadata_type': 'add_method_type_info',
         'type_string': 'xAOD::Vertex_v1',
         'method_name': 'isAvailable',
         'return_type': 'bool',
     },
 }
 
-_enum_map = {      
-}
 
 T = TypeVar('T')
 
 
 def _add_method_metadata(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     '''Add metadata for a collection to the func_adl stream if we know about it
     '''
@@ -170,26 +167,23 @@
     if a.func.attr in _method_map:
         s_update = s.MetaData(_method_map[a.func.attr])
         s_update = s_update.MetaData({
             'metadata_type': 'inject_code',
             'name': 'xAODTracking/versions/Vertex_v1.h',
             'body_includes': ["xAODTracking/versions/Vertex_v1.h"],
         })
-        for md in _enum_map.get(a.func.attr, []):
-            s_update = s_update.MetaData(md)
         return s_update, a
     else:
         return s, a
 
 
 @func_adl_callback(_add_method_metadata)
 class Vertex_v1:
     "A class"
 
-
     def x(self) -> float:
         "A method"
         ...
 
     def y(self) -> float:
         "A method"
         ...
@@ -272,16 +266,16 @@
 
     def clearDecorations(self) -> bool:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('auxdataConst', s, a, param_1))
     @property
-    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def auxdataConst(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
 
     @func_adl_parameterized_call(lambda s, a, param_1: func_adl_servicex_xaodr21.type_support.cpp_generic_1arg_callback('isAvailable', s, a, param_1))
     @property
-    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[func_adl_servicex_xaodr21.str.str]:
+    def isAvailable(self) -> func_adl_servicex_xaodr21.type_support.index_type_forwarder[str]:
         "A method"
         ...
```

### Comparing `func_adl_servicex_xaodr21-2.0.0.21.2.231a11/PKG-INFO` & `func_adl_servicex_xaodr21-2.0.0.21.2.231a9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 Metadata-Version: 2.1
 Name: func_adl_servicex_xaodr21
-Version: 2.0.0.21.2.231a11
+Version: 2.0.0.21.2.231a9
 Summary: func-adl typed datasets for Servicex for xAOD R21 21.2.231
 Author: Gordon Watts
 Author-email: gwatts@uw.edu
-Requires-Python: >=3.8
+Requires-Python: >=3.7,<3.11
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: func_adl_servicex (>=2.0-beta.1,<3.0)
 Description-Content-Type: text/markdown
 
 # func_adl_servicex_xaodr21
 
 This package contains the types and metadata for xAOD R21 21.2.231.
 
 It was generated by the [`func_adl_servicex_type_generator`](https://github.com/gordonwatts/func_adl_servicex_type_generator) package.
 
 For examples on how to use this, please see the [jupyter-book](https://gordonwatts.github.io/xaod_usage).
 
-## Installation
-
-If you want to use `func_adl_servicex` and the older verison of the servicex frontend, make sure to install `func_adl_servicex` in addition.
-
-If you want to use the new 3.0 `servicex` frontend, just install that.
-
```

