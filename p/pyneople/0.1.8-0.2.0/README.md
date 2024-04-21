# Comparing `tmp/pyneople-0.1.8.tar.gz` & `tmp/pyneople-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneople-0.1.8.tar", last modified: Fri Dec 22 06:37:03 2023, max compression
+gzip compressed data, was "pyneople-0.2.0.tar", last modified: Sun Apr 21 12:13:29 2024, max compression
```

## Comparing `pyneople-0.1.8.tar` & `pyneople-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 06:37:03.701588 pyneople-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-22 06:36:51.000000 pyneople-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      562 2023-12-22 06:37:03.701588 pyneople-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-22 06:36:51.000000 pyneople-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-22 06:36:51.000000 pyneople-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 06:37:03.701588 pyneople-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-12-22 06:36:51.000000 pyneople-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 06:37:03.701588 pyneople-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 06:37:03.701588 pyneople-0.1.8/src/pyneople/
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2023-12-22 06:36:51.000000 pyneople-0.1.8/src/pyneople/METADATA.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2023-12-22 06:36:51.000000 pyneople-0.1.8/src/pyneople/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2023-12-22 06:36:51.000000 pyneople-0.1.8/src/pyneople/avatars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2023-12-22 06:36:51.000000 pyneople-0.1.8/src/pyneople/buff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2023-12-22 06:36:51.000000 pyneople-0.1.8/src/pyneople/character_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2023-12-22 06:36:51.000000 pyneople-0.1.8/src/pyneople/equipments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2023-12-22 06:36:51.000000 pyneople-0.1.8/src/pyneople/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2023-12-22 06:36:51.000000 pyneople-0.1.8/src/pyneople/others.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2023-12-22 06:36:51.000000 pyneople-0.1.8/src/pyneople/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2023-12-22 06:36:51.000000 pyneople-0.1.8/src/pyneople/timeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 06:37:03.701588 pyneople-0.1.8/src/pyneople.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2023-12-22 06:37:03.000000 pyneople-0.1.8/src/pyneople.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-22 06:37:03.000000 pyneople-0.1.8/src/pyneople.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 06:37:03.000000 pyneople-0.1.8/src/pyneople.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-22 06:37:03.000000 pyneople-0.1.8/src/pyneople.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:13:29.731375 pyneople-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 12:13:14.000000 pyneople-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-21 12:13:29.731375 pyneople-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-21 12:13:14.000000 pyneople-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-21 12:13:14.000000 pyneople-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 12:13:29.731375 pyneople-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-21 12:13:14.000000 pyneople-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:13:29.727375 pyneople-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:13:29.731375 pyneople-0.2.0/src/pyneople/
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-04-21 12:13:14.000000 pyneople-0.2.0/src/pyneople/METADATA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-21 12:13:14.000000 pyneople-0.2.0/src/pyneople/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-21 12:13:14.000000 pyneople-0.2.0/src/pyneople/avatars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-21 12:13:14.000000 pyneople-0.2.0/src/pyneople/buff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33657 2024-04-21 12:13:14.000000 pyneople-0.2.0/src/pyneople/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-21 12:13:14.000000 pyneople-0.2.0/src/pyneople/character_fame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-21 12:13:14.000000 pyneople-0.2.0/src/pyneople/character_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-21 12:13:14.000000 pyneople-0.2.0/src/pyneople/character_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-04-21 12:13:14.000000 pyneople-0.2.0/src/pyneople/equipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-21 12:13:14.000000 pyneople-0.2.0/src/pyneople/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-21 12:13:14.000000 pyneople-0.2.0/src/pyneople/others.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-21 12:13:14.000000 pyneople-0.2.0/src/pyneople/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-21 12:13:14.000000 pyneople-0.2.0/src/pyneople/timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:13:29.731375 pyneople-0.2.0/src/pyneople.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-21 12:13:29.000000 pyneople-0.2.0/src/pyneople.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-21 12:13:29.000000 pyneople-0.2.0/src/pyneople.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 12:13:29.000000 pyneople-0.2.0/src/pyneople.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 12:13:29.000000 pyneople-0.2.0/src/pyneople.egg-info/top_level.txt
```

### Comparing `pyneople-0.1.8/LICENSE` & `pyneople-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneople-0.1.8/setup.py` & `pyneople-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyneople",
-    version="0.1.8",
+    version="0.2.0",
     author="ippo252525",
     author_email="ippo252525@gmail.com",
     description="Neople Open API wrapper for data analyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ippo252525/pyneople",
     project_urls={
```

### Comparing `pyneople-0.1.8/src/pyneople/avatars.py` & `pyneople-0.2.0/src/pyneople/avatars.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,54 @@
-from .functions import get_request, one_slot
-from .METADATA import AVATAR_LIST
+from .functions import get_request
+from .METADATA import AVATAR_LIST, PLATINUM_AVATAR_LIST
 
 class Avatar():
     def __init__(self):
         self.item_name = None
         self.item_rarity = None
         self.option_ability = None
         self.emblem_1 = None
         self.emblem_2 = None
-        self.emblem_3 = None        
-    def get_avatar_data(self, arg_avatar_dict):
-        
-        try:
-            self.item_name = arg_avatar_dict["itemName"]
-            self.item_rarity = arg_avatar_dict["itemRarity"]
-        except:
-            pass    
         
-        try:
-            self.option_ability = arg_avatar_dict["optionAbility"]
-        except:
-            pass
-        
-        try:    
-            for index, emblem in enumerate(arg_avatar_dict['emblems']):
-                exec(f"self.emblem_{index+1} = '{emblem['itemName']}'")
-        except:
-            pass        
+    def get_avatar_data(self, arg_avatar_dict):
+        self.item_name = arg_avatar_dict.get("itemName")
+        self.item_rarity = arg_avatar_dict.get("itemRarity")
+        self.option_ability = arg_avatar_dict.get("optionAbility")
+        for i, emblem in enumerate(arg_avatar_dict.get('emblems', dict())):
+            setattr(self, f'emblem_{i+1}', emblem.get('itemName'))
 
+class PlatinumAvatar(Avatar):
+    def __init__(self):
+        super().__init__()
+        self.emblem_3 = None
+    def get_avatar_data(self, arg_avatar_dict):
+        super().get_avatar_data(arg_avatar_dict)
 
 class Avatars():
     def __init__(self, arg_api_key):
         """
         클래스 생성 시 Neople Open API key를 입력받는다
             Args :
                 arg_api_key(str) : Neople Open API key
         """        
-        self.__api_key = arg_api_key  
-        for avatar in AVATAR_LIST:
-            exec(f"self.{avatar} = Avatar()")  
+        self.__api_key = arg_api_key
+        # for avatar in AVATAR_LIST:
+        #     exec(f"self.{avatar} = Avatar()")  
 
     def get_data(self, arg_server_id, arg_character_id):    
         url = f'https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/avatar?apikey={self.__api_key}'
-        data = get_request(url)
-        data = data['avatar'] 
-        for avatar in AVATAR_LIST:
-            try:
-                exec(f"self.{avatar}.get_avatar_data(one_slot(data, '{avatar}'.upper()))")
-            except:
-                pass    
+        return get_request(url)
+
+    def parse_data(self, arg_data):
+        if arg_data.get('avatar'):
+            arg_data = arg_data['avatar'] 
+            for avatar in arg_data:
+                if avatar["slotId"].lower() in PLATINUM_AVATAR_LIST:
+                    avatar_data = PlatinumAvatar()    
+                else:
+                    avatar_data = Avatar()
+                avatar_data.get_avatar_data(avatar)
+                setattr(self, f'{avatar["slotId"].lower()}', avatar_data)
+
+                #exec(f"self.{avatar}.get_avatar_data(one_slot(data, '{avatar}'.upper()))")
+            # except:
+            #     pass
```

### Comparing `pyneople-0.1.8/src/pyneople/character_search.py` & `pyneople-0.2.0/src/pyneople/character_information.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,33 @@
-import urllib.parse
 from .functions import get_request
-from .METADATA import SERVER_NAME_2_ID
+from .METADATA import CHARACTER_INFORMATION_NAME
 
-class CharacterSearch():
+class CharacterInformation():
     
     def __init__(self, arg_api_key : str):
         """
         클래스 생성 시 Neople Open API key를 입력받는다
             Args :
                 arg_api_key(str) : Neople Open API key
         """        
         self.__api_key = arg_api_key
     
-    def get_data(self, arg_server_name : str, arg_character_name : str):
+    def get_data(self, arg_server_id : str, arg_character_id : str):
         """
-        서버명과 캐릭터 이름을 검색하면 기본 정보를 반환
+        영문 서버명과 캐릭터 ID 를 검색하면 기본 정보를 반환
             Args : 
-                arg_server_name(str) : 서버 이름 ex) 디레지에
+                arg_server_name(str) : 서버 이름  ex) diregie
                 
-                arg_character_name(str) : 캐릭터 이름 ex) 홍길동
-        """
+                arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
+        """    
+        url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}?apikey={self.__api_key}"
 
-        # 한글 서버명을 영문 서버명으로 변환
-        arg_server_name = SERVER_NAME_2_ID[arg_server_name]
-        
-        url = f"https://api.neople.co.kr/df/servers/{arg_server_name}/characters?characterName={urllib.parse.quote(arg_character_name)}&limit=1&apikey={self.__api_key}"
-        return get_request(url)
+        return get_request(url)        
     
-    def parse_data(self, arg_data):
+    def parse_data(self, arg_data, variable_list = CHARACTER_INFORMATION_NAME.keys()):
         """
         가져온 데이터를 정리해서 하위 attribute에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
         """
-        arg_data = arg_data['rows'][0]
-
-        self.server_id = arg_data.get('serverId')
-        self.character_name = arg_data.get('characterName')
-        self.character_id = arg_data.get('characterId')
-        self.job_name = arg_data.get('jobName')
-        self.job_grow_name = arg_data.get('jobGrowName')
-        self.level = arg_data.get('level')
+        for attribute_name in variable_list:
+            setattr(self, attribute_name, arg_data.get(CHARACTER_INFORMATION_NAME[attribute_name]))
```

### Comparing `pyneople-0.1.8/src/pyneople/functions.py` & `pyneople-0.2.0/src/pyneople/functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,56 +16,49 @@
             
             arg_time_sleep(float) : 한 번의 요청 후 쉬는 시간
     """
     global SETTINGS
     SETTINGS['request_time_out'] = arg_time_out
     SETTINGS['request_time_sleep'] = arg_time_sleep
 
-def get_request(arg_url):
+def get_request(arg_url : str):
     """
     url 입력시 data 가져오는 함수
-    arg_url : 원하는 url 주소
+        Args :
+            arg_url(str) : 원하는 url 주소
     """
-
-    # request.get 실패 할 경우 에러 발생시킴
-    #try:
+    start_time = time.time()
     data = requests.get(arg_url, timeout = SETTINGS['request_time_out'])
-    # except:
-    #    raise Exception("해당 url주소는 사용할 수 없습니다")    
-    
-    # 성공한다면 api 규칙에 따라 지정한 시간을 멈춘다
-    time.sleep(SETTINGS['request_time_sleep'])
-
-    # 데이터 저장
     data = json.loads(data.text)
-
-    # # request.get은 성공 했으나 받아온 데이터가 Open API 에서 error로 규정된 경우 에러 발생시킴
-    # if list(data.keys())[0] == 'error':  
-    #     raise Exception(f"apikey혹은 url에 문제가 있습니다. 코드를 확인해주세요. error : {data}")
-    # else:    
+    # Neople Open API 상에서 규정된 에러가 발생할 경우 에러를 발생시킨다.
+    if data.get("error"):
+        raise Exception(data.get("error"))
+    elapsed_time = time.time() - start_time
+    if elapsed_time < SETTINGS['request_time_sleep']:
+        time.sleep(SETTINGS['request_time_sleep'] - elapsed_time)
     return data
-    
 
-def _next(arg_dict, arg_list):
+def _next(arg_dict : dict, arg_list : list):
     """
     get_job_info 함수를 위해 쓰이는 함수
     """
     if 'next' in arg_dict.keys():
         arg_list.append(arg_dict["jobGrowName"])
         return _next(arg_dict['next'], arg_list)
     else :
         arg_list.append(arg_dict["jobGrowName"])
         return arg_dict["jobGrowName"]
 
 
-def get_job_info(arg_api_key):
+def get_job_info(arg_api_key : str):
     """
     직업 정보를 받아오는 함수
     전직명(각성명)을 1차 전직명으로 통일시키는 jobname_equalize 함수에 매개변수로 사용되는 객체를 반환함
-    arg_api_key : Neople Open API key
+        Args :
+            arg_api_key(str) : Neople Open API key
     """
     data = get_request(f"https://api.neople.co.kr/df/jobs?apikey={arg_api_key}")
     job_list = []
     jobGroW_total_list = []
     for job in data['rows']:
         job_list.append(job['jobName'])
         jobGroW_list = []
@@ -114,19 +107,21 @@
     except:
         return False    
     if (list(data.keys())[0] == 'error') and (data['error']['status'] == 503): 
         return True
     else:
         return False
 
-def explain_enchant(arg_enchant_dict):
+def explain_enchant(arg_enchant_dict : dict):
     """
     마법부여 정보를 정리해주는 함수
+        Args :
+            arg_enchant_dict(dict) : 마법부여 정보 dict
     """
-    if arg_enchant_dict == {}:
+    if arg_enchant_dict == {} or arg_enchant_dict == None:
         return None
     output = ""
     if "status" in arg_enchant_dict.keys():
         output = ", ".join([f"{s['name']} {s['value']}" for s in arg_enchant_dict['status']])
     if "reinforceSkill" in arg_enchant_dict.keys():
         output = ", ".join([f"{s['name']} {s['value']}" for r in arg_enchant_dict['reinforceSkill'] for s in r['skills']]) + ", " + output 
     if "explain" in arg_enchant_dict.keys():
@@ -190,23 +185,23 @@
     """
     객체를 입력받으면 모든 하위속성의 값을 list로 반환한다
     """
     arg_object = get_values(arg_object)
     arg_object = flatten(arg_object)
     return arg_object
 
-def one_slot(arg_equipment_list : list, arg_slot_name : str):
-    """
-    해당 부위의 정보만 반환하는 함수
-        Args:
-            arg_equipment_list(list) : 캐릭터 장비 데이터(dict)로 이루어진 list
+# def one_slot(arg_equipment_list : list, arg_slot_name : str):
+#     """
+#     해당 부위의 정보만 반환하는 함수
+#         Args:
+#             arg_equipment_list(list) : 캐릭터 장비 데이터(dict)로 이루어진 list
             
-            arg_slot_name(str) : 해당 장비의 이름
-        Returns:
-            해당 장비의 dict            
-    """
-    if arg_equipment_list == []:
-        return None
-    for equipment in arg_equipment_list:
-        if equipment['slotId'] == arg_slot_name :
-            return equipment
-    return None
+#             arg_slot_name(str) : 해당 장비의 이름
+#         Returns:
+#             해당 장비의 dict            
+#     """
+#     if arg_equipment_list == []:
+#         return None
+#     for equipment in arg_equipment_list:
+#         if equipment['slotId'] == arg_slot_name :
+#             return equipment
+#     return None
```

### Comparing `pyneople-0.1.8/src/pyneople/timeline.py` & `pyneople-0.2.0/src/pyneople/timeline.py`

 * *Files identical despite different names*

