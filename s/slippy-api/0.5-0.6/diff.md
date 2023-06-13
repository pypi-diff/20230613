# Comparing `tmp/slippy_api-0.5.tar.gz` & `tmp/slippy_api-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slippy_api-0.5.tar", last modified: Mon Jun 12 08:22:17 2023, max compression
+gzip compressed data, was "slippy_api-0.6.tar", last modified: Tue Jun 13 14:09:25 2023, max compression
```

## Comparing `slippy_api-0.5.tar` & `slippy_api-0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 08:22:17.126363 slippy_api-0.5/
--rw-rw-rw-   0        0        0     1088 2023-05-27 00:29:32.000000 slippy_api-0.5/LICENSE
--rw-rw-rw-   0        0        0      142 2023-05-27 00:29:32.000000 slippy_api-0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      486 2023-06-12 08:22:17.126363 slippy_api-0.5/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-05-27 00:29:32.000000 slippy_api-0.5/README.md
--rw-rw-rw-   0        0        0       88 2023-05-27 00:29:32.000000 slippy_api-0.5/pyproject.toml
--rw-rw-rw-   0        0        0       57 2023-05-27 00:29:32.000000 slippy_api-0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 08:22:17.127370 slippy_api-0.5/setup.cfg
--rw-rw-rw-   0        0        0      777 2023-06-12 08:21:19.000000 slippy_api-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:22:17.083526 slippy_api-0.5/slippi/
--rw-rw-rw-   0        0        0        0 2023-05-27 00:29:32.000000 slippy_api-0.5/slippi/__init__.py
--rw-rw-rw-   0        0        0     1408 2023-06-12 08:13:01.000000 slippy_api-0.5/slippi/custom_logging.py
--rw-rw-rw-   0        0        0      522 2023-06-12 08:05:15.000000 slippy_api-0.5/slippi/main.py
--rw-rw-rw-   0        0        0     4336 2023-06-12 08:20:16.000000 slippy_api-0.5/slippi/slippi_api.py
--rw-rw-rw-   0        0        0     2260 2023-06-12 08:20:16.000000 slippy_api-0.5/slippi/slippi_characters.py
--rw-rw-rw-   0        0        0     1678 2023-06-12 08:20:16.000000 slippy_api-0.5/slippi/slippi_ranks.py
--rw-rw-rw-   0        0        0     4407 2023-06-12 08:20:16.000000 slippy_api-0.5/slippi/slippi_user.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:22:17.102532 slippy_api-0.5/slippi/tests/
--rw-rw-rw-   0        0        0        0 2023-05-27 00:29:32.000000 slippy_api-0.5/slippi/tests/__init__.py
--rw-rw-rw-   0        0        0     2039 2023-05-27 00:29:32.000000 slippy_api-0.5/slippi/tests/test_slippi_api.py
--rw-rw-rw-   0        0        0      671 2023-05-27 00:29:32.000000 slippy_api-0.5/slippi/tests/test_slippi_characters.py
--rw-rw-rw-   0        0        0      885 2023-05-27 00:29:32.000000 slippy_api-0.5/slippi/tests/test_slippi_ranks.py
--rw-rw-rw-   0        0        0     4628 2023-05-27 00:29:32.000000 slippy_api-0.5/slippi/tests/test_slippi_user.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:22:17.124359 slippy_api-0.5/slippy_api.egg-info/
--rw-rw-rw-   0        0        0      486 2023-06-12 08:22:16.000000 slippy_api-0.5/slippy_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      555 2023-06-12 08:22:16.000000 slippy_api-0.5/slippy_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 08:22:16.000000 slippy_api-0.5/slippy_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-12 08:22:16.000000 slippy_api-0.5/slippy_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-12 08:22:16.000000 slippy_api-0.5/slippy_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 14:09:25.308989 slippy_api-0.6/
+-rw-rw-rw-   0        0        0     1088 2023-05-27 00:29:32.000000 slippy_api-0.6/LICENSE
+-rw-rw-rw-   0        0        0      142 2023-05-27 00:29:32.000000 slippy_api-0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      486 2023-06-13 14:09:25.307989 slippy_api-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2023-06-13 14:04:11.000000 slippy_api-0.6/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-27 00:29:32.000000 slippy_api-0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       57 2023-05-27 00:29:32.000000 slippy_api-0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 14:09:25.308989 slippy_api-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      777 2023-06-13 13:43:53.000000 slippy_api-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:09:25.283988 slippy_api-0.6/slippi/
+-rw-rw-rw-   0        0        0        0 2023-05-27 00:29:32.000000 slippy_api-0.6/slippi/__init__.py
+-rw-rw-rw-   0        0        0     1408 2023-06-12 08:13:01.000000 slippy_api-0.6/slippi/custom_logging.py
+-rw-rw-rw-   0        0        0      522 2023-06-12 08:05:15.000000 slippy_api-0.6/slippi/main.py
+-rw-rw-rw-   0        0        0     5479 2023-06-13 12:41:58.000000 slippy_api-0.6/slippi/slippi_api.py
+-rw-rw-rw-   0        0        0     3170 2023-06-13 12:48:50.000000 slippy_api-0.6/slippi/slippi_characters.py
+-rw-rw-rw-   0        0        0     2014 2023-06-13 12:55:21.000000 slippy_api-0.6/slippi/slippi_ranks.py
+-rw-rw-rw-   0        0        0     5562 2023-06-13 13:34:53.000000 slippy_api-0.6/slippi/slippi_user.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:09:25.291989 slippy_api-0.6/slippi/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-27 00:29:32.000000 slippy_api-0.6/slippi/tests/__init__.py
+-rw-rw-rw-   0        0        0     2039 2023-05-27 00:29:32.000000 slippy_api-0.6/slippi/tests/test_slippi_api.py
+-rw-rw-rw-   0        0        0      671 2023-05-27 00:29:32.000000 slippy_api-0.6/slippi/tests/test_slippi_characters.py
+-rw-rw-rw-   0        0        0      885 2023-05-27 00:29:32.000000 slippy_api-0.6/slippi/tests/test_slippi_ranks.py
+-rw-rw-rw-   0        0        0     4628 2023-05-27 00:29:32.000000 slippy_api-0.6/slippi/tests/test_slippi_user.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:09:25.306987 slippy_api-0.6/slippy_api.egg-info/
+-rw-rw-rw-   0        0        0      486 2023-06-13 14:09:25.000000 slippy_api-0.6/slippy_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2023-06-13 14:09:25.000000 slippy_api-0.6/slippy_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 14:09:25.000000 slippy_api-0.6/slippy_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-13 14:09:25.000000 slippy_api-0.6/slippy_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-13 14:09:25.000000 slippy_api-0.6/slippy_api.egg-info/top_level.txt
```

### Comparing `slippy_api-0.5/LICENSE` & `slippy_api-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `slippy_api-0.5/setup.py` & `slippy_api-0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='slippy_api',
-    version='0.5',
+    version='0.6',
     author='Sophia',
     author_email='sophimander@gmail.com',
     description='API wrapper for slippi.gg',
     long_description='Simple wrapper for the GraphQL api on slippi.gg',
     long_description_content_type='text/markdown',
     install_requires=[
         'requests~=2.29.0',
```

