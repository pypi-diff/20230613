# Comparing `tmp/mkdocs-publisher-0.5.0.tar.gz` & `tmp/mkdocs_publisher-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-publisher-0.5.0.tar", max compression
+gzip compressed data, was "mkdocs_publisher-1.0.0.tar", max compression
```

## Comparing `mkdocs-publisher-0.5.0.tar` & `mkdocs_publisher-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,47 @@
--rw-r--r--   0        0        0     1296 2023-01-30 14:12:38.164750 mkdocs-publisher-0.5.0/LICENSE
--rw-r--r--   0        0        0     5938 2023-04-04 20:35:38.735295 mkdocs-publisher-0.5.0/README.md
--rw-r--r--   0        0        0      865 2023-03-23 21:54:52.816280 mkdocs-publisher-0.5.0/mkdocs_publisher/_cli/_utils.py
--rw-r--r--   0        0        0      610 2023-03-23 21:54:52.816346 mkdocs-publisher-0.5.0/mkdocs_publisher/_cli/post.py
--rw-r--r--   0        0        0      310 2023-03-23 21:54:52.816398 mkdocs-publisher-0.5.0/mkdocs_publisher/_cli/publisher.py
--rw-r--r--   0        0        0        0 2023-03-23 21:54:52.816434 mkdocs-publisher-0.5.0/mkdocs_publisher/_extra/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 21:54:52.816482 mkdocs-publisher-0.5.0/mkdocs_publisher/_extra/assets/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 21:54:52.816540 mkdocs-publisher-0.5.0/mkdocs_publisher/_extra/assets/stylesheets/__init__.py
--rw-r--r--   0        0        0      851 2023-03-23 21:54:52.816604 mkdocs-publisher-0.5.0/mkdocs_publisher/_extra/assets/stylesheets/blog.css
--rw-r--r--   0        0        0     2406 2023-03-23 21:54:52.816668 mkdocs-publisher-0.5.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css
--rw-r--r--   0        0        0     1277 2023-03-23 21:54:52.816725 mkdocs-publisher-0.5.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css.map
--rw-r--r--   0        0        0        0 2023-03-23 21:54:52.816776 mkdocs-publisher-0.5.0/mkdocs_publisher/_extra/assets/templates/__init__.py
--rw-r--r--   0        0        0      679 2023-03-31 21:12:37.098222 mkdocs-publisher-0.5.0/mkdocs_publisher/_extra/assets/templates/posts-list.html
--rw-r--r--   0        0        0     2480 2023-03-23 21:54:52.816913 mkdocs-publisher-0.5.0/mkdocs_publisher/_utils.py
--rw-r--r--   0        0        0      356 2023-03-23 21:54:52.816974 mkdocs-publisher-0.5.0/mkdocs_publisher/auto_nav/config.py
--rw-r--r--   0        0        0     6548 2023-03-28 16:01:28.424265 mkdocs-publisher-0.5.0/mkdocs_publisher/auto_nav/plugin.py
--rw-r--r--   0        0        0     1645 2023-03-23 21:54:52.817131 mkdocs-publisher-0.5.0/mkdocs_publisher/blog/config.py
--rw-r--r--   0        0        0     7078 2023-03-28 16:01:28.424444 mkdocs-publisher-0.5.0/mkdocs_publisher/blog/creators.py
--rw-r--r--   0        0        0        0 2023-03-23 21:54:52.817229 mkdocs-publisher-0.5.0/mkdocs_publisher/blog/lang/__init__.py
--rw-r--r--   0        0        0      355 2023-03-23 21:54:52.817301 mkdocs-publisher-0.5.0/mkdocs_publisher/blog/lang/en.yaml
--rw-r--r--   0        0        0      368 2023-03-23 21:54:52.817348 mkdocs-publisher-0.5.0/mkdocs_publisher/blog/lang/pl.yaml
--rw-r--r--   0        0        0     4200 2023-04-02 19:02:05.858410 mkdocs-publisher-0.5.0/mkdocs_publisher/blog/modifiers.py
--rw-r--r--   0        0        0     6806 2023-03-28 16:01:28.424796 mkdocs-publisher-0.5.0/mkdocs_publisher/blog/parsers.py
--rw-r--r--   0        0        0     4856 2023-03-28 16:01:28.424935 mkdocs-publisher-0.5.0/mkdocs_publisher/blog/plugin.py
--rw-r--r--   0        0        0     2876 2023-03-28 16:01:28.425057 mkdocs-publisher-0.5.0/mkdocs_publisher/blog/structures.py
--rw-r--r--   0        0        0     1721 2023-03-28 16:01:28.425219 mkdocs-publisher-0.5.0/mkdocs_publisher/blog/translate.py
--rw-r--r--   0        0        0     5977 2023-03-28 16:01:28.425395 mkdocs-publisher-0.5.0/mkdocs_publisher/minifier/base.py
--rw-r--r--   0        0        0     3440 2023-03-23 21:54:52.817799 mkdocs-publisher-0.5.0/mkdocs_publisher/minifier/config.py
--rw-r--r--   0        0        0     9672 2023-03-28 16:01:28.425528 mkdocs-publisher-0.5.0/mkdocs_publisher/minifier/minifiers.py
--rw-r--r--   0        0        0     3094 2023-03-28 16:01:28.425677 mkdocs-publisher-0.5.0/mkdocs_publisher/minifier/plugin.py
--rw-r--r--   0        0        0      898 2023-04-04 21:15:54.664604 mkdocs-publisher-0.5.0/mkdocs_publisher/social/config.py
--rw-r--r--   0        0        0     4140 2023-04-04 21:18:54.995172 mkdocs-publisher-0.5.0/mkdocs_publisher/social/plugin.py
--rw-r--r--   0        0        0     2362 2023-04-04 21:22:19.978248 mkdocs-publisher-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     7711 1970-01-01 00:00:00.000000 mkdocs-publisher-0.5.0/setup.py
--rw-r--r--   0        0        0     7597 1970-01-01 00:00:00.000000 mkdocs-publisher-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-06-13 10:09:11.255323 mkdocs_publisher-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3946 2023-06-13 10:09:11.255631 mkdocs_publisher-1.0.0/README.md
+-rw-r--r--   0        0        0      610 2023-03-23 21:54:52.816346 mkdocs_publisher-1.0.0/mkdocs_publisher/_cli/post.py
+-rw-r--r--   0        0        0      310 2023-03-23 21:54:52.816398 mkdocs_publisher-1.0.0/mkdocs_publisher/_cli/publisher.py
+-rw-r--r--   0        0        0     1044 2023-06-13 10:09:11.351581 mkdocs_publisher-1.0.0/mkdocs_publisher/_common/html_modifiers.py
+-rw-r--r--   0        0        0      314 2023-06-13 10:09:11.351852 mkdocs_publisher-1.0.0/mkdocs_publisher/_common/mkdocs_utils.py
+-rw-r--r--   0        0        0     1116 2023-06-13 10:09:11.351969 mkdocs_publisher-1.0.0/mkdocs_publisher/_common/resources.py
+-rw-r--r--   0        0        0      337 2023-06-13 10:09:11.352076 mkdocs_publisher-1.0.0/mkdocs_publisher/_common/url.py
+-rw-r--r--   0        0        0        0 2023-03-23 21:54:52.816434 mkdocs_publisher-1.0.0/mkdocs_publisher/_extra/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-23 21:54:52.816482 mkdocs_publisher-1.0.0/mkdocs_publisher/_extra/assets/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-23 21:54:52.816540 mkdocs_publisher-1.0.0/mkdocs_publisher/_extra/assets/stylesheets/__init__.py
+-rw-r--r--   0        0        0      851 2023-04-14 09:31:43.946416 mkdocs_publisher-1.0.0/mkdocs_publisher/_extra/assets/stylesheets/blog.css
+-rw-r--r--   0        0        0      689 2023-06-13 10:09:11.352239 mkdocs_publisher-1.0.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css
+-rw-r--r--   0        0        0     1277 2023-05-20 10:18:53.045541 mkdocs_publisher-1.0.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css.map
+-rw-r--r--   0        0        0     3317 2023-06-13 10:09:11.352443 mkdocs_publisher-1.0.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.css
+-rw-r--r--   0        0        0     2792 2023-06-13 10:09:11.352535 mkdocs_publisher-1.0.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css
+-rw-r--r--   0        0        0     4010 2023-06-13 10:09:11.352653 mkdocs_publisher-1.0.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css.map
+-rw-r--r--   0        0        0        0 2023-03-23 21:54:52.816776 mkdocs_publisher-1.0.0/mkdocs_publisher/_extra/assets/templates/__init__.py
+-rw-r--r--   0        0        0      215 2023-06-13 10:09:11.352824 mkdocs_publisher-1.0.0/mkdocs_publisher/_extra/assets/templates/backlinks.html
+-rw-r--r--   0        0        0      677 2023-06-13 10:09:11.353130 mkdocs_publisher-1.0.0/mkdocs_publisher/_extra/assets/templates/posts-list.html
+-rw-r--r--   0        0        0     1598 2023-06-13 10:09:11.353370 mkdocs_publisher-1.0.0/mkdocs_publisher/_utils.py
+-rw-r--r--   0        0        0     1881 2023-06-13 10:09:11.353537 mkdocs_publisher-1.0.0/mkdocs_publisher/blog/config.py
+-rw-r--r--   0        0        0     7991 2023-06-13 10:09:11.353888 mkdocs_publisher-1.0.0/mkdocs_publisher/blog/creators.py
+-rw-r--r--   0        0        0        0 2023-03-23 21:54:52.817229 mkdocs_publisher-1.0.0/mkdocs_publisher/blog/lang/__init__.py
+-rw-r--r--   0        0        0      355 2023-03-23 21:54:52.817301 mkdocs_publisher-1.0.0/mkdocs_publisher/blog/lang/en.yaml
+-rw-r--r--   0        0        0      368 2023-03-23 21:54:52.817348 mkdocs_publisher-1.0.0/mkdocs_publisher/blog/lang/pl.yaml
+-rw-r--r--   0        0        0     3188 2023-06-13 10:09:11.354081 mkdocs_publisher-1.0.0/mkdocs_publisher/blog/modifiers.py
+-rw-r--r--   0        0        0     7176 2023-06-13 10:09:11.354272 mkdocs_publisher-1.0.0/mkdocs_publisher/blog/parsers.py
+-rw-r--r--   0        0        0     4385 2023-06-13 10:09:11.354501 mkdocs_publisher-1.0.0/mkdocs_publisher/blog/plugin.py
+-rw-r--r--   0        0        0     2941 2023-06-13 10:09:11.354707 mkdocs_publisher-1.0.0/mkdocs_publisher/blog/structures.py
+-rw-r--r--   0        0        0     1721 2023-04-14 11:40:46.664528 mkdocs_publisher-1.0.0/mkdocs_publisher/blog/translate.py
+-rw-r--r--   0        0        0     1180 2023-06-13 10:09:11.354906 mkdocs_publisher-1.0.0/mkdocs_publisher/meta/config.py
+-rw-r--r--   0        0        0    12656 2023-06-13 10:09:11.355286 mkdocs_publisher-1.0.0/mkdocs_publisher/meta/plugin.py
+-rw-r--r--   0        0        0     5978 2023-06-13 10:09:11.355596 mkdocs_publisher-1.0.0/mkdocs_publisher/minifier/base.py
+-rw-r--r--   0        0        0     3441 2023-06-13 10:09:11.355975 mkdocs_publisher-1.0.0/mkdocs_publisher/minifier/config.py
+-rw-r--r--   0        0        0     9672 2023-04-14 11:40:46.675141 mkdocs_publisher-1.0.0/mkdocs_publisher/minifier/minifiers.py
+-rw-r--r--   0        0        0     3094 2023-04-14 11:40:46.635558 mkdocs_publisher-1.0.0/mkdocs_publisher/minifier/plugin.py
+-rw-r--r--   0        0        0     5314 2023-06-13 10:09:11.356437 mkdocs_publisher-1.0.0/mkdocs_publisher/obsidian/backlinks.py
+-rw-r--r--   0        0        0     4863 2023-06-13 10:09:11.356755 mkdocs_publisher-1.0.0/mkdocs_publisher/obsidian/callout.py
+-rw-r--r--   0        0        0     1283 2023-06-13 10:09:11.357008 mkdocs_publisher-1.0.0/mkdocs_publisher/obsidian/config.py
+-rw-r--r--   0        0        0     4691 2023-06-13 10:09:11.357226 mkdocs_publisher-1.0.0/mkdocs_publisher/obsidian/md_links.py
+-rw-r--r--   0        0        0     6676 2023-06-13 10:09:11.357483 mkdocs_publisher-1.0.0/mkdocs_publisher/obsidian/plugin.py
+-rw-r--r--   0        0        0     3066 2023-06-13 10:09:11.357744 mkdocs_publisher-1.0.0/mkdocs_publisher/obsidian/vega.py
+-rw-r--r--   0        0        0      898 2023-06-13 10:09:11.357942 mkdocs_publisher-1.0.0/mkdocs_publisher/social/config.py
+-rw-r--r--   0        0        0     3873 2023-06-13 10:09:11.358280 mkdocs_publisher-1.0.0/mkdocs_publisher/social/plugin.py
+-rw-r--r--   0        0        0     2452 2023-06-13 10:09:11.359245 mkdocs_publisher-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5675 1970-01-01 00:00:00.000000 mkdocs_publisher-1.0.0/PKG-INFO
```

### Comparing `mkdocs-publisher-0.5.0/mkdocs_publisher/_cli/post.py` & `mkdocs_publisher-1.0.0/mkdocs_publisher/_cli/post.py`

 * *Files identical despite different names*

### Comparing `mkdocs-publisher-0.5.0/mkdocs_publisher/_extra/assets/stylesheets/blog.css` & `mkdocs_publisher-1.0.0/mkdocs_publisher/_extra/assets/stylesheets/blog.css`

 * *Files identical despite different names*

### Comparing `mkdocs-publisher-0.5.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css.map` & `mkdocs_publisher-1.0.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-publisher-0.5.0/mkdocs_publisher/_extra/assets/templates/posts-list.html` & `mkdocs_publisher-1.0.0/mkdocs_publisher/_extra/assets/templates/posts-list.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% for post in posts %}
-## [{{ post.title }}]({{ site_url }}/{{ config.slug }}/{{ post.slug }}/)
+## [{{ post.title }}]({{ site_url }}{{ config.slug }}/{{ post.slug }}/)
 
 <div class="post-extra">
     <div class="col">
         <p class="post-date">{{ post.date }}</p>
     </div>
     <div class="col">
     {% for tag in post.tags %}
