# Comparing `tmp/letterboxdpy-3.15.tar.gz` & `tmp/letterboxdpy-3.17.tar.gz`

## Comparing `letterboxdpy-3.15.tar` & `letterboxdpy-3.17.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 letterboxdpy-3.15/.gitattributes
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 letterboxdpy-3.15/letterboxdpy.egg-info/PKG-INFO
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 letterboxdpy-3.15/letterboxdpy.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 letterboxdpy-3.15/letterboxdpy.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 letterboxdpy-3.15/letterboxdpy.egg-info/requires.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 letterboxdpy-3.15/letterboxdpy.egg-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 letterboxdpy-3.15/src/letterboxdpy/__init__.py
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 letterboxdpy-3.15/src/letterboxdpy/list.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 letterboxdpy-3.15/src/letterboxdpy/movie.py
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 letterboxdpy-3.15/src/letterboxdpy/user.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 letterboxdpy-3.15/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 letterboxdpy-3.15/LICENSE
--rw-r--r--   0        0        0     9222 2020-02-02 00:00:00.000000 letterboxdpy-3.15/README.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 letterboxdpy-3.15/pyproject.toml
--rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 letterboxdpy-3.15/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 letterboxdpy-3.17/.gitattributes
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 letterboxdpy-3.17/letterboxdpy.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 letterboxdpy-3.17/letterboxdpy.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 letterboxdpy-3.17/letterboxdpy.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 letterboxdpy-3.17/letterboxdpy.egg-info/requires.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 letterboxdpy-3.17/letterboxdpy.egg-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 letterboxdpy-3.17/src/letterboxdpy/__init__.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 letterboxdpy-3.17/src/letterboxdpy/list.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 letterboxdpy-3.17/src/letterboxdpy/movie.py
+-rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 letterboxdpy-3.17/src/letterboxdpy/user.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 letterboxdpy-3.17/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 letterboxdpy-3.17/LICENSE
+-rw-r--r--   0        0        0     8894 2020-02-02 00:00:00.000000 letterboxdpy-3.17/README.md
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 letterboxdpy-3.17/pyproject.toml
+-rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 letterboxdpy-3.17/PKG-INFO
```

### Comparing `letterboxdpy-3.15/src/letterboxdpy/user.py` & `letterboxdpy-3.17/src/letterboxdpy/user.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-import json
-from json import JSONEncoder
-import re
-import requests
-from bs4 import BeautifulSoup
-
-class User:
-    def __init__(self, username: str) -> None:
-        if not re.match("^[A-Za-z0-9_]*$", username):
-            raise Exception("Invalid username")
-
-        self.username = username
-
-        page = self.get_parsed_page("https://letterboxd.com/" + self.username + "/")
-        
-        self.user_watchlist()
-        self.user_favorites(page)
-        self.user_stats(page)
-    
-    def __str__(self):
-        return self.jsonify()
-
-    def jsonify(self) -> str:
-        return json.dumps(self, indent=4,cls=Encoder)
-
-    def get_parsed_page(self, url: str) -> None:
-        # This fixes a blocked by cloudflare error i've encountered
-        headers = {
-            "referer": "https://letterboxd.com",
-            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64)"
-        }
-
-        return BeautifulSoup(requests.get(url, headers=headers).text, "lxml")
-
-    def user_favorites(self, page: None) -> list:        
-        data = page.find("section", {"id": ["favourites"], }).findChildren("div")
-        names = []
-
-        for div in data:
-            img = div.find("img")
-            movie_url = img.parent['data-film-slug']
-            names.append((img['alt'], movie_url))
-            
-        self.favorites = names
-
-    def user_stats(self, page: None) -> dict:
-        span = []
-        stats = {}
-
-        data = page.find_all("h4", {"class": ["profile-statistic"], })
-
-        for item in data:
-            span.append(item.findChildren("span"))
-
-        for item in span:
-            stats[item[1].text.replace(u'\xa0', ' ')] = item[0].text
-
-        self.stats = stats
-
-    def user_watchlist(self) -> str:
-        page = self.get_parsed_page("https://letterboxd.com/" + self.username + "/watchlist/")
-
-        data = page.find("span", {"class": ["watchlist-count"], })
-        try:
-            ret = data.text.split('\xa0')[0] #remove 'films' from '76 films'
-        except:
-            raise Exception("No user found")
-
-        self.watchlist_length = ret
-
-def user_films_watched(user: User) -> list:
-    if type(user) != User:
-        raise Exception("Improper parameter")
-
-    #returns all movies
-    prev = count = 0
-    curr = 1
-    movie_list = []
-
-    while prev != curr:
-        count += 1
-        prev = len(movie_list)
-        page = user.get_parsed_page("https://letterboxd.com/" + user.username + "/films/page/" + str(count) + "/")
-
-        img = page.find_all("img", {"class": ["image"], })
-
-        for item in img:
-            movie_url = item.parent['data-film-slug']
-            movie_list.append((item['alt'], movie_url))
-
-        curr = len(movie_list)
-            
-    return movie_list
-
-def user_following(user: User) -> list:
-    if type(user) != User:
-        raise Exception("Improper parameter")
-
-    #returns the first page of following
-    page = user.get_parsed_page("https://letterboxd.com/" + user.username + "/following/")
-    data = page.find_all("img", attrs={'height': '40'})
-
-    ret = []
-
-    for person in data:
-        ret.append(person['alt'])
-
-    return ret
-
-def user_followers(user: User) -> list:
-    if type(user) != User:
-        raise Exception("Improper parameter")
-
-    #returns the first page of followers
-    page = user.get_parsed_page("https://letterboxd.com/" + user.username + "/followers/")
-    data = page.find_all("img", attrs={'height': '40'})
-
-    ret = []
-
-    for person in data:
-        ret.append(person['alt'])
-
-    return ret
-            
-def user_genre_info(user: User) -> dict:
-    if type(user) != User:
-        raise Exception("Improper parameter")
-
-    genres = ["action", "adventure", "animation", "comedy", "crime", "documentary",
-              "drama", "family", "fantasy", "history", "horror", "music", "mystery",
-              "romance", "science-fiction", "thriller", "tv-movie", "war", "western"]
-    ret = {}
-    for genre in genres:
-        page = user.get_parsed_page("https://letterboxd.com/" + user.username +
-                                    "/films/genre/" + genre + "/")
-        data = page.find("span", {"class": ["replace-if-you"], })
-        data = data.next_sibling
-        ret[genre] = [int(s) for s in data.split() if s.isdigit()][0]
-        
-    return ret
-
-#gives reviews that the user selected has made
-def user_reviews(user: User) -> list:
-    if type(user) != User:
-        raise Exception("Improper parameter")
-        
-    page = user.get_parsed_page("https://letterboxd.com/" + user.username + "/films/reviews/")
-    ret = []
-
-    data = page.find_all("div", {"class": ["film-detail-content"], })
-
-    for item in data:
-        curr = {}
-
-        curr['movie'] = item.find("a").text #movie title
-        curr['rating'] = item.find("span", {"class": ["rating"], }).text #movie rating
-        curr['date'] = item.find("span", {"class": ["_nobr"], }).text #rating date
-        curr['review'] = item.find("div", {"class": ["body-text"], }).findChildren()[0].text #review
-
-        ret.append(curr)
-
-    return ret
-
-class Encoder(JSONEncoder):
-    def default(self, o):
-        return o.__dict__
-
-if __name__ == "__main__":
-    nick = User("nmcassa")
-    #print(nick)
-    print(user_films_watched(nick))
+import json
+from json import JSONEncoder
+import re
+import requests
+from bs4 import BeautifulSoup
+
+class User:
+    def __init__(self, username: str) -> None:
+        if not re.match("^[A-Za-z0-9_]*$", username):
+            raise Exception("Invalid username")
+
+        self.username = username.lower()
+
+        page = self.get_parsed_page("https://letterboxd.com/" + self.username + "/")
+        
+        self.user_watchlist()
+        self.user_favorites(page)
+        self.user_stats(page)
+    
+    def __str__(self):
+        return self.jsonify()
+
+    def jsonify(self) -> str:
+        return json.dumps(self, indent=4,cls=Encoder)
+
+    def get_parsed_page(self, url: str) -> None:
+        # This fixes a blocked by cloudflare error i've encountered
+        headers = {
+            "referer": "https://letterboxd.com",
+            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64)"
+        }
+
+        return BeautifulSoup(requests.get(url, headers=headers).text, "lxml")
+
+    def user_favorites(self, page: None) -> list:        
+        data = page.find("section", {"id": ["favourites"], }).findChildren("div")
+        names = []
+
+        for div in data:
+            img = div.find("img")
+            movie_url = img.parent['data-film-slug']
+            names.append((img['alt'], movie_url))
+            
+        self.favorites = names
+
+    def user_stats(self, page: None) -> dict:
+        span = []
+        stats = {}
+
+        data = page.find_all("h4", {"class": ["profile-statistic"], })
+
+        for item in data:
+            span.append(item.findChildren("span"))
+
+        for item in span:
+            stats[item[1].text.replace(u'\xa0', ' ')] = item[0].text
+
+        self.stats = stats
+
+    def user_watchlist(self) -> str:
+        page = self.get_parsed_page("https://letterboxd.com/" + self.username + "/watchlist/")
+
+        data = page.find("span", {"class": ["watchlist-count"], })
+        try:
+            ret = data.text.split('\xa0')[0] #remove 'films' from '76 films'
+        except:
+            raise Exception("No user found")
+
+        self.watchlist_length = ret
+
+def user_films_watched(user: User) -> list:
+    if type(user) != User:
+        raise Exception("Improper parameter")
+
+    #returns all movies
+    prev = count = 0
+    curr = 1
+    movie_list = []
+
+    while prev != curr:
+        count += 1
+        prev = len(movie_list)
+        page = user.get_parsed_page("https://letterboxd.com/" + user.username + "/films/page/" + str(count) + "/")
+
+        img = page.find_all("img", {"class": ["image"], })
+
+        for item in img:
+            movie_url = item.parent['data-film-slug']
+            movie_list.append((item['alt'], movie_url))
+
+        curr = len(movie_list)
+            
+    return movie_list
+
+def user_following(user: User) -> list:
+    if type(user) != User:
+        raise Exception("Improper parameter")
+
+    #returns the first page of following
+    page = user.get_parsed_page("https://letterboxd.com/" + user.username + "/following/")
+    data = page.find_all("img", attrs={'height': '40'})
+
+    ret = []
+
+    for person in data:
+        ret.append(person['alt'])
+
+    return ret
+
+def user_followers(user: User) -> list:
+    if type(user) != User:
+        raise Exception("Improper parameter")
+
+    #returns the first page of followers
+    page = user.get_parsed_page("https://letterboxd.com/" + user.username + "/followers/")
+    data = page.find_all("img", attrs={'height': '40'})
+
+    ret = []
+
+    for person in data:
+        ret.append(person['alt'])
+
+    return ret
+            
+def user_genre_info(user: User) -> dict:
+    if type(user) != User:
+        raise Exception("Improper parameter")
+
+    genres = ["action", "adventure", "animation", "comedy", "crime", "documentary",
+              "drama", "family", "fantasy", "history", "horror", "music", "mystery",
+              "romance", "science-fiction", "thriller", "tv-movie", "war", "western"]
+    ret = {}
+    for genre in genres:
+        page = user.get_parsed_page("https://letterboxd.com/" + user.username +
+                                    "/films/genre/" + genre + "/")
+        data = page.find("span", {"class": ["replace-if-you"], })
+        data = data.next_sibling
+        ret[genre] = [int(s) for s in data.split() if s.isdigit()][0]
+        
+    return ret
+
+#gives reviews that the user selected has made
+def user_reviews(user: User) -> list:
+    if type(user) != User:
+        raise Exception("Improper parameter")
+        
+    page = user.get_parsed_page("https://letterboxd.com/" + user.username + "/films/reviews/")
+    ret = []
+
+    data = page.find_all("div", {"class": ["film-detail-content"], })
+
+    for item in data:
+        curr = {}
+
+        curr['movie'] = item.find("a").text #movie title
+        curr['rating'] = item.find("span", {"class": ["rating"], }).text #movie rating
+        curr['date'] = item.find("span", {"class": ["_nobr"], }).text #rating date
+        curr['review'] = item.find("div", {"class": ["body-text"], }).findChildren()[0].text #review
+
+        ret.append(curr)
+
+    return ret
+
+class Encoder(JSONEncoder):
+    def default(self, o):
+        return o.__dict__
+
+if __name__ == "__main__":
+    nick = User("nmcassA")
+    #print(nick)
+    print(user_films_watched(nick))
```

### Comparing `letterboxdpy-3.15/LICENSE` & `letterboxdpy-3.17/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 nmcassa
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 nmcassa
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `letterboxdpy-3.15/PKG-INFO` & `letterboxdpy-3.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letterboxdpy
-Version: 3.15
+Version: 3.17
 Summary: A letterboxd webscraper
 Project-URL: Homepage, https://github.com/nmcassa/letterboxdpy
 Project-URL: Bug Tracker, https://github.com/nmcassa/letterboxdpy/issues
 Author-email: Nicholas Cassarino <nmcassa804@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