### Comparing `slippy_api-0.5/slippi/custom_logging.py` & `slippy_api-0.6/slippi/custom_logging.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.5/slippi/main.py` & `slippy_api-0.6/slippi/main.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.5/slippi/slippi_api.py` & `slippy_api-0.6/slippi/slippi_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 from re import match
 
 import logging
 
 from slippi.custom_logging import CustomFormatter
 from slippi.slippi_user import SlippiUser
 
+# Get the logger instance from custom formatter
 logger = CustomFormatter().get_logger()
 
+# GraphQL query for maximum player data
 query_max = """
 fragment userProfilePage on User {
   fbUid
   displayName
   connectCode {
     code
     __typename
@@ -54,64 +56,85 @@
     }
     __typename
   }
 }
 
 """
 
+# GraphQL query for minimum player data
 query_min = """
-                fragment userProfilePage on User {
-                    displayName
-                    connectCode {
-                        code
-                        __typename
-                    }
-                    rankedNetplayProfile {
-                        id
-                        ratingOrdinal
-                        ratingUpdateCount
-                        wins
-                        losses
-                        dailyGlobalPlacement
-                        dailyRegionalPlacement
-                        continent
-                        characters {
-                            id
-                            character
-                            gameCount
-                            __typename
-                        }
-                        __typename
-                    }
-                    __typename
-                }
-                query AccountManagementPageQuery($cc: String!) {
-                    getConnectCode(code: $cc) {
-                        user {
-                            ...userProfilePage
-                            __typename
-                        }
-                        __typename
-                    }
-                }
-            """
+fragment userProfilePage on User {
+    displayName
+    connectCode {
+        code
+        __typename
+    }
+    rankedNetplayProfile {
+        id
+        ratingOrdinal
+        ratingUpdateCount
+        wins
+        losses
+        dailyGlobalPlacement
+        dailyRegionalPlacement
+        continent
+        characters {
+            id
+            character
+            gameCount
+            __typename
+        }
+        __typename
+    }
+    __typename
+}
+query AccountManagementPageQuery($cc: String!) {
+    getConnectCode(code: $cc) {
+        user {
+            ...userProfilePage
+            __typename
+        }
+        __typename
+    }
+}
+"""
 
 
 class SlippiRankedAPI:
     def __init__(self):
+        # Initialize a rate limiter with maximum 1 call per second
         self._limiter = RateLimiter(max_calls=1, period=1)
 
     @staticmethod
     def is_valid_connect_code(connect_code: str) -> bool:
+        """
+        Check if the given connect code is valid.
+
+        Args:
+            connect_code (str): The connect code to validate.
+
+        Returns:
+            bool: True if the connect code is valid, False otherwise.
+        """
         logger.info(f'is_valid_connect_code: {connect_code}')
         return True if (match(r"^(?=.{3,9}$)[a-zA-Z]{1,7}#[0-9]{1,7}$", connect_code)) else False
 
     @staticmethod
     def _get_player_data(self, connect_code: str, is_max: bool = False):
+        """
+        Get player data from the Slippi API.
 