@@ -15,15 +15,15 @@
 {{ post.teaser }}
 
 {{ post.is_short }}
 
 
 <div class="post-link">
 {% if post.is_teaser %}
-    <a href="{{ site_url }}/{{ config.slug }}/{{ post.slug }}/" title="{ post.title }">
+    <a href="{{ site_url }}{{ config.slug }}/{{ post.slug }}/" title="{ post.title }">
         {{ translation.teaser_link_text }}
     </a>
 {% else %}
     &nbsp;
 {% endif %}
 </div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% for post in posts %} ## [{{ post.title }}]({{ site_url }}/{{ config.slug }}/
-{{ post.slug }}/)
+{% for post in posts %} ## [{{ post.title }}]({{ site_url }}{{ config.slug }}/{
+{ post.slug }}/)
 {{ post.date }}
 {% for tag in post.tags %} #{{_tag_}} {% endfor %}
 {{ post.teaser }} {{ post.is_short }}
 {% if post.is_teaser %} {{_translation.teaser_link_text_}} {% else %}   {%
 endif %}
 {% endfor %}
```

### Comparing `mkdocs-publisher-0.5.0/mkdocs_publisher/blog/config.py` & `mkdocs_publisher-1.0.0/mkdocs_publisher/blog/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,24 +13,30 @@
     categories_navigation_name = option.Optional(option.Type(str))
     tags_page_title = option.Optional(option.Type(str))
     tags_navigation_name = option.Optional(option.Type(str))
     newer_posts = option.Optional(option.Type(str))
     older_posts = option.Optional(option.Type(str))
 
 
