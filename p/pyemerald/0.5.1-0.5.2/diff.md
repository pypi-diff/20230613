# Comparing `tmp/pyemerald-0.5.1.tar.gz` & `tmp/pyemerald-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyemerald-0.5.1.tar", max compression
+gzip compressed data, was "pyemerald-0.5.2.tar", max compression
```

## Comparing `pyemerald-0.5.1.tar` & `pyemerald-0.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1046 2023-05-24 15:11:53.898358 pyemerald-0.5.1/LICENSE.txt
--rw-r--r--   0        0        0     1928 2023-05-26 09:18:23.811297 pyemerald-0.5.1/README.md
--rw-r--r--   0        0        0        0 2023-05-06 11:52:31.804082 pyemerald-0.5.1/pyemerald/__init__.py
--rw-r--r--   0        0        0    12667 2023-05-26 09:18:23.811297 pyemerald-0.5.1/pyemerald/codec.py
--rw-r--r--   0        0        0      660 2023-05-28 17:50:30.794623 pyemerald-0.5.1/pyemerald/constants.py
--rw-r--r--   0        0        0     1798 2023-05-28 13:55:20.016336 pyemerald-0.5.1/pyemerald/game.py
--rw-r--r--   0        0        0     9108 2023-05-26 09:18:23.811297 pyemerald-0.5.1/pyemerald/items.py
--rw-r--r--   0        0        0     3045 2023-05-28 13:55:20.016336 pyemerald-0.5.1/pyemerald/level.py
--rw-r--r--   0        0        0    60162 2023-05-23 13:28:34.600939 pyemerald-0.5.1/pyemerald/moves.py
--rw-r--r--   0        0        0     3843 2023-05-26 09:18:23.811297 pyemerald-0.5.1/pyemerald/nature_stats.py
--rw-r--r--   0        0        0    36653 2023-05-28 13:55:20.016336 pyemerald-0.5.1/pyemerald/pokemon.py
--rw-r--r--   0        0        0    98431 2023-05-28 13:55:20.016336 pyemerald-0.5.1/pyemerald/pokemon_info.py
--rw-r--r--   0        0        0     4510 2023-05-23 13:28:34.600939 pyemerald-0.5.1/pyemerald/raw_section.py
--rw-r--r--   0        0        0     6425 2023-05-28 13:55:20.016336 pyemerald-0.5.1/pyemerald/save.py
--rw-r--r--   0        0        0     7141 2023-05-28 17:50:30.794623 pyemerald-0.5.1/pyemerald/section.py
--rw-r--r--   0        0        0     2497 2023-05-25 18:51:11.499441 pyemerald-0.5.1/pyemerald/utils.py
--rw-r--r--   0        0        0      531 2023-05-28 17:50:30.794623 pyemerald-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2568 2023-05-28 17:51:35.934300 pyemerald-0.5.1/setup.py
--rw-r--r--   0        0        0     2551 2023-05-28 17:51:35.934617 pyemerald-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1046 2023-05-24 15:11:53.898358 pyemerald-0.5.2/LICENSE.txt
+-rw-r--r--   0        0        0     1928 2023-05-26 09:18:23.811297 pyemerald-0.5.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 11:52:31.804082 pyemerald-0.5.2/pyemerald/__init__.py
+-rw-r--r--   0        0        0    12667 2023-05-26 09:18:23.811297 pyemerald-0.5.2/pyemerald/codec.py
+-rw-r--r--   0        0        0      660 2023-05-28 17:50:30.794623 pyemerald-0.5.2/pyemerald/constants.py
+-rw-r--r--   0        0        0     1798 2023-05-28 13:55:20.016336 pyemerald-0.5.2/pyemerald/game.py
+-rw-r--r--   0        0        0     9108 2023-05-26 09:18:23.811297 pyemerald-0.5.2/pyemerald/items.py
+-rw-r--r--   0        0        0     3045 2023-05-28 13:55:20.016336 pyemerald-0.5.2/pyemerald/level.py
+-rw-r--r--   0        0        0    60162 2023-05-23 13:28:34.600939 pyemerald-0.5.2/pyemerald/moves.py
+-rw-r--r--   0        0        0     3843 2023-05-26 09:18:23.811297 pyemerald-0.5.2/pyemerald/nature_stats.py
+-rw-r--r--   0        0        0    37122 2023-06-13 08:07:58.440873 pyemerald-0.5.2/pyemerald/pokemon.py
+-rw-r--r--   0        0        0    98431 2023-05-28 13:55:20.016336 pyemerald-0.5.2/pyemerald/pokemon_info.py
+-rw-r--r--   0        0        0     4510 2023-05-23 13:28:34.600939 pyemerald-0.5.2/pyemerald/raw_section.py
+-rw-r--r--   0        0        0     6425 2023-05-28 13:55:20.016336 pyemerald-0.5.2/pyemerald/save.py
+-rw-r--r--   0        0        0     7130 2023-06-13 08:07:58.440873 pyemerald-0.5.2/pyemerald/section.py
+-rw-r--r--   0        0        0     2497 2023-05-25 18:51:11.499441 pyemerald-0.5.2/pyemerald/utils.py
+-rw-r--r--   0        0        0      531 2023-06-13 08:07:58.440873 pyemerald-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2568 2023-06-13 08:08:23.223170 pyemerald-0.5.2/setup.py
+-rw-r--r--   0        0        0     2551 2023-06-13 08:08:23.223490 pyemerald-0.5.2/PKG-INFO
```

### Comparing `pyemerald-0.5.1/LICENSE.txt` & `pyemerald-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.1/README.md` & `pyemerald-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.1/pyemerald/codec.py` & `pyemerald-0.5.2/pyemerald/codec.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.1/pyemerald/constants.py` & `pyemerald-0.5.2/pyemerald/constants.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.1/pyemerald/game.py` & `pyemerald-0.5.2/pyemerald/game.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.1/pyemerald/items.py` & `pyemerald-0.5.2/pyemerald/items.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.1/pyemerald/level.py` & `pyemerald-0.5.2/pyemerald/level.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.1/pyemerald/moves.py` & `pyemerald-0.5.2/pyemerald/moves.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.1/pyemerald/nature_stats.py` & `pyemerald-0.5.2/pyemerald/nature_stats.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.1/pyemerald/pokemon.py` & `pyemerald-0.5.2/pyemerald/pokemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -583,26 +583,29 @@
         self.original_trainer_name = original_trainer_name
         self.markings = markings
         self.raw_checksum = checksum
         self.padding = padding
         self.pokemon_data = pokemon_data
 
     @classmethod