+        Args:
+            self: The instance of the SlippiRankedAPI class.
+            connect_code (str): The connect code of the player.
+            is_max (bool): Whether to fetch maximum player data or not.
+
+        Returns:
+            dict: The player data in JSON format.
+        """
         if not self.is_valid_connect_code(connect_code):
             logger.warning(f'Invalid connect_code: {connect_code}')
             return
 
         variables = {
             "cc": connect_code.upper(),
             "uid": connect_code.upper()
@@ -126,27 +149,56 @@
         }
         response = requests.post('https://gql-gateway-dot-slippi.uc.r.appspot.com/graphql', json=payload,
                                  headers=headers)
         logger.debug(f'response: {response.json()}')
         return response.json()
 
     def get_player_data_throttled(self, connect_code: str, is_max: bool = False):
+        """
+        Get player data with rate limiting.
+
+        Args:
+            connect_code (str): The connect code of the player.
+            is_max (bool): Whether to fetch maximum player data or not.
+
+        Returns:
+            dict: The player data in JSON format.
+        """
         with self._limiter:
             return self._get_player_data(self, connect_code, is_max)
 
     def get_player_ranked_data(self, connect_code: str, is_max: bool = False) -> SlippiUser | None:
+        """
+        Get ranked player data.
+
+        Args:
+            connect_code (str): The connect code of the player.
+            is_max (bool): Whether to fetch maximum player data or not.
+
+        Returns:
+            SlippiUser | None: An instance of SlippiUser class if player data is available, None otherwise.
+        """
         logger.info(f'get_player_ranked_data: {connect_code}')
         player_data = self.get_player_data_throttled(connect_code, is_max)
 
         logger.debug(f'player_data: {player_data}')
         if not player_data or not player_data['data']['getConnectCode']:
             return
 
         return SlippiUser(player_data)
 
     def does_exist(self, connect_code: str) -> bool:
+        """
+        Check if a player with the given connect code exists.
+
+        Args:
+            connect_code (str): The connect code of the player.
+
+        Returns:
+            bool: True if the player exists, False otherwise.
+        """
         results = self.get_player_data_throttled(connect_code)
 
         if not results or not results['data']['getConnectCode']:
             return False
 
         return True
```

### Comparing `slippy_api-0.5/slippi/slippi_characters.py` & `slippy_api-0.6/slippi/slippi_characters.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from slippi.custom_logging import CustomFormatter
 
 logger = CustomFormatter().get_logger()
 
+# Define the base URL for Slippi character stock icons
 slippi_character_url = 'https://slippi.gg/images/characters/stock-icon-?-0.png'
 
-
+# A dictionary that maps character names to their corresponding IDs
 SlippiCharacterId = {
     'DONKEY_KONG': 0,  # Mapped to 255 in database
     'CAPTAIN_FALCON': 1,
     'FOX': 2,
     'GAME_AND_WATCH': 3,
     'KIRBY': 4,
     'BOWSER': 5,
@@ -31,15 +32,15 @@
     'DR_MARIO': 22,
     'ROY': 23,
     'PICHU': 24,
     'GANONDORF': 25,
     'None': 256
 }
 
-
+# A dictionary that maps character names to their corresponding colors
 SlippiCharacterColors = {
     'DONKEY_KONG': '#2f1003',
     'CAPTAIN_FALCON': '#353c5e',
     'FOX': '#ffb242',
     'GAME_AND_WATCH': '#000000',
     'KIRBY': '#ffbed8',
     'BOWSER': '#376218',
@@ -63,31 +64,54 @@
     'ROY': '#962000',
     'PICHU': '#ffff1b',
     'GANONDORF': '#91763e',
 }
 
 
 def get_key_from_value(value, dict):
+    """Retrieve the key from a dictionary based on its value."""
     for key, val in dict.items():
         if val == value:
             return key
     return None
 
-
 def get_character_name(char_id: int) -> str:
+    """Get the character name based on its ID.
+
+    Args:
+        char_id (int): The ID of the character.
+
+    Returns:
+        str: The name of the character.
+    """
     logger.info(f'get_character_name: {char_id}')
     if char_id == 255:
         char_id = 0
     return get_key_from_value(char_id, SlippiCharacterId)
 
-
 def get_character_id(name: str, dk_claus: bool = False) -> int:
+    """Get the character ID based on its name.
+
+    Args:
+        name (str): The name of the character.
+        dk_claus (bool, optional): Whether to handle Donkey Kong Claus mapping. Defaults to False.
+
+    Returns:
+        int: The ID of the character.
+    """
     logger.info(f'get_character_id: {name}')
     character_id = SlippiCharacterId.get(name)
     if dk_claus and character_id == 0:
         character_id = 255
     return character_id
 
-
 def get_character_url(name: str) -> str:
+    """Get the URL of the character's stock icon based on its name.
+
+    Args:
+        name (str): The name of the character.
+
+    Returns:
+        str: The URL of the character's stock icon.
+    """
     logger.info(f'get_character_url: {name}')
     return slippi_character_url.replace('?', str(get_character_id(name)))
```

### Comparing `slippy_api-0.5/slippi/slippi_user.py` & `slippy_api-0.6/slippi/slippi_user.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,72 @@
 from dataclasses import dataclass, field
-
 from slippi.custom_logging import CustomFormatter
 
 from slippi.slippi_ranks import get_rank
 from slippi.slippi_characters import get_character_id, get_character_url
 
 logger = CustomFormatter().get_logger()
 
 
 @dataclass
 class Characters:
+    """Represents a character with its ID, name, and game count."""
     id: int = 0
     character: str = ''
     game_count: int = 0
 
     def get_character_icon_url(self):
+        """Get the URL of the character's icon."""
         return get_character_url(self.character)
 
     def get_true_character_id(self):
