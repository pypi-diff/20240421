# Comparing `tmp/rttm_manager-0.1.7-py3-none-any.whl.zip` & `tmp/rttm_manager-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1869 bytes, number of entries: 7
--rw-r--r--  2.0 unx      110 b- defN 20-Feb-02 00:00 rttm_manager/__init__.py
--rw-r--r--  2.0 unx      285 b- defN 20-Feb-02 00:00 rttm_manager/entity/rttm.py
--rw-r--r--  2.0 unx        1 b- defN 20-Feb-02 00:00 rttm_manager/service/exporter.py
--rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 rttm_manager/service/importer.py
-?rw-r--r--  2.0 unx      296 b- defN 20-Feb-02 00:00 rttm_manager-0.1.7.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 rttm_manager-0.1.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx      555 b- defN 20-Feb-02 00:00 rttm_manager-0.1.7.dist-info/RECORD
-7 files, 1334 bytes uncompressed, 873 bytes compressed:  34.6%
+Zip file size: 3231 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      357 b- defN 20-Feb-02 00:00 rttm_manager/__init__.py
+-rw-r--r--  2.0 unx      404 b- defN 20-Feb-02 00:00 rttm_manager/entity/rttm.py
+-rw-r--r--  2.0 unx     1204 b- defN 20-Feb-02 00:00 rttm_manager/service/exporter.py
+-rw-r--r--  2.0 unx     1095 b- defN 20-Feb-02 00:00 rttm_manager/service/importer.py
+?rw-r--r--  2.0 unx     1107 b- defN 20-Feb-02 00:00 rttm_manager-0.1.8.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 rttm_manager-0.1.8.dist-info/WHEEL
+?rw-r--r--  2.0 unx      562 b- defN 20-Feb-02 00:00 rttm_manager-0.1.8.dist-info/RECORD
+7 files, 4816 bytes uncompressed, 2235 bytes compressed:  53.6%
```

## zipnote {}

```diff
@@ -6,17 +6,17 @@
 
 Filename: rttm_manager/service/exporter.py
 Comment: 
 
 Filename: rttm_manager/service/importer.py
 Comment: 
 
-Filename: rttm_manager-0.1.7.dist-info/METADATA
+Filename: rttm_manager-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: rttm_manager-0.1.7.dist-info/WHEEL
+Filename: rttm_manager-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: rttm_manager-0.1.7.dist-info/RECORD
+Filename: rttm_manager-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rttm_manager/__init__.py

```diff
@@ -1,6 +1,11 @@
-def import_rttm() -> str:
-    return "Imported rttm!"
+from rttm_manager.entity.rttm import RTTM
+from rttm_manager.service.importer import RTTMImporter
+from rttm_manager.service.exporter import RTTMExporter
 
 
-def export_rttm() -> str:
-    return "Exported rttm!"
+def import_rttm(file_path: str) -> list[RTTM]:
+    return RTTMImporter.rttm_import(file_path)
+
+
+def export_rttm(rttms: list[RTTM], file_path: str) -> None:
+    RTTMExporter.rttm_export(rttms, file_path)
```

## rttm_manager/entity/rttm.py

```diff
@@ -1,15 +1,15 @@
-from dataclasses import dataclass
+from typing import Union
+from pydantic import BaseModel
 
 
-@dataclass
-class RTTM:
+class RTTM(BaseModel, frozen=True):
     type: str
     file_id: str
     channel_id: int
     turn_onset: float
     turn_duration: float
-    orthography_field: str
-    speaker_type: str
     speaker_name: str
-    confidence_score: str
-    signal_lookahead_time: str
+    orthography_field: Union[str, None] = None
+    speaker_type: Union[str, None] = None
+    confidence_score: Union[float, None] = None
+    signal_lookahead_time: Union[float, None] = None
```

## rttm_manager/service/exporter.py