+class _BlogCommentsConfig(Config):
+    enabled = option.Type(bool, default=False)
+    key_name = option.Type(str, default="comments")
+
+
 class BlogPluginConfig(Config):
     # General settings
     lang = option.Choice(["en", "pl"], default="en")  # TODO: auto update based on files
     teaser_marker = option.Type(str, default="<!-- more -->")
+    searchable_non_posts = option.Type(bool, default=False)
     posts_per_page = option.Type(int, default=5)
-    start_page = option.Type(bool, default=False)
     slug = option.Type(str, default="blog")
 
     # Directories
     temp_dir = option.Type(str, default=".temp")
     blog_dir = option.Type(str, default="blog")
     archive_subdir = option.Type(str, default="archive")
     categories_subdir = option.Type(str, default="categories")
     tags_subdir = option.Type(str, default="tags")
 
+    comments: _BlogCommentsConfig = option.SubConfig(_BlogCommentsConfig)  # type: ignore
     # Values that are in lang files and can be overriden
     translation: _BlogTranslationConfig = option.SubConfig(_BlogTranslationConfig)  # type: ignore
```

### Comparing `mkdocs-publisher-0.5.0/mkdocs_publisher/blog/creators.py` & `mkdocs_publisher-1.0.0/mkdocs_publisher/blog/creators.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 from typing import cast
 
 import frontmatter
 import jinja2
 from mkdocs.structure.files import File
 from mkdocs.structure.files import Files
 
+from mkdocs_publisher._common.url import slugify
 from mkdocs_publisher._extra.assets import templates
 from mkdocs_publisher.blog.structures import BlogConfig
+from mkdocs_publisher.obsidian.md_links import MarkdownLinks
 
 log = logging.getLogger("mkdocs.plugins.publisher.blog")
 
 
 def create_blog_files(
     blog_config: BlogConfig,
     files: Files,
@@ -34,36 +36,33 @@
             )
             files.append(file)
         except ValueError:
             pass
 
 
 def create_blog_post_pages(
+    start_page: bool,
     blog_config: BlogConfig,
     config_nav: OrderedDict,
 ) -> None:
     """Create blog posts index files."""
 
     log.info("Creating blog posts index files")
-
     posts_chunks: Dict[str, list] = {}
     archive_chunks: Dict[str, list] = {}
     categories_chunks: Dict[str, list] = {}
     tags_chunks: Dict[str, list] = {}
 
     # Build post index pages
     for index, date in enumerate(sorted(blog_config.blog_posts, reverse=True)):
         index = (
             "index"
-            if blog_config.plugin_config.start_page
-            and index < blog_config.plugin_config.posts_per_page
+            if start_page and index < blog_config.plugin_config.posts_per_page
             else f"index-{str(index//blog_config.plugin_config.posts_per_page)}"
         )
