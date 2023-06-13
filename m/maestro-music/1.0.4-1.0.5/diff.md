# Comparing `tmp/maestro-music-1.0.4.tar.gz` & `tmp/maestro-music-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestro-music-1.0.4.tar", last modified: Sun Jun 11 17:24:11 2023, max compression
+gzip compressed data, was "maestro-music-1.0.5.tar", last modified: Tue Jun 13 05:40:21 2023, max compression
```

## Comparing `maestro-music-1.0.4.tar` & `maestro-music-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-06-11 17:24:11.975870 maestro-music-1.0.4/
--rw-r--r--   0 sysadmin   (501) staff       (20)     1067 2023-06-06 05:56:48.000000 maestro-music-1.0.4/LICENSE
--rw-r--r--   0 sysadmin   (501) staff       (20)    10945 2023-06-11 17:24:11.975650 maestro-music-1.0.4/PKG-INFO
--rw-r--r--   0 sysadmin   (501) staff       (20)    40729 2023-06-11 17:22:31.000000 maestro-music-1.0.4/helpers.py
--rw-r--r--   0 sysadmin   (501) staff       (20)   146639 2023-03-25 20:23:16.000000 maestro-music-1.0.4/icon.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     8837 2023-06-08 00:47:48.000000 maestro-music-1.0.4/mac_presence.py
--rw-r--r--   0 sysadmin   (501) staff       (20)   111717 2023-06-08 06:29:07.000000 maestro-music-1.0.4/maestro.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-06-11 17:24:11.975391 maestro-music-1.0.4/maestro_music.egg-info/
--rw-r--r--   0 sysadmin   (501) staff       (20)    10945 2023-06-11 17:24:11.000000 maestro-music-1.0.4/maestro_music.egg-info/PKG-INFO
--rw-r--r--   0 sysadmin   (501) staff       (20)      286 2023-06-11 17:24:11.000000 maestro-music-1.0.4/maestro_music.egg-info/SOURCES.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)        1 2023-06-11 17:24:11.000000 maestro-music-1.0.4/maestro_music.egg-info/dependency_links.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)       40 2023-06-11 17:24:11.000000 maestro-music-1.0.4/maestro_music.egg-info/entry_points.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)      367 2023-06-11 17:24:11.000000 maestro-music-1.0.4/maestro_music.egg-info/requires.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)       34 2023-06-11 17:24:11.000000 maestro-music-1.0.4/maestro_music.egg-info/top_level.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)       38 2023-06-11 17:24:11.975937 maestro-music-1.0.4/setup.cfg
--rw-r--r--   0 sysadmin   (501) staff       (20)     1646 2023-06-11 17:24:07.000000 maestro-music-1.0.4/setup.py
+drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-06-13 05:40:21.330181 maestro-music-1.0.5/
+-rw-r--r--   0 sysadmin   (501) staff       (20)     1067 2023-06-06 05:56:48.000000 maestro-music-1.0.5/LICENSE
+-rw-r--r--   0 sysadmin   (501) staff       (20)    11718 2023-06-13 05:40:21.329937 maestro-music-1.0.5/PKG-INFO
+-rw-r--r--   0 sysadmin   (501) staff       (20)    40840 2023-06-13 05:39:50.000000 maestro-music-1.0.5/helpers.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)   146639 2023-03-25 20:23:16.000000 maestro-music-1.0.5/icon.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)     8837 2023-06-08 00:47:48.000000 maestro-music-1.0.5/mac_presence.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)   111717 2023-06-08 06:29:07.000000 maestro-music-1.0.5/maestro.py
+drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-06-13 05:40:21.329698 maestro-music-1.0.5/maestro_music.egg-info/
+-rw-r--r--   0 sysadmin   (501) staff       (20)    11718 2023-06-13 05:40:21.000000 maestro-music-1.0.5/maestro_music.egg-info/PKG-INFO
+-rw-r--r--   0 sysadmin   (501) staff       (20)      286 2023-06-13 05:40:21.000000 maestro-music-1.0.5/maestro_music.egg-info/SOURCES.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)        1 2023-06-13 05:40:21.000000 maestro-music-1.0.5/maestro_music.egg-info/dependency_links.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)       40 2023-06-13 05:40:21.000000 maestro-music-1.0.5/maestro_music.egg-info/entry_points.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)      367 2023-06-13 05:40:21.000000 maestro-music-1.0.5/maestro_music.egg-info/requires.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)       34 2023-06-13 05:40:21.000000 maestro-music-1.0.5/maestro_music.egg-info/top_level.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)       38 2023-06-13 05:40:21.330245 maestro-music-1.0.5/setup.cfg
+-rw-r--r--   0 sysadmin   (501) staff       (20)     1646 2023-06-13 05:40:20.000000 maestro-music-1.0.5/setup.py
```

### Comparing `maestro-music-1.0.4/LICENSE` & `maestro-music-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `maestro-music-1.0.4/PKG-INFO` & `maestro-music-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 Metadata-Version: 2.1
 Name: maestro-music
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple command line tool to play songs (or any audio files, really).
 Home-page: https://github.com/PrajwalVandana/maestro-cli
 Author: Prajwal Vandana
 License: MIT
 Keywords: music,sound,audio,music-player,cli,ogg,flac,mp3,wav,spotify,youtube,audio-visualization,audio-visualizer
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# maestro
-`maestro` is a command-line tool to play songs (or any audio, really) in the terminal.
+# maestro-cli
+[![Downloads](https://static.pepy.tech/badge/maestro-music)](https://pepy.tech/project/maestro-music) [![PyPI version](https://badge.fury.io/py/maestro-music.svg)](https://badge.fury.io/py/maestro-music) [![Support Server](https://img.shields.io/discord/1117677384846544896.svg?color=7289da&label=maestro-cli&logo=discord)](https://discord.gg/AW8fh2QEav)
+
+`maestro-cli` is a command-line tool to play songs (or any audio, really) in the terminal.
+
+Check out the [Discord server](https://discord.gg/AW8fh2QEav)!
 
 ## Features
 
 - cross-platform!
 - add songs directly from YouTube, YouTube Music, or Spotify!
-- audio visualization directly in the terminal!
+- audio visualization directly in the terminal! ![maestro play example](data/player.png)
 - Discord integration!
+
+![maestro play example](data/discord.png)
+- Mac integration (Touch Bar, Now Playing center, headphone controls)! ![maestro play example](data/now_playing.png)
 - [clips!](#maestro-clip)
 - shuffle! (along with precise control over the behavior of shuffling when repeating)
 - filter by [tags](#usage)!
 
 ## Installation
 
 Make sure you have Python 3 and `pip` installed.
 
 First, run
 ```
 pip install maestro-music
 ```
 
-**NOTE**: `pip install maestro` will NOT work, this downloads a totally unrelated package from PyPI.
+**NOTE**: `pip install maestro` and `pip install maestro-cli` will NOT work, they are totally unrelated PyPI packages.
 
 Now, if you want to be able to directly download songs from YouTube or Spotify, you'll need to install [FFmpeg](https://github.com/FFmpeg/FFmpeg). You can also download the songs yourself and pass the path to the downloaded file to `maestro add`.
 
 ### Installing FFmpeg
 
 **EASIEST**: `conda install -c conda-forge ffmpeg`
 
@@ -66,35 +73,35 @@
 ```
 
 Also, if you have `conda`, see if running the following fixes your issue before trying anything below:
 ```
 conda install libsndfile ffmpeg cffi
 ```
 