```diff
@@ -1 +1,76 @@
-00000000: 0a                                       .
+00000000: 6672 6f6d 2072 7474 6d5f 6d61 6e61 6765  from rttm_manage
+00000010: 722e 656e 7469 7479 2e72 7474 6d20 696d  r.entity.rttm im
+00000020: 706f 7274 2052 5454 4d0a 6672 6f6d 2070  port RTTM.from p
+00000030: 6174 686c 6962 2069 6d70 6f72 7420 5061  athlib import Pa
+00000040: 7468 0a0a 0a63 6c61 7373 2052 5454 4d45  th...class RTTME
+00000050: 7870 6f72 7465 723a 0a0a 2020 2020 4073  xporter:..    @s
+00000060: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+00000070: 6465 6620 5f67 656e 6572 6174 655f 7274  def _generate_rt
+00000080: 746d 5f6c 696e 6528 7274 746d 3a20 5254  tm_line(rttm: RT
+00000090: 544d 293a 0a20 2020 2020 2020 206c 696e  TM):.        lin
+000000a0: 6520 3d20 5b0a 2020 2020 2020 2020 2020  e = [.          
+000000b0: 2020 7274 746d 2e74 7970 652c 0a20 2020    rttm.type,.   
+000000c0: 2020 2020 2020 2020 2072 7474 6d2e 6669           rttm.fi
+000000d0: 6c65 5f69 642c 0a20 2020 2020 2020 2020  le_id,.         
+000000e0: 2020 2066 227b 7274 746d 2e63 6861 6e6e     f"{rttm.chann
+000000f0: 656c 5f69 647d 222c 0a20 2020 2020 2020  el_id}",.       
+00000100: 2020 2020 2066 227b 7274 746d 2e74 7572       f"{rttm.tur
+00000110: 6e5f 6f6e 7365 743a 2e32 667d 222c 0a20  n_onset:.2f}",. 
+00000120: 2020 2020 2020 2020 2020 2066 227b 7274             f"{rt
+00000130: 746d 2e74 7572 6e5f 6475 7261 7469 6f6e  tm.turn_duration
+00000140: 3a2e 3266 7d22 2c0a 2020 2020 2020 2020  :.2f}",.        
+00000150: 2020 2020 7274 746d 2e6f 7274 686f 6772      rttm.orthogr
+00000160: 6170 6879 5f66 6965 6c64 2069 6620 7274  aphy_field if rt
+00000170: 746d 2e6f 7274 686f 6772 6170 6879 5f66  tm.orthography_f
+00000180: 6965 6c64 2069 7320 6e6f 7420 4e6f 6e65  ield is not None
+00000190: 2065 6c73 6520 223c 4e41 3e22 2c0a 2020   else "<NA>",.  
+000001a0: 2020 2020 2020 2020 2020 7274 746d 2e73            rttm.s
+000001b0: 7065 616b 6572 5f74 7970 6520 6966 2072  peaker_type if r
+000001c0: 7474 6d2e 7370 6561 6b65 725f 7479 7065  ttm.speaker_type
+000001d0: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
+000001e0: 6520 223c 4e41 3e22 2c0a 2020 2020 2020  e "<NA>",.      
+000001f0: 2020 2020 2020 7274 746d 2e73 7065 616b        rttm.speak
+00000200: 6572 5f6e 616d 652c 0a20 2020 2020 2020  er_name,.       
+00000210: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
+00000220: 2020 2020 2020 2066 227b 7274 746d 2e63         f"{rttm.c
+00000230: 6f6e 6669 6465 6e63 655f 7363 6f72 653a  onfidence_score:
+00000240: 2e32 667d 220a 2020 2020 2020 2020 2020  .2f}".          
+00000250: 2020 2020 2020 6966 2072 7474 6d2e 636f        if rttm.co
+00000260: 6e66 6964 656e 6365 5f73 636f 7265 2069  nfidence_score i
+00000270: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
+00000280: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
+00000290: 223c 4e41 3e22 0a20 2020 2020 2020 2020  "<NA>".         
+000002a0: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
+000002b0: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
+000002c0: 2020 2020 6622 7b72 7474 6d2e 7369 676e      f"{rttm.sign
+000002d0: 616c 5f6c 6f6f 6b61 6865 6164 5f74 696d  al_lookahead_tim
+000002e0: 653a 2e32 667d 220a 2020 2020 2020 2020  e:.2f}".        
+000002f0: 2020 2020 2020 2020 6966 2072 7474 6d2e          if rttm.
+00000300: 7369 676e 616c 5f6c 6f6f 6b61 6865 6164  signal_lookahead
+00000310: 5f74 696d 6520 6973 206e 6f74 204e 6f6e  _time is not Non
+00000320: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00000330: 2020 656c 7365 2022 3c4e 413e 220a 2020    else "<NA>".  
+00000340: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+00000350: 2020 2020 205d 0a20 2020 2020 2020 2072       ].        r
+00000360: 6574 7572 6e20 2220 222e 6a6f 696e 286c  eturn " ".join(l
+00000370: 696e 6529 202b 2022 5c6e 220a 0a20 2020  ine) + "\n"..   
+00000380: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
+00000390: 2020 2064 6566 2072 7474 6d5f 6578 706f     def rttm_expo
+000003a0: 7274 2872 7474 6d73 3a20 6c69 7374 5b52  rt(rttms: list[R
+000003b0: 5454 4d5d 2c20 6669 6c65 5f6e 616d 653a  TTM], file_name:
+000003c0: 2073 7472 2920 2d3e 204e 6f6e 653a 0a20   str) -> None:. 
+000003d0: 2020 2020 2020 2066 696c 655f 7061 7468         file_path
+000003e0: 203d 2050 6174 6828 6669 6c65 5f6e 616d   = Path(file_nam
+000003f0: 6529 0a20 2020 2020 2020 2061 7373 6572  e).        asser
+00000400: 7420 6973 696e 7374 616e 6365 2872 7474  t isinstance(rtt
+00000410: 6d73 2c20 6c69 7374 290a 0a20 2020 2020  ms, list)..     
+00000420: 2020 206c 696e 6573 203d 205b 5254 544d     lines = [RTTM
+00000430: 4578 706f 7274 6572 2e5f 6765 6e65 7261  Exporter._genera
+00000440: 7465 5f72 7474 6d5f 6c69 6e65 2872 7474  te_rttm_line(rtt
+00000450: 6d29 2066 6f72 2072 7474 6d20 696e 2072  m) for rttm in r
+00000460: 7474 6d73 5d0a 0a20 2020 2020 2020 2077  ttms]..        w
+00000470: 6974 6820 6f70 656e 2873 7472 2866 696c  ith open(str(fil
+00000480: 655f 7061 7468 292c 2022 7722 2920 6173  e_path), "w") as
+00000490: 2066 3a0a 2020 2020 2020 2020 2020 2020   f:.            
+000004a0: 662e 7772 6974 656c 696e 6573 286c 696e  f.writelines(lin
+000004b0: 6573 290a                                es).
```