-        # if not blog_config.plugin_config.start_page and index == "index-0":
-        #     index = blog_config.plugin_config.slug
         if index not in posts_chunks:
             posts_chunks[index] = []
         posts_chunks[index].append(blog_config.blog_posts[date])
 
     # Build archive, category and tag pages
     for date in sorted(blog_config.blog_posts, reverse=True):
         date: datetime
@@ -86,15 +85,15 @@
             tags_chunks[tag].append(blog_config.blog_posts[date].as_dict)
 
     # Reorder categories alphabetically
     categories_chunks = {cat: categories_chunks[cat] for cat in sorted(categories_chunks)}
 
     # Reorder tags alphabetically
     tags_chunks = {tag: tags_chunks[tag] for tag in sorted(tags_chunks)}
-    config_nav[blog_config.translation.blog_navigation_name] = {}
+    config_nav[blog_config.translation.blog_navigation_name] = []
 
     for key, single_posts_chunk in posts_chunks.items():
         file_name = f"{key}.md"
         file_path = blog_config.temp_dir / file_name
 
         _render_and_write_page(
             single_posts_chunk=single_posts_chunk,
@@ -102,53 +101,57 @@
             blog_config=blog_config,
             page_title=blog_config.translation.blog_page_title,
         )
 
         blog_config.temp_files[f"{blog_config.translation.blog_navigation_name}/{key}"] = file_path
         log.debug(f"Creating blog post chunk file: {file_path}")
 
-        config_nav[blog_config.translation.blog_navigation_name][key] = f"{file_name}"
+        config_nav[blog_config.translation.blog_navigation_name].append({key: file_name})
 