-    def from_bytes(cls, data: bytes):
-        poke_obj = cls._codec(cls).to_object(data)
-
-        # data property is extracted as bytes, call to the PokemonData
-        # to create itself from the bytes
-        poke_data = PokemonData.from_bytes(
-            poke_obj.pokemon_data,
-            poke_obj.personality_value,
-            poke_obj.original_trainer_id,
-        )
-        poke_obj.pokemon_data = poke_data
-        return poke_obj
+    def from_bytes(cls, data: bytes) -> Optional[Union["PCPokemon", "Pokemon"]]:
+        
+        if data[:8] != PCPokemon.null_pokemon():
+            poke_obj = cls._codec(cls).to_object(data)
+
+            # data property is extracted as bytes, call to the PokemonData
+            # to create itself from the bytes
+            poke_data = PokemonData.from_bytes(
+                poke_obj.pokemon_data,
+                poke_obj.personality_value,
+                poke_obj.original_trainer_id,
+            )
+            poke_obj.pokemon_data = poke_data
+            return poke_obj
+        return None
 
     @staticmethod
     def default_values(
         name: str,
         level: int,
         move_1: Move,
         move_2: Move,
@@ -933,14 +936,23 @@
             self.original_trainer_name == other.original_trainer_name,
             self.pokemon_data == other.pokemon_data,
         ]
 
         return all(checks)
 
 