+        """Get the true character ID, accounting for special cases."""
         return get_character_id(self.character)
 
     def __eq__(self, other):
+        """Check if two Characters instances are equal."""
         return self.character == other.character and self.game_count == other.game_count
 
 
 @dataclass
 class RankedNetplayProfile:
+    """Represents a ranked netplay profile with its ID, rating, win/loss counts, placements, and character data."""
     id: int = None
     rating_ordinal: float = 1100
     rating_update_count: int = None
     wins: int = 0
     losses: int = 0
     daily_global_placement = None
     daily_regional_placement = None
     continent: str = None
     characters: list[Characters] = field(default_factory=list)
 
 
 @dataclass
 class SubscriptionStatus:
+    """Represents the subscription status with its active state and level."""
     active: bool = False
     level: str = 'NONE'
     gift: bool = False
 
 
 @dataclass
 class SlippiUser:
+    """Represents a Slippi user with their display name, connect code, subscription status, and ranked netplay profile."""
     display_name: str = ''
     connect_code: str = ''
     sub_status: SubscriptionStatus = SubscriptionStatus()
     ranked_profile: RankedNetplayProfile = RankedNetplayProfile()
 
     def __init__(self, slippi_data: dict):
+        """Initialize the SlippiUser object based on the provided Slippi data.
+
+        Args:
+            slippi_data (dict): The Slippi data containing the user information.
+        """
         logger.info('SlippiUser created')
 
         # Check if dict exists correctly
         if not slippi_data['data']['getConnectCode']:
             return
 
         # Create local variables to use later