-    _create_pages(
-        blog_config=blog_config,
-        posts_chunks=archive_chunks,
-        config_nav=config_nav[blog_config.translation.blog_navigation_name],
-        sub_dir=Path(blog_config.plugin_config.archive_subdir),
-        navigation_name=blog_config.translation.archive_navigation_name,
-        page_title=blog_config.translation.archive_page_title,
+    config_nav[blog_config.translation.blog_navigation_name].append(
+        {
+            blog_config.translation.archive_navigation_name: _create_pages(
+                blog_config=blog_config,
+                posts_chunks=archive_chunks,
+                sub_dir=Path(blog_config.plugin_config.archive_subdir),
+                page_title=blog_config.translation.archive_page_title,
+            )
+        }
     )
 
-    _create_pages(
-        blog_config=blog_config,
-        posts_chunks=categories_chunks,
-        config_nav=config_nav[blog_config.translation.blog_navigation_name],
-        sub_dir=Path(blog_config.plugin_config.categories_subdir),
-        navigation_name=blog_config.translation.categories_navigation_name,
-        page_title=blog_config.translation.categories_page_title,
+    config_nav[blog_config.translation.blog_navigation_name].append(
+        {
+            blog_config.translation.categories_navigation_name: _create_pages(
+                blog_config=blog_config,
+                posts_chunks=categories_chunks,
+                sub_dir=Path(blog_config.plugin_config.categories_subdir),
+                page_title=blog_config.translation.categories_page_title,
+            )
+        }
     )
 
-    _create_pages(
-        blog_config=blog_config,
-        posts_chunks=tags_chunks,
-        config_nav=config_nav[blog_config.translation.blog_navigation_name],
-        sub_dir=Path(blog_config.plugin_config.tags_subdir),
-        navigation_name=blog_config.translation.tags_navigation_name,
-        page_title=blog_config.translation.tags_page_title,
+    config_nav[blog_config.translation.blog_navigation_name].append(
+        {
+            blog_config.translation.tags_navigation_name: _create_pages(
+                blog_config=blog_config,
+                posts_chunks=tags_chunks,
+                sub_dir=Path(blog_config.plugin_config.tags_subdir),
+                page_title=blog_config.translation.tags_page_title,
+            )
+        }
     )
 
 
 def _create_pages(
     blog_config: BlogConfig,
     posts_chunks: Dict[str, list],
-    config_nav: OrderedDict,
     sub_dir: Path,
-    navigation_name: str,
     page_title: str,
-):
-    config_nav[navigation_name] = {}
+) -> list[dict[str, str]]:
+    config_nav = []
 
     # pages_dir = blog_config.docs_dir / blog_config.blog_dir / sub_dir
 
     blog_temp_dir = blog_config.temp_dir / blog_config.plugin_config.slug
     blog_temp_dir.mkdir(exist_ok=True)
 
     pages_dir = blog_temp_dir / sub_dir
@@ -163,17 +166,16 @@
             blog_config=blog_config,
             page_title=f"{page_title} - {key}",
         )
 
         blog_config.temp_files[f"{sub_dir}/{key}"] = file_path
         log.debug(f"Creating blog post chunk file: {file_path}")
 
-        config_nav[navigation_name][
-            key
-        ] = f"{blog_config.plugin_config.slug}/{sub_dir}/{file_name}"
+        config_nav.append({key: f"{blog_config.plugin_config.slug}/{sub_dir}/{file_name}"})
+    return config_nav
 
 
 def _render_and_write_page(
     single_posts_chunk: list,
     file_path: Path,
     blog_config: BlogConfig,
     page_title: str,
@@ -186,13 +188,33 @@
     context = {
         "posts": single_posts_chunk,
         "site_url": str(blog_config.mkdocs_config.site_url),
         "config": blog_config.plugin_config,
         "translation": blog_config.translation,
     }
     template = jinja2.Environment(loader=jinja2.BaseLoader()).from_string(index_template)
+    markdown = template.render(context)
+
+    md_links = MarkdownLinks(
+        mkdocs_config=blog_config.mkdocs_config, disable_lazy_loading_override=True
+    )
+    markdown = md_links.normalize(markdown=markdown, file_path=str(file_path))
+    markdown = md_links.fix_relative_paths(markdown=markdown)
 
-    page = frontmatter.Post(content=template.render(context))
+    # TODO: when using pub-meta key name should be taken from plugin config
+    page = frontmatter.Post(content=markdown)
     page["title"] = page_title
+    # TODO: consider moving slugify configuration to mkdocs.yaml
+    if file_path.name.startswith("index-0"):
+        slug = blog_config.plugin_config.slug
+    elif file_path.name.startswith("index"):
+        slug = f"{blog_config.plugin_config.slug}/{file_path.stem.split('-')[-1]}"
+    else:
+        slug = slugify(text=page_title.split("-")[-1].strip())
+    page["slug"] = slug
+
+    page["status"] = "published"
+    if not blog_config.plugin_config.searchable_non_posts:
+        page["search"] = {"exclude": True}
 
     with open(file_path, mode="wb") as teasers_index:
         frontmatter.dump(page, teasers_index)
```

### Comparing `mkdocs-publisher-0.5.0/mkdocs_publisher/blog/parsers.py` & `mkdocs_publisher-1.0.0/mkdocs_publisher/blog/parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,65 +19,73 @@
     """Count words in markdown content.
 
     This code is based on: https://github.com/gandreadis/markdown-word-count
     """
     content = re.sub(r"<!--(.*?)-->", "", content, flags=re.MULTILINE)  # Comments
     content = content.replace("\t", "    ")  # Tabs to spaces
     content = re.sub(r"[ ]{2,}", "    ", content)  # More than 1 space to 4 spaces
-    content = re.sub(r"^\[[^]]*\][^(].*", "", content, flags=re.MULTILINE)  # Footnotes
+    content = re.sub(r"^\[[^]]*][^(].*", "", content, flags=re.MULTILINE)  # Footnotes
     content = re.sub(
         r"^( {4,}[^-*]).*", "", content, flags=re.MULTILINE
     )  # Indented blocks of code
     content = re.sub(r"{#.*}", "", content)  # Custom header IDs
     content = content.replace("\n", " ")  # Replace newlines with spaces for uniform handling
-    content = re.sub(r"!\[[^\]]*\]\([^)]*\)", "", content)  # Remove images
+    content = re.sub(r"!\[[^]]*]\([^)]*\)", "", content)  # Remove images
     content = re.sub(r"</?[^>]*>", "", content)  # Remove HTML tags
     content = re.sub(r"[#*`~\-–^=<>+|/:]", "", content)  # Remove special characters
-    content = re.sub(r"\[[0-9]*\]", "", content)  # Remove footnote references
+    content = re.sub(r"\[[0-9]*]", "", content)  # Remove footnote references
     content = re.sub(r"[0-9#]*\.", "", content)  # Remove enumerations
 
     return len(content.split())
 
 
+# from mkdocs.utils import meta as meta_parser
+# with file.open(encoding="utf-8-sig", errors="strict") as md_file:
+#     markdown, meta = meta_parser.get_data(md_file.read())
+
+
 def parse_markdown_files(
     blog_config: BlogConfig,
     config_nav: OrderedDict,
+    on_serve: bool = False,
 ):
     """Parse all markdown files and extract blog posts from `blog_dir` (default: 'posts').
     BlogPost object is created and filled with content and metadata of the post.
     """
     log.info(f"Parsing blog posts from '{blog_config.blog_dir}' directory")
-    for file_path in blog_config.docs_dir.glob("**/*"):
-        if blog_config.auto_nav_config is not None:
-            if file_path.parts[-1] == blog_config.auto_nav_config.meta_file_name:
+    for file_path in blog_config.docs_dir.glob("**/*.md"):
+        if blog_config.meta_config is not None:
+            if file_path.parts[-1] == blog_config.meta_config.dir_meta_file:
                 continue
         file_path = Path(file_path)
         path = Path(file_path).relative_to(blog_config.docs_dir)
-        if (
-            file_path.is_file()
-            and path.is_relative_to(blog_config.blog_dir)
-            and path.suffix == ".md"
-        ):
+        if path.is_relative_to(blog_config.blog_dir):
             parents = list(path.parents)[:-1]
             with open(file_path) as markdown_file:
                 post: frontmatter.Post = frontmatter.load(markdown_file)
                 if not parents:
                     for line in post.content.split("\n"):
                         if line.startswith("# "):
                             config_nav[line[2:]] = str(path)
                 elif str(parents[0]) == str(blog_config.blog_dir):
                     post_meta = dict(post)
 
                     if "status" not in post_meta:
+                        # TODO: read default value from meta config
                         log.info(
                             f"File: {file_path} - missing 1 required positional argument: "
                             f"'status' (setting to default: draft)"
                         )
                         post_meta["status"] = "draft"
 
+                    # Skip non published
+                    if not on_serve and post_meta["status"] != "published":
+                        # TODO: make it configurable
+                        continue
+
                     # Convert tags format
                     if "tags" in post_meta and post_meta["tags"] is not None:
                         if "," in post_meta["tags"]:
                             post_meta["tags"] = [t.strip() for t in post_meta["tags"].split(",")]
                         elif isinstance(post_meta["tags"], str):
                             post_meta["tags"] = [post_meta["tags"]]
                     else:
```

### Comparing `mkdocs-publisher-0.5.0/mkdocs_publisher/blog/plugin.py` & `mkdocs_publisher-1.0.0/mkdocs_publisher/blog/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,135 +1,126 @@
-import importlib
-import importlib.resources
-import importlib.util
 import logging
 from collections import OrderedDict
-from datetime import datetime
 from pathlib import Path
 from typing import Any
 from typing import Dict
+from typing import Literal
 from typing import Optional
 from typing import cast
 
 from mkdocs.config import Config
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.plugins import BasePlugin
 from mkdocs.plugins import event_priority
-from mkdocs.structure.files import File
 from mkdocs.structure.files import Files
 from mkdocs.structure.nav import Navigation
 from mkdocs.structure.pages import Page
 
 from mkdocs_publisher import _utils
+from mkdocs_publisher._common import resources
 from mkdocs_publisher.blog import creators
 from mkdocs_publisher.blog import modifiers
 from mkdocs_publisher.blog import parsers
 from mkdocs_publisher.blog.config import BlogPluginConfig
 from mkdocs_publisher.blog.structures import BlogConfig
 
 log = logging.getLogger("mkdocs.plugins.publisher.blog")
 
 
 class BlogPlugin(BasePlugin[BlogPluginConfig]):
     def __init__(self):
         self.blog_config = BlogConfig()  # Empty instance
-        self.temp_files: Dict[str, Path] = {}
+        self._start_page: bool = False
+        self._on_serve: bool = False
+
+    def on_startup(self, *, command: Literal["build", "gh-deploy", "serve"], dirty: bool) -> None:
+        if command == "serve":
+            self._on_serve = True
 
     def on_config(self, config: MkDocsConfig) -> Config:
 
         # Initialization of all the values
         self.blog_config.parse_configs(mkdocs_config=config, plugin_config=self.config)
 
+        # Modify nav section
+        if config.nav is None:
+            config.nav = [{str(self.blog_config.blog_dir): str(self.blog_config.blog_dir)}]
+
+        # Detect if blog is a starting page
+        if len(config.nav) > 0:
+            first_value = list(config.nav[0].values())[0]
+            if isinstance(first_value, str) and first_value == str(self.blog_config.blog_dir):
+                self._start_page = True
+
         # New config navigation
         config_nav = OrderedDict()
         parsers.parse_markdown_files(
             blog_config=self.blog_config,
             config_nav=config_nav,
+            on_serve=self._on_serve,
         )
 
         parsers.create_blog_post_teaser(
             blog_config=self.blog_config,
         )
 
         creators.create_blog_post_pages(
+            start_page=self._start_page,
             blog_config=self.blog_config,
             config_nav=config_nav,
         )
 
         modifiers.blog_post_nav_sorter(
             blog_config=self.blog_config,
             config_nav=config_nav,
         )
 
-        # Modify nav section
+        # Inject blog into navigation
         new_nav = []
-        if config.nav is None:
-            if self.blog_config.plugin_config.start_page:
-                config.nav = [{str(self.blog_config.blog_dir): str(self.blog_config.blog_dir)}]
-            else:
-                config.nav = []
-        for n in cast(list, config.nav):
-            if str(self.blog_config.blog_dir) in n.values():
+        for nav_item in cast(list, config.nav):
+            if str(self.blog_config.blog_dir) in nav_item.values():
                 for k, v in config_nav.items():
                     new_nav.append({k: v})
             else:
-                new_nav.append(n)
+                new_nav.append(nav_item)
         config.nav = new_nav
 
         return config
 
     def on_nav(self, nav: Navigation, config: MkDocsConfig, files: Files) -> Navigation:
 
-        modifiers.blog_post_nav_remove(blog_config=self.blog_config, nav=nav)
+        modifiers.blog_post_nav_remove(
+            start_page=self._start_page, blog_config=self.blog_config, nav=nav
+        )
 
         return nav
 
     def on_files(self, files: Files, config: MkDocsConfig) -> Files:
 
         creators.create_blog_files(blog_config=self.blog_config, files=files)
 
-        new_files = modifiers.blog_post_slug_modifier(
-            blog_config=self.blog_config,
-            files=files,
-        )
-
-        # TODO: add as _utils and split into blog specific path
-        config.extra_css.append("assets/stylesheets/blog.min.css")
+        resources.add_extra_css(stylesheet_file_name="blog.min.css", config=config, files=files)
 
-        with importlib.resources.path(
-            importlib.import_module("mkdocs_publisher._extra"), "__init__.py"
-        ) as extra_path:
-            s = importlib.import_module("mkdocs_publisher._extra.assets.stylesheets")
-            with importlib.resources.path(s, "blog.min.css") as blog_stylesheets:
-                new_files.append(
-                    File(
-                        path=str(blog_stylesheets.relative_to(extra_path.parent)),
-                        src_dir=str(extra_path.parent),
-                        dest_dir=str(self.blog_config.site_dir),
-                        use_directory_urls=self.blog_config.mkdocs_config.use_directory_urls,
-                    )
-                )
-
-        return new_files
-
-    def on_page_markdown(self, markdown: str, *, page: Page, config: MkDocsConfig, files: Files):
-        # Modify page update date
-        # TODO: move to meta-apply plugin
-        # TODO: move date format to config
-        update_date: datetime = page.meta.get(
-            "update", page.meta.get("date", datetime.strptime(page.update_date, "%Y-%m-%d"))
-        )
-        page.update_date = update_date.strftime("%Y-%m-%d")
+        return files
 
     @event_priority(-100)  # Run after all other plugins
     def on_page_context(
         self, context: Dict[str, Any], *, page: Page, config: MkDocsConfig, nav: Navigation
     ) -> Optional[Dict[str, Any]]:
 
-        modifiers.blog_post_nav_next_prev_change(blog_config=self.blog_config, page=page)
+        if Path(page.file.src_path).parts[0] == self.config.blog_dir:
+            page.meta[self.config.comments.key_name] = self.config.comments.enabled
+
+        # Temporary created files cannot be edited
+        if page.file.src_uri in self.blog_config.temp_files_list:
+            page.edit_url = None
+
+        modifiers.blog_post_nav_next_prev_change(
+            start_page=self._start_page, blog_config=self.blog_config, page=page
+        )
         return context
 
     @event_priority(-100)  # Run after all other plugins
     def on_build_error(self, error: Exception) -> None:
 
         _utils.remove_dir(directory=self.blog_config.temp_dir)
```

### Comparing `mkdocs-publisher-0.5.0/mkdocs_publisher/blog/structures.py` & `mkdocs_publisher-1.0.0/mkdocs_publisher/blog/structures.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import cast
 
 from mkdocs.config.defaults import MkDocsConfig
 
-from mkdocs_publisher import _utils
-from mkdocs_publisher.auto_nav.config import AutoNavPluginConfig
-from mkdocs_publisher.auto_nav.plugin import AutoNavPlugin
+from mkdocs_publisher._common import mkdocs_utils
 from mkdocs_publisher.blog.config import BlogPluginConfig
+from mkdocs_publisher.meta.config import MetaPluginConfig
 
 
 @dataclass
 class BlogPost:
     """Single blog post data container"""
 
     title: str
@@ -55,35 +54,38 @@
         return asdict(self)
 
 
 @dataclass
 class BlogConfig:
     mkdocs_config: MkDocsConfig = field(init=False)
     plugin_config: BlogPluginConfig = field(init=False)
-    auto_nav_config: Optional[AutoNavPluginConfig] = field(init=False, default=None)
+    meta_config: Optional[MetaPluginConfig] = field(init=False, default=None)
     translation: Translation = field(init=False)
     temp_dir: Path = field(init=False)
     docs_dir: Path = field(init=False)
     blog_dir: Path = field(init=False)
     site_dir: Path = field(init=False)
     blog_posts: Dict[datetime, BlogPost] = field(init=False, default_factory=lambda: dict())
     temp_files: Dict[str, Path] = field(init=False, default_factory=lambda: dict())
 
+    @property
+    def temp_files_list(self) -> List[str]:
+        temp_files = []
+        for path in self.temp_files.values():
+            temp_files.append(str(path.relative_to(self.temp_dir)))
+        return temp_files
+
     def parse_configs(self, mkdocs_config: MkDocsConfig, plugin_config: BlogPluginConfig):
         from mkdocs_publisher.blog.translate import Translate
 
         self.mkdocs_config = mkdocs_config
         self.plugin_config = plugin_config
-        self.auto_nav_config = cast(
-            AutoNavPluginConfig,
-            _utils.get_plugin_config(
-                plugin=AutoNavPlugin(),
-                config_file_path=cast(str, plugin_config.config_file_path),
-                yaml_config_key="pub-auto-nav",
-            ),
+        self.meta_config: Optional[MetaPluginConfig] = cast(
+            MetaPluginConfig,
+            mkdocs_utils.get_plugin_config(mkdocs_config=mkdocs_config, plugin_name="pub-meta"),
         )
         self.temp_dir = Path(plugin_config.temp_dir)
         self.docs_dir = Path(mkdocs_config.docs_dir)
         self.blog_dir = Path(plugin_config.blog_dir)
         self.site_dir = Path(mkdocs_config.site_dir)
         self.translation = Translate(config=plugin_config).translation
```

### Comparing `mkdocs-publisher-0.5.0/mkdocs_publisher/blog/translate.py` & `mkdocs_publisher-1.0.0/mkdocs_publisher/blog/translate.py`

 * *Files identical despite different names*

### Comparing `mkdocs-publisher-0.5.0/mkdocs_publisher/minifier/base.py` & `mkdocs_publisher-1.0.0/mkdocs_publisher/minifier/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     def minifier(self, cached_file: CachedFile) -> Optional[CachedFile]:
         raise NotImplementedError
 
     def __call__(self):
         log.info(f"Minifying {self.extensions} files")
 
         if self._plugin_config.threads < 1:
-            log.warning("Number of 'threads' cannot be smaller than 1 (changing to default 8")
+            log.warning("Number of 'threads' cannot be smaller than 1 (changing to default 8)")
             self._plugin_config.threads = 1
 
         semaphore = Semaphore(self._plugin_config.threads)
         threads = []
 
         # TODO: add possibility to exclude some files
         for file in _utils.list_files(
```

### Comparing `mkdocs-publisher-0.5.0/mkdocs_publisher/minifier/config.py` & `mkdocs_publisher-1.0.0/mkdocs_publisher/minifier/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class _MinifierHtmlConfig(Config):
     enabled = option.Type(bool, default=True)
     html_minifier_path = option.Type(str, default="html-minifier")
     case_sensitive = option.Type(bool, default=True)
     minify_css = option.Type(bool, default=True)
     minify_js = option.Type(bool, default=True)
     remove_comments = option.Type(bool, default=True)
-    remove_tag_whitespace = option.Type(bool, default=True)
+    remove_tag_whitespace = option.Type(bool, default=False)
     collapse_whitespace = option.Type(bool, default=True)
     conservative_collapse = option.Type(bool, default=True)
     collapse_boolean_attributes = option.Type(bool, default=True)
     preserve_line_breaks = option.Type(bool, default=True)
     sort_attributes = option.Type(bool, default=True)
     sort_class_name = option.Type(bool, default=True)
     max_line_length = option.Choice(
```

### Comparing `mkdocs-publisher-0.5.0/mkdocs_publisher/minifier/minifiers.py` & `mkdocs_publisher-1.0.0/mkdocs_publisher/minifier/minifiers.py`

 * *Files identical despite different names*

### Comparing `mkdocs-publisher-0.5.0/mkdocs_publisher/minifier/plugin.py` & `mkdocs_publisher-1.0.0/mkdocs_publisher/minifier/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-publisher-0.5.0/mkdocs_publisher/social/config.py` & `mkdocs_publisher-1.0.0/mkdocs_publisher/social/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from mkdocs.config import config_options as option
 from mkdocs.config.base import Config
 
 
 class _SocialOpenGraphConfig(Config):
     enabled = option.Type(bool, default=True)
-    locale = option.Type(str, default="en_us")
+    locale = option.Type(str, default="en_US")
 
 
 class _SocialTwitterConfig(Config):
     enabled = option.Type(bool, default=True)
     website = option.Type(str, default="")
     author = option.Type(str, default="")
```

### Comparing `mkdocs-publisher-0.5.0/mkdocs_publisher/social/plugin.py` & `mkdocs_publisher-1.0.0/mkdocs_publisher/social/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import logging
 from pathlib import Path
-from typing import List
 from typing import Optional
 
-from bs4 import BeautifulSoup
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.plugins import BasePlugin
 from mkdocs.plugins import event_priority
 from mkdocs.structure.pages import Page
 
+from mkdocs_publisher._common.html_modifiers import HTMLModifier
 from mkdocs_publisher.social.config import SocialConfig
 
 log = logging.getLogger("mkdocs.plugins.publisher.social")
 
 TWITTER_PROPERTIES = [
     "twitter:title",
     "twitter:description",
@@ -28,78 +27,71 @@
     "og:url",
     "og:image",
     "og:site_name",
     "og:locale",
 ]
 
 
-def _remove_properties_from_head(soup: BeautifulSoup, properties: List[str]):
-    """Remove meta tags with given properties from HTML head section"""
-    for prop in properties:
-        head_property = soup.head.find(name="meta", attr={"property": prop})  # type: ignore
-        if head_property is not None:
-            head_property.extract()
-
-
-def _add_meta_property(soup: BeautifulSoup, name: str, value: str):
-    soup.head.append(soup.new_tag(name="meta", attrs={"property": name, "content": value}))  # type: ignore
-
-
 class SocialPlugin(BasePlugin[SocialConfig]):
     @event_priority(-99)
     def on_post_page(self, output: str, *, page: Page, config: MkDocsConfig) -> Optional[str]:
-        soup: BeautifulSoup = BeautifulSoup(markup=output, features="html.parser")
+        html_modifier = HTMLModifier(markup=output)
 
-        # Remove old values
-        _remove_properties_from_head(soup=soup, properties=OPEN_GRAPH_PROPERTIES)
-        _remove_properties_from_head(soup=soup, properties=TWITTER_PROPERTIES)
+        log.debug("Removing old properties")
+        html_modifier.remove_meta_properties(properties=OPEN_GRAPH_PROPERTIES)
+        html_modifier.remove_meta_properties(properties=TWITTER_PROPERTIES)
 
         # Get all needed meta values
         title = page.meta.get(self.config.meta_keys.title_key, None)
         description = page.meta.get(self.config.meta_keys.description_key, None)
         image = page.meta.get(self.config.meta_keys.image_key, None)
         if image is not None:
-            image_path = Path(config.docs_dir) / Path(
-                image[1:] if str(image).startswith("/") else image
-            )
+            image = str(image)
+            # TODO: use obsidian path link solver when it will be developed
+            if image.startswith("../"):
+                image = f"/{image.replace('../', '')}"
+            if image.startswith("/"):
+                image = image[1:]
+            image_path = Path(config.docs_dir) / Path(image)
             if not image_path.exists():
                 log.warning(
                     f"File: '{str(image)}' doesn't exists!\n"
                     f"('{self.config.meta_keys.image_key}' meta key"
                     f" from '{page.file.src_path}' file.)"
                 )
-            image = f"{config.site_url}{image}".replace("//", "/")
+            image = f'{config.site_url}{image.replace("//", "/")}'
         url = f"{config.site_url}{page.url}"
         site_name = config.site_name
-        # Add all open graph values
+
         if self.config.og.enabled and title and description:
-            _add_meta_property(soup=soup, name="og:type", value="article")
-            _add_meta_property(soup=soup, name="og:title", value=title)
-            _add_meta_property(soup=soup, name="og:description", value=description)
-            _add_meta_property(soup=soup, name="og:site_name", value=site_name)
-            _add_meta_property(soup=soup, name="og:locale", value=self.config.og.locale)
-            _add_meta_property(soup=soup, name="og:url", value=url)
+            log.debug("Adding open graph properties")
+            html_modifier.add_meta_property(name="og:type", value="article")
+            html_modifier.add_meta_property(name="og:title", value=title)
+            html_modifier.add_meta_property(name="og:description", value=description)
+            html_modifier.add_meta_property(name="og:site_name", value=site_name)
+            html_modifier.add_meta_property(name="og:locale", value=self.config.og.locale)
+            html_modifier.add_meta_property(name="og:url", value=url)
 
             if image is not None:
-                _add_meta_property(soup=soup, name="og:image", value=image)
+                html_modifier.add_meta_property(name="og:image", value=image)
 
-        # Add all twitter values
         if self.config.twitter.enabled and title and description:
+            log.debug("Adding Twitter cards values")
             card_type = "summary_large_image" if image else "summary"
-            _add_meta_property(soup=soup, name="twitter:card", value=card_type)
-            _add_meta_property(soup=soup, name="twitter:title", value=title)
-            _add_meta_property(soup=soup, name="twitter:description", value=description)
+            html_modifier.add_meta_property(name="twitter:card", value=card_type)
+            html_modifier.add_meta_property(name="twitter:title", value=title)
+            html_modifier.add_meta_property(name="twitter:description", value=description)
 
             if image is not None:
-                _add_meta_property(soup=soup, name="twitter:image", value=image)
+                html_modifier.add_meta_property(name="twitter:image", value=image)
 
             if self.config.twitter.website:
-                _add_meta_property(
-                    soup=soup, name="twitter:site", value=self.config.twitter.website
+                html_modifier.add_meta_property(
+                    name="twitter:site", value=self.config.twitter.website
                 )
 
             if self.config.twitter.author:
-                _add_meta_property(
-                    soup=soup, name="twitter:creator", value=self.config.twitter.author
+                html_modifier.add_meta_property(
+                    name="twitter:creator", value=self.config.twitter.author
                 )
 
-        return soup.prettify()
+        return str(html_modifier)
```

### Comparing `mkdocs-publisher-0.5.0/pyproject.toml` & `mkdocs_publisher-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 [tool.poetry]
 name = "mkdocs-publisher"
-version = "0.5.0"
+version = "1.0.0"
 description = "Publishing plugins for MkDocs"
 authors = ["Maciej 'maQ' Kusz <maciej.kusz@gmail.com>"]
 license = "BSD"
 readme = "README.md"
 keywords = [
     "mkdocs",
     "mkdocs-plugin",
     "publisher",
     "blog",
     "minifier",
     "frontmatter",
     "tags",
-    "navigation"
+    "navigation",
+    "documentation",
+    "obsidian"
 ]
 packages = [
     {include = "mkdocs_publisher"},
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
-    "License :: OSI Approved :: BSD License",
+    "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
@@ -42,15 +44,15 @@
 "Bug Tracker" = "https://github.com/mkusz/mkdocs-publisher/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-frontmatter = "^1.0.0"
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.1.3"
-pymdown-extensions = "^9.10"
+pymdown-extensions = "^10"
 beautifulsoup4 = "^4.12.0"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 black = "^22.12.0"
 pyright = "^1.1.291"
 flake8 = "^6.0.0"
@@ -83,14 +85,15 @@
     "tests",
 ]
 reportMissingImports = false
 reportMissingTypeStubs = false
 typeCheckingMode = "basic"
 
 [tool.poetry.plugins."mkdocs.plugins"]
-pub-auto-nav = "mkdocs_publisher.auto_nav.plugin:AutoNavPlugin"
 pub-blog = "mkdocs_publisher.blog.plugin:BlogPlugin"
+pub-meta = "mkdocs_publisher.meta.plugin:MetaPlugin"
 pub-minifier = "mkdocs_publisher.minifier.plugin:MinifierPlugin"
+pub-obsidian = "mkdocs_publisher.obsidian.plugin:ObsidianPlugin"
 pub-social = "mkdocs_publisher.social.plugin:SocialPlugin"
 
 [tool.poetry.scripts]
-publisher = "mkdocs_publisher._cli.publisher:app"
+mkdocs-pub = "mkdocs_publisher._cli.publisher:app"
```