+    @staticmethod
+    def null_pokemon():
+        # Seems to work when checking first 8 bytes
+        # This corresponds to personality value, 
+        # original trainer ID and nickname
+        # Checking that all bytes are x00 doesnt work
+        # as there can be xff in there
+        return 8 * b"\x00"
+
 class Pokemon(PCPokemon):
     """Pokemon class for Pokemon in the party"""
 
     _codec = PokemonCodec
 
     def __init__(
         self,
```

### Comparing `pyemerald-0.5.1/pyemerald/pokemon_info.py` & `pyemerald-0.5.2/pyemerald/pokemon_info.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.1/pyemerald/raw_section.py` & `pyemerald-0.5.2/pyemerald/raw_section.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.1/pyemerald/save.py` & `pyemerald-0.5.2/pyemerald/save.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.1/pyemerald/section.py` & `pyemerald-0.5.2/pyemerald/section.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,16 +123,17 @@
         # we need to create parse 6 * 100 bytes
         party = []
         for i in range(6):
             cur_pokemon_bytes = team.party[
                 BYTES_PER_PARTY_POKEMON * i : BYTES_PER_PARTY_POKEMON * (i + 1)
             ]
 
-            if cur_pokemon_bytes != TeamItemSection.null_pokemon():
-                party.append(Pokemon.from_bytes(cur_pokemon_bytes))
+            pokemon = Pokemon.from_bytes(cur_pokemon_bytes)
+            if pokemon is not None:
+                party.append(pokemon)
 
         team.party = party
 
         # PC items
         pc_items = []
         for i in range(PC_ITEM_COUNT):
             cur_item_bytes = team.pc_items[ITEM_SIZE * i : ITEM_SIZE * (i + 1)]
@@ -163,17 +164,14 @@
     def add_pc_item(self, item: Item):
 
         if len(self.pc_items) < PC_ITEM_COUNT:
             self.pc_items.append(item)
         else:
             raise ValueError("Cannot add more PC Items")
 
-    @staticmethod
-    def null_pokemon():
-        return BYTES_PER_PARTY_POKEMON * b"\x00"
 
     @staticmethod
     def null_item():
         return BYTES_PER_ITEM * b"\x00"
 
 
 @dataclass
@@ -197,15 +195,17 @@
         # Each pokemon in a party is 100 bytes, thus
         # we need to create parse 6 * 100 bytes
         pokemon = []
         for i in range(6):
             cur_pokemon_bytes = pc.pokemon[
                 BYTES_PER_PC_POKEMON * i : BYTES_PER_PC_POKEMON * (i + 1)
             ]
-            pokemon.append(PCPokemon.from_bytes(cur_pokemon_bytes))
+            cur_pokemon = PCPokemon.from_bytes(cur_pokemon_bytes)
+            if cur_pokemon is not None:
+                pokemon.append(cur_pokemon)
 
         pc.pokemon = pokemon
 
         return pc
 
     def add_pc_pokemon(self, pokemon: PCPokemon):
         self.pokemon.append(pokemon)
```

### Comparing `pyemerald-0.5.1/pyemerald/utils.py` & `pyemerald-0.5.2/pyemerald/utils.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.5.1/pyproject.toml` & `pyemerald-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyemerald"
-version = "0.5.1"
+version = "0.5.2"
 description = "A package to modify save files from Pokemon Emerald"
 authors = ["matkvist <kvistanalytics@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://gitlab.com/magnetos_son/pyemerald"
 
 [tool.poetry.dependencies]
```

### Comparing `pyemerald-0.5.1/setup.py` & `pyemerald-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['pyemerald']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'pyemerald',
-    'version': '0.5.1',
+    'version': '0.5.2',
     'description': 'A package to modify save files from Pokemon Emerald',
     'long_description': '# pyemerald\n\nPyemerald is a python package which lets you modify save files from Pokemon Emerald (Sapphire, Ruby, Leaf Green and Fire Red to come). It lets you modify Pokemon in your team and on the PC, and lets you modify items on the PC. It can also be used to inspect a Pokemons attributes like EV\'s (IV\'s to come).\n\nOther and more advanced projects exist e.g. [pkHex](https://projectpokemon.org/home/files/file/1-pkhex/) which inspired this project. However, it annoyed me that I was unable to run pkHex on Linux, and thus pyemerald was created.\n\nPlease make sure to never overwrite your original save file, as this software could accidentially make an invalid save file. You are responsible for using the software correctly.\n## Installation\n\nPyemerald can be installed from pypi with the following command:\n\n```\npip install pyemerald\n```\n\nIt has no dependencies so it should be a simple install.\n\n## Usage\n\nSeveral examples are available in the `examples` folder. But basically it works by loading an `.sav` file using a `Save` object, which can then emit a `Game` object that is modifiable. Once modification is done, the `Game` object is passed back to the `Save` object and saved to a new file (Please always save to a new file, so you don\'t accidentially delete your current save file!).\n\n```python\nfrom pyemerald.save import Save\nfrom pyemerald.pokemon import PCPokemon\nfrom pyemerald.moves import Move\n\nsave = Save.from_file("data/marie_treecko_pokedex_pc.sav")\n\ngame = save.to_game()\n\n# Simple create pokemon\nflygon = PCPokemon.from_name(\n    name="Flygon",\n    level=48,\n    move_1=Move.from_name("Thunder"),\n    move_2=Move.from_name("Thunder Punch"),\n    move_3=Move.from_name("Ice Beam"),\n    move_4=Move.from_name("Fly"),\n)\n\n# Add Pokemon to user PC\ngame.add_pc_pokemon(flygon)\n\n# Put modification back to the Save Object\nsave.update_from_game(game)\n\n# Write new Save file\nsave.to_file("data/emerald.sav")\n\n```\n',
     'author': 'matkvist',
     'author_email': 'kvistanalytics@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/magnetos_son/pyemerald',
```

### Comparing `pyemerald-0.5.1/PKG-INFO` & `pyemerald-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyemerald
-Version: 0.5.1
+Version: 0.5.2
 Summary: A package to modify save files from Pokemon Emerald
 Home-page: https://gitlab.com/magnetos_son/pyemerald
 License: MIT
 Author: matkvist
 Author-email: kvistanalytics@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