@@ -99,25 +110,39 @@
             continent=ranked_data['continent'] or 'NONE',
             characters=characters_list
         )
         self.ranked_profile.daily_global_placement = ranked_data['dailyGlobalPlacement'] or 0
         self.ranked_profile.daily_regional_placement = ranked_data['dailyRegionalPlacement'] or 0
 
     def get_rank(self) -> str:
+        """Get the rank of the Slippi user based on their ranked profile.
+
+        Returns:
+            str: The name of the rank.
+        """
         # Check if they've played their placement games, or else return 'None'
         if (self.ranked_profile.wins + self.ranked_profile.losses) < 5:
             return 'None' if not self.ranked_profile.wins and self.ranked_profile.losses else 'Pending'
         return get_rank(self.ranked_profile.rating_ordinal,
-                        self.ranked_profile.daily_regional_placement,
                         self.ranked_profile.daily_global_placement)
 
     def get_user_profile_page(self) -> str:
+        """Get the URL of the user's profile page.
+
+        Returns:
+            str: The URL of the user's profile page.
+        """
         return f'https://slippi.gg/user/{self.connect_code.replace("#", "-")}'
 
     def get_main_character(self) -> Characters:
+        """Get the main character of the Slippi user based on game count.
+
+        Returns:
+            Characters: The character with the highest game count.
+        """
         character_to_return = None
         highest_game_count = 0
         for guy in self.ranked_profile.characters:
             if guy.game_count > highest_game_count:
                 highest_game_count = guy.game_count
                 character_to_return = guy
```

### Comparing `slippy_api-0.5/slippi/tests/test_slippi_api.py` & `slippy_api-0.6/slippi/tests/test_slippi_api.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.5/slippi/tests/test_slippi_characters.py` & `slippy_api-0.6/slippi/tests/test_slippi_characters.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.5/slippi/tests/test_slippi_ranks.py` & `slippy_api-0.6/slippi/tests/test_slippi_ranks.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.5/slippi/tests/test_slippi_user.py` & `slippy_api-0.6/slippi/tests/test_slippi_user.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.5/slippy_api.egg-info/SOURCES.txt` & `slippy_api-0.6/slippy_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