## rttm_manager/service/importer.py

```diff
@@ -0,0 +1,69 @@
+00000000: 6672 6f6d 2072 7474 6d5f 6d61 6e61 6765  from rttm_manage
+00000010: 722e 656e 7469 7479 2e72 7474 6d20 696d  r.entity.rttm im
+00000020: 706f 7274 2052 5454 4d0a 6672 6f6d 2070  port RTTM.from p
+00000030: 6174 686c 6962 2069 6d70 6f72 7420 5061  athlib import Pa
+00000040: 7468 0a0a 0a63 6c61 7373 2052 5454 4d49  th...class RTTMI
+00000050: 6d70 6f72 7465 723a 0a0a 2020 2020 4073  mporter:..    @s
+00000060: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+00000070: 6465 6620 5f67 6574 5f72 7474 6d5f 6672  def _get_rttm_fr
+00000080: 6f6d 5f6c 696e 6528 6c69 6e65 3a20 7374  om_line(line: st
+00000090: 7229 202d 3e20 5254 544d 3a0a 2020 2020  r) -> RTTM:.    
+000000a0: 2020 2020 6c69 6e65 203d 206c 696e 652e      line = line.
+000000b0: 7273 7472 6970 2829 2020 2320 e694 b9e8  rstrip()  # ....
+000000c0: a18c e382 84e3 82b9 e383 9ae3 83bc e382  ................
+000000d0: b9e5 898a e999 a40a 2020 2020 2020 2020  ........        
+000000e0: 7661 6c75 6573 203d 206c 696e 652e 7370  values = line.sp
+000000f0: 6c69 7428 2220 2229 0a20 2020 2020 2020  lit(" ").       
+00000100: 2061 7373 6572 7420 6c65 6e28 7661 6c75   assert len(valu
+00000110: 6573 2920 3d3d 2031 300a 0a20 2020 2020  es) == 10..     
+00000120: 2020 2072 6574 7572 6e20 5254 544d 280a     return RTTM(.
+00000130: 2020 2020 2020 2020 2020 2020 7479 7065              type
+00000140: 3d76 616c 7565 735b 305d 2c0a 2020 2020  =values[0],.    
+00000150: 2020 2020 2020 2020 6669 6c65 5f69 643d          file_id=
+00000160: 7661 6c75 6573 5b31 5d2c 0a20 2020 2020  values[1],.     
+00000170: 2020 2020 2020 2063 6861 6e6e 656c 5f69         channel_i
+00000180: 643d 696e 7428 7661 6c75 6573 5b32 5d29  d=int(values[2])
+00000190: 2c0a 2020 2020 2020 2020 2020 2020 7475  ,.            tu
+000001a0: 726e 5f6f 6e73 6574 3d66 6c6f 6174 2876  rn_onset=float(v
+000001b0: 616c 7565 735b 335d 292c 0a20 2020 2020  alues[3]),.     
+000001c0: 2020 2020 2020 2074 7572 6e5f 6475 7261         turn_dura
+000001d0: 7469 6f6e 3d66 6c6f 6174 2876 616c 7565  tion=float(value
+000001e0: 735b 345d 292c 0a20 2020 2020 2020 2020  s[4]),.         
+000001f0: 2020 206f 7274 686f 6772 6170 6879 5f66     orthography_f
+00000200: 6965 6c64 3d4e 6f6e 6520 6966 2076 616c  ield=None if val
+00000210: 7565 735b 355d 203d 3d20 223c 4e41 3e22  ues[5] == "<NA>"
+00000220: 2065 6c73 6520 7661 6c75 6573 5b35 5d2c   else values[5],
+00000230: 0a20 2020 2020 2020 2020 2020 2073 7065  .            spe
+00000240: 616b 6572 5f74 7970 653d 4e6f 6e65 2069  aker_type=None i
+00000250: 6620 7661 6c75 6573 5b36 5d20 3d3d 2022  f values[6] == "
+00000260: 3c4e 413e 2220 656c 7365 2076 616c 7565  <NA>" else value
+00000270: 735b 365d 2c0a 2020 2020 2020 2020 2020  s[6],.          
+00000280: 2020 7370 6561 6b65 725f 6e61 6d65 3d76    speaker_name=v
+00000290: 616c 7565 735b 375d 2c0a 2020 2020 2020  alues[7],.      
+000002a0: 2020 2020 2020 636f 6e66 6964 656e 6365        confidence
+000002b0: 5f73 636f 7265 3d4e 6f6e 6520 6966 2076  _score=None if v
+000002c0: 616c 7565 735b 385d 203d 3d20 223c 4e41  alues[8] == "<NA
+000002d0: 3e22 2065 6c73 6520 666c 6f61 7428 7661  >" else float(va
+000002e0: 6c75 6573 5b38 5d29 2c0a 2020 2020 2020  lues[8]),.      
+000002f0: 2020 2020 2020 7369 676e 616c 5f6c 6f6f        signal_loo
+00000300: 6b61 6865 6164 5f74 696d 653d 4e6f 6e65  kahead_time=None
+00000310: 2069 6620 7661 6c75 6573 5b39 5d20 3d3d   if values[9] ==
+00000320: 2022 3c4e 413e 2220 656c 7365 2066 6c6f   "<NA>" else flo
+00000330: 6174 2876 616c 7565 735b 395d 292c 0a20  at(values[9]),. 
+00000340: 2020 2020 2020 2029 0a0a 2020 2020 4073         )..    @s
+00000350: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+00000360: 6465 6620 7274 746d 5f69 6d70 6f72 7428  def rttm_import(
+00000370: 6669 6c65 5f6e 616d 653a 2073 7472 2920  file_name: str) 
+00000380: 2d3e 206c 6973 745b 5254 544d 5d3a 0a20  -> list[RTTM]:. 
+00000390: 2020 2020 2020 2066 696c 655f 7061 7468         file_path
+000003a0: 203d 2050 6174 6828 6669 6c65 5f6e 616d   = Path(file_nam
+000003b0: 6529 0a20 2020 2020 2020 2077 6974 6820  e).        with 
+000003c0: 6f70 656e 2873 7472 2866 696c 655f 7061  open(str(file_pa
+000003d0: 7468 2929 2061 7320 663a 0a20 2020 2020  th)) as f:.     
+000003e0: 2020 2020 2020 206c 696e 6573 203d 2066         lines = f
+000003f0: 2e72 6561 646c 696e 6573 2829 0a20 2020  .readlines().   
+00000400: 2020 2020 2072 6574 7572 6e20 5b52 5454       return [RTT
+00000410: 4d49 6d70 6f72 7465 722e 5f67 6574 5f72  MImporter._get_r
+00000420: 7474 6d5f 6672 6f6d 5f6c 696e 6528 6c69  ttm_from_line(li
+00000430: 6e65 2920 666f 7220 6c69 6e65 2069 6e20  ne) for line in 
+00000440: 6c69 6e65 735d 0a                        lines].
```