-`maestro` uses [just_playback](https://github.com/cheofusi/just_playback) to play sound, which uses a C library called [miniaudio](https://github.com/mackron/miniaudio). Unfortunately, the creators did not provide wheels, so installation of `just_playback` and therefore `maestro` usually fails if there's any (compatibility or otherwise) problems with your C/C++ compiler. Here are platforms where there are known issues:
+`maestro-cli` uses [just_playback](https://github.com/cheofusi/just_playback) to play sound, which uses a C library called [miniaudio](https://github.com/mackron/miniaudio). Unfortunately, the creators did not provide wheels, so installation of `just_playback` and therefore `maestro-cli` usually fails if there's any (compatibility or otherwise) problems with your C/C++ compiler. Here are platforms where there are known issues:
 
 #### Apple Silicon
 
 There's a problem with the flag `-march=native` for older versions of the `clang` compiler. I manually removed this from the `just_playback` code and built an Apple Silicon-compatible version. Just check out the `dependency_builds/` folder in this repo, and look for the wheel that says `arm64`. Download it, then run
 ```
 pip install PATH_TO_DOWNLOADED_ARM64_WHEEL
 ```
-and *now* installing `maestro` should work.
+and *now* `pip install maestro-music` should work.
 
 #### Windows
 
 If you get this error on a 64-bit Windows
 ```
 error: Microsoft Visual C++ 14.0 or greater is required. Get it with "Microsoft C++ Build Tools": https://visualstudio.microsoft.com/visual-cpp-build-tools/
 ```
 find and download the `win_amd64` wheel of `just_playback` in `dependency_builds`, then run
 ```
 pip install PATH_TO_DOWNLOADED_WIN64_WHEEL
 ```
-and *now* installing `maestro` should work. Another option (especially if you're on a 32-bit Windows) is to just get Visual C++ Build Tools.
+and *now* `pip install maestro-music` should work. Another option (especially if you're on a 32-bit Windows) is to just get Visual C++ Build Tools.
 
 #### Linux
 
 If you have issues (especially if you get `Illegal instruction (core dumped)` when running `maestro play`, even after installing succesfully), try:
  * upgrading pip: `pip install --upgrade pip`
  * uninstalling `just_playback`: `pip uninstall just_playback`
  * reinstalling `just_playback` with the `--no-binary` flag: `pip install just_playback --no-binary just_playback --force-reinstall --upgrade`
@@ -107,27 +114,27 @@
 ```pip uninstall maestro-music```
 and also remove the `~/.maestro-files` folder.
 
 WARNING: this will delete all your songs! You should probably back up your `~/.maestro-files/songs/` folder first.
 
 ## Platforms
 
-Tested heavily on macOS Monterey, barely at all on Windows and Linux. `maestro` was coded to be cross-platform, but if there are any problems, please open an issue (or PR if you know how to fix it!).
+Tested heavily on macOS Monterey, lightly on Windows and Linux. `maestro-cli` was coded to be cross-platform, but if there are any problems, please open an issue (or PR if you know how to fix it!). You can also join the [Discord server](https://discord.gg/AW8fh2QEav) and ask for help there.
 
 Supports `.mp3`, `.wav`, `.flac`, and `.ogg` (Ogg Vorbis).
 
 ## Usage
 
 Run `maestro -h` to get a list of commands. Run `maestro <some command> -h` to get comprehensive help for that command—the below is just an overview.
 
-`maestro` uses the concept of a positive integer **song ID** to uniquely refer to each song.
+`maestro-cli` uses the concept of a positive integer **song ID** to uniquely refer to each song.
 
-Also, playlists don't exist—`maestro` uses **tags**. For example, let's say you want to be able to listen to all your Jon Bellion songs together. Instead of adding them all to a playlist, run `maestro tag <song IDs for each Jon Bellion song> -t jon-bellion `. Then `maestro play jon-bellion`. If song `s` has tag `t`, then you can think of song `s` as belonging to the playlist defined by tag `t`.
+Also, playlists don't exist—`maestro-cli` uses **tags**. For example, let's say you want to be able to listen to all your Jon Bellion songs together. Instead of adding them all to a playlist, run `maestro tag <song IDs for each Jon Bellion song> -t jon-bellion `. Then `maestro play jon-bellion`. If song `s` has tag `t`, then you can think of song `s` as belonging to the playlist defined by tag `t`.
 
-`maestro` also tracks your listen time—total and by year. You can see this with `maestro list` and/or `maestro entry`. For example, to see your top 10 listened songs (by average number of times listened; note that this is NOT the number of times the song was played but rather the total listen time for that song divided by the duration), run `maestro list -s times_listened -T 10 -y cur`—replace 'cur' with e.g. '2020' to get the listen times for 2020 instead.
+`maestro-cli` also tracks your listen time—total and by year. You can see this with `maestro list` and/or `maestro entry`. For example, to see your top 10 listened songs (by average number of times listened; note that this is NOT the number of times the song was played but rather the total listen time for that song divided by the duration), run `maestro list -s times_listened -T 10 -y cur`—replace 'cur' with e.g. '2020' to get the listen times for 2020 instead.
 
 ### `maestro add`
 
 Add a song (can be a folder of songs too!) given a file path.
 
 Pass the `-Y` or `--youtube` flag to download from a YouTube or YouTube Music URL instead of a file path. This requires installing [FFmpeg](https://github.com/FFmpeg/FFmpeg). Passing a YouTube Music **song** URL (not "Video") is recommended, as passing "Video"s (i.e. just normal YouTube videos) can sometimes mess up the artist/album data.
```

### Comparing `maestro-music-1.0.4/helpers.py` & `maestro-music-1.0.5/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,15 @@
         self.can_show_visualization = (
             self.visualize
             and self.can_visualize
             and self.stdscr.getmaxyx()[0] > VISUALIZER_HEIGHT + 5
         )
         if self.visualize and self.can_visualize:
             t = threading.Thread(
-                target=self.load_visualizer_data,
+                target=self._load_visualizer_data,
                 daemon=True,
             )
             self.visualizer_data = {}
             t.start()
         else:
             self.visualizer_data = None
 
@@ -319,27 +319,27 @@
         self.duration = 0
         self.paused = False
         self.ending = False
         self.prompting: None | tuple = None
         self.clip = (0, 0)
         self.discord_connected = multiprocessing.Value("i", 2)
 
-    def load_visualizer_data(self):
+    def _load_visualizer_data(self):
         while True:
             cur_song_ids = set(
                 map(lambda x: x[0], self.playlist[self.i : self.i + 5])
             )
             keys_to_delete = []
             for k in self.visualizer_data:
                 if k not in cur_song_ids:
                     keys_to_delete.append(k)
             for k in keys_to_delete:
                 del self.visualizer_data[k]
 
-            for i in range(self.i, self.i + 5):
+            for i in range(self.i, min(self.i + 5, len(self.playlist))):
                 if self.playlist[i][0] in self.visualizer_data:
                     continue
                 song_path = os.path.join(SONGS_DIR, self.playlist[i][1])
                 cur_song_data = LIBROSA.load(
                     song_path, mono=False, sr=SAMPLE_RATE
                 )[0]
 
@@ -354,14 +354,16 @@
 
                 self.visualizer_data[self.playlist[i][0]] = (
                     LIBROSA.amplitude_to_db(
                         np.abs(LIBROSA.stft(cur_song_data)), ref=np.max
                     )
                     + 80
                 )
+                # except Exception as e:
+                #     print_to_logfile(e)
             sleep(1)
 
     @property
     def song_path(self):
         return os.path.join(SONGS_DIR, self.playlist[self.i][1])
 
     def output(self, pos):
@@ -414,15 +416,15 @@
                 )
 
         visualize_message = ""
         visualize_color = 12
         if self.visualize:
             if self.visualizer_data is None and self.can_visualize:
                 t = threading.Thread(
-                    target=self.load_visualizer_data,
+                    target=self._load_visualizer_data,
                     daemon=True,
                 )
                 self.visualizer_data = {}
                 t.start()
 
             if not self.can_visualize:
                 visualize_message = "Librosa is required for visualization."
```

### Comparing `maestro-music-1.0.4/icon.py` & `maestro-music-1.0.5/icon.py`

 * *Files identical despite different names*

### Comparing `maestro-music-1.0.4/mac_presence.py` & `maestro-music-1.0.5/mac_presence.py`

 * *Files identical despite different names*

### Comparing `maestro-music-1.0.4/maestro.py` & `maestro-music-1.0.5/maestro.py`

 * *Files identical despite different names*

### Comparing `maestro-music-1.0.4/maestro_music.egg-info/PKG-INFO` & `maestro-music-1.0.5/maestro_music.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 Metadata-Version: 2.1
 Name: maestro-music
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple command line tool to play songs (or any audio files, really).
 Home-page: https://github.com/PrajwalVandana/maestro-cli
 Author: Prajwal Vandana
 License: MIT
 Keywords: music,sound,audio,music-player,cli,ogg,flac,mp3,wav,spotify,youtube,audio-visualization,audio-visualizer
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# maestro
-`maestro` is a command-line tool to play songs (or any audio, really) in the terminal.
+# maestro-cli
+[![Downloads](https://static.pepy.tech/badge/maestro-music)](https://pepy.tech/project/maestro-music) [![PyPI version](https://badge.fury.io/py/maestro-music.svg)](https://badge.fury.io/py/maestro-music) [![Support Server](https://img.shields.io/discord/1117677384846544896.svg?color=7289da&label=maestro-cli&logo=discord)](https://discord.gg/AW8fh2QEav)
+
+`maestro-cli` is a command-line tool to play songs (or any audio, really) in the terminal.
+
+Check out the [Discord server](https://discord.gg/AW8fh2QEav)!
 
 ## Features
 
 - cross-platform!
 - add songs directly from YouTube, YouTube Music, or Spotify!
-- audio visualization directly in the terminal!
+- audio visualization directly in the terminal! ![maestro play example](data/player.png)
 - Discord integration!
+
+![maestro play example](data/discord.png)
+- Mac integration (Touch Bar, Now Playing center, headphone controls)! ![maestro play example](data/now_playing.png)
 - [clips!](#maestro-clip)
 - shuffle! (along with precise control over the behavior of shuffling when repeating)
 - filter by [tags](#usage)!
 
 ## Installation
 
 Make sure you have Python 3 and `pip` installed.
 
 First, run
 ```
 pip install maestro-music
 ```
 
-**NOTE**: `pip install maestro` will NOT work, this downloads a totally unrelated package from PyPI.
+**NOTE**: `pip install maestro` and `pip install maestro-cli` will NOT work, they are totally unrelated PyPI packages.
 
 Now, if you want to be able to directly download songs from YouTube or Spotify, you'll need to install [FFmpeg](https://github.com/FFmpeg/FFmpeg). You can also download the songs yourself and pass the path to the downloaded file to `maestro add`.
 
 ### Installing FFmpeg
 
 **EASIEST**: `conda install -c conda-forge ffmpeg`
 
@@ -66,35 +73,35 @@
 ```
 
 Also, if you have `conda`, see if running the following fixes your issue before trying anything below:
 ```
 conda install libsndfile ffmpeg cffi
 ```
 
-`maestro` uses [just_playback](https://github.com/cheofusi/just_playback) to play sound, which uses a C library called [miniaudio](https://github.com/mackron/miniaudio). Unfortunately, the creators did not provide wheels, so installation of `just_playback` and therefore `maestro` usually fails if there's any (compatibility or otherwise) problems with your C/C++ compiler. Here are platforms where there are known issues:
+`maestro-cli` uses [just_playback](https://github.com/cheofusi/just_playback) to play sound, which uses a C library called [miniaudio](https://github.com/mackron/miniaudio). Unfortunately, the creators did not provide wheels, so installation of `just_playback` and therefore `maestro-cli` usually fails if there's any (compatibility or otherwise) problems with your C/C++ compiler. Here are platforms where there are known issues:
 
 #### Apple Silicon
 
 There's a problem with the flag `-march=native` for older versions of the `clang` compiler. I manually removed this from the `just_playback` code and built an Apple Silicon-compatible version. Just check out the `dependency_builds/` folder in this repo, and look for the wheel that says `arm64`. Download it, then run
 ```
 pip install PATH_TO_DOWNLOADED_ARM64_WHEEL
 ```
-and *now* installing `maestro` should work.
+and *now* `pip install maestro-music` should work.
 
 #### Windows
 
 If you get this error on a 64-bit Windows
 ```
 error: Microsoft Visual C++ 14.0 or greater is required. Get it with "Microsoft C++ Build Tools": https://visualstudio.microsoft.com/visual-cpp-build-tools/
 ```
 find and download the `win_amd64` wheel of `just_playback` in `dependency_builds`, then run
 ```
 pip install PATH_TO_DOWNLOADED_WIN64_WHEEL
 ```
-and *now* installing `maestro` should work. Another option (especially if you're on a 32-bit Windows) is to just get Visual C++ Build Tools.
+and *now* `pip install maestro-music` should work. Another option (especially if you're on a 32-bit Windows) is to just get Visual C++ Build Tools.
 
 #### Linux
 
 If you have issues (especially if you get `Illegal instruction (core dumped)` when running `maestro play`, even after installing succesfully), try:
  * upgrading pip: `pip install --upgrade pip`
  * uninstalling `just_playback`: `pip uninstall just_playback`
  * reinstalling `just_playback` with the `--no-binary` flag: `pip install just_playback --no-binary just_playback --force-reinstall --upgrade`
@@ -107,27 +114,27 @@
 ```pip uninstall maestro-music```
 and also remove the `~/.maestro-files` folder.
 
 WARNING: this will delete all your songs! You should probably back up your `~/.maestro-files/songs/` folder first.
 
 ## Platforms
 
-Tested heavily on macOS Monterey, barely at all on Windows and Linux. `maestro` was coded to be cross-platform, but if there are any problems, please open an issue (or PR if you know how to fix it!).
+Tested heavily on macOS Monterey, lightly on Windows and Linux. `maestro-cli` was coded to be cross-platform, but if there are any problems, please open an issue (or PR if you know how to fix it!). You can also join the [Discord server](https://discord.gg/AW8fh2QEav) and ask for help there.
 
 Supports `.mp3`, `.wav`, `.flac`, and `.ogg` (Ogg Vorbis).
 
 ## Usage
 
 Run `maestro -h` to get a list of commands. Run `maestro <some command> -h` to get comprehensive help for that command—the below is just an overview.
 
-`maestro` uses the concept of a positive integer **song ID** to uniquely refer to each song.
+`maestro-cli` uses the concept of a positive integer **song ID** to uniquely refer to each song.
 
-Also, playlists don't exist—`maestro` uses **tags**. For example, let's say you want to be able to listen to all your Jon Bellion songs together. Instead of adding them all to a playlist, run `maestro tag <song IDs for each Jon Bellion song> -t jon-bellion `. Then `maestro play jon-bellion`. If song `s` has tag `t`, then you can think of song `s` as belonging to the playlist defined by tag `t`.
+Also, playlists don't exist—`maestro-cli` uses **tags**. For example, let's say you want to be able to listen to all your Jon Bellion songs together. Instead of adding them all to a playlist, run `maestro tag <song IDs for each Jon Bellion song> -t jon-bellion `. Then `maestro play jon-bellion`. If song `s` has tag `t`, then you can think of song `s` as belonging to the playlist defined by tag `t`.
 
-`maestro` also tracks your listen time—total and by year. You can see this with `maestro list` and/or `maestro entry`. For example, to see your top 10 listened songs (by average number of times listened; note that this is NOT the number of times the song was played but rather the total listen time for that song divided by the duration), run `maestro list -s times_listened -T 10 -y cur`—replace 'cur' with e.g. '2020' to get the listen times for 2020 instead.
+`maestro-cli` also tracks your listen time—total and by year. You can see this with `maestro list` and/or `maestro entry`. For example, to see your top 10 listened songs (by average number of times listened; note that this is NOT the number of times the song was played but rather the total listen time for that song divided by the duration), run `maestro list -s times_listened -T 10 -y cur`—replace 'cur' with e.g. '2020' to get the listen times for 2020 instead.
 
 ### `maestro add`
 
 Add a song (can be a folder of songs too!) given a file path.
 
 Pass the `-Y` or `--youtube` flag to download from a YouTube or YouTube Music URL instead of a file path. This requires installing [FFmpeg](https://github.com/FFmpeg/FFmpeg). Passing a YouTube Music **song** URL (not "Video") is recommended, as passing "Video"s (i.e. just normal YouTube videos) can sometimes mess up the artist/album data.
```

### Comparing `maestro-music-1.0.4/setup.py` & `maestro-music-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "pyobjc-framework-CoreMedia; sys_platform == 'darwin'",
     "pyobjc-framework-MediaPlayer; sys_platform == 'darwin'",
     "pyobjc-framework-Quartz; sys_platform == 'darwin'",
 ]
 
 setup(
     name="maestro-music",
-    version="1.0.4",
+    version="1.0.5",
     author="Prajwal Vandana",
     url="https://github.com/PrajwalVandana/maestro-cli",
     description="A simple command line tool to play songs (or any audio files, really).",
     long_description=open("readme.md", encoding="utf-8").read(),
     license="MIT",
     license_files=["LICENSE"],
     long_description_content_type="text/markdown",
```

