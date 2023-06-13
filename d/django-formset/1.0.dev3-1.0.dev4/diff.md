# Comparing `tmp/django-formset-1.0.dev3.tar.gz` & `tmp/django-formset-1.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-formset-1.0.dev3.tar", last modified: Mon Jun 12 21:30:44 2023, max compression
+gzip compressed data, was "django-formset-1.0.dev4.tar", last modified: Tue Jun 13 15:44:47 2023, max compression
```

## Comparing `django-formset-1.0.dev3.tar` & `django-formset-1.0.dev4.tar`

### file list

```diff
@@ -1,262 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.435379 django-formset-1.0.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-12 21:30:44.435379 django-formset-1.0.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.395378 django-formset-1.0.dev3/django_formset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-12 21:30:44.000000 django-formset-1.0.dev3/django_formset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-06-12 21:30:44.000000 django-formset-1.0.dev3/django_formset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:30:44.000000 django-formset-1.0.dev3/django_formset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:30:44.000000 django-formset-1.0.dev3/django_formset.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 21:30:44.000000 django-formset-1.0.dev3/django_formset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 21:30:44.000000 django-formset-1.0.dev3/django_formset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.395378 django-formset-1.0.dev3/formset/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/boundfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20763 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/fieldset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.387378 django-formset-1.0.dev3/formset/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.387378 django-formset-1.0.dev3/formset/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.395378 django-formset-1.0.dev3/formset/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-12 21:30:36.000000 django-formset-1.0.dev3/formset/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.399378 django-formset-1.0.dev3/formset/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/renderers/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/renderers/bulma.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/renderers/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/renderers/foundation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/renderers/tailwind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/renderers/uikit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.399378 django-formset-1.0.dev3/formset/richtext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/richtext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/richtext/controls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/richtext/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/richtext/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/richtext/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.387378 django-formset-1.0.dev3/formset/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.387378 django-formset-1.0.dev3/formset/static/formset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.399378 django-formset-1.0.dev3/formset/static/formset/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-12 21:30:33.000000 django-formset-1.0.dev3/formset/static/formset/css/bootstrap5-extra.css
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-12 21:30:33.000000 django-formset-1.0.dev3/formset/static/formset/css/bootstrap5-extra.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-12 21:30:33.000000 django-formset-1.0.dev3/formset/static/formset/css/collections.css
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-12 21:30:33.000000 django-formset-1.0.dev3/formset/static/formset/css/collections.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-06-12 21:30:34.000000 django-formset-1.0.dev3/formset/static/formset/css/tailwind.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.403378 django-formset-1.0.dev3/formset/static/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-audio.svg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-font.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-missing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-picture.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-video.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-zip.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.407378 django-formset-1.0.dev3/formset/static/formset/js/
--rw-r--r--   0 runner    (1001) docker     (123)    25407 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/DateTimePicker-OYPFNQAF.js
--rw-r--r--   0 runner    (1001) docker     (123)    55721 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/DjangoSelectize-H6QF7W4R.js
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/DjangoSlug-226MVQ6E.js
--rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/DualSelector-GVLJZFWV.js
--rw-r--r--   0 runner    (1001) docker     (123)   316874 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/RichtextArea-UTSZPGIP.js
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/SortableSelect-4MNY532K.js
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/chunk-AELXO3WZ.js
--rw-r--r--   0 runner    (1001) docker     (123)    43947 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/chunk-APVD22ED.js
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/chunk-IE6INVWL.js
--rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/chunk-ISEEQP4V.js
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/chunk-KDP4ZIAK.js
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/chunk-NLMHZ7JJ.js
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/chunk-O5UGFU32.js
--rw-r--r--   0 runner    (1001) docker     (123)   106347 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/django-formset.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.407378 django-formset-1.0.dev3/formset/static/formset/scss/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/scss/bootstrap5-extra.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/scss/collections.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.391378 django-formset-1.0.dev3/formset/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.387378 django-formset-1.0.dev3/formset/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.407378 django-formset-1.0.dev3/formset/templates/admin/formset/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/admin/formset/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.407378 django-formset-1.0.dev3/formset/templates/calendar/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/calendar/hours.html
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/calendar/months.html
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/calendar/weeks.html
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/calendar/years.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.407378 django-formset-1.0.dev3/formset/templates/formset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.407378 django-formset-1.0.dev3/formset/templates/formset/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.407378 django-formset-1.0.dev3/formset/templates/formset/bootstrap/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/buttons/richtext_align.html
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/buttons/richtext_color.html
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/buttons/richtext_heading.html
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.411378 django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/richtextarea.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.411378 django-formset-1.0.dev3/formset/templates/formset/bulma/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.411378 django-formset-1.0.dev3/formset/templates/formset/bulma/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.411378 django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/select.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.411378 django-formset-1.0.dev3/formset/templates/formset/default/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.415378 django-formset-1.0.dev3/formset/templates/formset/default/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/move_all_left.html
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/move_all_right.html
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/move_selected_left.html
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/move_selected_right.html
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/redo_selected.html
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/richtext_align.html
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/richtext_color.html
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/richtext_control.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/richtext_heading.html
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/richtext_separator.html
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/undo_selected.html
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/dialog_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/field_errors.html
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.415378 django-formset-1.0.dev3/formset/templates/formset/default/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/widgets/datetimepicker.html
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/widgets/richtextarea.html
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/widgets/selectize.html
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/form_attrs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.415378 django-formset-1.0.dev3/formset/templates/formset/foundation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.419378 django-formset-1.0.dev3/formset/templates/formset/foundation/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.419378 django-formset-1.0.dev3/formset/templates/formset/foundation/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/widgets/inlined_input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.427379 django-formset-1.0.dev3/formset/templates/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/add-fill.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/align-center.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/align-justify.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/align-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/align-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/arrow-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/arrow-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/arrow-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/blockquote.svg
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/bold.svg
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/bulletlist.svg
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/calendar-today.svg
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/chevron-double-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/chevron-double-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/clearformat.svg
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/codeblock.svg
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/decreasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/delete-back.svg
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/double-chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/double-chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/hardbreak.svg
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/heading.svg
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/heading1.svg
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/heading2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/heading3.svg
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/heading4.svg
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/heading5.svg
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/heading6.svg
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/horizontalrule.svg
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/increasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/indentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/italic.svg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/letters.svg
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/orderedlist.svg
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/outdentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/placeholder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/questionmark.svg
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/redo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/send.svg
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/separator.svg
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/subscript.svg
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/superscript.svg
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/textcolor.svg
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/trash.svg
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/underline.svg
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/undo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/unlink.svg
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/non_field_errors.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.427379 django-formset-1.0.dev3/formset/templates/formset/tailwind/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.431378 django-formset-1.0.dev3/formset/templates/formset/tailwind/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.431378 django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/radio.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.431378 django-formset-1.0.dev3/formset/templates/formset/uikit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.431378 django-formset-1.0.dev3/formset/templates/formset/uikit/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/uikit/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/uikit/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/uikit/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/uikit/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.431378 django-formset-1.0.dev3/formset/templates/formset/uikit/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/uikit/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/uikit/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/uikit/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/uikit/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.435379 django-formset-1.0.dev3/formset/templates/richtext/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/bulletlist.html
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/doc.html
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/heading.html
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/horizontalrule.html
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/listitem.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.435379 django-formset-1.0.dev3/formset/templates/richtext/marks/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/marks/bold.html
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/marks/code.html
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/marks/italic.html
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/marks/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/marks/textcolor.html
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/marks/underline.html
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/orderedlist.html
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/paragraph.html
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.435379 django-formset-1.0.dev3/formset/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templatetags/formsetify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templatetags/richtext.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 21:30:44.435379 django-formset-1.0.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.719149 django-formset-1.0.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-13 15:44:47.715149 django-formset-1.0.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.675145 django-formset-1.0.dev4/django_formset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-13 15:44:47.000000 django-formset-1.0.dev4/django_formset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-06-13 15:44:47.000000 django-formset-1.0.dev4/django_formset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:44:47.000000 django-formset-1.0.dev4/django_formset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:44:47.000000 django-formset-1.0.dev4/django_formset.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 15:44:47.000000 django-formset-1.0.dev4/django_formset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 15:44:47.000000 django-formset-1.0.dev4/django_formset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.679145 django-formset-1.0.dev4/formset/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/boundfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20763 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/fieldset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.671145 django-formset-1.0.dev4/formset/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.671145 django-formset-1.0.dev4/formset/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.679145 django-formset-1.0.dev4/formset/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-13 15:44:39.000000 django-formset-1.0.dev4/formset/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.679145 django-formset-1.0.dev4/formset/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/renderers/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/renderers/bulma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/renderers/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/renderers/foundation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/renderers/tailwind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/renderers/uikit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.679145 django-formset-1.0.dev4/formset/richtext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/richtext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/richtext/controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/richtext/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/richtext/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/richtext/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.671145 django-formset-1.0.dev4/formset/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.671145 django-formset-1.0.dev4/formset/static/formset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.683146 django-formset-1.0.dev4/formset/static/formset/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-13 15:44:35.000000 django-formset-1.0.dev4/formset/static/formset/css/bootstrap5-extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-13 15:44:35.000000 django-formset-1.0.dev4/formset/static/formset/css/bootstrap5-extra.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-13 15:44:36.000000 django-formset-1.0.dev4/formset/static/formset/css/collections.css
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-13 15:44:36.000000 django-formset-1.0.dev4/formset/static/formset/css/collections.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-06-13 15:44:37.000000 django-formset-1.0.dev4/formset/static/formset/css/tailwind.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.683146 django-formset-1.0.dev4/formset/static/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-audio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-font.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-missing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-picture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-video.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-zip.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.687146 django-formset-1.0.dev4/formset/static/formset/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/DateTimePicker-BBOUOZRC.js
+-rw-r--r--   0 runner    (1001) docker     (123)    55693 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/DjangoSelectize-OIQWF5I5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/DjangoSlug-226MVQ6E.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/DualSelector-2ALH4RIS.js
+-rw-r--r--   0 runner    (1001) docker     (123)   316874 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/RichtextArea-XKK27UIM.js
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/SortableSelect-CEPX3LH6.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43947 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/chunk-APVD22ED.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/chunk-EJ4RWPXK.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/chunk-ISEEQP4V.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/chunk-KDP4ZIAK.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/chunk-MD4VW33H.js
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/chunk-NLMHZ7JJ.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/chunk-R2VNGMYE.js
+-rw-r--r--   0 runner    (1001) docker     (123)   105257 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/django-formset.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.687146 django-formset-1.0.dev4/formset/static/formset/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/scss/bootstrap5-extra.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/scss/collections.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.671145 django-formset-1.0.dev4/formset/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.671145 django-formset-1.0.dev4/formset/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.687146 django-formset-1.0.dev4/formset/templates/admin/formset/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/admin/formset/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.691146 django-formset-1.0.dev4/formset/templates/calendar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/calendar/hours.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/calendar/months.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/calendar/weeks.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/calendar/years.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.691146 django-formset-1.0.dev4/formset/templates/formset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.691146 django-formset-1.0.dev4/formset/templates/formset/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.691146 django-formset-1.0.dev4/formset/templates/formset/bootstrap/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/buttons/richtext_align.html
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/buttons/richtext_color.html
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/buttons/richtext_heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.691146 django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/richtextarea.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.691146 django-formset-1.0.dev4/formset/templates/formset/bulma/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.691146 django-formset-1.0.dev4/formset/templates/formset/bulma/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.695147 django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/select.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.695147 django-formset-1.0.dev4/formset/templates/formset/default/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.695147 django-formset-1.0.dev4/formset/templates/formset/default/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/move_all_left.html
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/move_all_right.html
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/move_selected_left.html
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/move_selected_right.html
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/redo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/richtext_align.html
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/richtext_color.html
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/richtext_control.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/richtext_heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/richtext_separator.html
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/undo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/dialog_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/field_errors.html
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.699147 django-formset-1.0.dev4/formset/templates/formset/default/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/widgets/datetimepicker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/widgets/richtextarea.html
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/widgets/selectize.html
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/form_attrs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.699147 django-formset-1.0.dev4/formset/templates/formset/foundation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.699147 django-formset-1.0.dev4/formset/templates/formset/foundation/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.699147 django-formset-1.0.dev4/formset/templates/formset/foundation/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/widgets/inlined_input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.711148 django-formset-1.0.dev4/formset/templates/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/add-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/align-center.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/align-justify.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/align-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/align-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/arrow-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/arrow-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/arrow-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/blockquote.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/bold.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/bulletlist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/calendar-today.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/chevron-double-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/chevron-double-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/clearformat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/codeblock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/decreasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/delete-back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/double-chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/double-chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/hardbreak.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/heading.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/heading1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/heading2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/heading3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/heading4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/heading5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/heading6.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/horizontalrule.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/increasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/indentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/italic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/letters.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/orderedlist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/outdentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/placeholder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/questionmark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/send.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/separator.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/subscript.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/superscript.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/textcolor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/trash.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/underline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/unlink.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/non_field_errors.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.711148 django-formset-1.0.dev4/formset/templates/formset/tailwind/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.711148 django-formset-1.0.dev4/formset/templates/formset/tailwind/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.711148 django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/radio.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.711148 django-formset-1.0.dev4/formset/templates/formset/uikit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.711148 django-formset-1.0.dev4/formset/templates/formset/uikit/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/uikit/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/uikit/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/uikit/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/uikit/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.715149 django-formset-1.0.dev4/formset/templates/formset/uikit/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/uikit/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/uikit/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/uikit/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/uikit/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.715149 django-formset-1.0.dev4/formset/templates/richtext/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/bulletlist.html
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/doc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/horizontalrule.html
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/listitem.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.715149 django-formset-1.0.dev4/formset/templates/richtext/marks/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/marks/bold.html
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/marks/code.html
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/marks/italic.html
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/marks/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/marks/textcolor.html
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/marks/underline.html
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/orderedlist.html
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.715149 django-formset-1.0.dev4/formset/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templatetags/formsetify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templatetags/richtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 15:44:47.719149 django-formset-1.0.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/setup.py
```

### Comparing `django-formset-1.0.dev3/LICENSE` & `django-formset-1.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/PKG-INFO` & `django-formset-1.0.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.0.dev3
+Version: 1.0.dev4
 Summary: Prevalidate Django Forms in the browser
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
```

### Comparing `django-formset-1.0.dev3/README.md` & `django-formset-1.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/django_formset.egg-info/PKG-INFO` & `django-formset-1.0.dev4/django_formset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.0.dev3
+Version: 1.0.dev4
 Summary: Prevalidate Django Forms in the browser
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
```

### Comparing `django-formset-1.0.dev3/django_formset.egg-info/SOURCES.txt` & `django-formset-1.0.dev4/django_formset.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,27 +43,27 @@
 formset/static/formset/icons/file-font.svg
 formset/static/formset/icons/file-missing.svg
 formset/static/formset/icons/file-pdf.svg
 formset/static/formset/icons/file-picture.svg
 formset/static/formset/icons/file-unknown.svg
 formset/static/formset/icons/file-video.svg
 formset/static/formset/icons/file-zip.svg
-formset/static/formset/js/DateTimePicker-OYPFNQAF.js
-formset/static/formset/js/DjangoSelectize-H6QF7W4R.js
+formset/static/formset/js/DateTimePicker-BBOUOZRC.js
+formset/static/formset/js/DjangoSelectize-OIQWF5I5.js
 formset/static/formset/js/DjangoSlug-226MVQ6E.js
-formset/static/formset/js/DualSelector-GVLJZFWV.js
-formset/static/formset/js/RichtextArea-UTSZPGIP.js
-formset/static/formset/js/SortableSelect-4MNY532K.js
-formset/static/formset/js/chunk-AELXO3WZ.js
+formset/static/formset/js/DualSelector-2ALH4RIS.js
+formset/static/formset/js/RichtextArea-XKK27UIM.js
+formset/static/formset/js/SortableSelect-CEPX3LH6.js
 formset/static/formset/js/chunk-APVD22ED.js
-formset/static/formset/js/chunk-IE6INVWL.js
+formset/static/formset/js/chunk-EJ4RWPXK.js
 formset/static/formset/js/chunk-ISEEQP4V.js
 formset/static/formset/js/chunk-KDP4ZIAK.js
+formset/static/formset/js/chunk-MD4VW33H.js
 formset/static/formset/js/chunk-NLMHZ7JJ.js
-formset/static/formset/js/chunk-O5UGFU32.js
+formset/static/formset/js/chunk-R2VNGMYE.js
 formset/static/formset/js/django-formset.js
 formset/static/formset/scss/bootstrap5-extra.scss
 formset/static/formset/scss/collections.scss
 formset/templates/admin/formset/change_form.html
 formset/templates/calendar/hours.html
 formset/templates/calendar/months.html
 formset/templates/calendar/weeks.html
```

### Comparing `django-formset-1.0.dev3/formset/boundfield.py` & `django-formset-1.0.dev4/formset/boundfield.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/calendar.py` & `django-formset-1.0.dev4/formset/calendar.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/collection.py` & `django-formset-1.0.dev4/formset/collection.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/fields.py` & `django-formset-1.0.dev4/formset/fields.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/fieldset.py` & `django-formset-1.0.dev4/formset/fieldset.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/locale/de/LC_MESSAGES/django.mo` & `django-formset-1.0.dev4/formset/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/locale/de/LC_MESSAGES/django.po` & `django-formset-1.0.dev4/formset/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/renderers/bootstrap.py` & `django-formset-1.0.dev4/formset/renderers/bootstrap.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/renderers/bulma.py` & `django-formset-1.0.dev4/formset/renderers/bulma.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/renderers/default.py` & `django-formset-1.0.dev4/formset/renderers/default.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/renderers/foundation.py` & `django-formset-1.0.dev4/formset/renderers/foundation.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/renderers/tailwind.py` & `django-formset-1.0.dev4/formset/renderers/tailwind.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/renderers/uikit.py` & `django-formset-1.0.dev4/formset/renderers/uikit.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/richtext/controls.py` & `django-formset-1.0.dev4/formset/richtext/controls.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/richtext/dialogs.py` & `django-formset-1.0.dev4/formset/richtext/dialogs.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/richtext/widgets.py` & `django-formset-1.0.dev4/formset/richtext/widgets.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/css/bootstrap5-extra.css` & `django-formset-1.0.dev4/formset/static/formset/css/bootstrap5-extra.css`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/css/bootstrap5-extra.css.map` & `django-formset-1.0.dev4/formset/static/formset/css/bootstrap5-extra.css.map`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/css/collections.css` & `django-formset-1.0.dev4/formset/static/formset/css/collections.css`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/css/tailwind.css` & `django-formset-1.0.dev4/formset/static/formset/css/tailwind.css`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/icons/file-audio.svg` & `django-formset-1.0.dev4/formset/static/formset/icons/file-audio.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/icons/file-empty.svg` & `django-formset-1.0.dev4/formset/static/formset/icons/file-empty.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/icons/file-font.svg` & `django-formset-1.0.dev4/formset/static/formset/icons/file-font.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/icons/file-missing.svg` & `django-formset-1.0.dev4/formset/static/formset/icons/file-missing.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/icons/file-pdf.svg` & `django-formset-1.0.dev4/formset/static/formset/icons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/icons/file-picture.svg` & `django-formset-1.0.dev4/formset/static/formset/icons/file-picture.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/icons/file-unknown.svg` & `django-formset-1.0.dev4/formset/static/formset/icons/file-unknown.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/icons/file-video.svg` & `django-formset-1.0.dev4/formset/static/formset/icons/file-video.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/icons/file-zip.svg` & `django-formset-1.0.dev4/formset/static/formset/icons/file-zip.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/js/DateTimePicker-OYPFNQAF.js` & `django-formset-1.0.dev4/formset/static/formset/js/DateTimePicker-BBOUOZRC.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -3,15 +3,15 @@
     b as m,
     c as E,
     d as f
 } from "./chunk-ISEEQP4V.js";
 import {
     a as d,
     b as p
-} from "./chunk-O5UGFU32.js";
+} from "./chunk-R2VNGMYE.js";
 import "./chunk-NLMHZ7JJ.js";
 var D = ':is([is=django-datepicker],[is=django-datetimepicker]){--dummy-style: none}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar{box-shadow:#d3d3d3 0 0 1rem;width:max-content;position:absolute;top:0;left:0}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar [hidden]{display:none !important}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .controls{display:flex;justify-content:space-between;align-items:center;border-bottom:1px solid #d3d3d3}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .controls button{display:inline-flex;background-color:rgba(0,0,0,0);border:none;padding:0;min-width:28px}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .controls button:hover{background-color:#f0f0f0}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .controls button>svg{margin:0 auto}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .controls time{width:10rem;text-align:center}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .controls.years-view time{opacity:.75}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges{--dummy-style: none}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul{list-style:none;margin:0;padding:0;text-align:center;display:grid;gap:2px}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul.hours{grid-template-columns:repeat(6, 1fr)}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul.hours>li.preselected{border:1px solid #d3d3d3;border-bottom-color:#fff;border-top-left-radius:5px;border-top-right-radius:5px}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul.weekdays,:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul.monthdays{grid-template-columns:repeat(7, 1fr)}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul.monthdays>li.adjacent{color:#606060}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul.months{grid-template-columns:repeat(3, 1fr)}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul.years{grid-template-columns:repeat(4, 1fr)}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul.weekdays{font-weight:bold}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul:not(.weekdays){--dummy-style: none}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul:not(.weekdays)>li{width:2em}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul:not(.weekdays)>li.selected{background-color:#009cff;color:#fff}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul:not(.weekdays)>li.selected.today::after{border-color:rgba(0,0,0,0) rgba(0,0,0,0) #fff rgba(0,0,0,0)}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul:not(.weekdays)>li[disabled]{opacity:.5}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul:not(.weekdays)>li:not([disabled]):hover{opacity:1;background-color:#f0f0f0;cursor:pointer}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul.minutes{font-size:smaller;border:1px solid #d3d3d3;margin:-1px 0 3px;padding:0 5px;line-height:inherit}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul.minutes>li{width:inherit}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul>li.today{position:relative}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges ul>li.today::after{position:absolute;content:"";bottom:0;right:0;border-style:solid;border-width:0 0 10px 10px;border-color:rgba(0,0,0,0) rgba(0,0,0,0) #009cff rgba(0,0,0,0)}:is([is=django-datepicker],[is=django-datetimepicker])+.dj-calendar .ranges abbr[title]{text-decoration:none}:is([is=django-datepicker],[is=django-datetimepicker])[aria-expanded=false]+.dj-calendar{display:none}:is([is=django-datepicker],[is=django-datetimepicker])[aria-expanded=true]+.dj-calendar{display:block}';
 var c = class extends p {
         constructor(e, t) {
             super(e);
             this.autoZeroRegExps = [];
             this.autoDelimiterRegExps = [];
@@ -499,27 +499,27 @@
             let e = this.asDate();
             return e ? (this.localTime || e.setTime(e.getTime() - 6e4 * e.getTimezoneOffset()), e) : null
         }
     },
     o = Symbol("DateTimePickerElement"),
     v = class extends HTMLInputElement {
         connectedCallback() {
-            let e = this.closest("django-field-group");
+            let e = this.closest('[role="group"]');
             if (!e) throw new Error(`Attempt to initialize ${this} outside <django-formset>`);
             let t = e.querySelector('[aria-label="calendar"]');
             this[o] = new c(this, t)
         }
         get valueAsDate() {
             return this[o].valueAsDate()
         }
     };
 o;
 var w = class extends HTMLInputElement {
     connectedCallback() {
-        let e = this.closest("django-field-group");
+        let e = this.closest('[role="group"]');
         if (!e) throw new Error(`Attempt to initialize ${this} outside <django-formset>`);
         let t = e.querySelector('[aria-label="calendar"]');
         this[o] = new c(this, t)
     }
     get valueAsDate() {
         return this[o].valueAsDate()
     }
```

### Comparing `django-formset-1.0.dev3/formset/static/formset/js/DjangoSelectize-H6QF7W4R.js` & `django-formset-1.0.dev4/formset/static/formset/js/DjangoSelectize-OIQWF5I5.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,24 @@
 import {
     a as Pe
-} from "./chunk-AELXO3WZ.js";
+} from "./chunk-MD4VW33H.js";
 import {
     a as nt
 } from "./chunk-KDP4ZIAK.js";
 import {
     a as se
-} from "./chunk-O5UGFU32.js";
+} from "./chunk-R2VNGMYE.js";
 import {
     a as ke,
     b as ve
 } from "./chunk-NLMHZ7JJ.js";
 var $e = ke((be, Re) => {
-    (function(r, u) {
-        typeof be == "object" && typeof Re < "u" ? u(be) : typeof define == "function" && define.amd ? define(["exports"], u) : (r = typeof globalThis < "u" ? globalThis : r || self, u(r.sifter = {}))
-    })(be, function(r) {
+    (function(i, u) {
+        typeof be == "object" && typeof Re < "u" ? u(be) : typeof define == "function" && define.amd ? define(["exports"], u) : (i = typeof globalThis < "u" ? globalThis : i || self, u(i.sifter = {}))
+    })(be, function(i) {
         "use strict";
         let u = l => (l = l.filter(Boolean), l.length < 2 ? l[0] || "" : o(l) == 1 ? "[" + l.join("") + "]" : "(?:" + l.join("|") + ")"),
             e = l => {
                 if (!n(l)) return l.join("");
                 let a = "",
                     c = 0,
                     d = () => {
@@ -34,16 +34,16 @@
             },
             t = l => {
                 let a = f(l);
                 return u(a)
             },
             n = l => new Set(l).size !== l.length,
             s = l => (l + "").replace(/([\$\(-\+\.\?\[-\^\{-\}])/g, "\\$1"),
-            o = l => l.reduce((a, c) => Math.max(a, i(c)), 0),
-            i = l => f(l).length,
+            o = l => l.reduce((a, c) => Math.max(a, r(c)), 0),
+            r = l => f(l).length,
             f = l => Array.from(l);
         let p = l => {
             if (l.length === 1) return [
                 [l]
             ];
             let a = [],
                 c = l.substring(1);
@@ -279,15 +279,15 @@
                 c && !Array.isArray(c) && (l[a] = [c])
             },
             x = (l, a) => {
                 if (Array.isArray(l)) l.forEach(a);
                 else
                     for (var c in l) l.hasOwnProperty(c) && a(l[c], c)
             },
-            j = (l, a) => typeof l == "number" && typeof a == "number" ? l > a ? 1 : l < a ? -1 : 0 : (l = P(l + "").toLowerCase(), a = P(a + "").toLowerCase(), l > a ? 1 : a > l ? -1 : 0);
+            K = (l, a) => typeof l == "number" && typeof a == "number" ? l > a ? 1 : l < a ? -1 : 0 : (l = P(l + "").toLowerCase(), a = P(a + "").toLowerCase(), l > a ? 1 : a > l ? -1 : 0);
         class z {
             constructor(a, c) {
                 this.items = void 0, this.settings = void 0, this.items = a, this.settings = c || {
                     diacritics: !0
                 }
             }
             tokenize(a, c, d) {
@@ -378,15 +378,15 @@
                         field: "$score",
                         direction: "desc"
                     })
                 } else d = d.filter(I => I.field !== "$score");
                 return d.length ? function(I, L) {
                     var F, U;
                     for (let ae of d)
-                        if (U = ae.field, F = (ae.direction === "desc" ? -1 : 1) * j(C(U, I), C(U, L)), F) return F;
+                        if (U = ae.field, F = (ae.direction === "desc" ? -1 : 1) * K(C(U, I), C(U, L)), F) return F;
                     return 0
                 } : null
             }
             prepareSearch(a, c) {
                 let d = {};
                 var _ = Object.assign({}, c);
                 if (k(_, "sort"), k(_, "sort_empty"), _.fields) {
@@ -425,23 +425,23 @@
                         id: I
                     })
                 });
                 let C = d._getSortFunction(v);
                 return C && v.items.sort(C), v.total = v.items.length, typeof c.limit == "number" && (v.items = v.items.slice(0, c.limit)), v
             }
         }
-        r.Sifter = z, r.cmp = j, r.getAttr = T, r.getAttrNesting = O, r.getPattern = h, r.iterate = x, r.propToArray = k, r.scoreValue = y, Object.defineProperty(r, "__esModule", {
+        i.Sifter = z, i.cmp = K, i.getAttr = T, i.getAttrNesting = O, i.getPattern = h, i.iterate = x, i.propToArray = k, i.scoreValue = y, Object.defineProperty(i, "__esModule", {
             value: !0
         })
     })
 });
-var xe = ke((ye, je) => {
-    (function(r, u) {
-        typeof ye == "object" && typeof je < "u" ? u(ye) : typeof define == "function" && define.amd ? define(["exports"], u) : (r = typeof globalThis < "u" ? globalThis : r || self, u(r.diacritics = {}))
-    })(ye, function(r) {
+var xe = ke((ye, Ke) => {
+    (function(i, u) {
+        typeof ye == "object" && typeof Ke < "u" ? u(ye) : typeof define == "function" && define.amd ? define(["exports"], u) : (i = typeof globalThis < "u" ? globalThis : i || self, u(i.diacritics = {}))
+    })(ye, function(i) {
         "use strict";
         let u = h => (h = h.filter(Boolean), h.length < 2 ? h[0] || "" : o(h) == 1 ? "[" + h.join("") + "]" : "(?:" + h.join("|") + ")"),
             e = h => {
                 if (!n(h)) return h.join("");
                 let T = "",
                     O = 0,
                     y = () => {
@@ -457,16 +457,16 @@
             },
             t = h => {
                 let T = f(h);
                 return u(T)
             },
             n = h => new Set(h).size !== h.length,
             s = h => (h + "").replace(/([\$\(\)\*\+\.\?\[\]\^\{\|\}\\])/gu, "\\$1"),
-            o = h => h.reduce((T, O) => Math.max(T, i(O)), 0),
-            i = h => f(h).length,
+            o = h => h.reduce((T, O) => Math.max(T, r(O)), 0),
+            r = h => f(h).length,
             f = h => Array.from(h),
             p = h => {
                 if (h.length === 1) return [
                     [h]
                 ];
                 let T = [],
                     O = h.substring(1);
@@ -475,15 +475,15 @@
                     x[0] = h.charAt(0) + x[0], T.push(x), x = k.slice(0), x.unshift(h.charAt(0)), T.push(x)
                 }), T
             },
             m = [
                 [0, 65535]
             ],
             w = "[\u0300-\u036F\xB7\u02BE\u02BC]";
-        r.unicode_map = void 0;
+        i.unicode_map = void 0;
         let A, J = 3,
             Q = {},
             g = {
                 "/": "\u2044\u2215",
                 0: "\u07C0",
                 a: "\u2C65\u0250\u0251",
                 aa: "\uA733",
@@ -530,15 +530,15 @@
             for (let O = 0; O < T.length; O++) {
                 let y = T.substring(O, O + 1);
                 Q[y] = h
             }
         }
         let q = new RegExp(Object.keys(Q).join("|") + "|" + w, "gu"),
             H = h => {
-                r.unicode_map === void 0 && (r.unicode_map = M(h || m))
+                i.unicode_map === void 0 && (i.unicode_map = M(h || m))
             },
             N = (h, T = "NFKD") => h.normalize(T),
             b = h => f(h).reduce((T, O) => T + P(O), ""),
             P = h => (h = N(h).toLowerCase().replace(q, T => Q[T] || ""), N(h, "NFC"));
 
         function* X(h) {
             for (let [T, O] of h)
@@ -552,54 +552,54 @@
                     }))
                 }
         }
         let R = h => {
                 let T = {},
                     O = (y, k) => {
                         let x = T[y] || new Set,
-                            j = new RegExp("^" + t(x) + "$", "iu");
-                        k.match(j) || (x.add(s(k)), T[y] = x)
+                            K = new RegExp("^" + t(x) + "$", "iu");
+                        k.match(K) || (x.add(s(k)), T[y] = x)
                     };
                 for (let y of X(h)) O(y.folded, y.folded), O(y.folded, y.composed);
                 return T
             },
             M = h => {
                 let T = R(h),
                     O = {},
                     y = [];
                 for (let x in T) {
-                    let j = T[x];
-                    j && (O[x] = t(j)), x.length > 1 && y.push(s(x))
+                    let K = T[x];
+                    K && (O[x] = t(K)), x.length > 1 && y.push(s(x))
                 }
-                y.sort((x, j) => j.length - x.length);
+                y.sort((x, K) => K.length - x.length);
                 let k = u(y);
                 return A = new RegExp("^" + k, "u"), O
             },
             E = (h, T = 1) => {
                 let O = 0;
-                return h = h.map(y => (r.unicode_map[y] && (O += y.length), r.unicode_map[y] || y)), O >= T ? e(h) : ""
+                return h = h.map(y => (i.unicode_map[y] && (O += y.length), i.unicode_map[y] || y)), O >= T ? e(h) : ""
             },
             V = (h, T = 1) => (T = Math.max(T, h.length - 1), u(p(h).map(O => E(O, T)))),
             $ = (h, T = !0) => {
                 let O = h.length > 1 ? 1 : 0;
                 return u(h.map(y => {
                     let k = [],
                         x = T ? y.length() : y.length() - 1;
-                    for (let j = 0; j < x; j++) k.push(V(y.substrs[j] || "", O));
+                    for (let K = 0; K < x; K++) k.push(V(y.substrs[K] || "", O));
                     return e(k)
                 }))
             },
             G = (h, T) => {
                 for (let O of T) {
                     if (O.start != h.start || O.end != h.end || O.substrs.join("") !== h.substrs.join("")) continue;
                     let y = h.parts,
-                        k = j => {
+                        k = K => {
                             for (let z of y) {
-                                if (z.start === j.start && z.substr === j.substr) return !1;
-                                if (!(j.length == 1 || z.length == 1) && (j.start < z.start && j.end > z.start || z.start < j.start && z.end > j.start)) return !0
+                                if (z.start === K.start && z.substr === K.substr) return !1;
+                                if (!(K.length == 1 || z.length == 1) && (K.start < z.start && K.end > z.start || z.start < K.start && z.end > K.start)) return !0
                             }
                             return !1
                         };
                     if (!(O.parts.filter(k).length > 0)) return !0
                 }
                 return !1
             };
@@ -617,31 +617,31 @@
                 return this.parts.length
             }
             clone(T, O) {
                 let y = new W,
                     k = JSON.parse(JSON.stringify(this.parts)),
                     x = k.pop();
                 for (let l of k) y.add(l);
-                let j = O.substr.substring(0, T - x.start),
-                    z = j.length;
+                let K = O.substr.substring(0, T - x.start),
+                    z = K.length;
                 return y.add({
                     start: x.start,
                     end: x.start + z,
                     length: z,
-                    substr: j
+                    substr: K
                 }), y
             }
         }
         let ce = h => {
             H(), h = b(h);
             let T = "",
                 O = [new W];
             for (let y = 0; y < h.length; y++) {
                 let x = h.substring(y).match(A),
-                    j = h.substring(y, y + 1),
+                    K = h.substring(y, y + 1),
                     z = x ? x[0] : null,
                     l = [],
                     a = new Set;
                 for (let c of O) {
                     let d = c.last();
                     if (!d || d.length == 1 || d.end <= y)
                         if (z) {
@@ -652,15 +652,15 @@
                                 length: _,
                                 substr: z
                             }), a.add("1")
                         } else c.add({
                             start: y,
                             end: y + 1,
                             length: 1,
-                            substr: j
+                            substr: K
                         }), a.add("2");
                     else if (z) {
                         let _ = c.clone(y, d),
                             v = z.length;
                         _.add({
                             start: y,
                             end: y + v,
@@ -679,22 +679,22 @@
                     let c = new W,
                         d = O[0];
                     d && c.add(d.last()), O = [c]
                 }
             }
             return T += $(O, !0), T
         };
-        r._asciifold = P, r.asciifold = b, r.code_points = m, r.escape_regex = s, r.generateMap = M, r.generateSets = R, r.generator = X, r.getPattern = ce, r.initialize = H, r.mapSequence = E, r.normalize = N, r.substringsToPattern = V, Object.defineProperty(r, "__esModule", {
+        i._asciifold = P, i.asciifold = b, i.code_points = m, i.escape_regex = s, i.generateMap = M, i.generateSets = R, i.generator = X, i.getPattern = ce, i.initialize = H, i.mapSequence = E, i.normalize = N, i.substringsToPattern = V, Object.defineProperty(i, "__esModule", {
             value: !0
         })
     })
 });
 
-function Se(r, u) {
-    r.split(/\s+/).forEach(e => {
+function Se(i, u) {
+    i.split(/\s+/).forEach(e => {
         u(e)
     })
 }
 var pe = class {
     constructor() {
         this._events = {}
     }
@@ -726,47 +726,47 @@
             s !== void 0 && s.forEach(o => {
                 o.apply(t, e)
             })
         })
     }
 };
 
-function Ee(r) {
-    return r.plugins = {}, class extends r {
+function Ee(i) {
+    return i.plugins = {}, class extends i {
         constructor() {
             super(...arguments);
             this.plugins = {
                 names: [],
                 settings: {},
                 requested: {},
                 loaded: {}
             }
         }
         static define(e, t) {
-            r.plugins[e] = {
+            i.plugins[e] = {
                 name: e,
                 fn: t
             }
         }
         initializePlugins(e) {
             var t, n;
             let s = this,
                 o = [];
-            if (Array.isArray(e)) e.forEach(i => {
-                typeof i == "string" ? o.push(i) : (s.plugins.settings[i.name] = i.options, o.push(i.name))
+            if (Array.isArray(e)) e.forEach(r => {
+                typeof r == "string" ? o.push(r) : (s.plugins.settings[r.name] = r.options, o.push(r.name))
             });
             else if (e)
                 for (t in e) e.hasOwnProperty(t) && (s.plugins.settings[t] = e[t], o.push(t));
             for (; n = o.shift();) s.require(n)
         }
         loadPlugin(e) {
             var t = this,
                 n = t.plugins,
-                s = r.plugins[e];
-            if (!r.plugins.hasOwnProperty(e)) throw new Error('Unable to find "' + e + '" plugin');
+                s = i.plugins[e];
+            if (!i.plugins.hasOwnProperty(e)) throw new Error('Unable to find "' + e + '" plugin');
             n.requested[e] = !0, n.loaded[e] = s.fn.apply(t, [t.plugins.settings[e] || {}]), n.names.push(e)
         }
         require(e) {
             var t = this,
                 n = t.plugins;
             if (!t.plugins.loaded.hasOwnProperty(e)) {
                 if (n.requested[e]) throw new Error('Plugin has circular dependency ("' + e + '")');
@@ -775,118 +775,118 @@
             return n.loaded[e]
         }
     }
 }
 var te = ve($e()),
     Je = ve(xe());
 var st = ve(xe());
-var re = (r, u) => {
-    if (Array.isArray(r)) r.forEach(u);
+var ie = (i, u) => {
+    if (Array.isArray(i)) i.forEach(u);
     else
-        for (var e in r) r.hasOwnProperty(e) && u(r[e], e)
+        for (var e in i) i.hasOwnProperty(e) && u(i[e], e)
 };
-var Z = r => {
-        if (r.jquery) return r[0];
-        if (r instanceof HTMLElement) return r;
-        if (Le(r)) {
+var Z = i => {
+        if (i.jquery) return i[0];
+        if (i instanceof HTMLElement) return i;
+        if (Le(i)) {
             var u = document.createElement("template");
-            return u.innerHTML = r.trim(), u.content.firstChild
+            return u.innerHTML = i.trim(), u.content.firstChild
         }
-        return document.querySelector(r)
+        return document.querySelector(i)
     },
-    Le = r => typeof r == "string" && r.indexOf("<") > -1,
-    Ke = r => r.replace(/['"\\]/g, "\\$&"),
-    _e = (r, u) => {
+    Le = i => typeof i == "string" && i.indexOf("<") > -1,
+    je = i => i.replace(/['"\\]/g, "\\$&"),
+    _e = (i, u) => {
         var e = document.createEvent("HTMLEvents");
-        e.initEvent(u, !0, !1), r.dispatchEvent(e)
+        e.initEvent(u, !0, !1), i.dispatchEvent(e)
     },
-    fe = (r, u) => {
-        Object.assign(r.style, u)
+    fe = (i, u) => {
+        Object.assign(i.style, u)
     },
-    ee = (r, ...u) => {
+    ee = (i, ...u) => {
         var e = De(u);
-        r = Ne(r), r.map(t => {
+        i = Ne(i), i.map(t => {
             e.map(n => {
                 t.classList.add(n)
             })
         })
     },
-    ie = (r, ...u) => {
+    re = (i, ...u) => {
         var e = De(u);
-        r = Ne(r), r.map(t => {
+        i = Ne(i), i.map(t => {
             e.map(n => {
                 t.classList.remove(n)
             })
         })
     },
-    De = r => {
+    De = i => {
         var u = [];
-        return re(r, e => {
+        return ie(i, e => {
             typeof e == "string" && (e = e.trim().split(/[\11\12\14\15\40]/)), Array.isArray(e) && (u = u.concat(e))
         }), u.filter(Boolean)
     },
-    Ne = r => (Array.isArray(r) || (r = [r]), r),
-    Te = (r, u, e) => {
-        if (!(e && !e.contains(r)))
-            for (; r && r.matches;) {
-                if (r.matches(u)) return r;
-                r = r.parentNode
+    Ne = i => (Array.isArray(i) || (i = [i]), i),
+    Te = (i, u, e) => {
+        if (!(e && !e.contains(i)))
+            for (; i && i.matches;) {
+                if (i.matches(u)) return i;
+                i = i.parentNode
             }
     },
-    Ie = (r, u = 0) => u > 0 ? r[r.length - 1] : r[0],
-    Ve = r => Object.keys(r).length === 0,
-    Ae = (r, u) => {
-        if (!r) return -1;
-        u = u || r.nodeName;
-        for (var e = 0; r = r.previousElementSibling;) r.matches(u) && e++;
+    Ie = (i, u = 0) => u > 0 ? i[i.length - 1] : i[0],
+    Ve = i => Object.keys(i).length === 0,
+    Ae = (i, u) => {
+        if (!i) return -1;
+        u = u || i.nodeName;
+        for (var e = 0; i = i.previousElementSibling;) i.matches(u) && e++;
         return e
     },
-    D = (r, u) => {
-        re(u, (e, t) => {
-            e == null ? r.removeAttribute(t) : r.setAttribute(t, "" + e)
+    D = (i, u) => {
+        ie(u, (e, t) => {
+            e == null ? i.removeAttribute(t) : i.setAttribute(t, "" + e)
         })
     },
-    ge = (r, u) => {
-        r.parentNode && r.parentNode.replaceChild(u, r)
+    ge = (i, u) => {
+        i.parentNode && i.parentNode.replaceChild(u, i)
     };
-var qe = (r, u) => {
+var qe = (i, u) => {
         if (u === null) return;
         if (typeof u == "string") {
             if (!u.length) return;
             u = new RegExp(u, "i")
         }
         let e = s => {
                 var o = s.data.match(u);
                 if (o && s.data.length > 0) {
-                    var i = document.createElement("span");
-                    i.className = "highlight";
+                    var r = document.createElement("span");
+                    r.className = "highlight";
                     var f = s.splitText(o.index);
                     f.splitText(o[0].length);
                     var p = f.cloneNode(!0);
-                    return i.appendChild(p), ge(f, i), 1
+                    return r.appendChild(p), ge(f, r), 1
                 }
                 return 0
             },
             t = s => {
                 s.nodeType === 1 && s.childNodes && !/(script|style)/i.test(s.tagName) && (s.className !== "highlight" || s.tagName !== "SPAN") && Array.from(s.childNodes).forEach(o => {
                     n(o)
                 })
             },
             n = s => s.nodeType === 3 ? e(s) : (t(s), 0);
-        n(r)
+        n(i)
     },
-    ze = r => {
-        var u = r.querySelectorAll("span.highlight");
+    ze = i => {
+        var u = i.querySelectorAll("span.highlight");
         Array.prototype.forEach.call(u, function(e) {
             var t = e.parentNode;
             t.replaceChild(e.firstChild, e), t.normalize()
         })
     };
-var it = typeof navigator > "u" ? !1 : /Mac/.test(navigator.userAgent),
-    he = it ? "metaKey" : "ctrlKey";
+var rt = typeof navigator > "u" ? !1 : /Mac/.test(navigator.userAgent),
+    he = rt ? "metaKey" : "ctrlKey";
 var Ce = {
     options: [],
     optgroups: [],
     plugins: [],
     delimiter: ",",
     splitOn: null,
     persist: !0,
@@ -926,78 +926,78 @@
     itemClass: "item",
     optionClass: "option",
     dropdownParent: null,
     controlInput: '<input type="text" autocomplete="off" size="1" />',
     copyClassesToDropdown: !1,
     placeholder: null,
     hidePlaceholder: null,
-    shouldLoad: function(r) {
-        return r.length > 0
+    shouldLoad: function(i) {
+        return i.length > 0
     },
     render: {}
 };
-var ne = r => typeof r > "u" || r === null ? null : me(r),
-    me = r => typeof r == "boolean" ? r ? "1" : "0" : r + "",
-    ue = r => (r + "").replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/>/g, "&gt;").replace(/"/g, "&quot;"),
-    Ye = (r, u) => {
+var ne = i => typeof i > "u" || i === null ? null : me(i),
+    me = i => typeof i == "boolean" ? i ? "1" : "0" : i + "",
+    ue = i => (i + "").replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/>/g, "&gt;").replace(/"/g, "&quot;"),
+    Ye = (i, u) => {
         var e;
         return function(t, n) {
             var s = this;
             e && (s.loading = Math.max(s.loading - 1, 0), clearTimeout(e)), e = setTimeout(function() {
-                e = null, s.loadedSearches[t] = !0, r.call(s, t, n)
+                e = null, s.loadedSearches[t] = !0, i.call(s, t, n)
             }, u)
         }
     },
-    Me = (r, u, e) => {
-        var t, n = r.trigger,
+    Me = (i, u, e) => {
+        var t, n = i.trigger,
             s = {};
-        r.trigger = function() {
+        i.trigger = function() {
             var o = arguments[0];
             if (u.indexOf(o) !== -1) s[o] = arguments;
-            else return n.apply(r, arguments)
-        }, e.apply(r, []), r.trigger = n;
-        for (t of u) t in s && n.apply(r, s[t])
+            else return n.apply(i, arguments)
+        }, e.apply(i, []), i.trigger = n;
+        for (t of u) t in s && n.apply(i, s[t])
     },
-    Be = r => ({
-        start: r.selectionStart || 0,
-        length: (r.selectionEnd || 0) - (r.selectionStart || 0)
+    Be = i => ({
+        start: i.selectionStart || 0,
+        length: (i.selectionEnd || 0) - (i.selectionStart || 0)
     }),
-    K = (r, u = !1) => {
-        r && (r.preventDefault(), u && r.stopPropagation())
+    j = (i, u = !1) => {
+        i && (i.preventDefault(), u && i.stopPropagation())
     },
-    B = (r, u, e, t) => {
-        r.addEventListener(u, e, t)
+    B = (i, u, e, t) => {
+        i.addEventListener(u, e, t)
     },
-    oe = (r, u) => {
-        if (!u || !u[r]) return !1;
+    oe = (i, u) => {
+        if (!u || !u[i]) return !1;
         var e = (u.altKey ? 1 : 0) + (u.ctrlKey ? 1 : 0) + (u.shiftKey ? 1 : 0) + (u.metaKey ? 1 : 0);
         return e === 1
     },
-    we = (r, u) => {
-        let e = r.getAttribute("id");
-        return e || (r.setAttribute("id", u), u)
+    we = (i, u) => {
+        let e = i.getAttribute("id");
+        return e || (i.setAttribute("id", u), u)
     },
-    Fe = r => r.replace(/[\\"']/g, "\\$&"),
-    le = (r, u) => {
-        u && r.append(u)
+    Fe = i => i.replace(/[\\"']/g, "\\$&"),
+    le = (i, u) => {
+        u && i.append(u)
     };
 
-function Oe(r, u) {
+function Oe(i, u) {
     var e = Object.assign({}, Ce, u),
         t = e.dataAttr,
         n = e.labelField,
         s = e.valueField,
         o = e.disabledField,
-        i = e.optgroupField,
+        r = e.optgroupField,
         f = e.optgroupLabelField,
         p = e.optgroupValueField,
-        m = r.tagName.toLowerCase(),
-        w = r.getAttribute("placeholder") || r.getAttribute("data-placeholder");
+        m = i.tagName.toLowerCase(),
+        w = i.getAttribute("placeholder") || i.getAttribute("data-placeholder");
     if (!w && !e.allowEmptyOption) {
-        let g = r.querySelector('option[value=""]');
+        let g = i.querySelector('option[value=""]');
         g && (w = g.textContent)
     }
     var A = {
             placeholder: w,
             options: [],
             optgroups: [],
             items: [],
@@ -1013,44 +1013,44 @@
                     return typeof E == "string" && E.length && (M = Object.assign(M, JSON.parse(E))), M
                 },
                 P = (R, M) => {
                     var E = ne(R.value);
                     if (E != null && !(!E && !e.allowEmptyOption)) {
                         if (H.hasOwnProperty(E)) {
                             if (M) {
-                                var V = H[E][i];
-                                V ? Array.isArray(V) ? V.push(M) : H[E][i] = [V, M] : H[E][i] = M
+                                var V = H[E][r];
+                                V ? Array.isArray(V) ? V.push(M) : H[E][r] = [V, M] : H[E][r] = M
                             }
                         } else {
                             var $ = b(R);
-                            $[n] = $[n] || R.textContent, $[s] = $[s] || E, $[o] = $[o] || R.disabled, $[i] = $[i] || M, $.$option = R, H[E] = $, q.push($)
+                            $[n] = $[n] || R.textContent, $[s] = $[s] || E, $[o] = $[o] || R.disabled, $[r] = $[r] || M, $.$option = R, H[E] = $, q.push($)
                         }
                         R.selected && A.items.push(E)
                     }
                 },
                 X = R => {
                     var M, E;
-                    E = b(R), E[f] = E[f] || R.getAttribute("label") || "", E[p] = E[p] || N++, E[o] = E[o] || R.disabled, A.optgroups.push(E), M = E[p], re(R.children, V => {
+                    E = b(R), E[f] = E[f] || R.getAttribute("label") || "", E[p] = E[p] || N++, E[o] = E[o] || R.disabled, A.optgroups.push(E), M = E[p], ie(R.children, V => {
                         P(V, M)
                     })
                 };
-            A.maxItems = r.hasAttribute("multiple") ? null : 1, re(r.children, R => {
+            A.maxItems = i.hasAttribute("multiple") ? null : 1, ie(i.children, R => {
                 g = R.tagName.toLowerCase(), g === "optgroup" ? X(R) : g === "option" && P(R)
             })
         },
         Q = () => {
-            let g = r.getAttribute(t);
-            if (g) A.options = JSON.parse(g), re(A.options, H => {
+            let g = i.getAttribute(t);
+            if (g) A.options = JSON.parse(g), ie(A.options, H => {
                 A.items.push(H[s])
             });
             else {
-                var q = r.value.trim() || "";
+                var q = i.value.trim() || "";
                 if (!e.allowEmptyOption && !q.length) return;
                 let H = q.split(e.delimiter);
-                re(H, N => {
+                ie(H, N => {
                     let b = {};
                     b[n] = N, b[s] = N, A.options.push(b)
                 }), A.items = H
             }
         };
     return m === "select" ? J() : Q(), Object.assign({}, Ce, A, u)
 }
@@ -1082,45 +1082,45 @@
             this.items = [];
             Ue++;
             var n, s = Z(e);
             if (s.tomselect) throw new Error("Tom Select already initialized on this element");
             s.tomselect = this;
             var o = window.getComputedStyle && window.getComputedStyle(s, null);
             n = o.getPropertyValue("direction");
-            let i = Oe(s, t);
-            this.settings = i, this.input = s, this.tabIndex = s.tabIndex || 0, this.is_select_tag = s.tagName.toLowerCase() === "select", this.rtl = /rtl/i.test(n), this.inputId = we(s, "tomselect-" + Ue), this.isRequired = s.required, this.sifter = new te.Sifter(this.options, {
-                diacritics: i.diacritics
-            }), i.mode = i.mode || (i.maxItems === 1 ? "single" : "multi"), typeof i.hideSelected != "boolean" && (i.hideSelected = i.mode === "multi"), typeof i.hidePlaceholder != "boolean" && (i.hidePlaceholder = i.mode !== "multi");
-            var f = i.createFilter;
-            typeof f != "function" && (typeof f == "string" && (f = new RegExp(f)), f instanceof RegExp ? i.createFilter = H => f.test(H) : i.createFilter = H => this.settings.duplicates || !this.options[H]), this.initializePlugins(i.plugins), this.setupCallbacks(), this.setupTemplates();
+            let r = Oe(s, t);
+            this.settings = r, this.input = s, this.tabIndex = s.tabIndex || 0, this.is_select_tag = s.tagName.toLowerCase() === "select", this.rtl = /rtl/i.test(n), this.inputId = we(s, "tomselect-" + Ue), this.isRequired = s.required, this.sifter = new te.Sifter(this.options, {
+                diacritics: r.diacritics
+            }), r.mode = r.mode || (r.maxItems === 1 ? "single" : "multi"), typeof r.hideSelected != "boolean" && (r.hideSelected = r.mode === "multi"), typeof r.hidePlaceholder != "boolean" && (r.hidePlaceholder = r.mode !== "multi");
+            var f = r.createFilter;
+            typeof f != "function" && (typeof f == "string" && (f = new RegExp(f)), f instanceof RegExp ? r.createFilter = H => f.test(H) : r.createFilter = H => this.settings.duplicates || !this.options[H]), this.initializePlugins(r.plugins), this.setupCallbacks(), this.setupTemplates();
             let p = Z("<div>"),
                 m = Z("<div>"),
                 w = this._render("dropdown"),
                 A = Z('<div role="listbox" tabindex="-1">'),
                 J = this.input.getAttribute("class") || "",
-                Q = i.mode;
+                Q = r.mode;
             var g;
-            if (ee(p, i.wrapperClass, J, Q), ee(m, i.controlClass), le(p, m), ee(w, i.dropdownClass, Q), i.copyClassesToDropdown && ee(w, J), ee(A, i.dropdownContentClass), le(w, A), Z(i.dropdownParent || p).appendChild(w), Le(i.controlInput)) {
-                g = Z(i.controlInput);
+            if (ee(p, r.wrapperClass, J, Q), ee(m, r.controlClass), le(p, m), ee(w, r.dropdownClass, Q), r.copyClassesToDropdown && ee(w, J), ee(A, r.dropdownContentClass), le(w, A), Z(r.dropdownParent || p).appendChild(w), Le(r.controlInput)) {
+                g = Z(r.controlInput);
                 var q = ["autocorrect", "autocapitalize", "autocomplete"];
                 (0, te.iterate)(q, H => {
                     s.getAttribute(H) && D(g, {
                         [H]: s.getAttribute(H)
                     })
                 }), g.tabIndex = -1, m.appendChild(g), this.focus_node = g
-            } else i.controlInput ? (g = Z(i.controlInput), this.focus_node = g) : (g = Z("<input/>"), this.focus_node = m);
+            } else r.controlInput ? (g = Z(r.controlInput), this.focus_node = g) : (g = Z("<input/>"), this.focus_node = m);
             this.wrapper = p, this.dropdown = w, this.dropdown_content = A, this.control = m, this.control_input = g, this.setup()
         }
         setup() {
             let e = this,
                 t = e.settings,
                 n = e.control_input,
                 s = e.dropdown,
                 o = e.dropdown_content,
-                i = e.wrapper,
+                r = e.wrapper,
                 f = e.control,
                 p = e.input,
                 m = e.focus_node,
                 w = {
                     passive: !0
                 },
                 A = e.inputId + "-ts-dropdown";
@@ -1129,60 +1129,60 @@
             }), D(m, {
                 role: "combobox",
                 "aria-haspopup": "listbox",
                 "aria-expanded": "false",
                 "aria-controls": A
             });
             let J = we(m, e.inputId + "-ts-control"),
-                Q = "label[for='" + Ke(e.inputId) + "']",
+                Q = "label[for='" + je(e.inputId) + "']",
                 g = document.querySelector(Q),
                 q = e.focus.bind(e);
             if (g) {
                 B(g, "click", q), D(g, {
                     for: J
                 });
                 let b = we(g, e.inputId + "-ts-label");
                 D(m, {
                     "aria-labelledby": b
                 }), D(o, {
                     "aria-labelledby": b
                 })
             }
-            if (i.style.width = p.style.width, e.plugins.names.length) {
+            if (r.style.width = p.style.width, e.plugins.names.length) {
                 let b = "plugin-" + e.plugins.names.join(" plugin-");
-                ee([i, s], b)
+                ee([r, s], b)
             }(t.maxItems === null || t.maxItems > 1) && e.is_select_tag && D(p, {
                 multiple: "multiple"
             }), t.placeholder && D(n, {
                 placeholder: t.placeholder
             }), !t.splitOn && t.delimiter && (t.splitOn = new RegExp("\\s*" + (0, Je.escape_regex)(t.delimiter) + "+\\s*")), t.load && t.loadThrottle && (t.load = Ye(t.load, t.loadThrottle)), e.control_input.type = p.type, B(s, "mousemove", () => {
                 e.ignoreHover = !1
             }), B(s, "mouseenter", b => {
                 var P = Te(b.target, "[data-selectable]", s);
                 P && e.onOptionHover(b, P)
             }, {
                 capture: !0
             }), B(s, "click", b => {
                 let P = Te(b.target, "[data-selectable]");
-                P && (e.onOptionSelect(b, P), K(b, !0))
+                P && (e.onOptionSelect(b, P), j(b, !0))
             }), B(f, "click", b => {
                 var P = Te(b.target, "[data-ts-item]", f);
                 if (P && e.onItemSelect(b, P)) {
-                    K(b, !0);
+                    j(b, !0);
                     return
                 }
-                n.value == "" && (e.onClick(), K(b, !0))
+                n.value == "" && (e.onClick(), j(b, !0))
             }), B(m, "keydown", b => e.onKeyDown(b)), B(n, "keypress", b => e.onKeyPress(b)), B(n, "input", b => e.onInput(b)), B(m, "blur", b => e.onBlur(b)), B(m, "focus", b => e.onFocus(b)), B(n, "paste", b => e.onPaste(b));
             let H = b => {
                     let P = b.composedPath()[0];
-                    if (!i.contains(P) && !s.contains(P)) {
+                    if (!r.contains(P) && !s.contains(P)) {
                         e.isFocused && e.blur(), e.inputState();
                         return
                     }
-                    P == n && e.isOpen ? b.stopPropagation() : K(b, !0)
+                    P == n && e.isOpen ? b.stopPropagation() : j(b, !0)
                 },
                 N = () => {
                     e.isOpen && e.positionDropdown()
                 };
             B(document, "mousedown", H), B(window, "scroll", N, w), B(window, "resize", N, w), this._destroy = () => {
                 document.removeEventListener("mousedown", H), window.removeEventListener("scroll", N), window.removeEventListener("resize", N), g && g.removeEventListener("click", q)
             }, this.revertSettings = {
@@ -1199,21 +1199,21 @@
         }
         setupTemplates() {
             var e = this,
                 t = e.settings.labelField,
                 n = e.settings.optgroupLabelField,
                 s = {
                     optgroup: o => {
-                        let i = document.createElement("div");
-                        return i.className = "optgroup", i.appendChild(o.options), i
+                        let r = document.createElement("div");
+                        return r.className = "optgroup", r.appendChild(o.options), r
                     },
-                    optgroup_header: (o, i) => '<div class="optgroup-header">' + i(o[n]) + "</div>",
-                    option: (o, i) => "<div>" + i(o[t]) + "</div>",
-                    item: (o, i) => "<div>" + i(o[t]) + "</div>",
-                    option_create: (o, i) => '<div class="create">Add <strong>' + i(o.input) + "</strong>&hellip;</div>",
+                    optgroup_header: (o, r) => '<div class="optgroup-header">' + r(o[n]) + "</div>",
+                    option: (o, r) => "<div>" + r(o[t]) + "</div>",
+                    item: (o, r) => "<div>" + r(o[t]) + "</div>",
+                    option_create: (o, r) => '<div class="create">Add <strong>' + r(o.input) + "</strong>&hellip;</div>",
                     no_results: () => '<div class="no-results">No results found</div>',
                     loading: () => '<div class="spinner"></div>',
                     not_loading: () => {},
                     dropdown: () => "<div></div>"
                 };
             e.settings.render = Object.assign({}, s, e.settings.render)
         }
@@ -1258,15 +1258,15 @@
         onMouseDown() {}
         onChange() {
             _e(this.input, "input"), _e(this.input, "change")
         }
         onPaste(e) {
             var t = this;
             if (t.isInputHidden || t.isLocked) {
-                K(e);
+                j(e);
                 return
             }
             t.settings.splitOn && setTimeout(() => {
                 var n = t.inputValue();
                 if (n.match(t.settings.splitOn)) {
                     var s = n.trim().split(t.settings.splitOn);
                     (0, te.iterate)(s, o => {
@@ -1274,72 +1274,72 @@
                     })
                 }
             }, 0)
         }
         onKeyPress(e) {
             var t = this;
             if (t.isLocked) {
-                K(e);
+                j(e);
                 return
             }
             var n = String.fromCharCode(e.keyCode || e.which);
             if (t.settings.create && t.settings.mode === "multi" && n === t.settings.delimiter) {
-                t.createItem(), K(e);
+                t.createItem(), j(e);
                 return
             }
         }
         onKeyDown(e) {
             var t = this;
             if (t.ignoreHover = !0, t.isLocked) {
-                e.keyCode !== 9 && K(e);
+                e.keyCode !== 9 && j(e);
                 return
             }
             switch (e.keyCode) {
                 case 65:
                     if (oe(he, e) && t.control_input.value == "") {
-                        K(e), t.selectAll();
+                        j(e), t.selectAll();
                         return
                     }
                     break;
                 case 27:
-                    t.isOpen && (K(e, !0), t.close()), t.clearActiveItems();
+                    t.isOpen && (j(e, !0), t.close()), t.clearActiveItems();
                     return;
                 case 40:
                     if (!t.isOpen && t.hasOptions) t.open();
                     else if (t.activeOption) {
                         let n = t.getAdjacent(t.activeOption, 1);
                         n && t.setActiveOption(n)
                     }
-                    K(e);
+                    j(e);
                     return;
                 case 38:
                     if (t.activeOption) {
                         let n = t.getAdjacent(t.activeOption, -1);
                         n && t.setActiveOption(n)
                     }
-                    K(e);
+                    j(e);
                     return;
                 case 13:
-                    t.canSelect(t.activeOption) ? (t.onOptionSelect(e, t.activeOption), K(e)) : t.settings.create && t.createItem() ? K(e) : document.activeElement == t.control_input && t.isOpen && K(e);
+                    t.canSelect(t.activeOption) ? (t.onOptionSelect(e, t.activeOption), j(e)) : t.settings.create && t.createItem() ? j(e) : document.activeElement == t.control_input && t.isOpen && j(e);
                     return;
                 case 37:
                     t.advanceSelection(-1, e);
                     return;
                 case 39:
                     t.advanceSelection(1, e);
                     return;
                 case 9:
-                    t.settings.selectOnTab && (t.canSelect(t.activeOption) && (t.onOptionSelect(e, t.activeOption), K(e)), t.settings.create && t.createItem() && K(e));
+                    t.settings.selectOnTab && (t.canSelect(t.activeOption) && (t.onOptionSelect(e, t.activeOption), j(e)), t.settings.create && t.createItem() && j(e));
                     return;
                 case 8:
                 case 46:
                     t.deleteSelection(e);
                     return
             }
-            t.isInputHidden && !oe(he, e) && K(e)
+            t.isInputHidden && !oe(he, e) && j(e)
         }
         onInput(e) {
             var t = this;
             if (!t.isLocked) {
                 var n = t.inputValue();
                 t.lastValue !== n && (t.lastValue = n, t.settings.shouldLoad.call(t, n) && t.load(n), t.refreshOptions(), t.trigger("type", n))
             }
@@ -1347,15 +1347,15 @@
         onOptionHover(e, t) {
             this.ignoreHover || this.setActiveOption(t, !1)
         }
         onFocus(e) {
             var t = this,
                 n = t.isFocused;
             if (t.isDisabled) {
-                t.blur(), K(e);
+                t.blur(), j(e);
                 return
             }
             t.ignoreFocus || (t.isFocused = !0, t.settings.preload === "focus" && t.preload(), n || t.trigger("focus"), t.activeItems.length || (t.showInput(), t.refreshOptions(!!t.settings.openOnFocus)), t.refreshState())
         }
         onBlur(e) {
             if (document.hasFocus() !== !1) {
                 var t = this;
@@ -1375,29 +1375,29 @@
             }) : (n = t.dataset.value, typeof n < "u" && (s.lastQuery = null, s.addItem(n), s.settings.closeAfterSelect && s.close(), !s.settings.hideSelected && e.type && /click/.test(e.type) && s.setActiveOption(t))))
         }
         canSelect(e) {
             return !!(this.isOpen && e && this.dropdown_content.contains(e))
         }
         onItemSelect(e, t) {
             var n = this;
-            return !n.isLocked && n.settings.mode === "multi" ? (K(e), n.setActiveItem(t, e), !0) : !1
+            return !n.isLocked && n.settings.mode === "multi" ? (j(e), n.setActiveItem(t, e), !0) : !1
         }
         canLoad(e) {
             return !(!this.settings.load || this.loadedSearches.hasOwnProperty(e))
         }
         load(e) {
             let t = this;
             if (!t.canLoad(e)) return;
             ee(t.wrapper, t.settings.loadingClass), t.loading++;
             let n = t.loadCallback.bind(t);
             t.settings.load.call(t, e, n)
         }
         loadCallback(e, t) {
             let n = this;
-            n.loading = Math.max(n.loading - 1, 0), n.lastQuery = null, n.clearActiveOption(), n.setupOptions(e, t), n.refreshOptions(n.isFocused && !n.isInputHidden), n.loading || ie(n.wrapper, n.settings.loadingClass), n.trigger("load", e, t)
+            n.loading = Math.max(n.loading - 1, 0), n.lastQuery = null, n.clearActiveOption(), n.setupOptions(e, t), n.refreshOptions(n.isFocused && !n.isInputHidden), n.loading || re(n.wrapper, n.settings.loadingClass), n.trigger("load", e, t)
         }
         preload() {
             var e = this.wrapper.classList;
             e.contains("preloaded") || (e.add("preloaded"), this.load(""))
         }
         setTextboxValue(e = "") {
             var t = this.control_input,
@@ -1414,61 +1414,61 @@
             })
         }
         setMaxItems(e) {
             e === 0 && (e = null), this.settings.maxItems = e, this.refreshState()
         }
         setActiveItem(e, t) {
             var n = this,
-                s, o, i, f, p, m;
+                s, o, r, f, p, m;
             if (n.settings.mode !== "single") {
                 if (!e) {
                     n.clearActiveItems(), n.isFocused && n.showInput();
                     return
                 }
                 if (s = t && t.type.toLowerCase(), s === "click" && oe("shiftKey", t) && n.activeItems.length) {
-                    for (m = n.getLastActive(), i = Array.prototype.indexOf.call(n.control.children, m), f = Array.prototype.indexOf.call(n.control.children, e), i > f && (p = i, i = f, f = p), o = i; o <= f; o++) e = n.control.children[o], n.activeItems.indexOf(e) === -1 && n.setActiveItemClass(e);
-                    K(t)
+                    for (m = n.getLastActive(), r = Array.prototype.indexOf.call(n.control.children, m), f = Array.prototype.indexOf.call(n.control.children, e), r > f && (p = r, r = f, f = p), o = r; o <= f; o++) e = n.control.children[o], n.activeItems.indexOf(e) === -1 && n.setActiveItemClass(e);
+                    j(t)
                 } else s === "click" && oe(he, t) || s === "keydown" && oe("shiftKey", t) ? e.classList.contains("active") ? n.removeActiveItem(e) : n.setActiveItemClass(e) : (n.clearActiveItems(), n.setActiveItemClass(e));
                 n.hideInput(), n.isFocused || n.focus()
             }
         }
         setActiveItemClass(e) {
             let t = this,
                 n = t.control.querySelector(".last-active");
-            n && ie(n, "last-active"), ee(e, "active last-active"), t.trigger("item_select", e), t.activeItems.indexOf(e) == -1 && t.activeItems.push(e)
+            n && re(n, "last-active"), ee(e, "active last-active"), t.trigger("item_select", e), t.activeItems.indexOf(e) == -1 && t.activeItems.push(e)
         }
         removeActiveItem(e) {
             var t = this.activeItems.indexOf(e);
-            this.activeItems.splice(t, 1), ie(e, "active")
+            this.activeItems.splice(t, 1), re(e, "active")
         }
         clearActiveItems() {
-            ie(this.activeItems, "active"), this.activeItems = []
+            re(this.activeItems, "active"), this.activeItems = []
         }
         setActiveOption(e, t = !0) {
             e !== this.activeOption && (this.clearActiveOption(), e && (this.activeOption = e, D(this.focus_node, {
                 "aria-activedescendant": e.getAttribute("id")
             }), D(e, {
                 "aria-selected": "true"
             }), ee(e, "active"), t && this.scrollToOption(e)))
         }
         scrollToOption(e, t) {
             if (!e) return;
             let n = this.dropdown_content,
                 s = n.clientHeight,
                 o = n.scrollTop || 0,
-                i = e.offsetHeight,
+                r = e.offsetHeight,
                 f = e.getBoundingClientRect().top - n.getBoundingClientRect().top + o;
-            f + i > s + o ? this.scroll(f - s + i, t) : f < o && this.scroll(f, t)
+            f + r > s + o ? this.scroll(f - s + r, t) : f < o && this.scroll(f, t)
         }
         scroll(e, t) {
             let n = this.dropdown_content;
             t && (n.style.scrollBehavior = t), n.scrollTop = e, n.style.scrollBehavior = ""
         }
         clearActiveOption() {
-            this.activeOption && (ie(this.activeOption, "active"), D(this.activeOption, {
+            this.activeOption && (re(this.activeOption, "active"), D(this.activeOption, {
                 "aria-selected": null
             })), this.activeOption = null, D(this.focus_node, {
                 "aria-activedescendant": null
             })
         }
         selectAll() {
             let e = this;
@@ -1521,21 +1521,21 @@
         }
         search(e) {
             var t, n, s = this,
                 o = this.getSearchOptions();
             if (s.settings.score && (n = s.settings.score.call(s, e), typeof n != "function")) throw new Error('Tom Select "score" setting must be a function that returns a function');
             return e !== s.lastQuery ? (s.lastQuery = e, t = s.sifter.search(e, Object.assign(o, {
                 score: n
-            })), s.currentResults = t) : t = Object.assign({}, s.currentResults), s.settings.hideSelected && (t.items = t.items.filter(i => {
-                let f = ne(i.id);
+            })), s.currentResults = t) : t = Object.assign({}, s.currentResults), s.settings.hideSelected && (t.items = t.items.filter(r => {
+                let f = ne(r.id);
                 return !(f && s.items.indexOf(f) !== -1)
             })), t
         }
         refreshOptions(e = !0) {
-            var t, n, s, o, i, f, p, m, w, A;
+            var t, n, s, o, r, f, p, m, w, A;
             let J = {},
                 Q = [];
             var g = this,
                 q = g.inputValue();
             let H = q === g.lastQuery || q == "" && g.lastQuery == null;
             var N = g.search(q),
                 b = null,
@@ -1545,21 +1545,21 @@
                 let M = N.items[t];
                 if (!M) continue;
                 let E = M.id,
                     V = g.options[E];
                 if (V === void 0) continue;
                 let $ = me(E),
                     G = g.getOption($, !0);
-                for (g.settings.hideSelected || G.classList.toggle("selected", g.items.includes($)), i = V[g.settings.optgroupField] || "", f = Array.isArray(i) ? i : [i], n = 0, s = f && f.length; n < s; n++) {
-                    i = f[n], g.optgroups.hasOwnProperty(i) || (i = "");
-                    let W = J[i];
-                    W === void 0 && (W = document.createDocumentFragment(), Q.push(i)), n > 0 && (G = G.cloneNode(!0), D(G, {
+                for (g.settings.hideSelected || G.classList.toggle("selected", g.items.includes($)), r = V[g.settings.optgroupField] || "", f = Array.isArray(r) ? r : [r], n = 0, s = f && f.length; n < s; n++) {
+                    r = f[n], g.optgroups.hasOwnProperty(r) || (r = "");
+                    let W = J[r];
+                    W === void 0 && (W = document.createDocumentFragment(), Q.push(r)), n > 0 && (G = G.cloneNode(!0), D(G, {
                         id: V.$id + "-clone-" + n,
                         "aria-selected": null
-                    }), G.classList.add("ts-cloned"), ie(G, "active"), g.activeOption && g.activeOption.dataset.value == E && w && w.dataset.group === i.toString() && (b = G)), W.appendChild(G), J[i] = W
+                    }), G.classList.add("ts-cloned"), re(G, "active"), g.activeOption && g.activeOption.dataset.value == E && w && w.dataset.group === r.toString() && (b = G)), W.appendChild(G), J[r] = W
                 }
             }
             g.settings.lockOptgroupOrder && Q.sort((M, E) => {
                 let V = g.optgroups[M],
                     $ = g.optgroups[E],
                     G = V && V.$order || 0,
                     W = $ && $.$order || 0;
@@ -1627,30 +1627,30 @@
         }
         clearOptionGroups() {
             this.optgroups = {}, this.clearCache(), this.trigger("optgroup_clear")
         }
         updateOption(e, t) {
             let n = this;
             var s, o;
-            let i = ne(e),
+            let r = ne(e),
                 f = ne(t[n.settings.valueField]);
-            if (i === null) return;
-            let p = n.options[i];
+            if (r === null) return;
+            let p = n.options[r];
             if (p == null) return;
             if (typeof f != "string") throw new Error("Value must be set in option data");
-            let m = n.getOption(i),
-                w = n.getItem(i);
-            if (t.$order = t.$order || p.$order, delete n.options[i], n.uncacheValue(f), n.options[f] = t, m) {
+            let m = n.getOption(r),
+                w = n.getItem(r);
+            if (t.$order = t.$order || p.$order, delete n.options[r], n.uncacheValue(f), n.options[f] = t, m) {
                 if (n.dropdown_content.contains(m)) {
                     let A = n._render("option", t);
                     ge(m, A), n.activeOption === m && n.setActiveOption(A)
                 }
                 m.remove()
             }
-            w && (o = n.items.indexOf(i), o !== -1 && n.items.splice(o, 1, f), s = n._render("item", t), w.classList.contains("active") && ee(s, "active"), ge(w, s)), n.lastQuery = null
+            w && (o = n.items.indexOf(r), o !== -1 && n.items.splice(o, 1, f), s = n._render("item", t), w.classList.contains("active") && ee(s, "active"), ge(w, s)), n.lastQuery = null
         }
         removeOption(e, t) {
             let n = this;
             e = me(e), n.uncacheValue(e), delete n.userOptions[e], delete n.options[e], n.lastQuery = null, n.trigger("option_remove", e), n.removeItem(e, t)
         }
         clearOptions(e) {
             let t = (e || this.clearFilter).bind(this);
@@ -1674,79 +1674,79 @@
             return null
         }
         getAdjacent(e, t, n = "option") {
             var s = this,
                 o;
             if (!e) return null;
             n == "item" ? o = s.controlChildren() : o = s.dropdown_content.querySelectorAll("[data-selectable]");
-            for (let i = 0; i < o.length; i++)
-                if (o[i] == e) return t > 0 ? o[i + 1] : o[i - 1];
+            for (let r = 0; r < o.length; r++)
+                if (o[r] == e) return t > 0 ? o[r + 1] : o[r - 1];
             return null
         }
         getItem(e) {
             if (typeof e == "object") return e;
             var t = ne(e);
             return t !== null ? this.control.querySelector(`[data-value="${Fe(t)}"]`) : null
         }
         addItems(e, t) {
             var n = this,
                 s = Array.isArray(e) ? e : [e];
-            s = s.filter(i => n.items.indexOf(i) === -1);
+            s = s.filter(r => n.items.indexOf(r) === -1);
             let o = s[s.length - 1];
-            s.forEach(i => {
-                n.isPending = i !== o, n.addItem(i, t)
+            s.forEach(r => {
+                n.isPending = r !== o, n.addItem(r, t)
             })
         }
         addItem(e, t) {
             var n = t ? [] : ["change", "dropdown_close"];
             Me(this, n, () => {
                 var s, o;
-                let i = this,
-                    f = i.settings.mode,
+                let r = this,
+                    f = r.settings.mode,
                     p = ne(e);
-                if (!(p && i.items.indexOf(p) !== -1 && (f === "single" && i.close(), f === "single" || !i.settings.duplicates)) && !(p === null || !i.options.hasOwnProperty(p)) && (f === "single" && i.clear(t), !(f === "multi" && i.isFull()))) {
-                    if (s = i._render("item", i.options[p]), i.control.contains(s) && (s = s.cloneNode(!0)), o = i.isFull(), i.items.splice(i.caretPos, 0, p), i.insertAtCaret(s), i.isSetup) {
-                        if (!i.isPending && i.settings.hideSelected) {
-                            let m = i.getOption(p),
-                                w = i.getAdjacent(m, 1);
-                            w && i.setActiveOption(w)
-                        }!i.isPending && !i.settings.closeAfterSelect && i.refreshOptions(i.isFocused && f !== "single"), i.settings.closeAfterSelect != !1 && i.isFull() ? i.close() : i.isPending || i.positionDropdown(), i.trigger("item_add", p, s), i.isPending || i.updateOriginalInput({
+                if (!(p && r.items.indexOf(p) !== -1 && (f === "single" && r.close(), f === "single" || !r.settings.duplicates)) && !(p === null || !r.options.hasOwnProperty(p)) && (f === "single" && r.clear(t), !(f === "multi" && r.isFull()))) {
+                    if (s = r._render("item", r.options[p]), r.control.contains(s) && (s = s.cloneNode(!0)), o = r.isFull(), r.items.splice(r.caretPos, 0, p), r.insertAtCaret(s), r.isSetup) {
+                        if (!r.isPending && r.settings.hideSelected) {
+                            let m = r.getOption(p),
+                                w = r.getAdjacent(m, 1);
+                            w && r.setActiveOption(w)
+                        }!r.isPending && !r.settings.closeAfterSelect && r.refreshOptions(r.isFocused && f !== "single"), r.settings.closeAfterSelect != !1 && r.isFull() ? r.close() : r.isPending || r.positionDropdown(), r.trigger("item_add", p, s), r.isPending || r.updateOriginalInput({
                             silent: t
                         })
-                    }(!i.isPending || !o && i.isFull()) && (i.inputState(), i.refreshState())
+                    }(!r.isPending || !o && r.isFull()) && (r.inputState(), r.refreshState())
                 }
             })
         }
         removeItem(e = null, t) {
             let n = this;
             if (e = n.getItem(e), !e) return;
             var s, o;
-            let i = e.dataset.value;
-            s = Ae(e), e.remove(), e.classList.contains("active") && (o = n.activeItems.indexOf(e), n.activeItems.splice(o, 1), ie(e, "active")), n.items.splice(s, 1), n.lastQuery = null, !n.settings.persist && n.userOptions.hasOwnProperty(i) && n.removeOption(i, t), s < n.caretPos && n.setCaret(n.caretPos - 1), n.updateOriginalInput({
+            let r = e.dataset.value;
+            s = Ae(e), e.remove(), e.classList.contains("active") && (o = n.activeItems.indexOf(e), n.activeItems.splice(o, 1), re(e, "active")), n.items.splice(s, 1), n.lastQuery = null, !n.settings.persist && n.userOptions.hasOwnProperty(r) && n.removeOption(r, t), s < n.caretPos && n.setCaret(n.caretPos - 1), n.updateOriginalInput({
                 silent: t
-            }), n.refreshState(), n.positionDropdown(), n.trigger("item_remove", i, e)
+            }), n.refreshState(), n.positionDropdown(), n.trigger("item_remove", r, e)
         }
         createItem(e = null, t = () => {}) {
             arguments.length === 3 && (t = arguments[2]), typeof t != "function" && (t = () => {});
             var n = this,
                 s = n.caretPos,
                 o;
             if (e = e || n.inputValue(), !n.canCreate(e)) return t(), !1;
             n.lock();
-            var i = !1,
+            var r = !1,
                 f = p => {
                     if (n.unlock(), !p || typeof p != "object") return t();
                     var m = ne(p[n.settings.valueField]);
                     if (typeof m != "string") return t();
-                    n.setTextboxValue(), n.addOption(p, !0), n.setCaret(s), n.addItem(m), t(p), i = !0
+                    n.setTextboxValue(), n.addOption(p, !0), n.setCaret(s), n.addItem(m), t(p), r = !0
                 };
             return typeof n.settings.create == "function" ? o = n.settings.create.call(this, e, f) : o = {
                 [n.settings.labelField]: e,
                 [n.settings.valueField]: e
-            }, i || f(o), !0
+            }, r || f(o), !0
         }
         refreshItems() {
             var e = this;
             e.lastQuery = null, e.isSetup && e.addItems(e.items), e.updateOriginalInput(), e.refreshState()
         }
         refreshState() {
             let e = this;
@@ -1766,22 +1766,22 @@
         }
         updateOriginalInput(e = {}) {
             let t = this;
             var n, s;
             let o = t.input.querySelector('option[value=""]');
             if (t.is_select_tag) {
                 let p = function(m, w, A) {
-                        return m || (m = Z('<option value="' + ue(w) + '">' + ue(A) + "</option>")), m != o && t.input.append(m), i.push(m), (m != o || f > 0) && (m.selected = !0), m
+                        return m || (m = Z('<option value="' + ue(w) + '">' + ue(A) + "</option>")), m != o && t.input.append(m), r.push(m), (m != o || f > 0) && (m.selected = !0), m
                     },
-                    i = [],
+                    r = [],
                     f = t.input.querySelectorAll("option:checked").length;
                 t.input.querySelectorAll("option:checked").forEach(m => {
                     m.selected = !1
                 }), t.items.length == 0 && t.settings.mode == "single" ? p(o, "", "") : t.items.forEach(m => {
-                    if (n = t.options[m], s = n[t.settings.labelField] || "", i.includes(n.$option)) {
+                    if (n = t.options[m], s = n[t.settings.labelField] || "", r.includes(n.$option)) {
                         let w = t.input.querySelector(`option[value="${Fe(m)}"]:not(:checked)`);
                         p(w, m, s)
                     } else n.$option = p(n.$option, m, s)
                 })
             } else t.input.value = t.getValue();
             t.isSetup && (e.silent || t.trigger("change", t.getValue()))
         }
@@ -1831,26 +1831,26 @@
         insertAtCaret(e) {
             let t = this,
                 n = t.caretPos,
                 s = t.control;
             s.insertBefore(e, s.children[n] || null), t.setCaret(n + 1)
         }
         deleteSelection(e) {
-            var t, n, s, o, i = this;
-            t = e && e.keyCode === 8 ? -1 : 1, n = Be(i.control_input);
+            var t, n, s, o, r = this;
+            t = e && e.keyCode === 8 ? -1 : 1, n = Be(r.control_input);
             let f = [];
-            if (i.activeItems.length) o = Ie(i.activeItems, t), s = Ae(o), t > 0 && s++, (0, te.iterate)(i.activeItems, p => f.push(p));
-            else if ((i.isFocused || i.settings.mode === "single") && i.items.length) {
-                let p = i.controlChildren(),
+            if (r.activeItems.length) o = Ie(r.activeItems, t), s = Ae(o), t > 0 && s++, (0, te.iterate)(r.activeItems, p => f.push(p));
+            else if ((r.isFocused || r.settings.mode === "single") && r.items.length) {
+                let p = r.controlChildren(),
                     m;
-                t < 0 && n.start === 0 && n.length === 0 ? m = p[i.caretPos - 1] : t > 0 && n.start === i.inputValue().length && (m = p[i.caretPos]), m !== void 0 && f.push(m)
+                t < 0 && n.start === 0 && n.length === 0 ? m = p[r.caretPos - 1] : t > 0 && n.start === r.inputValue().length && (m = p[r.caretPos]), m !== void 0 && f.push(m)
             }
-            if (!i.shouldDelete(f, e)) return !1;
-            for (K(e, !0), typeof s < "u" && i.setCaret(s); f.length;) i.removeItem(f.pop());
-            return i.showInput(), i.positionDropdown(), i.refreshOptions(!1), !0
+            if (!r.shouldDelete(f, e)) return !1;
+            for (j(e, !0), typeof s < "u" && r.setCaret(s); f.length;) r.removeItem(f.pop());
+            return r.showInput(), r.positionDropdown(), r.refreshOptions(!1), !0
         }
         shouldDelete(e, t) {
             let n = e.map(s => s.dataset.value);
             return !(!n.length || typeof this.settings.onDelete == "function" && this.settings.onDelete(n, t) === !1)
         }
         advanceSelection(e, t) {
             var n, s, o = this;
@@ -1882,38 +1882,38 @@
         enable() {
             var e = this;
             e.input.disabled = !1, e.control_input.disabled = !1, e.focus_node.tabIndex = e.tabIndex, e.isDisabled = !1, e.unlock()
         }
         destroy() {
             var e = this,
                 t = e.revertSettings;
-            e.trigger("destroy"), e.off(), e.wrapper.remove(), e.dropdown.remove(), e.input.innerHTML = t.innerHTML, e.input.tabIndex = t.tabIndex, ie(e.input, "tomselected", "ts-hidden-accessible"), e._destroy(), delete e.input.tomselect
+            e.trigger("destroy"), e.off(), e.wrapper.remove(), e.dropdown.remove(), e.input.innerHTML = t.innerHTML, e.input.tabIndex = t.tabIndex, re(e.input, "tomselected", "ts-hidden-accessible"), e._destroy(), delete e.input.tomselect
         }
         render(e, t) {
             var n, s;
             let o = this;
             if (typeof this.settings.render[e] != "function" || (s = o.settings.render[e].call(this, t, ue), !s)) return null;
             if (s = Z(s), e === "option" || e === "option_create" ? t[o.settings.disabledField] ? D(s, {
                     "aria-disabled": "true"
                 }) : D(s, {
                     "data-selectable": ""
                 }) : e === "optgroup" && (n = t.group[o.settings.optgroupValueField], D(s, {
                     "data-group": n
                 }), t.group[o.settings.disabledField] && D(s, {
                     "data-disabled": ""
                 })), e === "option" || e === "item") {
-                let i = me(t[o.settings.valueField]);
+                let r = me(t[o.settings.valueField]);
                 D(s, {
-                    "data-value": i
+                    "data-value": r
                 }), e === "item" ? (ee(s, o.settings.itemClass), D(s, {
                     "data-ts-item": ""
                 })) : (ee(s, o.settings.optionClass), D(s, {
                     role: "option",
                     id: t.$id
-                }), t.$div = s, o.options[i] = t)
+                }), t.$div = s, o.options[r] = t)
             }
             return s
         }
         _render(e, t) {
             let n = this.render(e, t);
             if (n == null) throw "HTMLElement expected";
             return n
@@ -1930,50 +1930,50 @@
         canCreate(e) {
             return this.settings.create && e.length > 0 && this.settings.createFilter.call(this, e)
         }
         hook(e, t, n) {
             var s = this,
                 o = s[t];
             s[t] = function() {
-                var i, f;
-                return e === "after" && (i = o.apply(s, arguments)), f = n.apply(s, arguments), e === "instead" ? f : (e === "before" && (i = o.apply(s, arguments)), i)
+                var r, f;
+                return e === "after" && (r = o.apply(s, arguments)), f = n.apply(s, arguments), e === "instead" ? f : (e === "before" && (r = o.apply(s, arguments)), r)
             }
         }
     };
 
-function We(r) {
+function We(i) {
     let u = Object.assign({
         label: "&times;",
         title: "Remove",
         className: "remove",
         append: !0
-    }, r);
+    }, i);
     var e = this;
     if (u.append) {
         var t = '<a href="javascript:void(0)" class="' + u.className + '" tabindex="-1" title="' + ue(u.title) + '">' + u.label + "</a>";
         e.hook("after", "setupTemplates", () => {
             var n = e.settings.render.item;
             e.settings.render.item = (s, o) => {
-                var i = Z(n.call(e, s, o)),
+                var r = Z(n.call(e, s, o)),
                     f = Z(t);
-                return i.appendChild(f), B(f, "mousedown", p => {
-                    K(p, !0)
+                return r.appendChild(f), B(f, "mousedown", p => {
+                    j(p, !0)
                 }), B(f, "click", p => {
-                    K(p, !0), !e.isLocked && e.shouldDelete([i], p) && (e.removeItem(i), e.refreshOptions(!1), e.inputState())
-                }), i
+                    j(p, !0), !e.isLocked && e.shouldDelete([r], p) && (e.removeItem(r), e.refreshOptions(!1), e.inputState())
+                }), r
             }
         })
     }
 }
 var tt = ve(nt());
-var Xe = ".ts-wrapper{position:relative}.ts-wrapper .ts-control{overflow:hidden;box-sizing:border-box;display:flex;flex-wrap:wrap;align-content:center}.ts-wrapper .ts-control>input{flex:1 1 auto;box-sizing:border-box;user-select:auto;box-shadow:none;border:none;padding:0;font-size:inherit;font-weight:inherit;font-style:inherit;font-family:inherit;caret-color:rgba(0,0,0,.15)}.ts-wrapper .ts-control>input::placeholder{opacity:1}.ts-wrapper .ts-control>input::-ms-clear{display:none}.ts-wrapper .ts-control>input:focus{outline:none !important}.ts-wrapper .ts-control>div{flex:0 1 auto;box-sizing:border-box}.ts-wrapper.multi .ts-control{padding:0 6px 3px 10px}.ts-wrapper.multi .ts-control>div{border:1px solid rgba(0,0,0,.15);border-radius:3px;margin:3px 3px 0 0}.ts-wrapper.multi .ts-control>div .remove{text-decoration:none;color:rgba(0,0,0,.15);border-left:1px solid rgba(0,0,0,.15);padding-left:2px;margin-left:2px}.ts-wrapper.multi .ts-control>div .remove:hover{color:inherit}.ts-wrapper.multi .ts-control>div.active{background-color:rgba(0,0,0,.05)}.ts-wrapper.multi.full .ts-control>input{visibility:hidden}.ts-wrapper.multi.has-items:not(.dirty) .ts-control>input::placeholder{opacity:0}.ts-wrapper.focus .ts-control{opacity:1}.ts-wrapper.disabled .ts-control{opacity:1}.ts-wrapper.input-hidden .ts-control>input{opacity:0;position:absolute;left:-10000px}.ts-wrapper:not(.multi).dirty.focus .ts-control .item{display:none}.ts-wrapper .ts-dropdown{position:absolute;top:100%;left:0;width:100%;z-index:10;background:#f4f4f4;backdrop-filter:blur(0.5rem);margin:.125rem 0 0 0;border-top:0 none;box-sizing:border-box}.ts-wrapper .ts-dropdown [data-selectable]{cursor:pointer;overflow:hidden}.ts-wrapper .ts-dropdown [data-selectable]:hover{background-color:#e0ecf4}.ts-wrapper .ts-dropdown [data-selectable] .highlight{background:rgba(255,237,40,.4);border-radius:1px}.ts-wrapper .ts-dropdown .ts-dropdown-content{overflow-y:auto;overflow-x:hidden;overflow-scrolling:touch;scroll-behavior:smooth}.ts-wrapper .ts-dropdown .optgroup .optgroup-header{opacity:.5}.ts-wrapper .ts-dropdown .optgroup .option{margin-left:1em}:host-context(django-field-group.dj-touched) .ts-wrapper.has-items:not(.input-active) .ts-control{border-color:var(--django-formset-color-valid)}:host-context(django-field-group.dj-touched) .ts-wrapper.invalid:not(.input-active) .ts-control{border-color:var(--django-formset-color-invalid)}:host-context(django-field-group.dj-submitted) .ts-wrapper.invalid .ts-control{border-color:var(--django-formset-color-invalid)}:host-context(django-field-group.dj-submitted) .ts-wrapper.invalid.focus .ts-control{opacity:1}";
+var Xe = ".ts-wrapper{position:relative}.ts-wrapper .ts-control{overflow:hidden;box-sizing:border-box;display:flex;flex-wrap:wrap;align-content:center}.ts-wrapper .ts-control>input{flex:1 1 auto;box-sizing:border-box;user-select:auto;box-shadow:none;border:none;padding:0;font-size:inherit;font-weight:inherit;font-style:inherit;font-family:inherit;caret-color:rgba(0,0,0,.15)}.ts-wrapper .ts-control>input::placeholder{opacity:1}.ts-wrapper .ts-control>input::-ms-clear{display:none}.ts-wrapper .ts-control>input:focus{outline:none !important}.ts-wrapper .ts-control>div{flex:0 1 auto;box-sizing:border-box}.ts-wrapper.multi .ts-control{padding:0 6px 3px 10px}.ts-wrapper.multi .ts-control>div{border:1px solid rgba(0,0,0,.15);border-radius:3px;margin:3px 3px 0 0}.ts-wrapper.multi .ts-control>div .remove{text-decoration:none;color:rgba(0,0,0,.15);border-left:1px solid rgba(0,0,0,.15);padding-left:2px;margin-left:2px}.ts-wrapper.multi .ts-control>div .remove:hover{color:inherit}.ts-wrapper.multi .ts-control>div.active{background-color:rgba(0,0,0,.05)}.ts-wrapper.multi.full .ts-control>input{visibility:hidden}.ts-wrapper.multi.has-items:not(.dirty) .ts-control>input::placeholder{opacity:0}.ts-wrapper.focus .ts-control{opacity:1}.ts-wrapper.disabled .ts-control{opacity:1}.ts-wrapper.input-hidden .ts-control>input{opacity:0;position:absolute;left:-10000px}.ts-wrapper:not(.multi).dirty.focus .ts-control .item{display:none}.ts-wrapper .ts-dropdown{position:absolute;top:100%;left:0;width:100%;z-index:10;background:#f4f4f4;backdrop-filter:blur(0.5rem);margin:.125rem 0 0 0;border-top:0 none;box-sizing:border-box}.ts-wrapper .ts-dropdown [data-selectable]{cursor:pointer;overflow:hidden}.ts-wrapper .ts-dropdown [data-selectable]:hover{background-color:#e0ecf4}.ts-wrapper .ts-dropdown [data-selectable] .highlight{background:rgba(255,237,40,.4);border-radius:1px}.ts-wrapper .ts-dropdown .ts-dropdown-content{overflow-y:auto;overflow-x:hidden;overflow-scrolling:touch;scroll-behavior:smooth}.ts-wrapper .ts-dropdown .optgroup .optgroup-header{opacity:.5}.ts-wrapper .ts-dropdown .optgroup .option{margin-left:1em}:host-context([role=group].dj-touched) .ts-wrapper.has-items:not(.input-active) .ts-control{border-color:var(--django-formset-color-valid)}:host-context([role=group].dj-touched) .ts-wrapper.invalid:not(.input-active) .ts-control{border-color:var(--django-formset-color-invalid)}:host-context([role=group].dj-submitted) .ts-wrapper.invalid .ts-control{border-color:var(--django-formset-color-invalid)}:host-context([role=group].dj-submitted) .ts-wrapper.invalid.focus .ts-control{opacity:1}";
 de.define("remove_button", We);
 var He = class extends Pe {
         constructor(e) {
-            var o, i;
+            var o, r;
             super(e);
             this.numOptions = 12;
             this.load = (e, t) => {
                 this.loadOptions(this.buildFetchQuery(0, e), n => {
                     t(n, this.extractOptGroups(n))
                 })
             };
@@ -2015,15 +2015,15 @@
                 let f = (o = e.parentElement) == null ? void 0 : o.querySelector("template.selectize-remove-item");
                 t.plugins = {
                     remove_button: {
                         title: (f == null ? void 0 : f.innerHTML) ?? "Remove item"
                     }
                 };
                 let p = `${e.getAttribute("id")}_initial`;
-                t.items = JSON.parse(((i = document.getElementById(p)) == null ? void 0 : i.textContent) ?? "[]"), e.removeAttribute("multiple"), n = !0
+                t.items = JSON.parse(((r = document.getElementById(p)) == null ? void 0 : r.textContent) ?? "[]"), e.removeAttribute("multiple"), n = !0
             }
             let s = {
                 ...window.getComputedStyle(e)
             };
             n && e.setAttribute("multiple", "multiple"), this.numOptions = parseInt(e.getAttribute("options") ?? this.numOptions.toString()), this.tomSelect = new de(e, t), this.observer = new MutationObserver(this.attributesChanged), this.observer.observe(this.tomInput, {
                 attributes: !0
             }), this.initialValue = this.tomSelect.getValue(), this.shadowRoot = this.wrapInShadowRoot(), this.transferStyles(e, s), e.classList.add("dj-concealed"), this.validateInput(this.initialValue), this.tomSelect.on("change", f => this.validateInput(f)), this.setupFilters(e)
@@ -2070,47 +2070,47 @@
             let s = this.tomInput.parentElement.removeChild(this.tomSelect.wrapper);
             return t.appendChild(s), t
         }
         transferStyles(e, t) {
             this.shadowRoot.host.style.setProperty("display", t.display);
             let s = window.getComputedStyle(e).getPropertyValue("line-height"),
                 o = e.querySelector("option"),
-                i = this.shadowRoot.styleSheets.item(0),
+                r = this.shadowRoot.styleSheets.item(0),
                 f = Math.min(Math.max(this.numOptions, 8), 25);
-            for (let p = 0; i && p < i.cssRules.length; p++) {
-                let m = i.cssRules.item(p),
+            for (let p = 0; r && p < r.cssRules.length; p++) {
+                let m = r.cssRules.item(p),
                     w;
                 switch (m.selectorText) {
                     case ".ts-wrapper":
-                        w = se.extractStyles(e, ["font-family", "font-size", "font-strech", "font-style", "font-weight", "letter-spacing", "white-space"]), i.insertRule(`${m.selectorText}{${w}}`, ++p);
+                        w = se.extractStyles(e, ["font-family", "font-size", "font-strech", "font-style", "font-weight", "letter-spacing", "white-space"]), r.insertRule(`${m.selectorText}{${w}}`, ++p);
                         break;
                     case ".ts-wrapper .ts-control":
-                        w = se.extractStyles(e, ["background-color", "border", "border-radius", "box-shadow", "color", "padding"]).concat(`width: ${t.width}; min-height: ${t.height};`), i.insertRule(`${m.selectorText}{${w}}`, ++p);
+                        w = se.extractStyles(e, ["background-color", "border", "border-radius", "box-shadow", "color", "padding"]).concat(`width: ${t.width}; min-height: ${t.height};`), r.insertRule(`${m.selectorText}{${w}}`, ++p);
                         break;
                     case ".ts-wrapper .ts-control > input":
                     case ".ts-wrapper .ts-control > div":
-                        o && (w = se.extractStyles(o, ["padding-left", "padding-right"]), i.insertRule(`${m.selectorText}{${w}}`, ++p));
+                        o && (w = se.extractStyles(o, ["padding-left", "padding-right"]), r.insertRule(`${m.selectorText}{${w}}`, ++p));
                         break;
                     case ".ts-wrapper .ts-control > input::placeholder":
-                        e.classList.add("-placeholder-"), w = se.extractStyles(e, ["background-color", "color"]), e.classList.remove("-placeholder-"), i.insertRule(`${m.selectorText}{${w}}`, ++p);
+                        e.classList.add("-placeholder-"), w = se.extractStyles(e, ["background-color", "color"]), e.classList.remove("-placeholder-"), r.insertRule(`${m.selectorText}{${w}}`, ++p);
                         break;
                     case ".ts-wrapper.focus .ts-control":
-                        e.style.transition = "none", e.classList.add("-focus-"), w = se.extractStyles(e, ["background-color", "border", "box-shadow", "color", "outline", "transition"]), e.classList.remove("-focus-"), i.insertRule(`${m.selectorText}{${w}}`, ++p), e.style.transition = "";
+                        e.style.transition = "none", e.classList.add("-focus-"), w = se.extractStyles(e, ["background-color", "border", "box-shadow", "color", "outline", "transition"]), e.classList.remove("-focus-"), r.insertRule(`${m.selectorText}{${w}}`, ++p), e.style.transition = "";
                         break;
                     case ".ts-wrapper.disabled .ts-control":
-                        e.classList.add("-disabled-"), w = se.extractStyles(e, ["background-color", "border", "box-shadow", "color", "opacity", "outline", "transition"]), e.classList.remove("-disabled-"), i.insertRule(`${m.selectorText}{${w}}`, ++p);
+                        e.classList.add("-disabled-"), w = se.extractStyles(e, ["background-color", "border", "box-shadow", "color", "opacity", "outline", "transition"]), e.classList.remove("-disabled-"), r.insertRule(`${m.selectorText}{${w}}`, ++p);
                         break;
                     case ".ts-wrapper .ts-dropdown":
-                        w = se.extractStyles(e, ["border-right", "border-bottom", "border-left", "color", "padding-left"]).concat(parseFloat(s) > 0 ? `line-height: calc(${s} * 1.2);` : "line-height: 1.4em;"), i.insertRule(`${m.selectorText}{${w}}`, ++p);
+                        w = se.extractStyles(e, ["border-right", "border-bottom", "border-left", "color", "padding-left"]).concat(parseFloat(s) > 0 ? `line-height: calc(${s} * 1.2);` : "line-height: 1.4em;"), r.insertRule(`${m.selectorText}{${w}}`, ++p);
                         break;
                     case ".ts-wrapper .ts-dropdown .ts-dropdown-content":
-                        parseFloat(s) > 0 ? w = `max-height: calc(${s} * 1.2 * ${f});` : w = `max-height: ${f*1.4}em;`, i.insertRule(`${m.selectorText}{${w}}`, ++p);
+                        parseFloat(s) > 0 ? w = `max-height: calc(${s} * 1.2 * ${f});` : w = `max-height: ${f*1.4}em;`, r.insertRule(`${m.selectorText}{${w}}`, ++p);
                         break;
-                    case ":host-context(django-field-group.dj-submitted) .ts-wrapper.invalid.focus .ts-control":
-                        e.style.transition = "none", e.classList.add("-focus-", "-invalid-", "is-invalid"), w = se.extractStyles(e, ["background-color", "border", "box-shadow", "color", "outline", "transition"]), e.classList.remove("-focus-", "-invalid-", "is-invalid"), i.insertRule(`${m.selectorText}{${w}}`, ++p), e.style.transition = "";
+                    case ':host-context([role="group"].dj-submitted) .ts-wrapper.invalid.focus .ts-control':
+                        e.style.transition = "none", e.classList.add("-focus-", "-invalid-", "is-invalid"), w = se.extractStyles(e, ["background-color", "border", "box-shadow", "color", "outline", "transition"]), e.classList.remove("-focus-", "-invalid-", "is-invalid"), r.insertRule(`${m.selectorText}{${w}}`, ++p), e.style.transition = "";
                         break;
                     default:
                         break
                 }
             }
         }
         setupRender(e) {
```

### Comparing `django-formset-1.0.dev3/formset/static/formset/js/DjangoSlug-226MVQ6E.js` & `django-formset-1.0.dev4/formset/static/formset/js/DjangoSlug-226MVQ6E.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/js/DualSelector-GVLJZFWV.js` & `django-formset-1.0.dev4/formset/static/formset/js/DualSelector-2ALH4RIS.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
 import {
     a as d
-} from "./chunk-AELXO3WZ.js";
+} from "./chunk-MD4VW33H.js";
 import {
     a as u,
     b as p
-} from "./chunk-IE6INVWL.js";
+} from "./chunk-EJ4RWPXK.js";
 import "./chunk-APVD22ED.js";
 import {
     a as g
 } from "./chunk-KDP4ZIAK.js";
 import {
     a as r
-} from "./chunk-O5UGFU32.js";
+} from "./chunk-R2VNGMYE.js";
 import {
     b as L
 } from "./chunk-NLMHZ7JJ.js";
 var f = L(g());
 var h = class extends d {
         constructor(e, t) {
             var o;
@@ -208,15 +208,15 @@
         }
         setHistoryCursor(e) {
             this.historyCursor = e, this.undoButton && (this.undoButton.disabled = e === 0), this.redoButton && (this.redoButton.disabled = e === this.historicalValues.length - 1)
         }
         transferStyles() {
             let e = this.declaredStyles.sheet,
                 t = r.extractStyles(this.selectLeftElement, ["background-color"]);
-            e.insertRule(`django-formset django-field-group .dj-dual-selector .left-column{${t}}`, 0), t = r.extractStyles(this.selectRightElement, ["background-color"]), e.insertRule(`django-formset django-field-group .dj-dual-selector .right-column{${t}}`, 1), e.insertRule(".dj-dual-selector select, .dj-dual-selector input{background-color: transparent;}", 2), t = r.extractStyles(this.selectLeftElement, ["height"]), e.insertRule(`django-formset django-field-group .dj-dual-selector select{${t}}`, 3)
+            e.insertRule(`django-formset [role="group"] .dj-dual-selector .left-column{${t}}`, 0), t = r.extractStyles(this.selectRightElement, ["background-color"]), e.insertRule(`django-formset [role="group"] .dj-dual-selector .right-column{${t}}`, 1), e.insertRule(".dj-dual-selector select, .dj-dual-selector input{background-color: transparent;}", 2), t = r.extractStyles(this.selectLeftElement, ["height"]), e.insertRule(`django-formset [role="group"] .dj-dual-selector select{${t}}`, 3)
         }
         formResetted(e) {
             var i;
             this.clearSearchFields();
             let t = this.historicalValues[0];
             this.historicalValues.splice(1), this.setHistoryCursor(0), Array.from(this.selectRightElement.querySelectorAll("option")).filter(o => t.indexOf(o.value) === -1).forEach(o => {
                 this.moveOptionToSelectElement(o, this.selectLeftElement)
```

### Comparing `django-formset-1.0.dev3/formset/static/formset/js/RichtextArea-UTSZPGIP.js` & `django-formset-1.0.dev4/formset/static/formset/js/RichtextArea-XKK27UIM.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2,15 +2,15 @@
     a as bc
 } from "./chunk-KDP4ZIAK.js";
 import {
     d as Vs
 } from "./chunk-ISEEQP4V.js";
 import {
     a as Ue
-} from "./chunk-O5UGFU32.js";
+} from "./chunk-R2VNGMYE.js";
 import {
     b as yc
 } from "./chunk-NLMHZ7JJ.js";
 var Js = '.dj-richtext-wrapper{--button-active: rgba(0, 0, 0, 0.1);--button-opacity: 0.5;position:relative;overflow:auto}.dj-richtext-wrapper [role=menubar]{border:none;position:absolute;inset:0 0 auto 0;padding:.125rem .25rem}.dj-richtext-wrapper [role=menubar] [role=separator]{display:inline-block;padding:.25rem 0;vertical-align:middle}.dj-richtext-wrapper [role=menubar] button{display:inline-block;text-align:center;text-decoration:none;vertical-align:middle;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;user-select:none;border:none;border-radius:.25rem;padding:.25rem;background-color:inherit;opacity:var(--button-opacity)}.dj-richtext-wrapper [role=menubar] button:hover{opacity:1}.dj-richtext-wrapper [role=menubar] button.active{opacity:1;background-color:var(--button-active)}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]:after{border-bottom:0;border-left:.3em solid rgba(0,0,0,0);border-right:.3em solid rgba(0,0,0,0);border-top:.3em solid;margin-right:.125rem;content:"";display:inline-block;transition:transform 250ms ease-in-out}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true][aria-expanded=true]:after{transform:scaleY(-1)}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]+ul[role=menu]{display:none;position:absolute;width:max-content;top:0;left:0;padding:inherit;list-style:none;background-color:inherit;border-color:#000}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]+ul[role=menu]>li{background-color:inherit;opacity:var(--button-opacity)}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]+ul[role=menu]>li:hover{opacity:1}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]+ul[role=menu]>li.active{color:inherit;opacity:1;background-color:var(--button-active)}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true][aria-expanded=true]+ul[role=menu]{display:block}.dj-richtext-wrapper [role=menubar] button>svg{vertical-align:middle;display:inline}.dj-richtext-wrapper .character-count{position:absolute;bottom:3px;right:6px;color:rgba(0,0,0,.2)}.dj-richtext-wrapper .ProseMirror{border:none;position:absolute;left:0;right:0;bottom:0;word-wrap:break-word;white-space:break-spaces;font-variant-ligatures:none;font-feature-settings:"liga" 0;overflow:hidden}.dj-richtext-wrapper .ProseMirror[contenteditable=false]{white-space:normal}.dj-richtext-wrapper .ProseMirror p{margin-bottom:.5rem}.dj-richtext-wrapper .ProseMirror p.is-editor-empty:first-child::before{color:rgba(0,0,0,.2);content:attr(data-placeholder);float:left;height:0;pointer-events:none}.dj-richtext-wrapper .ProseMirror p[data-text=indent]{text-indent:3em}.dj-richtext-wrapper .ProseMirror p[data-text=outdent]{text-indent:-3em;padding-left:3em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="1"]{margin-left:2em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="2"]{margin-left:4em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="3"]{margin-left:6em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="4"]{margin-left:8em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="5"]{margin-left:10em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="6"]{margin-left:12em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="7"]{margin-left:14em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="8"]{margin-left:16em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="9"]{margin-left:18em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="10"]{margin-left:20em}.dj-richtext-wrapper .ProseMirror li>p{margin:0}.dj-richtext-wrapper .ProseMirror:focus-visible{outline:none}.dj-richtext-wrapper .ProseMirror blockquote{border-left:3px solid rgba(0,0,0,.2);padding-left:1rem}.dj-richtext-wrapper .ProseMirror output[role=placeholder]{background-color:rgba(0,0,0,.03);box-shadow:inset 0 0 5px rgba(0,0,0,.7)}.dj-richtext-wrapper .ProseMirror pre{padding:.5rem 1rem;background-color:rgba(0,0,0,.03);font-family:monospace}.dj-richtext-wrapper .ProseMirror pre{white-space:pre-wrap}.dj-richtext-wrapper.focused{opacity:1}.dj-submitted .dj-richtext-wrapper.focused.invalid{opacity:1}.dj-richtext-wrapper:not(.focused).invalid{border-color:var(--django-formset-color-invalid)}.dj-richtext-wrapper:not(.focused).valid{border-color:var(--django-formset-color-valid)}';
 
 function te(n) {
     this.content = n
```

### Comparing `django-formset-1.0.dev3/formset/static/formset/js/chunk-AELXO3WZ.js` & `django-formset-1.0.dev4/formset/static/formset/js/chunk-MD4VW33H.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     b as c
-} from "./chunk-O5UGFU32.js";
+} from "./chunk-R2VNGMYE.js";
 var l = class extends c {
     constructor(n) {
         super(n);
         this.filterByValues = new Map;
         this.touch = () => {
             this.fieldGroup.classList.remove("dj-untouched", "dj-validated"), this.fieldGroup.classList.add("dj-touched")
         };
```

### Comparing `django-formset-1.0.dev3/formset/static/formset/js/chunk-APVD22ED.js` & `django-formset-1.0.dev4/formset/static/formset/js/chunk-APVD22ED.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/js/chunk-IE6INVWL.js` & `django-formset-1.0.dev4/formset/static/formset/js/chunk-EJ4RWPXK.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     a as i,
     b as l
 } from "./chunk-APVD22ED.js";
 import {
     a as r
-} from "./chunk-O5UGFU32.js";
+} from "./chunk-R2VNGMYE.js";
 var c = "django-sortable-select{background-color:rgba(0,0,0,0) !important}django-sortable-select.focus{opacity:1}django-sortable-select option.sortable-selected,django-sortable-select optgroup.sortable-selected{opacity:1;cursor:grab}django-sortable-select option.sortable-chosen,django-sortable-select option.sortable-ghost,django-sortable-select optgroup.sortable-chosen,django-sortable-select optgroup.sortable-ghost{opacity:1;cursor:grabbing !important}django-sortable-select option{display:block;line-height:normal;cursor:default}django-sortable-select option.sortable-chosen,django-sortable-select option.sortable-selected{opacity:1}django-sortable-select optgroup option::before{opacity:1}";
 l.mount(new i);
 var d = class extends HTMLElement {
         constructor() {
             super();
             this.lastSelected = null;
             this.declaredStyles = document.createElement("style"), this.declaredStyles.innerText = c, document.head.appendChild(this.declaredStyles), this.addEventListener("click", e => this.optionSelected(e)), window.addEventListener("click", e => this.elementFocus(e))
```

### Comparing `django-formset-1.0.dev3/formset/static/formset/js/chunk-ISEEQP4V.js` & `django-formset-1.0.dev4/formset/static/formset/js/chunk-ISEEQP4V.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/js/chunk-KDP4ZIAK.js` & `django-formset-1.0.dev4/formset/static/formset/js/chunk-KDP4ZIAK.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/js/chunk-NLMHZ7JJ.js` & `django-formset-1.0.dev4/formset/static/formset/js/chunk-NLMHZ7JJ.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/js/chunk-O5UGFU32.js` & `django-formset-1.0.dev4/formset/static/formset/js/chunk-R2VNGMYE.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -40,15 +40,15 @@
             let e = t.selectorText.replaceAll(":focus", ".-focus-").replaceAll(":focus-visible", ".-focus-visible-").replaceAll(":hover", ".-hover-").replaceAll(":disabled", ".-disabled-").replaceAll(":invalid", ".-invalid-").replaceAll(":valid", ".-valid-").replaceAll("::placeholder-shown", ".-placeholder-shown").replaceAll(":placeholder-shown", ".-placeholder-shown").replaceAll("::placeholder", ".-placeholder-").replaceAll(":placeholder", ".-placeholder-");
             e !== t.selectorText && o.insertRule(`${e}{${t.style.cssText}}`)
         }
     }
 })(a || (a = {}));
 var d = class {
     constructor(r) {
-        let n = r.closest("django-field-group"),
+        let n = r.closest('[role="group"]'),
             s = r.form,
             t = r.closest("django-formset");
         if (!n || !s || !t) throw new Error(`Attempt to initialize ${r} outside <django-formset>`);
         let o = s.getAttribute("name") ?? "__default__";
         this.fieldGroup = n, this.endpoint = t.getAttribute("endpoint"), this.fieldName = `${o}.${r.getAttribute("name")}`, s.addEventListener("reset", e => this.formResetted(e)), s.addEventListener("submitted", e => this.formSubmitted(e))
     }
 };
```

### Comparing `django-formset-1.0.dev3/formset/static/formset/js/django-formset.js` & `django-formset-1.0.dev4/formset/static/formset/js/django-formset.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -2,23 +2,23 @@
     b as lr
 } from "./chunk-APVD22ED.js";
 import {
     a as sr
 } from "./chunk-KDP4ZIAK.js";
 import {
     a as dr
-} from "./chunk-O5UGFU32.js";
+} from "./chunk-R2VNGMYE.js";
 import {
-    a as vt,
+    a as yt,
     b as _e
 } from "./chunk-NLMHZ7JJ.js";
-var Er = vt((ks, wr) => {
+var wr = yt((ks, Er) => {
     var qn = "Expected a function",
-        gr = "__lodash_hash_undefined__",
-        mr = 1 / 0,
+        mr = "__lodash_hash_undefined__",
+        gr = 1 / 0,
         zn = "[object Function]",
         Un = "[object GeneratorFunction]",
         Kn = "[object Symbol]",
         Jn = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
         Wn = /^\w*$/,
         Xn = /^\./,
         Zn = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
@@ -39,27 +39,27 @@
             e = !!(t + "")
         } catch {}
         return e
     }
     var io = Array.prototype,
         ao = Function.prototype,
         hr = Object.prototype,
-        yt = xt["__core-js_shared__"],
+        jt = xt["__core-js_shared__"],
         cr = function() {
-            var t = /[^.]+$/.exec(yt && yt.keys && yt.keys.IE_PROTO || "");
+            var t = /[^.]+$/.exec(jt && jt.keys && jt.keys.IE_PROTO || "");
             return t ? "Symbol(src)_1." + t : ""
         }(),
         br = ao.toString,
-        wt = hr.hasOwnProperty,
-        jr = hr.toString,
-        so = RegExp("^" + br.call(wt).replace(Yn, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
+        Et = hr.hasOwnProperty,
+        vr = hr.toString,
+        so = RegExp("^" + br.call(Et).replace(Yn, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
         ur = xt.Symbol,
         lo = io.splice,
-        co = vr(xt, "Map"),
-        Ce = vr(Object, "create"),
+        co = yr(xt, "Map"),
+        Ce = yr(Object, "create"),
         fr = ur ? ur.prototype : void 0,
         pr = fr ? fr.toString : void 0;
 
     function ne(t) {
         var e = -1,
             r = t ? t.length : 0;
         for (this.clear(); ++e < r;) {
@@ -76,35 +76,35 @@
         return this.has(t) && delete this.__data__[t]
     }
 
     function po(t) {
         var e = this.__data__;
         if (Ce) {
             var r = e[t];
-            return r === gr ? void 0 : r
+            return r === mr ? void 0 : r
         }
-        return wt.call(e, t) ? e[t] : void 0
+        return Et.call(e, t) ? e[t] : void 0
     }
 
-    function go(t) {
+    function mo(t) {
         var e = this.__data__;
-        return Ce ? e[t] !== void 0 : wt.call(e, t)
+        return Ce ? e[t] !== void 0 : Et.call(e, t)
     }
 
-    function mo(t, e) {
+    function go(t, e) {
         var r = this.__data__;
-        return r[t] = Ce && e === void 0 ? gr : e, this
+        return r[t] = Ce && e === void 0 ? mr : e, this
     }
     ne.prototype.clear = uo;
     ne.prototype.delete = fo;
     ne.prototype.get = po;
-    ne.prototype.has = go;
-    ne.prototype.set = mo;
+    ne.prototype.has = mo;
+    ne.prototype.set = go;
 
-    function ge(t) {
+    function me(t) {
         var e = -1,
             r = t ? t.length : 0;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
@@ -117,70 +117,70 @@
         var e = this.__data__,
             r = Ue(e, t);
         if (r < 0) return !1;
         var n = e.length - 1;
         return r == n ? e.pop() : lo.call(e, r, 1), !0
     }
 
-    function jo(t) {
+    function vo(t) {
         var e = this.__data__,
             r = Ue(e, t);
         return r < 0 ? void 0 : e[r][1]
     }
 
-    function vo(t) {
+    function yo(t) {
         return Ue(this.__data__, t) > -1
     }
 
-    function yo(t, e) {
+    function jo(t, e) {
         var r = this.__data__,
             n = Ue(r, t);
         return n < 0 ? r.push([t, e]) : r[n][1] = e, this
     }
-    ge.prototype.clear = ho;
-    ge.prototype.delete = bo;
-    ge.prototype.get = jo;
-    ge.prototype.has = vo;
-    ge.prototype.set = yo;
+    me.prototype.clear = ho;
+    me.prototype.delete = bo;
+    me.prototype.get = vo;
+    me.prototype.has = yo;
+    me.prototype.set = jo;
 
     function oe(t) {
         var e = -1,
             r = t ? t.length : 0;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
     function xo() {
         this.__data__ = {
             hash: new ne,
-            map: new(co || ge),
+            map: new(co || me),
             string: new ne
         }
     }
 
-    function wo(t) {
+    function Eo(t) {
         return Ke(this, t).delete(t)
     }
 
-    function Eo(t) {
+    function wo(t) {
         return Ke(this, t).get(t)
     }
 
     function ko(t) {
         return Ke(this, t).has(t)
     }
 
     function Ao(t, e) {
         return Ke(this, t).set(t, e), this
     }
     oe.prototype.clear = xo;
-    oe.prototype.delete = wo;
-    oe.prototype.get = Eo;
+    oe.prototype.delete = Eo;
+    oe.prototype.get = wo;
     oe.prototype.has = ko;
     oe.prototype.set = Ao;
 
     function Ue(t, e) {
         for (var r = t.length; r--;)
             if (Do(t[r][0], e)) return r;
         return -1
@@ -198,119 +198,119 @@
         return e.test(Po(t))
     }
 
     function Co(t) {
         if (typeof t == "string") return t;
         if (kt(t)) return pr ? pr.call(t) : "";
         var e = t + "";
-        return e == "0" && 1 / t == -mr ? "-0" : e
+        return e == "0" && 1 / t == -gr ? "-0" : e
     }
 
     function Fo(t) {
-        return yr(t) ? t : Mo(t)
+        return jr(t) ? t : Mo(t)
     }
 
     function Ke(t, e) {
         var r = t.__data__;
         return Lo(e) ? r[typeof e == "string" ? "string" : "hash"] : r.map
     }
 
-    function vr(t, e) {
+    function yr(t, e) {
         var r = no(t, e);
         return _o(r) ? r : void 0
     }
 
     function So(t, e) {
-        if (yr(t)) return !1;
+        if (jr(t)) return !1;
         var r = typeof t;
         return r == "number" || r == "symbol" || r == "boolean" || t == null || kt(t) ? !0 : Wn.test(t) || !Jn.test(t) || e != null && t in Object(e)
     }
 
     function Lo(t) {
         var e = typeof t;
         return e == "string" || e == "number" || e == "symbol" || e == "boolean" ? t !== "__proto__" : t === null
     }
 
     function $o(t) {
         return !!cr && cr in t
     }
-    var Mo = Et(function(t) {
+    var Mo = wt(function(t) {
         t = Ro(t);
         var e = [];
         return Xn.test(t) && e.push(""), t.replace(Zn, function(r, n, i, o) {
             e.push(i ? o.replace(Qn, "$1") : n || r)
         }), e
     });
 
     function Io(t) {
         if (typeof t == "string" || kt(t)) return t;
         var e = t + "";
-        return e == "0" && 1 / t == -mr ? "-0" : e
+        return e == "0" && 1 / t == -gr ? "-0" : e
     }
 
     function Po(t) {
         if (t != null) {
             try {
                 return br.call(t)
             } catch {}
             try {
                 return t + ""
             } catch {}
         }
         return ""
     }
 
-    function Et(t, e) {
+    function wt(t, e) {
         if (typeof t != "function" || e && typeof e != "function") throw new TypeError(qn);
         var r = function() {
             var n = arguments,
                 i = e ? e.apply(this, n) : n[0],
                 o = r.cache;
             if (o.has(i)) return o.get(i);
             var s = t.apply(this, n);
             return r.cache = o.set(i, s), s
         };
-        return r.cache = new(Et.Cache || oe), r
+        return r.cache = new(wt.Cache || oe), r
     }
-    Et.Cache = oe;
+    wt.Cache = oe;
 
     function Do(t, e) {
         return t === e || t !== t && e !== e
     }
-    var yr = Array.isArray;
+    var jr = Array.isArray;
 
     function Oo(t) {
-        var e = xr(t) ? jr.call(t) : "";
+        var e = xr(t) ? vr.call(t) : "";
         return e == zn || e == Un
     }
 
     function xr(t) {
         var e = typeof t;
         return !!t && (e == "object" || e == "function")
     }
 
     function Ho(t) {
         return !!t && typeof t == "object"
     }
 
     function kt(t) {
-        return typeof t == "symbol" || Ho(t) && jr.call(t) == Kn
+        return typeof t == "symbol" || Ho(t) && vr.call(t) == Kn
     }
 
     function Ro(t) {
         return t == null ? "" : Co(t)
     }
 
     function Bo(t, e, r) {
         var n = t == null ? void 0 : To(t, e);
         return n === void 0 ? r : n
     }
-    wr.exports = Bo
+    Er.exports = Bo
 });
-var Or = vt((As, Dr) => {
+var Or = yt((As, Dr) => {
     var No = "Expected a function",
         Cr = "__lodash_hash_undefined__",
         Fr = 1 / 0,
         Vo = 9007199254740991,
         Go = "[object Function]",
         qo = "[object GeneratorFunction]",
         zo = "[object Symbol]",
@@ -393,28 +393,28 @@
     }
     ie.prototype.clear = di;
     ie.prototype.delete = ci;
     ie.prototype.get = ui;
     ie.prototype.has = fi;
     ie.prototype.set = pi;
 
-    function me(t) {
+    function ge(t) {
         var e = -1,
             r = t ? t.length : 0;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function gi() {
+    function mi() {
         this.__data__ = []
     }
 
-    function mi(t) {
+    function gi(t) {
         var e = this.__data__,
             r = Xe(e, t);
         if (r < 0) return !1;
         var n = e.length - 1;
         return r == n ? e.pop() : si.call(e, r, 1), !0
     }
 
@@ -424,62 +424,62 @@
         return r < 0 ? void 0 : e[r][1]
     }
 
     function bi(t) {
         return Xe(this.__data__, t) > -1
     }
 
-    function ji(t, e) {
+    function vi(t, e) {
         var r = this.__data__,
             n = Xe(r, t);
         return n < 0 ? r.push([t, e]) : r[n][1] = e, this
     }
-    me.prototype.clear = gi;
-    me.prototype.delete = mi;
-    me.prototype.get = hi;
-    me.prototype.has = bi;
-    me.prototype.set = ji;
+    ge.prototype.clear = mi;
+    ge.prototype.delete = gi;
+    ge.prototype.get = hi;
+    ge.prototype.has = bi;
+    ge.prototype.set = vi;
 
     function ae(t) {
         var e = -1,
             r = t ? t.length : 0;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function vi() {
+    function yi() {
         this.__data__ = {
             hash: new ie,
-            map: new(li || me),
+            map: new(li || ge),
             string: new ie
         }
     }
 
-    function yi(t) {
+    function ji(t) {
         return Ze(this, t).delete(t)
     }
 
     function xi(t) {
         return Ze(this, t).get(t)
     }
 
-    function wi(t) {
+    function Ei(t) {
         return Ze(this, t).has(t)
     }
 
-    function Ei(t, e) {
+    function wi(t, e) {
         return Ze(this, t).set(t, e), this
     }
-    ae.prototype.clear = vi;
-    ae.prototype.delete = yi;
+    ae.prototype.clear = yi;
+    ae.prototype.delete = ji;
     ae.prototype.get = xi;
-    ae.prototype.has = wi;
-    ae.prototype.set = Ei;
+    ae.prototype.has = Ei;
+    ae.prototype.set = wi;
 
     function ki(t, e, r) {
         var n = t[e];
         (!(We.call(t, e) && Ir(n, r)) || r === void 0 && !(e in t)) && (t[e] = r)
     }
 
     function Xe(t, e) {
@@ -616,15 +616,15 @@
     }
 
     function Ri(t, e, r) {
         return t == null ? t : Ti(t, e, r)
     }
     Dr.exports = Ri
 });
-var vn = vt((Se, be) => {
+var yn = yt((Se, be) => {
     var Bi = 200,
         Rt = "__lodash_hash_undefined__",
         it = 1,
         Wr = 2,
         Xr = 9007199254740991,
         Ye = "[object Arguments]",
         $t = "[object Array]",
@@ -719,21 +719,21 @@
         var e = -1,
             r = Array(t.size);
         return t.forEach(function(n, i) {
             r[++e] = [i, n]
         }), r
     }
 
-    function ga(t, e) {
+    function ma(t, e) {
         return function(r) {
             return t(e(r))
         }
     }
 
-    function ma(t) {
+    function ga(t) {
         var e = -1,
             r = Array(t.size);
         return t.forEach(function(n) {
             r[++e] = n
         }), r
     }
     var ha = Array.prototype,
@@ -743,32 +743,32 @@
         dn = ba.toString,
         K = at.hasOwnProperty,
         Vr = function() {
             var t = /[^.]+$/.exec(St && St.keys && St.keys.IE_PROTO || "");
             return t ? "Symbol(src)_1." + t : ""
         }(),
         cn = at.toString,
-        ja = RegExp("^" + dn.call(K).replace(ra, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
+        va = RegExp("^" + dn.call(K).replace(ra, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
         Gr = ln ? W.Buffer : void 0,
         rt = W.Symbol,
         qr = W.Uint8Array,
         un = at.propertyIsEnumerable,
-        va = ha.splice,
+        ya = ha.splice,
         se = rt ? rt.toStringTag : void 0,
         zr = Object.getOwnPropertySymbols,
-        ya = Gr ? Gr.isBuffer : void 0,
-        xa = ga(Object.keys, Object),
-        It = je(W, "DataView"),
-        Le = je(W, "Map"),
-        Pt = je(W, "Promise"),
-        Dt = je(W, "Set"),
-        Ot = je(W, "WeakMap"),
-        $e = je(Object, "create"),
-        wa = ce(It),
-        Ea = ce(Le),
+        ja = Gr ? Gr.isBuffer : void 0,
+        xa = ma(Object.keys, Object),
+        It = ve(W, "DataView"),
+        Le = ve(W, "Map"),
+        Pt = ve(W, "Promise"),
+        Dt = ve(W, "Set"),
+        Ot = ve(W, "WeakMap"),
+        $e = ve(Object, "create"),
+        Ea = ce(It),
+        wa = ce(Le),
         ka = ce(Pt),
         Aa = ce(Dt),
         Ta = ce(Ot),
         Ur = rt ? rt.prototype : void 0,
         Lt = Ur ? Ur.valueOf : void 0;
 
     function le(t) {
@@ -827,15 +827,15 @@
     }
 
     function Ma(t) {
         var e = this.__data__,
             r = st(e, t);
         if (r < 0) return !1;
         var n = e.length - 1;
-        return r == n ? e.pop() : va.call(e, r, 1), --this.size, !0
+        return r == n ? e.pop() : ya.call(e, r, 1), --this.size, !0
     }
 
     function Ia(t) {
         var e = this.__data__,
             r = st(e, t);
         return r < 0 ? void 0 : e[r][1]
     }
@@ -950,25 +950,25 @@
     re.prototype.has = Ka;
     re.prototype.set = Ja;
 
     function Wa(t, e) {
         var r = ot(t),
             n = !r && cs(t),
             i = !r && !n && Ht(t),
-            o = !r && !n && !i && jn(t),
+            o = !r && !n && !i && vn(t),
             s = r || n || i || o,
             u = s ? da(t.length, String) : [],
             f = u.length;
         for (var d in t)(e || K.call(t, d)) && !(s && (d == "length" || i && (d == "offset" || d == "parent") || o && (d == "buffer" || d == "byteLength" || d == "byteOffset") || is(d, f))) && u.push(d);
         return u
     }
 
     function st(t, e) {
         for (var r = t.length; r--;)
-            if (gn(t[r][0], e)) return r;
+            if (mn(t[r][0], e)) return r;
         return -1
     }
 
     function Xa(t, e, r) {
         var n = e(t);
         return ot(t) ? n : sa(n, r(t))
     }
@@ -988,36 +988,36 @@
     function Za(t, e, r, n, i, o) {
         var s = ot(t),
             u = ot(e),
             f = s ? $t : te(t),
             d = u ? $t : te(e);
         f = f == Ye ? he : f, d = d == Ye ? he : d;
         var h = f == he,
-            j = d == he,
+            v = d == he,
             A = f == d;
         if (A && Ht(t)) {
             if (!Ht(e)) return !1;
             s = !0, h = !1
         }
-        if (A && !h) return o || (o = new re), s || jn(t) ? pn(t, e, r, n, i, o) : ts(t, e, f, r, n, i, o);
+        if (A && !h) return o || (o = new re), s || vn(t) ? pn(t, e, r, n, i, o) : ts(t, e, f, r, n, i, o);
         if (!(r & it)) {
             var L = h && K.call(t, "__wrapped__"),
-                I = j && K.call(e, "__wrapped__");
+                I = v && K.call(e, "__wrapped__");
             if (L || I) {
                 var B = L ? t.value() : t,
                     N = I ? e.value() : e;
                 return o || (o = new re), i(B, N, r, n, o)
             }
         }
         return A ? (o || (o = new re), rs(t, e, r, n, i, o)) : !1
     }
 
     function Ya(t) {
         if (!bn(t) || ss(t)) return !1;
-        var e = mn(t) ? ja : na;
+        var e = gn(t) ? va : na;
         return e.test(ce(t))
     }
 
     function Qa(t) {
         return Me(t) && hn(t.length) && !!S[Ie(t)]
     }
 
@@ -1032,61 +1032,61 @@
         var s = r & it,
             u = t.length,
             f = e.length;
         if (u != f && !(s && f > u)) return !1;
         var d = o.get(t);
         if (d && o.get(e)) return d == e;
         var h = -1,
-            j = !0,
+            v = !0,
             A = r & Wr ? new nt : void 0;
         for (o.set(t, e), o.set(e, t); ++h < u;) {
             var L = t[h],
                 I = e[h];
             if (n) var B = s ? n(I, L, h, e, t, o) : n(L, I, h, t, e, o);
             if (B !== void 0) {
                 if (B) continue;
-                j = !1;
+                v = !1;
                 break
             }
             if (A) {
                 if (!la(e, function(N, q) {
                         if (!ua(A, q) && (L === N || i(L, N, r, n, o))) return A.push(q)
                     })) {
-                    j = !1;
+                    v = !1;
                     break
                 }
             } else if (!(L === I || i(L, I, r, n, o))) {
-                j = !1;
+                v = !1;
                 break
             }
         }
-        return o.delete(t), o.delete(e), j
+        return o.delete(t), o.delete(e), v
     }
 
     function ts(t, e, r, n, i, o, s) {
         switch (r) {
             case tt:
                 if (t.byteLength != e.byteLength || t.byteOffset != e.byteOffset) return !1;
                 t = t.buffer, e = e.buffer;
             case on:
                 return !(t.byteLength != e.byteLength || !o(new qr(t), new qr(e)));
             case Zr:
             case Yr:
             case tn:
-                return gn(+t, +e);
+                return mn(+t, +e);
             case Qr:
                 return t.name == e.name && t.message == e.message;
             case rn:
             case nn:
                 return t == e + "";
             case Qe:
                 var u = pa;
             case et:
                 var f = n & it;
-                if (u || (u = ma), t.size != e.size && !f) return !1;
+                if (u || (u = ga), t.size != e.size && !f) return !1;
                 var d = s.get(t);
                 if (d) return d == e;
                 n |= Wr, s.set(t, e);
                 var h = pn(u(t), u(e), n, i, o, s);
                 return s.delete(t), h;
             case zi:
                 if (Lt) return Lt.call(t) == Lt.call(e)
@@ -1097,24 +1097,24 @@
     function rs(t, e, r, n, i, o) {
         var s = r & it,
             u = Jr(t),
             f = u.length,
             d = Jr(e),
             h = d.length;
         if (f != h && !s) return !1;
-        for (var j = f; j--;) {
-            var A = u[j];
+        for (var v = f; v--;) {
+            var A = u[v];
             if (!(s ? A in e : K.call(e, A))) return !1
         }
         var L = o.get(t);
         if (L && o.get(e)) return L == e;
         var I = !0;
         o.set(t, e), o.set(e, t);
-        for (var B = s; ++j < f;) {
-            A = u[j];
+        for (var B = s; ++v < f;) {
+            A = u[v];
             var N = t[A],
                 q = e[A];
             if (n) var O = s ? n(q, N, A, e, t, o) : n(N, q, A, t, e, o);
             if (!(O === void 0 ? N === q || i(N, q, r, n, o) : O)) {
                 I = !1;
                 break
             }
@@ -1133,15 +1133,15 @@
     }
 
     function lt(t, e) {
         var r = t.__data__;
         return as(e) ? r[typeof e == "string" ? "string" : "hash"] : r.map
     }
 
-    function je(t, e) {
+    function ve(t, e) {
         var r = fa(t, e);
         return Ya(r) ? r : void 0
     }
 
     function ns(t) {
         var e = K.call(t, se),
             r = t[se];
@@ -1152,24 +1152,24 @@
         var i = cn.call(t);
         return n && (e ? t[se] = r : delete t[se]), i
     }
     var os = zr ? function(t) {
             return t == null ? [] : (t = Object(t), aa(zr(t), function(e) {
                 return un.call(t, e)
             }))
-        } : gs,
+        } : ms,
         te = Ie;
     (It && te(new It(new ArrayBuffer(1))) != tt || Le && te(new Le) != Qe || Pt && te(Pt.resolve()) != Hr || Dt && te(new Dt) != et || Ot && te(new Ot) != Mt) && (te = function(t) {
         var e = Ie(t),
             r = e == he ? t.constructor : void 0,
             n = r ? ce(r) : "";
         if (n) switch (n) {
-            case wa:
-                return tt;
             case Ea:
+                return tt;
+            case wa:
                 return Qe;
             case ka:
                 return Hr;
             case Aa:
                 return et;
             case Ta:
                 return Mt
@@ -1208,34 +1208,34 @@
             try {
                 return t + ""
             } catch {}
         }
         return ""
     }
 
-    function gn(t, e) {
+    function mn(t, e) {
         return t === e || t !== t && e !== e
     }
     var cs = Kr(function() {
             return arguments
         }()) ? Kr : function(t) {
             return Me(t) && K.call(t, "callee") && !un.call(t, "callee")
         },
         ot = Array.isArray;
 
     function us(t) {
-        return t != null && hn(t.length) && !mn(t)
+        return t != null && hn(t.length) && !gn(t)
     }
-    var Ht = ya || ms;
+    var Ht = ja || gs;
 
     function fs(t, e) {
         return fn(t, e)
     }
 
-    function mn(t) {
+    function gn(t) {
         if (!bn(t)) return !1;
         var e = Ie(t);
         return e == en || e == Vi || e == Ni || e == qi
     }
 
     function hn(t) {
         return typeof t == "number" && t > -1 && t % 1 == 0 && t <= Xr
@@ -1245,144 +1245,144 @@
         var e = typeof t;
         return t != null && (e == "object" || e == "function")
     }
 
     function Me(t) {
         return t != null && typeof t == "object"
     }
-    var jn = Nr ? ca(Nr) : Qa;
+    var vn = Nr ? ca(Nr) : Qa;
 
     function ps(t) {
         return us(t) ? Wa(t) : es(t)
     }
 
-    function gs() {
+    function ms() {
         return []
     }
 
-    function ms() {
+    function gs() {
         return !1
     }
     be.exports = fs
 });
 (function() {
     "use strict";
-    var t = function(g, c) {
-        var m = function(T) {
-                for (var E = 0, $ = T.length; E < $; E++) y(T[E])
+    var t = function(m, c) {
+        var g = function(T) {
+                for (var w = 0, $ = T.length; w < $; w++) j(T[w])
             },
-            y = function(T) {
-                var E = T.target,
+            j = function(T) {
+                var w = T.target,
                     $ = T.attributeName,
                     P = T.oldValue;
-                E.attributeChangedCallback($, P, E.getAttribute($))
+                w.attributeChangedCallback($, P, w.getAttribute($))
             };
         return function(x, T) {
-            var E = x.constructor.observedAttributes;
-            return E && g(T).then(function() {
-                new c(m).observe(x, {
+            var w = x.constructor.observedAttributes;
+            return w && m(T).then(function() {
+                new c(g).observe(x, {
                     attributes: !0,
                     attributeOldValue: !0,
-                    attributeFilter: E
+                    attributeFilter: w
                 });
-                for (var $ = 0, P = E.length; $ < P; $++) x.hasAttribute(E[$]) && y({
+                for (var $ = 0, P = w.length; $ < P; $++) x.hasAttribute(w[$]) && j({
                     target: x,
-                    attributeName: E[$],
+                    attributeName: w[$],
                     oldValue: null
                 })
             }), x
         }
     };
 
-    function e(g, c) {
-        if (g) {
-            if (typeof g == "string") return r(g, c);
-            var m = Object.prototype.toString.call(g).slice(8, -1);
-            if (m === "Object" && g.constructor && (m = g.constructor.name), m === "Map" || m === "Set") return Array.from(g);
-            if (m === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(m)) return r(g, c)
+    function e(m, c) {
+        if (m) {
+            if (typeof m == "string") return r(m, c);
+            var g = Object.prototype.toString.call(m).slice(8, -1);
+            if (g === "Object" && m.constructor && (g = m.constructor.name), g === "Map" || g === "Set") return Array.from(m);
+            if (g === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(g)) return r(m, c)
         }
     }
 
-    function r(g, c) {
-        (c == null || c > g.length) && (c = g.length);
-        for (var m = 0, y = new Array(c); m < c; m++) y[m] = g[m];
-        return y
-    }
-
-    function n(g, c) {
-        var m = typeof Symbol < "u" && g[Symbol.iterator] || g["@@iterator"];
-        if (!m) {
-            if (Array.isArray(g) || (m = e(g)) || c && g && typeof g.length == "number") {
-                m && (g = m);
-                var y = 0,
+    function r(m, c) {
+        (c == null || c > m.length) && (c = m.length);
+        for (var g = 0, j = new Array(c); g < c; g++) j[g] = m[g];
+        return j
+    }
+
+    function n(m, c) {
+        var g = typeof Symbol < "u" && m[Symbol.iterator] || m["@@iterator"];
+        if (!g) {
+            if (Array.isArray(m) || (g = e(m)) || c && m && typeof m.length == "number") {
+                g && (m = g);
+                var j = 0,
                     x = function() {};
                 return {
                     s: x,
                     n: function() {
-                        return y >= g.length ? {
+                        return j >= m.length ? {
                             done: !0
                         } : {
                             done: !1,
-                            value: g[y++]
+                            value: m[j++]
                         }
                     },
                     e: function(P) {
                         throw P
                     },
                     f: x
                 }
             }
             throw new TypeError(`Invalid attempt to iterate non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
         }
         var T = !0,
-            E = !1,
+            w = !1,
             $;
         return {
             s: function() {
-                m = m.call(g)
+                g = g.call(m)
             },
             n: function() {
-                var P = m.next();
+                var P = g.next();
                 return T = P.done, P
             },
             e: function(P) {
-                E = !0, $ = P
+                w = !0, $ = P
             },
             f: function() {
                 try {
-                    !T && m.return != null && m.return()
+                    !T && g.return != null && g.return()
                 } finally {
-                    if (E) throw $
+                    if (w) throw $
                 }
             }
         }
     }
     var i = !0,
         o = !1,
         s = "querySelectorAll",
         u = function(c) {
-            var m = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : document,
-                y = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : MutationObserver,
+            var g = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : document,
+                j = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : MutationObserver,
                 x = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : ["*"],
                 T = function P(Q, ee, R, k, M, D) {
                     var G = n(Q),
                         pe;
                     try {
                         for (G.s(); !(pe = G.n()).done;) {
                             var H = pe.value;
                             (D || s in H) && (M ? R.has(H) || (R.add(H), k.delete(H), c(H, M)) : k.has(H) || (k.add(H), R.delete(H), c(H, M)), D || P(H[s](ee), ee, R, k, M, i))
                         }
-                    } catch (jt) {
-                        G.e(jt)
+                    } catch (vt) {
+                        G.e(vt)
                     } finally {
                         G.f()
                     }
                 },
-                E = new y(function(P) {
+                w = new j(function(P) {
                     if (x.length) {
                         var Q = x.join(","),
                             ee = new Set,
                             R = new Set,
                             k = n(P),
                             M;
                         try {
@@ -1395,317 +1395,317 @@
                         } catch (H) {
                             k.e(H)
                         } finally {
                             k.f()
                         }
                     }
                 }),
-                $ = E.observe;
-            return (E.observe = function(P) {
-                return $.call(E, P, {
+                $ = w.observe;
+            return (w.observe = function(P) {
+                return $.call(w, P, {
                     subtree: i,
                     childList: i
                 })
-            })(m), E
+            })(g), w
         },
         f = "querySelectorAll",
         d = self,
         h = d.document,
-        j = d.Element,
+        v = d.Element,
         A = d.MutationObserver,
         L = d.Set,
         I = d.WeakMap,
         B = function(c) {
             return f in c
         },
         N = [].filter,
-        q = function(g) {
+        q = function(m) {
             var c = new I,
-                m = function(k) {
+                g = function(k) {
                     for (var M = 0, D = k.length; M < D; M++) c.delete(k[M])
                 },
-                y = function() {
-                    for (var k = Q.takeRecords(), M = 0, D = k.length; M < D; M++) E(N.call(k[M].removedNodes, B), !1), E(N.call(k[M].addedNodes, B), !0)
+                j = function() {
+                    for (var k = Q.takeRecords(), M = 0, D = k.length; M < D; M++) w(N.call(k[M].removedNodes, B), !1), w(N.call(k[M].addedNodes, B), !0)
                 },
                 x = function(k) {
                     return k.matches || k.webkitMatchesSelector || k.msMatchesSelector
                 },
                 T = function(k, M) {
                     var D;
                     if (M)
-                        for (var G, pe = x(k), H = 0, jt = $.length; H < jt; H++) pe.call(k, G = $[H]) && (c.has(k) || c.set(k, new L), D = c.get(k), D.has(G) || (D.add(G), g.handle(k, M, G)));
+                        for (var G, pe = x(k), H = 0, vt = $.length; H < vt; H++) pe.call(k, G = $[H]) && (c.has(k) || c.set(k, new L), D = c.get(k), D.has(G) || (D.add(G), m.handle(k, M, G)));
                     else c.has(k) && (D = c.get(k), c.delete(k), D.forEach(function(Gn) {
-                        g.handle(k, M, Gn)
+                        m.handle(k, M, Gn)
                     }))
                 },
-                E = function(k) {
+                w = function(k) {
                     for (var M = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !0, D = 0, G = k.length; D < G; D++) T(k[D], M)
                 },
-                $ = g.query,
-                P = g.root || h,
+                $ = m.query,
+                P = m.root || h,
                 Q = u(T, P, A, $),
-                ee = j.prototype.attachShadow;
-            return ee && (j.prototype.attachShadow = function(R) {
+                ee = v.prototype.attachShadow;
+            return ee && (v.prototype.attachShadow = function(R) {
                 var k = ee.call(this, R);
                 return Q.observe(k), k
-            }), $.length && E(P[f]($)), {
-                drop: m,
-                flush: y,
+            }), $.length && w(P[f]($)), {
+                drop: g,
+                flush: j,
                 observer: Q,
-                parse: E
+                parse: w
             }
         },
         O = self,
         b = O.document,
         F = O.Map,
         ft = O.MutationObserver,
         ue = O.Object,
         fe = O.Set,
         Pe = O.WeakMap,
         Y = O.Element,
         De = O.HTMLElement,
         Oe = O.Node,
-        Ee = O.Error,
-        v = O.TypeError,
+        we = O.Error,
+        y = O.TypeError,
         He = O.Reflect,
         p = ue.defineProperty,
         l = ue.keys,
         a = ue.getOwnPropertyNames,
         C = ue.setPrototypeOf,
         _ = !self.customElements,
         V = function(c) {
-            for (var m = l(c), y = [], x = m.length, T = 0; T < x; T++) y[T] = c[m[T]], delete c[m[T]];
+            for (var g = l(c), j = [], x = g.length, T = 0; T < x; T++) j[T] = c[g[T]], delete c[g[T]];
             return function() {
-                for (var E = 0; E < x; E++) c[m[E]] = y[E]
+                for (var w = 0; w < x; w++) c[g[w]] = j[w]
             }
         };
     if (_) {
-        var w = function() {
+        var E = function() {
                 var c = this.constructor;
-                if (!Ae.has(c)) throw new v("Illegal constructor");
-                var m = Ae.get(c);
-                if (Be) return Xt(Be, m);
-                var y = ke.call(b, m);
-                return Xt(C(y, c.prototype), m)
+                if (!Ae.has(c)) throw new y("Illegal constructor");
+                var g = Ae.get(c);
+                if (Be) return Xt(Be, g);
+                var j = ke.call(b, g);
+                return Xt(C(j, c.prototype), g)
             },
             ke = b.createElement,
             Ae = new F,
             Re = new F,
             Jt = new F,
             Te = new F,
             Wt = [],
-            Fn = function(c, m, y) {
-                var x = Jt.get(y);
-                if (m && !x.isPrototypeOf(c)) {
+            Fn = function(c, g, j) {
+                var x = Jt.get(j);
+                if (g && !x.isPrototypeOf(c)) {
                     var T = V(c);
                     Be = C(c, x);
                     try {
                         new x.constructor
                     } finally {
                         Be = null, T()
                     }
                 }
-                var E = "".concat(m ? "" : "dis", "connectedCallback");
-                E in x && c[E]()
+                var w = "".concat(g ? "" : "dis", "connectedCallback");
+                w in x && c[w]()
             },
             Sn = q({
                 query: Wt,
                 handle: Fn
             }),
             Ln = Sn.parse,
             Be = null,
             pt = function(c) {
                 if (!Re.has(c)) {
-                    var m, y = new Promise(function(x) {
-                        m = x
+                    var g, j = new Promise(function(x) {
+                        g = x
                     });
                     Re.set(c, {
-                        $: y,
-                        _: m
+                        $: j,
+                        _: g
                     })
                 }
                 return Re.get(c).$
             },
             Xt = t(pt, ft);
         self.customElements = {
-            define: function(c, m) {
-                if (Te.has(c)) throw new Ee('the name "'.concat(c, '" has already been used with this registry'));
-                Ae.set(m, c), Jt.set(c, m.prototype), Te.set(c, m), Wt.push(c), pt(c).then(function() {
+            define: function(c, g) {
+                if (Te.has(c)) throw new we('the name "'.concat(c, '" has already been used with this registry'));
+                Ae.set(g, c), Jt.set(c, g.prototype), Te.set(c, g), Wt.push(c), pt(c).then(function() {
                     Ln(b.querySelectorAll(c))
-                }), Re.get(c)._(m)
+                }), Re.get(c)._(g)
             },
             get: function(c) {
                 return Te.get(c)
             },
             whenDefined: pt
-        }, p(w.prototype = De.prototype, "constructor", {
-            value: w
-        }), self.HTMLElement = w, b.createElement = function(g, c) {
-            var m = c && c.is,
-                y = m ? Te.get(m) : Te.get(g);
-            return y ? new y : ke.call(b, g)
+        }, p(E.prototype = De.prototype, "constructor", {
+            value: E
+        }), self.HTMLElement = E, b.createElement = function(m, c) {
+            var g = c && c.is,
+                j = g ? Te.get(g) : Te.get(m);
+            return j ? new j : ke.call(b, m)
         }, "isConnected" in Oe.prototype || p(Oe.prototype, "isConnected", {
             configurable: !0,
             get: function() {
                 return !(this.ownerDocument.compareDocumentPosition(this) & this.DOCUMENT_POSITION_DISCONNECTED)
             }
         })
     } else if (_ = !self.customElements.get("extends-li"), _) try {
-        var Zt = function g() {
-            return self.Reflect.construct(HTMLLIElement, [], g)
+        var Zt = function m() {
+            return self.Reflect.construct(HTMLLIElement, [], m)
         };
         Zt.prototype = HTMLLIElement.prototype;
         var Yt = "extends-li";
         self.customElements.define("extends-li", Zt, {
             extends: "li"
         }), _ = b.createElement("li", {
             is: Yt
         }).outerHTML.indexOf(Yt) < 0;
         var Qt = self.customElements,
             $n = Qt.get,
             Mn = Qt.whenDefined;
-        self.customElements.whenDefined = function(g) {
+        self.customElements.whenDefined = function(m) {
             var c = this;
-            return Mn.call(this, g).then(function(m) {
-                return m || $n.call(c, g)
+            return Mn.call(this, m).then(function(g) {
+                return g || $n.call(c, m)
             })
         }
     } catch {}
     if (_) {
         var er = function(c) {
-                var m = gt.get(c);
-                ir(m.querySelectorAll(this), c.isConnected)
+                var g = mt.get(c);
+                ir(g.querySelectorAll(this), c.isConnected)
             },
             U = self.customElements,
             tr = b.createElement,
             In = U.define,
             Pn = U.get,
             Dn = U.upgrade,
             On = He || {
                 construct: function(c) {
                     return c.call(this)
                 }
             },
             Hn = On.construct,
-            gt = new Pe,
-            mt = new fe,
+            mt = new Pe,
+            gt = new fe,
             Ne = new F,
             Ve = new F,
             rr = new F,
             Ge = new F,
             nr = [],
             qe = [],
             or = function(c) {
                 return Ge.get(c) || Pn.call(U, c)
             },
-            Rn = function(c, m, y) {
-                var x = rr.get(y);
-                if (m && !x.isPrototypeOf(c)) {
+            Rn = function(c, g, j) {
+                var x = rr.get(j);
+                if (g && !x.isPrototypeOf(c)) {
                     var T = V(c);
                     ze = C(c, x);
                     try {
                         new x.constructor
                     } finally {
                         ze = null, T()
                     }
                 }
-                var E = "".concat(m ? "" : "dis", "connectedCallback");
-                E in x && c[E]()
+                var w = "".concat(g ? "" : "dis", "connectedCallback");
+                w in x && c[w]()
             },
             Bn = q({
                 query: qe,
                 handle: Rn
             }),
             ir = Bn.parse,
             Nn = q({
                 query: nr,
-                handle: function(c, m) {
-                    gt.has(c) && (m ? mt.add(c) : mt.delete(c), qe.length && er.call(qe, c))
+                handle: function(c, g) {
+                    mt.has(c) && (g ? gt.add(c) : gt.delete(c), qe.length && er.call(qe, c))
                 }
             }),
             Vn = Nn.parse,
             ar = Y.prototype.attachShadow;
-        ar && (Y.prototype.attachShadow = function(g) {
-            var c = ar.call(this, g);
-            return gt.set(this, c), c
+        ar && (Y.prototype.attachShadow = function(m) {
+            var c = ar.call(this, m);
+            return mt.set(this, c), c
         });
         var ht = function(c) {
                 if (!Ve.has(c)) {
-                    var m, y = new Promise(function(x) {
-                        m = x
+                    var g, j = new Promise(function(x) {
+                        g = x
                     });
                     Ve.set(c, {
-                        $: y,
-                        _: m
+                        $: j,
+                        _: g
                     })
                 }
                 return Ve.get(c).$
             },
             bt = t(ht, ft),
             ze = null;
-        a(self).filter(function(g) {
-            return /^HTML.*Element$/.test(g)
-        }).forEach(function(g) {
-            var c = self[g];
-
-            function m() {
-                var y = this.constructor;
-                if (!Ne.has(y)) throw new v("Illegal constructor");
-                var x = Ne.get(y),
+        a(self).filter(function(m) {
+            return /^HTML.*Element$/.test(m)
+        }).forEach(function(m) {
+            var c = self[m];
+
+            function g() {
+                var j = this.constructor;
+                if (!Ne.has(j)) throw new y("Illegal constructor");
+                var x = Ne.get(j),
                     T = x.is,
-                    E = x.tag;
+                    w = x.tag;
                 if (T) {
                     if (ze) return bt(ze, T);
-                    var $ = tr.call(b, E);
-                    return $.setAttribute("is", T), bt(C($, y.prototype), T)
-                } else return Hn.call(this, c, [], y)
-            }
-            p(m.prototype = c.prototype, "constructor", {
-                value: m
-            }), p(self, g, {
-                value: m
+                    var $ = tr.call(b, w);
+                    return $.setAttribute("is", T), bt(C($, j.prototype), T)
+                } else return Hn.call(this, c, [], j)
+            }
+            p(g.prototype = c.prototype, "constructor", {
+                value: g
+            }), p(self, m, {
+                value: g
             })
-        }), b.createElement = function(g, c) {
-            var m = c && c.is;
-            if (m) {
-                var y = Ge.get(m);
-                if (y && Ne.get(y).tag === g) return new y
-            }
-            var x = tr.call(b, g);
-            return m && x.setAttribute("is", m), x
-        }, U.get = or, U.whenDefined = ht, U.upgrade = function(g) {
-            var c = g.getAttribute("is");
+        }), b.createElement = function(m, c) {
+            var g = c && c.is;
+            if (g) {
+                var j = Ge.get(g);
+                if (j && Ne.get(j).tag === m) return new j
+            }
+            var x = tr.call(b, m);
+            return g && x.setAttribute("is", g), x
+        }, U.get = or, U.whenDefined = ht, U.upgrade = function(m) {
+            var c = m.getAttribute("is");
             if (c) {
-                var m = Ge.get(c);
-                if (m) {
-                    bt(C(g, m.prototype), c);
+                var g = Ge.get(c);
+                if (g) {
+                    bt(C(m, g.prototype), c);
                     return
                 }
             }
-            Dn.call(U, g)
-        }, U.define = function(g, c, m) {
-            if (or(g)) throw new Ee("'".concat(g, "' has already been defined as a custom element"));
-            var y, x = m && m.extends;
+            Dn.call(U, m)
+        }, U.define = function(m, c, g) {
+            if (or(m)) throw new we("'".concat(m, "' has already been defined as a custom element"));
+            var j, x = g && g.extends;
             Ne.set(c, x ? {
-                is: g,
+                is: m,
                 tag: x
             } : {
                 is: "",
-                tag: g
-            }), x ? (y = "".concat(x, '[is="').concat(g, '"]'), rr.set(y, c.prototype), Ge.set(g, c), qe.push(y)) : (In.apply(U, arguments), nr.push(y = g)), ht(g).then(function() {
-                x ? (ir(b.querySelectorAll(y)), mt.forEach(er, [y])) : Vn(b.querySelectorAll(y))
-            }), Ve.get(g)._(c)
+                tag: m
+            }), x ? (j = "".concat(x, '[is="').concat(m, '"]'), rr.set(j, c.prototype), Ge.set(m, c), qe.push(j)) : (In.apply(U, arguments), nr.push(j = m)), ht(m).then(function() {
+                x ? (ir(b.querySelectorAll(j)), gt.forEach(er, [j])) : Vn(b.querySelectorAll(j))
+            }), Ve.get(m)._(c)
         }
     }
 })();
-var xe = _e(Er()),
+var xe = _e(wr()),
     An = _e(Or()),
-    Tn = _e(vn()),
+    Tn = _e(yn()),
     _n = _e(sr());
-var yn = _e(sr()),
+var jn = _e(sr()),
     dt = class {
         constructor(e, r) {
             this.progressBar = null;
             this.fileDrop = e => {
                 this.swallowEvent(e), e.dataTransfer && (this.fieldGroup.touch(), this.inputElement.files = e.dataTransfer.files, this.uploadFiles(this.inputElement.files).then(() => {
                     this.fieldGroup.inputted(), this.fieldGroup.validate()
                 }))
@@ -1713,20 +1713,20 @@
             this.fileRemove = () => {
                 for (this.inputElement.value = "", this.uploadedFiles = this.initialData.length > 0 ? [{}] : []; this.dropbox.firstChild;) this.dropbox.removeChild(this.dropbox.firstChild);
                 this.dropbox.appendChild(this.emptyDropboxItem), this.fieldGroup.touch(), this.fieldGroup.inputted(), this.fieldGroup.validate()
             };
             this.swallowEvent = e => {
                 e.stopPropagation(), e.preventDefault()
             };
-            if (this.fieldGroup = e, this.inputElement = r, this.dropbox = this.fieldGroup.element.querySelector("figure.dj-dropbox"), !this.dropbox) throw new Error('Element <input type="file"> requires sibling element <figure class="dj-dropbox"></figure>');
+            if (this.fieldGroup = e, this.inputElement = r, this.maxUploadSize = parseInt(this.inputElement.getAttribute("max-size") ?? "0"), this.dropbox = this.fieldGroup.element.querySelector("figure.dj-dropbox"), !this.dropbox) throw new Error('Element <input type="file"> requires sibling element <figure class="dj-dropbox"></figure>');
             if (this.chooseFileButton = this.fieldGroup.element.querySelector("button.dj-choose-file"), !this.chooseFileButton) throw new Error('Element <input type="file"> requires sibling element <button class="dj-choose-file"></button>');
             if (this.progressBar = this.fieldGroup.element.querySelector("progress"), this.progressBar && (this.progressBar.style.visibility = "hidden"), this.emptyDropboxItem = this.dropbox.querySelector("div.dj-empty-item"), !this.emptyDropboxItem) throw new Error('Element <input type="file"> requires sibling element <figure><div class="dj-empty-item"></div></figure>');
             let n = this.fieldGroup.element.querySelector(".dj-dropbox-items");
             if (!n) throw new Error('Element <input type="file"> requires sibling element <template class="dj-dropbox-items"></template>');
-            this.dropboxItemTemplate = (0, yn.default)(n.innerHTML), this.observer = new MutationObserver(o => this.attributesChanged(o)), this.observer.observe(this.inputElement, {
+            this.dropboxItemTemplate = (0, jn.default)(n.innerHTML), this.observer = new MutationObserver(o => this.attributesChanged(o)), this.observer.observe(this.inputElement, {
                 attributes: !0
             }), this.chooseFileButton.disabled = r.disabled;
             let i = document.getElementById(`initial_${r.id}`);
             i != null && i.textContent ? (this.uploadedFiles = this.initialData = [JSON.parse(i.textContent)], this.renderDropbox()) : this.uploadedFiles = this.initialData = [], this.dropbox.addEventListener("dragenter", this.swallowEvent), this.dropbox.addEventListener("dragover", this.swallowEvent), this.dropbox.addEventListener("drop", this.fileDrop), this.chooseFileButton.addEventListener("click", () => {
                 r.click()
             }), r.addEventListener("change", () => this.uploadFiles(this.inputElement.files).then(() => {
                 this.fieldGroup.inputted(), this.fieldGroup.validate()
@@ -1735,15 +1735,15 @@
             }).finally(() => {
                 this.chooseFileButton.blur(), this.fieldGroup.touch()
             }))
         }
         async uploadFiles(e) {
             return !e || e.length === 0 ? Promise.reject() : new Promise((r, n) => {
                 let i = e.item(0);
-                i ? this.uploadFile(i, this.dropbox.clientHeight).then(o => {
+                i && (!this.maxUploadSize || i.size <= this.maxUploadSize) ? this.uploadFile(i, this.dropbox.clientHeight).then(o => {
                     this.uploadedFiles = [o], this.renderDropbox(), this.fieldGroup.inputted(), r()
                 }).catch(() => {
                     n()
                 }) : n()
             })
         }
         async uploadFile(e, r) {
@@ -1794,51 +1794,51 @@
     }
     static buildMessage(r, n) {
         function i(h) {
             return h.charCodeAt(0).toString(16).toUpperCase()
         }
 
         function o(h) {
-            return h.replace(/\\/g, "\\\\").replace(/"/g, '\\"').replace(/\0/g, "\\0").replace(/\t/g, "\\t").replace(/\n/g, "\\n").replace(/\r/g, "\\r").replace(/[\x00-\x0F]/g, j => "\\x0" + i(j)).replace(/[\x10-\x1F\x7F-\x9F]/g, j => "\\x" + i(j))
+            return h.replace(/\\/g, "\\\\").replace(/"/g, '\\"').replace(/\0/g, "\\0").replace(/\t/g, "\\t").replace(/\n/g, "\\n").replace(/\r/g, "\\r").replace(/[\x00-\x0F]/g, v => "\\x0" + i(v)).replace(/[\x10-\x1F\x7F-\x9F]/g, v => "\\x" + i(v))
         }
 
         function s(h) {
-            return h.replace(/\\/g, "\\\\").replace(/\]/g, "\\]").replace(/\^/g, "\\^").replace(/-/g, "\\-").replace(/\0/g, "\\0").replace(/\t/g, "\\t").replace(/\n/g, "\\n").replace(/\r/g, "\\r").replace(/[\x00-\x0F]/g, j => "\\x0" + i(j)).replace(/[\x10-\x1F\x7F-\x9F]/g, j => "\\x" + i(j))
+            return h.replace(/\\/g, "\\\\").replace(/\]/g, "\\]").replace(/\^/g, "\\^").replace(/-/g, "\\-").replace(/\0/g, "\\0").replace(/\t/g, "\\t").replace(/\n/g, "\\n").replace(/\r/g, "\\r").replace(/[\x00-\x0F]/g, v => "\\x0" + i(v)).replace(/[\x10-\x1F\x7F-\x9F]/g, v => "\\x" + i(v))
         }
 
         function u(h) {
             switch (h.type) {
                 case "literal":
                     return '"' + o(h.text) + '"';
                 case "class":
-                    let j = h.parts.map(A => Array.isArray(A) ? s(A[0]) + "-" + s(A[1]) : s(A));
-                    return "[" + (h.inverted ? "^" : "") + j + "]";
+                    let v = h.parts.map(A => Array.isArray(A) ? s(A[0]) + "-" + s(A[1]) : s(A));
+                    return "[" + (h.inverted ? "^" : "") + v + "]";
                 case "any":
                     return "any character";
                 case "end":
                     return "end of input";
                 case "other":
                     return h.description
             }
         }
 
         function f(h) {
-            let j = h.map(u),
+            let v = h.map(u),
                 A, L;
-            if (j.sort(), j.length > 0) {
-                for (A = 1, L = 1; A < j.length; A++) j[A - 1] !== j[A] && (j[L] = j[A], L++);
-                j.length = L
+            if (v.sort(), v.length > 0) {
+                for (A = 1, L = 1; A < v.length; A++) v[A - 1] !== v[A] && (v[L] = v[A], L++);
+                v.length = L
             }
-            switch (j.length) {
+            switch (v.length) {
                 case 1:
-                    return j[0];
+                    return v[0];
                 case 2:
-                    return j[0] + " or " + j[1];
+                    return v[0] + " or " + v[1];
                 default:
-                    return j.slice(0, -1).join(", ") + ", or " + j[j.length - 1]
+                    return v.slice(0, -1).join(", ") + ", or " + v[v.length - 1]
             }
         }
 
         function d(h) {
             return h ? '"' + o(h) + '"' : "end of input"
         }
         return "Expected " + f(r) + " but " + d(n) + " found."
@@ -1854,20 +1854,20 @@
                     break
                 } let s = this.location.start,
                 u = this.location.source + ":" + s.line + ":" + s.column;
             if (i) {
                 let f = this.location.end,
                     d = Bt("", s.line.toString().length, " "),
                     h = i[s.line - 1],
-                    j = s.line === f.line ? f.column : h.length + 1;
+                    v = s.line === f.line ? f.column : h.length + 1;
                 n += `
  --> ` + u + `
 ` + d + ` |
 ` + s.line + " | " + h + `
-` + d + " | " + Bt("", s.column - 1, " ") + Bt("", j - s.column, "^")
+` + d + " | " + Bt("", s.column - 1, " ") + Bt("", v - s.column, "^")
             } else n += `
  at ` + u
         }
         return n
     }
 };
 
@@ -1983,22 +1983,22 @@
             return p instanceof Array ? p.join("") : p
         }, /^[0-9]/, F([
             ["0", "9"]
         ], !1, !1), /^[0-9a-f]/i, F([
             ["0", "9"],
             ["a", "f"]
         ], !1, !0)],
-        u = [v(`%;*/\x9E#;#/\x95$;*/\x8C$$%;*/>#;!/5$;*/,$; /#$+$)($'#(#'#("'#&'#0H*%;*/>#;!/5$;*/,$; /#$+$)($'#(#'#("'#&'#&/2$;*/)$8%: %"#!)(%'#($'#(#'#("'#&'#.. &%;*/& 8!:!! )`), v(`2"""6"7#.\xD1 &2$""6$7%.\xC5 &2&""6&7'.\xB9 &2(""6(7).\xAD &2*""6*7+.\xA1 &2,""6,7-.\x95 &2.""6.7/.\x89 &20""6071.} &22""6273.q &24""6475.e &26""6677.Y &28""6879.M &2:""6:7;.A &2<""6<7=.5 &2>""6>7?.) &2@""6@7A`), v('2B""6B7C'), v(`%2D""6D7E/R#;*/I$; /@$;*/7$2F""6F7G/($8%:H%!")(%'#($'#(#'#("'#&'#.A &;6.; &;D.5 &;$./ &%;@/' 8!:I!! )`), v("%;H/' 8!:J!! )"), v(`%;&/\\#;*/S$2K""6K7L/D$;*/;$;&/2$;*/)$8&:M&"%!)(&'#(%'#($'#(#'#("'#&'#./ &%;&/' 8!:N!! )`), v(`%;'/\\#;*/S$2O""6O7P/D$;*/;$;&/2$;*/)$8&:Q&"%!)(&'#(%'#($'#(#'#("'#&'#./ &%;'/' 8!:R!! )`), v(`%;*/i#%;4/"!&,)/Y$2D""6D7E/J$;(/A$2F""6F7G/2$;*/)$8&:S&"$")(&'#(%'#($'#(#'#("'#&'#.a &%%;4/"!&,)/7#2T""6T7U/($8":V"!!)("'#&'#.6 &%%;4/"!&,)/' 8!:V!! )`), v(`%;)/S#;*/J$2W""6W7X/;$;*/2$;(/)$8%:Q%"$ )(%'#($'#(#'#("'#&'#./ &%;)/' 8!:Y!! )`), v(";6./ &;@.) &;2.# &;5"), v('$4Z""5!7[0)*4Z""5!7[&'), v(`%;*/;#2\\""6\\7]/,$;*/#$+#)(#'#("'#&'#`), v(`%;*/;#2^""6^7_/,$;*/#$+#)(#'#("'#&'#`), v(`%;*/;#2\`""6\`7a/,$;*/#$+#)(#'#("'#&'#`), v(`%;*/;#2b""6b7c/,$;*/#$+#)(#'#("'#&'#`), v(`%;*/;#2d""6d7e/,$;*/#$+#)(#'#("'#&'#`), v(`%;*/;#2W""6W7X/,$;*/#$+#)(#'#("'#&'#`), v(";D.5 &;2./ &;5.) &;6.# &;@"), v(`%;,/\x91#%;3/k#$%;0/2#;3/)$8":f""$ )("'#&'#0<*%;0/2#;3/)$8":f""$ )("'#&'#&/)$8":g""! )("'#&'#." &"/1$;./($8#:h#!!)(#'#("'#&'#`), v(`%;@/;#;//2$;1/)$8#:i#"" )(#'#("'#&'#.L &%%;4/"!&,)/;#;//2$;1/)$8#:i#"" )(#'#("'#&'#`), v(`%4j""5!7k/?#$4l""5!7m0)*4l""5!7m&/#$+")("'#&'#`), v(`%;+/\x91#%;1/k#$%;0/2#;1/)$8":n""$ )("'#&'#0<*%;0/2#;1/)$8":n""$ )("'#&'#&/)$8":o""! )("'#&'#." &"/1$;-/($8#:p#!!)(#'#("'#&'#`), v(`<%;=." &"/L#;</C$;;." &"/5$;:." &"/'$8$:r$ )($'#(#'#("'#&'#=." 7q`), v('2s""6s7t'), v('4u""5!7v'), v('4w""5!7x'), v(`%;9/M#;=.# &;>." &"/9$$;M/&#0#*;M&&&#/#$+#)(#'#("'#&'#`), v(`%;7/9#$;M/&#0#*;M&&&#/#$+")("'#&'#`), v(`;?.= &%;8/3#$;M0#*;M&/#$+")("'#&'#`), v('24""6475'), v('22""6273'), v('2y""6y7z'), v(`<%2|""6|7}/N#%$;A0#*;A&/"!&,)/7$2|""6|7}/($8#:~#!!)(#'#("'#&'#.^ &%2\x7F""6\x7F7\x80/N#%$;B0#*;B&/"!&,)/7$2\x7F""6\x7F7\x80/($8#:~#!!)(#'#("'#&'#=." 7{`), v('4\x81""5!7\x82.: &%2\x83""6\x837\x84/& 8!:\x85! ).# &;C'), v('4\x86""5!7\x87.: &%2\x88""6\x887\x89/& 8!:\x8A! ).# &;C'), v(`2\x8B""6\x8B7\x8C.\xA9 &2\x8D""6\x8D7\x8E.\x9D &2\x8F""6\x8F7\x90.\x91 &2\x91""6\x917\x92.\x85 &2\x93""6\x937\x94.y &2\x95""6\x957\x96.m &%2\x97""6\x977\x98/]#%%;N/>#;N/5$;N/,$;N/#$+$)($'#(#'#("'#&'#/"!&,)/($8":\x99"! )("'#&'#`), v('<%;F/& 8!:\x9B! ).? &%;E/& 8!:\x9C! ).. &%;G/& 8!:\x9D! )=." 7\x9A'), v('2\x9E""6\x9E7\x9F'), v('2\xA0""6\xA07\xA1'), v('2\xA2""6\xA27\xA3'), v(`%;I/\x91#$%2s""6s7t/?#;J.0 &$;M/&#0#*;M&&&#/#$+")("'#&'#0O*%2s""6s7t/?#;J.0 &$;M/&#0#*;M&&&#/#$+")("'#&'#&/)$8":\xA4""! )("'#&'#`), v(`%2\xA5""6\xA57\xA6.5 &2\xA7""6\xA77\xA8.) &2s""6s7t/2#;J/)$8":\xA9""! )("'#&'#.# &;J`), v(`%;K/2#;L/)$8":\xAA""! )("'#&'#`), v('4\xAB""5!7\xAC'), v(`%$4\xAD""5!7\xAE0)*4\xAD""5!7\xAE&/' 8!:\xAF!! )`), v('4\xB0""5!7\xB1'), v('4\xB2""5!7\xB3')],
+        u = [y(`%;*/\x9E#;#/\x95$;*/\x8C$$%;*/>#;!/5$;*/,$; /#$+$)($'#(#'#("'#&'#0H*%;*/>#;!/5$;*/,$; /#$+$)($'#(#'#("'#&'#&/2$;*/)$8%: %"#!)(%'#($'#(#'#("'#&'#.. &%;*/& 8!:!! )`), y(`2"""6"7#.\xD1 &2$""6$7%.\xC5 &2&""6&7'.\xB9 &2(""6(7).\xAD &2*""6*7+.\xA1 &2,""6,7-.\x95 &2.""6.7/.\x89 &20""6071.} &22""6273.q &24""6475.e &26""6677.Y &28""6879.M &2:""6:7;.A &2<""6<7=.5 &2>""6>7?.) &2@""6@7A`), y('2B""6B7C'), y(`%2D""6D7E/R#;*/I$; /@$;*/7$2F""6F7G/($8%:H%!")(%'#($'#(#'#("'#&'#.A &;6.; &;D.5 &;$./ &%;@/' 8!:I!! )`), y("%;H/' 8!:J!! )"), y(`%;&/\\#;*/S$2K""6K7L/D$;*/;$;&/2$;*/)$8&:M&"%!)(&'#(%'#($'#(#'#("'#&'#./ &%;&/' 8!:N!! )`), y(`%;'/\\#;*/S$2O""6O7P/D$;*/;$;&/2$;*/)$8&:Q&"%!)(&'#(%'#($'#(#'#("'#&'#./ &%;'/' 8!:R!! )`), y(`%;*/i#%;4/"!&,)/Y$2D""6D7E/J$;(/A$2F""6F7G/2$;*/)$8&:S&"$")(&'#(%'#($'#(#'#("'#&'#.a &%%;4/"!&,)/7#2T""6T7U/($8":V"!!)("'#&'#.6 &%%;4/"!&,)/' 8!:V!! )`), y(`%;)/S#;*/J$2W""6W7X/;$;*/2$;(/)$8%:Q%"$ )(%'#($'#(#'#("'#&'#./ &%;)/' 8!:Y!! )`), y(";6./ &;@.) &;2.# &;5"), y('$4Z""5!7[0)*4Z""5!7[&'), y(`%;*/;#2\\""6\\7]/,$;*/#$+#)(#'#("'#&'#`), y(`%;*/;#2^""6^7_/,$;*/#$+#)(#'#("'#&'#`), y(`%;*/;#2\`""6\`7a/,$;*/#$+#)(#'#("'#&'#`), y(`%;*/;#2b""6b7c/,$;*/#$+#)(#'#("'#&'#`), y(`%;*/;#2d""6d7e/,$;*/#$+#)(#'#("'#&'#`), y(`%;*/;#2W""6W7X/,$;*/#$+#)(#'#("'#&'#`), y(";D.5 &;2./ &;5.) &;6.# &;@"), y(`%;,/\x91#%;3/k#$%;0/2#;3/)$8":f""$ )("'#&'#0<*%;0/2#;3/)$8":f""$ )("'#&'#&/)$8":g""! )("'#&'#." &"/1$;./($8#:h#!!)(#'#("'#&'#`), y(`%;@/;#;//2$;1/)$8#:i#"" )(#'#("'#&'#.L &%%;4/"!&,)/;#;//2$;1/)$8#:i#"" )(#'#("'#&'#`), y(`%4j""5!7k/?#$4l""5!7m0)*4l""5!7m&/#$+")("'#&'#`), y(`%;+/\x91#%;1/k#$%;0/2#;1/)$8":n""$ )("'#&'#0<*%;0/2#;1/)$8":n""$ )("'#&'#&/)$8":o""! )("'#&'#." &"/1$;-/($8#:p#!!)(#'#("'#&'#`), y(`<%;=." &"/L#;</C$;;." &"/5$;:." &"/'$8$:r$ )($'#(#'#("'#&'#=." 7q`), y('2s""6s7t'), y('4u""5!7v'), y('4w""5!7x'), y(`%;9/M#;=.# &;>." &"/9$$;M/&#0#*;M&&&#/#$+#)(#'#("'#&'#`), y(`%;7/9#$;M/&#0#*;M&&&#/#$+")("'#&'#`), y(`;?.= &%;8/3#$;M0#*;M&/#$+")("'#&'#`), y('24""6475'), y('22""6273'), y('2y""6y7z'), y(`<%2|""6|7}/N#%$;A0#*;A&/"!&,)/7$2|""6|7}/($8#:~#!!)(#'#("'#&'#.^ &%2\x7F""6\x7F7\x80/N#%$;B0#*;B&/"!&,)/7$2\x7F""6\x7F7\x80/($8#:~#!!)(#'#("'#&'#=." 7{`), y('4\x81""5!7\x82.: &%2\x83""6\x837\x84/& 8!:\x85! ).# &;C'), y('4\x86""5!7\x87.: &%2\x88""6\x887\x89/& 8!:\x8A! ).# &;C'), y(`2\x8B""6\x8B7\x8C.\xA9 &2\x8D""6\x8D7\x8E.\x9D &2\x8F""6\x8F7\x90.\x91 &2\x91""6\x917\x92.\x85 &2\x93""6\x937\x94.y &2\x95""6\x957\x96.m &%2\x97""6\x977\x98/]#%%;N/>#;N/5$;N/,$;N/#$+$)($'#(#'#("'#&'#/"!&,)/($8":\x99"! )("'#&'#`), y('<%;F/& 8!:\x9B! ).? &%;E/& 8!:\x9C! ).. &%;G/& 8!:\x9D! )=." 7\x9A'), y('2\x9E""6\x9E7\x9F'), y('2\xA0""6\xA07\xA1'), y('2\xA2""6\xA27\xA3'), y(`%;I/\x91#$%2s""6s7t/?#;J.0 &$;M/&#0#*;M&&&#/#$+")("'#&'#0O*%2s""6s7t/?#;J.0 &$;M/&#0#*;M&&&#/#$+")("'#&'#&/)$8":\xA4""! )("'#&'#`), y(`%2\xA5""6\xA57\xA6.5 &2\xA7""6\xA77\xA8.) &2s""6s7t/2#;J/)$8":\xA9""! )("'#&'#.# &;J`), y(`%;K/2#;L/)$8":\xAA""! )("'#&'#`), y('4\xAB""5!7\xAC'), y(`%$4\xAD""5!7\xAE0)*4\xAD""5!7\xAE&/' 8!:\xAF!! )`), y('4\xB0""5!7\xB1'), y('4\xB2""5!7\xB3')],
         f = 0,
         d = 0,
         h = [{
             line: 1,
             column: 1
         }],
-        j = 0,
+        v = 0,
         A = [],
         L = 0,
         I;
     if (e.startRule !== void 0) {
         if (!(e.startRule in i)) throw new Error(`Can't start parsing from rule "` + e.startRule + '".');
         o = i[e.startRule]
     }
@@ -2008,15 +2008,15 @@
     }
 
     function N() {
         return Y(d, f)
     }
 
     function q(p, l) {
-        throw l = l !== void 0 ? l : Y(d, f), Ee([fe(p)], t.substring(d, f), l)
+        throw l = l !== void 0 ? l : Y(d, f), we([fe(p)], t.substring(d, f), l)
     }
 
     function O(p, l) {
         throw l = l !== void 0 ? l : Y(d, f), Oe(p, l)
     }
 
     function b(p, l) {
@@ -2082,180 +2082,180 @@
                 line: C.line,
                 column: C.column
             }
         }
     }
 
     function De(p) {
-        f < j || (f > j && (j = f, A = []), A.push(p))
+        f < v || (f > v && (v = f, A = []), A.push(p))
     }
 
     function Oe(p, l) {
         return new Z(p, [], "", l)
     }
 
-    function Ee(p, l, a) {
+    function we(p, l, a) {
         return new Z(Z.buildMessage(p, l), p, l, a)
     }
 
-    function v(p) {
+    function y(p) {
         return p.split("").map(l => l.charCodeAt(0) - 32)
     }
 
     function He(p) {
         let l = u[p],
             a = 0,
             C = [],
             _ = l.length,
             V = [],
-            w = [],
+            E = [],
             ke;
         for (;;) {
             for (; a < _;) switch (l[a]) {
                 case 0:
-                    w.push(s[l[a + 1]]), a += 2;
+                    E.push(s[l[a + 1]]), a += 2;
                     break;
                 case 1:
-                    w.push(void 0), a++;
+                    E.push(void 0), a++;
                     break;
                 case 2:
-                    w.push(null), a++;
+                    E.push(null), a++;
                     break;
                 case 3:
-                    w.push(r), a++;
+                    E.push(r), a++;
                     break;
                 case 4:
-                    w.push([]), a++;
+                    E.push([]), a++;
                     break;
                 case 5:
-                    w.push(f), a++;
+                    E.push(f), a++;
                     break;
                 case 6:
-                    w.pop(), a++;
+                    E.pop(), a++;
                     break;
                 case 7:
-                    f = w.pop(), a++;
+                    f = E.pop(), a++;
                     break;
                 case 8:
-                    w.length -= l[a + 1], a += 2;
+                    E.length -= l[a + 1], a += 2;
                     break;
                 case 9:
-                    w.splice(-2, 1), a++;
+                    E.splice(-2, 1), a++;
                     break;
                 case 10:
-                    w[w.length - 2].push(w.pop()), a++;
+                    E[E.length - 2].push(E.pop()), a++;
                     break;
                 case 11:
-                    w.push(w.splice(w.length - l[a + 1], l[a + 1])), a += 2;
+                    E.push(E.splice(E.length - l[a + 1], l[a + 1])), a += 2;
                     break;
                 case 12:
-                    w.push(t.substring(w.pop(), f)), a++;
+                    E.push(t.substring(E.pop(), f)), a++;
                     break;
                 case 13:
-                    V.push(_), C.push(a + 3 + l[a + 1] + l[a + 2]), w[w.length - 1] ? (_ = a + 3 + l[a + 1], a += 3) : (_ = a + 3 + l[a + 1] + l[a + 2], a += 3 + l[a + 1]);
+                    V.push(_), C.push(a + 3 + l[a + 1] + l[a + 2]), E[E.length - 1] ? (_ = a + 3 + l[a + 1], a += 3) : (_ = a + 3 + l[a + 1] + l[a + 2], a += 3 + l[a + 1]);
                     break;
                 case 14:
-                    V.push(_), C.push(a + 3 + l[a + 1] + l[a + 2]), w[w.length - 1] === r ? (_ = a + 3 + l[a + 1], a += 3) : (_ = a + 3 + l[a + 1] + l[a + 2], a += 3 + l[a + 1]);
+                    V.push(_), C.push(a + 3 + l[a + 1] + l[a + 2]), E[E.length - 1] === r ? (_ = a + 3 + l[a + 1], a += 3) : (_ = a + 3 + l[a + 1] + l[a + 2], a += 3 + l[a + 1]);
                     break;
                 case 15:
-                    V.push(_), C.push(a + 3 + l[a + 1] + l[a + 2]), w[w.length - 1] !== r ? (_ = a + 3 + l[a + 1], a += 3) : (_ = a + 3 + l[a + 1] + l[a + 2], a += 3 + l[a + 1]);
+                    V.push(_), C.push(a + 3 + l[a + 1] + l[a + 2]), E[E.length - 1] !== r ? (_ = a + 3 + l[a + 1], a += 3) : (_ = a + 3 + l[a + 1] + l[a + 2], a += 3 + l[a + 1]);
                     break;
                 case 16:
-                    w[w.length - 1] !== r ? (V.push(_), C.push(a), _ = a + 2 + l[a + 1], a += 2) : a += 2 + l[a + 1];
+                    E[E.length - 1] !== r ? (V.push(_), C.push(a), _ = a + 2 + l[a + 1], a += 2) : a += 2 + l[a + 1];
                     break;
                 case 17:
                     V.push(_), C.push(a + 3 + l[a + 1] + l[a + 2]), t.length > f ? (_ = a + 3 + l[a + 1], a += 3) : (_ = a + 3 + l[a + 1] + l[a + 2], a += 3 + l[a + 1]);
                     break;
                 case 18:
                     V.push(_), C.push(a + 4 + l[a + 2] + l[a + 3]), t.substr(f, s[l[a + 1]].length) === s[l[a + 1]] ? (_ = a + 4 + l[a + 2], a += 4) : (_ = a + 4 + l[a + 2] + l[a + 3], a += 4 + l[a + 2]);
                     break;
                 case 19:
                     V.push(_), C.push(a + 4 + l[a + 2] + l[a + 3]), t.substr(f, s[l[a + 1]].length).toLowerCase() === s[l[a + 1]] ? (_ = a + 4 + l[a + 2], a += 4) : (_ = a + 4 + l[a + 2] + l[a + 3], a += 4 + l[a + 2]);
                     break;
                 case 20:
                     V.push(_), C.push(a + 4 + l[a + 2] + l[a + 3]), s[l[a + 1]].test(t.charAt(f)) ? (_ = a + 4 + l[a + 2], a += 4) : (_ = a + 4 + l[a + 2] + l[a + 3], a += 4 + l[a + 2]);
                     break;
                 case 21:
-                    w.push(t.substr(f, l[a + 1])), f += l[a + 1], a += 2;
+                    E.push(t.substr(f, l[a + 1])), f += l[a + 1], a += 2;
                     break;
                 case 22:
-                    w.push(s[l[a + 1]]), f += s[l[a + 1]].length, a += 2;
+                    E.push(s[l[a + 1]]), f += s[l[a + 1]].length, a += 2;
                     break;
                 case 23:
-                    w.push(r), L === 0 && De(s[l[a + 1]]), a += 2;
+                    E.push(r), L === 0 && De(s[l[a + 1]]), a += 2;
                     break;
                 case 24:
-                    d = w[w.length - 1 - l[a + 1]], a += 2;
+                    d = E[E.length - 1 - l[a + 1]], a += 2;
                     break;
                 case 25:
                     d = f, a++;
                     break;
                 case 26:
                     ke = l.slice(a + 4, a + 4 + l[a + 3]).map(function(Ae) {
-                        return w[w.length - 1 - Ae]
-                    }), w.splice(w.length - l[a + 2], l[a + 2], s[l[a + 1]].apply(null, ke)), a += 4 + l[a + 3];
+                        return E[E.length - 1 - Ae]
+                    }), E.splice(E.length - l[a + 2], l[a + 2], s[l[a + 1]].apply(null, ke)), a += 4 + l[a + 3];
                     break;
                 case 27:
-                    w.push(He(l[a + 1])), a += 2;
+                    E.push(He(l[a + 1])), a += 2;
                     break;
                 case 28:
                     L++, a++;
                     break;
                 case 29:
                     L--, a++;
                     break;
                 default:
                     throw new Error("Invalid opcode: " + l[a] + ".")
             }
             if (V.length > 0) _ = V.pop(), a = C.pop();
             else break
         }
-        return w[0]
+        return E[0]
     }
     if (I = He(o), I !== r && f === t.length) return I;
-    throw I !== r && f < t.length && De(ue()), Ee(A, j < t.length ? t.charAt(j) : null, j < t.length ? Y(j, j + 1) : Y(j, j))
+    throw I !== r && f < t.length && De(ue()), we(A, v < t.length ? t.charAt(v) : null, v < t.length ? Y(v, v + 1) : Y(v, v))
 }
-var ve = hs;
-var xn = `select::placeholder{color:gray}select.ts-hidden-accessible{display:none}django-formset{--django-formset-color-invalid: rgb(255, 3, 0);--django-formset-shadow-invalid: rgb(255, 3, 0, 0.25);--django-formset-color-valid: rgb(0, 122, 0);--django-formset-icon-invalid: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(255, 3, 0)"><path fill-rule="evenodd" d="M8 15A7 7 0 1 0 8 1a7 7 0 0 0 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"/><path d="M7.002 11a1 1 0 1 1 2 0 1 1 0 0 1-2 0zM7.1 4.995a.905.905 0 1 1 1.8 0l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 4.995z"/></svg>');--django-formset-icon-warning: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(255, 165, 0)"><path fill-rule="evenodd" d="M7.938 2.016a.146.146 0 0 0-.054.057L1.027 13.74a.176.176 0 0 0-.002.183c.016.03.037.05.054.06.015.01.034.017.066.017h13.713a.12.12 0 0 0 .066-.017.163.163 0 0 0 .055-.06.176.176 0 0 0-.003-.183L8.12 2.073a.146.146 0 0 0-.054-.057A.13.13 0 0 0 8.002 2a.13.13 0 0 0-.064.016zm1.044-.45a1.13 1.13 0 0 0-1.96 0L.165 13.233c-.457.778.091 1.767.98 1.767h13.713c.889 0 1.438-.99.98-1.767L8.982 1.566z"/><path d="M7.002 12a1 1 0 1 1 2 0 1 1 0 0 1-2 0zM7.1 5.995a.905.905 0 1 1 1.8 0l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 5.995z"/></svg>');--django-formset-icon-valid: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(0, 122, 0)"><path fill-rule="evenodd" d="M10.97 4.97a.75.75 0 0 1 1.071 1.05l-3.992 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.236.236 0 0 1 .02-.022z"/></svg>')}django-formset ul.dj-errorlist{list-style:none;margin-top:0;margin-bottom:0;margin-left:0;padding-left:0;color:var(--django-formset-color-invalid)}django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted) :not(django-field-group)>input[type=email]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted) :not(django-field-group)>input[type=text]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted) :not(django-field-group)>input[type=number]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted) :not(django-field-group)>input[type=date]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted) :not(django-field-group)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted) :not(django-field-group)>input[type=url]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted) :not(django-field-group)>input[type=password]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted) :not(django-field-group)>select:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors django-field-group.dj-touched:not(.dj-submitted) :not(django-field-group)>textarea:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>input[type=email]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>input[type=text]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>input[type=number]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>input[type=date]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>input[type=url]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>input[type=password]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>select:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>textarea:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>input[type=email]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>input[type=text]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>input[type=number]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>input[type=date]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>input[type=url]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>input[type=password]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>select:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) django-field-group.dj-dirty:not(.dj-submitted) :not(django-field-group)>textarea:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-success django-field-group.dj-dirty>input[type=email]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success django-field-group.dj-dirty :not(django-field-group)>input[type=email]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success django-field-group.dj-dirty>input[type=text]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success django-field-group.dj-dirty :not(django-field-group)>input[type=text]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success django-field-group.dj-dirty>input[type=number]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success django-field-group.dj-dirty :not(django-field-group)>input[type=number]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success django-field-group.dj-dirty>input[type=date]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success django-field-group.dj-dirty :not(django-field-group)>input[type=date]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success django-field-group.dj-dirty>input[type=datetime-local]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success django-field-group.dj-dirty :not(django-field-group)>input[type=datetime-local]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success django-field-group.dj-dirty>input[type=url]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success django-field-group.dj-dirty :not(django-field-group)>input[type=url]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success django-field-group.dj-dirty>input[type=password]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success django-field-group.dj-dirty :not(django-field-group)>input[type=password]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success django-field-group.dj-dirty>select:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success django-field-group.dj-dirty :not(django-field-group)>select:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success django-field-group.dj-dirty>textarea:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success django-field-group.dj-dirty :not(django-field-group)>textarea:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success django-field-group.dj-dirty>input[type=email]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success django-field-group.dj-dirty :not(django-field-group)>input[type=email]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success django-field-group.dj-dirty>input[type=text]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success django-field-group.dj-dirty :not(django-field-group)>input[type=text]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success django-field-group.dj-dirty>input[type=number]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success django-field-group.dj-dirty :not(django-field-group)>input[type=number]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success django-field-group.dj-dirty>input[type=date]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success django-field-group.dj-dirty :not(django-field-group)>input[type=date]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success django-field-group.dj-dirty>input[type=datetime-local]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success django-field-group.dj-dirty :not(django-field-group)>input[type=datetime-local]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success django-field-group.dj-dirty>input[type=url]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success django-field-group.dj-dirty :not(django-field-group)>input[type=url]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success django-field-group.dj-dirty>input[type=password]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success django-field-group.dj-dirty :not(django-field-group)>input[type=password]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset django-field-group{display:block}django-formset django-field-group[hidden]{display:none}django-formset django-field-group.dj-required>label,django-formset django-field-group.dj-required-any>label{font-weight:bolder}django-formset django-field-group.dj-submitted>input[type=email]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset django-field-group.dj-submitted>input[type=email]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset django-field-group.dj-submitted>input[type=text]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset django-field-group.dj-submitted>input[type=text]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset django-field-group.dj-submitted>input[type=number]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset django-field-group.dj-submitted>input[type=number]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset django-field-group.dj-submitted>input[type=date]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset django-field-group.dj-submitted>input[type=date]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset django-field-group.dj-submitted>input[type=datetime-local]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset django-field-group.dj-submitted>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset django-field-group.dj-submitted>input[type=url]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset django-field-group.dj-submitted>input[type=url]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset django-field-group.dj-submitted>input[type=password]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset django-field-group.dj-submitted>input[type=password]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset django-field-group.dj-submitted>select:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset django-field-group.dj-submitted>select:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset django-field-group.dj-submitted>textarea:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset django-field-group.dj-submitted>textarea:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset django-field-group input{background-repeat:no-repeat !important;background-position:center right !important;background-origin:content-box !important}django-formset django-field-group input[type=date],django-formset django-field-group input[type=datetime-local]{position:relative}django-formset django-field-group input[type=date]::-webkit-datetime-edit-fields-wrapper,django-formset django-field-group input[type=datetime-local]::-webkit-datetime-edit-fields-wrapper{margin-left:1.75em}django-formset django-field-group input[type=date]::-webkit-calendar-picker-indicator,django-formset django-field-group input[type=datetime-local]::-webkit-calendar-picker-indicator{cursor:pointer;position:absolute;left:.75em}django-formset django-field-group input[type=date]:hover::-webkit-calendar-picker-indicator,django-formset django-field-group input[type=datetime-local]:hover::-webkit-calendar-picker-indicator{cursor:pointer}django-formset django-field-group select,django-formset django-field-group textarea{background-image:none !important}django-formset django-field-group select.dj-concealed,django-formset django-field-group textarea.dj-concealed{display:block !important;height:1px !important;min-height:initial !important;max-height:initial !important;padding:0 !important;margin:-1px 0 0 0 !important;border:none !important;opacity:0 !important;resize:none}django-formset django-field-group .dj-help-text{font-style:oblique}django-formset django-field-group .dj-form-optgroup{margin-bottom:.5rem}django-formset django-field-group .dj-form-optgroup>em{margin-left:.75rem}django-formset django-field-group .dj-form-inlined{display:inline-block}django-formset django-field-group input[type=file]{width:0 !important;height:0 !important}django-formset django-field-group .dj-control-panel{display:flex}django-formset django-field-group .dj-control-panel>div{height:fit-content;margin-left:.5rem}django-formset django-field-group .dj-control-panel>div progress{width:100%;margin-top:.25rem}django-formset django-field-group figure.dj-dropbox{all:unset;display:inline-flex;align-items:center;justify-content:space-between;background-color:#f5f5f5;margin:0 0 .25rem .25rem;padding:0;list-style:none;height:8rem;min-width:8rem;outline:gray thin dotted}django-formset django-field-group figure.dj-dropbox>div.dj-empty-item{flex-grow:1;text-align:center;height:auto}django-formset django-field-group figure.dj-dropbox>div.dj-empty-item p{padding-left:.5rem;padding-right:.5rem}django-formset django-field-group figure.dj-dropbox>img{all:unset;flex-grow:1;display:block;height:inherit;max-width:calc(100% - 12rem)}django-formset django-field-group figure.dj-dropbox>figcaption{all:unset;padding:.25rem .5rem;background-color:#fff;overflow-x:hidden;min-width:12rem}django-formset django-field-group figure.dj-dropbox>figcaption dl{font-size:small;margin:0 0 .25rem 0}django-formset django-field-group figure.dj-dropbox>figcaption dl dd{margin:0}django-formset django-field-group figure.dj-dropbox>figcaption .dj-delete-file,django-formset django-field-group figure.dj-dropbox>figcaption .dj-download-file{font-weight:bold;display:inline-block;cursor:pointer;text-decoration:none}django-formset django-field-group figure.dj-dropbox>figcaption .dj-delete-file:hover,django-formset django-field-group figure.dj-dropbox>figcaption .dj-download-file:hover{text-decoration:underline}django-formset django-field-group figure.dj-dropbox>figcaption .dj-download-file{margin-left:1rem;float:right}django-formset django-field-group .dj-dual-selector{display:flex}django-formset django-field-group .dj-dual-selector .left-column,django-formset django-field-group .dj-dual-selector .right-column,django-formset django-field-group .dj-dual-selector .control-column,django-formset django-field-group .dj-dual-selector .control-panel{display:flex;flex-direction:column}django-formset django-field-group .dj-dual-selector .control-column{justify-content:center;align-items:center}django-formset django-field-group .dj-dual-selector .control-panel{padding:1rem .5rem}django-formset django-field-group .dj-dual-selector select,django-formset django-field-group .dj-dual-selector django-sortable-select{min-width:10rem}django-formset django-field-group .dj-dual-selector select{height:auto}django-formset django-field-group .dj-dual-selector input{z-index:1}django-formset django-field-group .dj-dual-selector button svg{vertical-align:middle;width:16px;height:16px}django-formset django-field-group .dj-dual-selector.invalid .right-column input{border-color:var(--django-formset-color-invalid)}django-formset django-field-group .dj-dual-selector.invalid .right-column input:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset django-field-group .dj-dual-selector.invalid .right-column select,django-formset django-field-group .dj-dual-selector.invalid .right-column django-sortable-select{border-left-color:var(--django-formset-color-invalid);border-right-color:var(--django-formset-color-invalid);border-bottom-color:var(--django-formset-color-invalid)}django-formset django-field-group .dj-dual-selector.invalid .right-column select:focus,django-formset django-field-group .dj-dual-selector.invalid .right-column django-sortable-select.focus{border-top-color:var(--django-formset-color-invalid);box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}.dj-button-decorator{line-height:initial}.dj-button-decorator svg{vertical-align:baseline;width:1rem;height:1rem}.dj-button-decorator svg .path{stroke-dasharray:1000;stroke-dashoffset:0}.dj-button-decorator svg .path.circle{animation:dash .9s ease-in-out}.dj-button-decorator svg .path.line{stroke-dashoffset:1000;animation:dash .9s .35s ease-in-out forwards}.dj-button-decorator svg .path.check{stroke-dashoffset:-100;animation:dash-check .9s .35s ease-in-out forwards}.dj-button-decorator svg .spinner{transform-origin:center;animation:rotate 1.5s infinite linear}@keyframes dash{0%{stroke-dashoffset:1000}100%{stroke-dashoffset:0}}@keyframes dash-check{0%{stroke-dashoffset:-100}100%{stroke-dashoffset:900}}@keyframes rotate{from{transform:rotate(0deg)}to{transform:rotate(360deg)}}.dj-button-decorator .dj-icon{display:inline-block;width:1em;height:1em}`;
-var wn = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
+var ye = hs;
+var xn = `select::placeholder{color:gray}select.ts-hidden-accessible{display:none}django-formset{--django-formset-color-invalid: rgb(255, 3, 0);--django-formset-shadow-invalid: rgb(255, 3, 0, 0.25);--django-formset-color-valid: rgb(0, 122, 0);--django-formset-icon-invalid: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(255, 3, 0)"><path fill-rule="evenodd" d="M8 15A7 7 0 1 0 8 1a7 7 0 0 0 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"/><path d="M7.002 11a1 1 0 1 1 2 0 1 1 0 0 1-2 0zM7.1 4.995a.905.905 0 1 1 1.8 0l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 4.995z"/></svg>');--django-formset-icon-warning: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(255, 165, 0)"><path fill-rule="evenodd" d="M7.938 2.016a.146.146 0 0 0-.054.057L1.027 13.74a.176.176 0 0 0-.002.183c.016.03.037.05.054.06.015.01.034.017.066.017h13.713a.12.12 0 0 0 .066-.017.163.163 0 0 0 .055-.06.176.176 0 0 0-.003-.183L8.12 2.073a.146.146 0 0 0-.054-.057A.13.13 0 0 0 8.002 2a.13.13 0 0 0-.064.016zm1.044-.45a1.13 1.13 0 0 0-1.96 0L.165 13.233c-.457.778.091 1.767.98 1.767h13.713c.889 0 1.438-.99.98-1.767L8.982 1.566z"/><path d="M7.002 12a1 1 0 1 1 2 0 1 1 0 0 1-2 0zM7.1 5.995a.905.905 0 1 1 1.8 0l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 5.995z"/></svg>');--django-formset-icon-valid: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(0, 122, 0)"><path fill-rule="evenodd" d="M10.97 4.97a.75.75 0 0 1 1.071 1.05l-3.992 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.236.236 0 0 1 .02-.022z"/></svg>')}django-formset ul.dj-errorlist{list-style:none;margin-top:0;margin-bottom:0;margin-left:0;padding-left:0;color:var(--django-formset-color-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=email]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=text]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=number]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=date]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=url]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=password]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>select:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>textarea:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=email]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=text]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=number]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=date]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=url]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=password]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>select:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>textarea:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=email]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=text]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=number]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=date]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=url]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=password]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>select:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>textarea:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=email]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=email]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=text]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=text]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=number]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=number]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=date]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=date]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=datetime-local]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=url]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=url]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=password]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=password]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>select:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>select:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>textarea:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>textarea:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=email]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=email]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=text]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=text]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=number]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=number]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=date]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=date]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=datetime-local]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=url]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=url]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=password]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=password]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset [role=group]{display:block}django-formset [role=group][hidden]{display:none}django-formset [role=group].dj-required>label,django-formset [role=group].dj-required-any>label{font-weight:bolder}django-formset [role=group].dj-submitted>input[type=email]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=email]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=text]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=text]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=number]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=number]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=date]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=date]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=datetime-local]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=url]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=url]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=password]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=password]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>select:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>select:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>textarea:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>textarea:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group] input{background-repeat:no-repeat !important;background-position:center right !important;background-origin:content-box !important}django-formset [role=group] input[type=date],django-formset [role=group] input[type=datetime-local]{position:relative}django-formset [role=group] input[type=date]::-webkit-datetime-edit-fields-wrapper,django-formset [role=group] input[type=datetime-local]::-webkit-datetime-edit-fields-wrapper{margin-left:1.75em}django-formset [role=group] input[type=date]::-webkit-calendar-picker-indicator,django-formset [role=group] input[type=datetime-local]::-webkit-calendar-picker-indicator{cursor:pointer;position:absolute;left:.75em}django-formset [role=group] input[type=date]:hover::-webkit-calendar-picker-indicator,django-formset [role=group] input[type=datetime-local]:hover::-webkit-calendar-picker-indicator{cursor:pointer}django-formset [role=group] select,django-formset [role=group] textarea{background-image:none !important}django-formset [role=group] select.dj-concealed,django-formset [role=group] textarea.dj-concealed{display:block !important;height:1px !important;min-height:initial !important;max-height:initial !important;padding:0 !important;margin:-1px 0 0 0 !important;border:none !important;opacity:0 !important;resize:none}django-formset [role=group] .dj-help-text{font-style:oblique}django-formset [role=group] .dj-form-optgroup{margin-bottom:.5rem}django-formset [role=group] .dj-form-optgroup>em{margin-left:.75rem}django-formset [role=group] .dj-form-inlined{display:inline-block}django-formset [role=group] input[type=file]{width:0 !important;height:0 !important}django-formset [role=group] .dj-control-panel{display:flex}django-formset [role=group] .dj-control-panel>div{height:fit-content;margin-left:.5rem}django-formset [role=group] .dj-control-panel>div progress{width:100%;margin-top:.25rem}django-formset [role=group] figure.dj-dropbox{all:unset;display:inline-flex;align-items:center;justify-content:space-between;background-color:#f5f5f5;margin:0 0 .25rem .25rem;padding:0;list-style:none;height:8rem;min-width:8rem;outline:gray thin dotted}django-formset [role=group] figure.dj-dropbox>div.dj-empty-item{flex-grow:1;text-align:center;height:auto}django-formset [role=group] figure.dj-dropbox>div.dj-empty-item p{padding-left:.5rem;padding-right:.5rem}django-formset [role=group] figure.dj-dropbox>img{all:unset;flex-grow:1;display:block;height:inherit;max-width:calc(100% - 12rem)}django-formset [role=group] figure.dj-dropbox>figcaption{all:unset;padding:.25rem .5rem;background-color:#fff;overflow-x:hidden;min-width:12rem}django-formset [role=group] figure.dj-dropbox>figcaption dl{font-size:small;margin:0 0 .25rem 0}django-formset [role=group] figure.dj-dropbox>figcaption dl dd{margin:0}django-formset [role=group] figure.dj-dropbox>figcaption .dj-delete-file,django-formset [role=group] figure.dj-dropbox>figcaption .dj-download-file{font-weight:bold;display:inline-block;cursor:pointer;text-decoration:none}django-formset [role=group] figure.dj-dropbox>figcaption .dj-delete-file:hover,django-formset [role=group] figure.dj-dropbox>figcaption .dj-download-file:hover{text-decoration:underline}django-formset [role=group] figure.dj-dropbox>figcaption .dj-download-file{margin-left:1rem;float:right}django-formset [role=group] .dj-dual-selector{display:flex}django-formset [role=group] .dj-dual-selector .left-column,django-formset [role=group] .dj-dual-selector .right-column,django-formset [role=group] .dj-dual-selector .control-column,django-formset [role=group] .dj-dual-selector .control-panel{display:flex;flex-direction:column}django-formset [role=group] .dj-dual-selector .control-column{justify-content:center;align-items:center}django-formset [role=group] .dj-dual-selector .control-panel{padding:1rem .5rem}django-formset [role=group] .dj-dual-selector select,django-formset [role=group] .dj-dual-selector django-sortable-select{min-width:10rem}django-formset [role=group] .dj-dual-selector select{height:auto}django-formset [role=group] .dj-dual-selector input{z-index:1}django-formset [role=group] .dj-dual-selector button svg{vertical-align:middle;width:16px;height:16px}django-formset [role=group] .dj-dual-selector.invalid .right-column input{border-color:var(--django-formset-color-invalid)}django-formset [role=group] .dj-dual-selector.invalid .right-column input:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group] .dj-dual-selector.invalid .right-column select,django-formset [role=group] .dj-dual-selector.invalid .right-column django-sortable-select{border-left-color:var(--django-formset-color-invalid);border-right-color:var(--django-formset-color-invalid);border-bottom-color:var(--django-formset-color-invalid)}django-formset [role=group] .dj-dual-selector.invalid .right-column select:focus,django-formset [role=group] .dj-dual-selector.invalid .right-column django-sortable-select.focus{border-top-color:var(--django-formset-color-invalid);box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}.dj-button-decorator{line-height:initial}.dj-button-decorator svg{vertical-align:baseline;width:1rem;height:1rem}.dj-button-decorator svg .path{stroke-dasharray:1000;stroke-dashoffset:0}.dj-button-decorator svg .path.circle{animation:dash .9s ease-in-out}.dj-button-decorator svg .path.line{stroke-dashoffset:1000;animation:dash .9s .35s ease-in-out forwards}.dj-button-decorator svg .path.check{stroke-dashoffset:-100;animation:dash-check .9s .35s ease-in-out forwards}.dj-button-decorator svg .spinner{transform-origin:center;animation:rotate 1.5s infinite linear}@keyframes dash{0%{stroke-dashoffset:1000}100%{stroke-dashoffset:0}}@keyframes dash-check{0%{stroke-dashoffset:-100}100%{stroke-dashoffset:900}}@keyframes rotate{from{transform:rotate(0deg)}to{transform:rotate(360deg)}}.dj-button-decorator .dj-icon{display:inline-block;width:1em;height:1em}`;
+var En = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
 	<g class="spinner">
 		<path style="stroke-width:0.729" d="m 12.73285,23.212276 -10e-7,-4.393157 A 0.27932072,0.27932072 0 0 0 12.27476,18.604602 l -2.6367848,2.196577 a 0.27932072,0.27932072 0 0 0 -10e-8,0.429037 l 2.6367859,2.196577 a 0.27932072,0.27932072 0 0 0 0.458089,-0.214517 z" />
 		<path style="stroke-width:0.729" d="m 11.298326,5.191792 -10e-7,-4.39315704 a 0.27932072,0.27932072 0 0 1 0.458086,-0.214519 L 14.393193,2.780699 a 0.27932072,0.27932072 0 0 1 2e-6,0.429033 l -2.636785,2.19658 a 0.27932072,0.27932072 0 0 1 -0.458084,-0.21452 z" />
 		<path style="fill:none;stroke:currentColor;stroke-width:2;stroke-linecap:round;stroke-miterlimit:10;stroke-dashoffset:89.339;stroke-dasharray:none" d="M 12.5,2.9179688 C 12.333705,2.9010187 12.166975,2.8886442 12,2.8808594 6.9635919,2.8807514 2.8807499,6.9635934 2.8808594,12 c 0.00661,2.530252 1.064217,4.944009 2.9199218,6.664062" />
 		<path style="fill:none;stroke:currentColor;stroke-width:2;stroke-linecap:round;stroke-miterlimit:10;stroke-dashoffset:89.339;stroke-dasharray:none" d="m 11.458261,21.082031 c 0.166295,0.01695 0.333025,0.02933 0.5,0.03711 C 16.994669,21.119249 21.077511,17.036407 21.077402,12 21.070802,9.469748 20.013185,7.055991 18.15748,5.335938" />
 	</g>
 </svg>
 `;
-var En = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
+var wn = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
 	<circle class="path circle" fill="none" stroke="currentColor" stroke-width="1.93833" stroke-miterlimit="10" cx="12.000002" cy="12.000002" r="10.030837" />
 	<polyline class="path check" fill="none" stroke="currentColor" stroke-width="12" stroke-linecap="round" stroke-miterlimit="10" points="100.2,40.2 51.5,88.8 29.8,67.5 " transform="matrix(0.18,0,0,0.18,-0.284,0.544)" />
 </svg>
 `;
 var kn = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
 	<circle class="path circle" fill="none" stroke="currentColor" stroke-width="1.93833" stroke-miterlimit="10" cx="12.000002" cy="12.000002" r="10.030837" />
 	<line class="path line" fill="none" stroke="currentColor" stroke-width="2.12533" stroke-linecap="round" stroke-miterlimit="10" x1="6.562665" y1="7.1626649" x2="17.437328" y2="16.79755" />
 	<line class="path line" fill="none" stroke="currentColor" stroke-width="2.12534" stroke-linecap="round" stroke-miterlimit="10" x1="17.437338" y1="7.1626701" x2="6.5626698" y2="16.762127" />
 </svg>
 `;
 var xs = "__all__",
-    ws = "_collection_errors_",
-    Es = "_marked_for_removal_",
+    Es = "_collection_errors_",
+    ws = "_marked_for_removal_",
     Cn = document.createElement("style");
 Cn.innerText = xn;
 document.head.appendChild(Cn);
 var Nt = class {
         constructor(e) {
             this.value = e
         }
     },
     Vt = class extends Map {
         constructor(e) {
             super();
             let r = e.element.querySelector("django-error-messages");
-            if (!r) throw new Error(`<django-field-group> for '${e.name}' requires one <django-error-messages> tag.`);
+            if (!r) throw new Error(`<div role="group"> for '${e.name}' requires one <django-error-messages> tag.`);
             for (let n of r.getAttributeNames()) {
                 let i = n.replace(/([_][a-z])/g, s => s.toUpperCase().replace("_", "")),
                     o = r.getAttribute(n);
                 o && this.set(i, o)
             }
         }
     },
@@ -2324,15 +2324,15 @@
 
             function n(s) {
                 return Array.isArray(s) ? s.length !== 0 : !!s
             }
             let i = (o = this.fieldElements[0]) == null ? void 0 : o.getAttribute(e);
             if (typeof i != "string") return null;
             try {
-                let s = new Function("return " + ve(i, {
+                let s = new Function("return " + ye(i, {
                     startRule: "Expression"
                 }));
                 return () => {
                     let u = r != n(s.call(this));
                     this.element.hasAttribute("hidden") !== u && (this.fieldElements.forEach((f, d) => f.disabled = u || this.initialDisabled[d]), this.element.toggleAttribute("hidden", u))
                 }
             } catch (s) {
@@ -2340,15 +2340,15 @@
             }
         }
         evalDisable() {
             var r;
             let e = (r = this.fieldElements[0]) == null ? void 0 : r.getAttribute("disable-if");
             if (typeof e != "string") return () => {};
             try {
-                let n = new Function("return " + ve(e, {
+                let n = new Function("return " + ye(e, {
                     startRule: "Expression"
                 }));
                 return () => {
                     let i = n.call(this);
                     this.fieldElements.forEach((o, s) => o.disabled = i || this.initialDisabled[s])
                 }
             } catch (n) {
@@ -2458,15 +2458,15 @@
                 for (let [r, n] of this.successActions.entries()) e ? e = e.then(n.func.apply(this, n.args)) : e = n.func.apply(this, n.args)();
                 if (e) {
                     for (let [r, n] of this.rejectActions.entries()) r === 0 ? e = e.catch(n.func.apply(this, n.args)) : e = e.then(n.func.apply(this, n.args));
                     e.finally(this.restore.apply(this))
                 }
             };
             var n;
-            this.formset = e, this.element = r, this.initialClass = r.getAttribute("class") ?? "", this.isAutoDisabled = !!JSON.parse((r.getAttribute("auto-disable") ?? "false").toLowerCase()), this.decoratorElement = r.querySelector(".dj-button-decorator"), this.originalDecorator = (n = this.decoratorElement) == null ? void 0 : n.cloneNode(!0), this.spinnerElement = document.createElement("i"), this.spinnerElement.classList.add("dj-icon", "dj-spinner"), this.spinnerElement.innerHTML = wn, this.okayElement = document.createElement("i"), this.okayElement.classList.add("dj-icon", "dj-okay"), this.okayElement.innerHTML = En, this.bummerElement = document.createElement("i"), this.bummerElement.classList.add("dj-icon", "dj-bummer"), this.bummerElement.innerHTML = kn, this.parseActionsQueue(r.getAttribute("click")), r.addEventListener("click", this.clicked)
+            this.formset = e, this.element = r, this.initialClass = r.getAttribute("class") ?? "", this.isAutoDisabled = !!JSON.parse((r.getAttribute("auto-disable") ?? "false").toLowerCase()), this.decoratorElement = r.querySelector(".dj-button-decorator"), this.originalDecorator = (n = this.decoratorElement) == null ? void 0 : n.cloneNode(!0), this.spinnerElement = document.createElement("i"), this.spinnerElement.classList.add("dj-icon", "dj-spinner"), this.spinnerElement.innerHTML = En, this.okayElement = document.createElement("i"), this.okayElement.classList.add("dj-icon", "dj-okay"), this.okayElement.innerHTML = wn, this.bummerElement = document.createElement("i"), this.bummerElement.classList.add("dj-icon", "dj-bummer"), this.bummerElement.innerHTML = kn, this.parseActionsQueue(r.getAttribute("click")), r.addEventListener("click", this.clicked)
         }
         autoDisable(e) {
             this.isAutoDisabled && (this.element.disabled = !e)
         }
         disable() {
             return e => (this.element.disabled = !0, Promise.resolve(e))
         }
@@ -2580,15 +2580,15 @@
                     let s = this[o.funcname];
                     if (typeof s != "function") throw new Error(`Unknown function '${o.funcname}'.`);
                     n.push(new ct(s, o.args))
                 }
                 n.length === 0 && n.push(new ct(this.noop, []))
             };
             try {
-                let n = ve(e, {
+                let n = ye(e, {
                     startRule: "Actions"
                 });
                 r(this.successActions, n.successChain), r(this.rejectActions, n.rejectChain)
             } catch (n) {
                 throw new Error(`Error while parsing <button click="${e}">: ${n}.`)
             }
         }
@@ -2604,30 +2604,30 @@
         constructor(e, r) {
             this.form = e, this.element = r, this.updateVisibility = this.evalVisibility("show-if", !0) ?? this.evalVisibility("hide-if", !1) ?? function() {}, this.updateDisabled = this.evalDisable()
         }
         evalVisibility(e, r) {
             let n = this.element.getAttribute(e);
             if (n === null) return null;
             try {
-                let i = new Function("return " + ve(n, {
+                let i = new Function("return " + ye(n, {
                     startRule: "Expression"
                 }));
                 return () => {
                     let o = r != !!i.call(this);
                     this.element.hasAttribute("hidden") !== o && this.element.toggleAttribute("hidden", o)
                 }
             } catch (i) {
                 throw new Error(`Error while parsing <fieldset show-if/hide-if="${n}">: ${i}.`)
             }
         }
         evalDisable() {
             let e = this.element.getAttribute("disable-if");
             if (typeof e != "string") return () => {};
             try {
-                let r = new Function("return " + ve(e, {
+                let r = new Function("return " + ye(e, {
                     startRule: "Expression"
                 }));
                 return () => this.element.disabled = r.call(this)
             } catch (r) {
                 throw new Error(`Error while parsing <fieldset disable-if="${e}">: ${r}.`)
             }
         }
@@ -2742,15 +2742,15 @@
             this.children = Array(0);
             this.markedForRemoval = !1;
             this.formset = e, this.element = r, this.parent = n, this.findFormCollections()
         }
         findFormCollections() {
             for (let e of J.getChildCollections(this.element)) this.children.push(e.hasAttribute("sibling-position") ? new z(this.formset, e, this) : new J(this.formset, e, this));
             for (let e of this.children) e.updateRemoveButtonAttrs();
-            this.formCollectionTemplate = we.findFormCollectionTemplate(this.formset, this.element, this)
+            this.formCollectionTemplate = Ee.findFormCollectionTemplate(this.formset, this.element, this)
         }
         assignForms(e) {
             this.forms = e.filter(r => {
                 var n;
                 return (n = r.element.parentElement) == null ? void 0 : n.isEqualNode(this.element)
             });
             for (let r of this.children) r.assignForms(e)
@@ -2834,15 +2834,15 @@
             let n = (((i = this.parent) == null ? void 0 : i.children) ?? this.formset.formCollections).filter(o => !o.markedForRemoval).length;
             this.markedForRemoval ? this.maxSiblings ? this.removeButton.disabled = n >= this.maxSiblings : this.removeButton.disabled = !1 : this.removeButton.disabled = n <= this.minSiblings
         }
         resetToInitial() {
             return this.justAdded ? (this.disconnect(), !0) : (super.resetToInitial(), !1)
         }
     },
-    we = class {
+    Ee = class {
         constructor(e, r, n) {
             this.maxSiblings = null;
             this.baseContext = new Map;
             this.markedForRemoval = !1;
             this.resortSiblings = e => {
                 var o;
                 let r = e.oldDraggableIndex ?? NaN,
@@ -2905,15 +2905,15 @@
             }
             let r = (((n = this.parent) == null ? void 0 : n.children) ?? this.formset.formCollections).filter(i => !i.markedForRemoval).length;
             this.addButton.disabled = this.maxSiblings === null ? !1 : r >= this.maxSiblings
         }
         static findFormCollectionTemplate(e, r, n) {
             let i = r.querySelector(":scope > .collection-siblings > template.empty-collection");
             if (i) {
-                let o = new we(e, i, n);
+                let o = new Ee(e, i, n);
                 return o.updateAddButtonAttrs(), o
             }
         }
     },
     Kt = class {
         constructor(e) {
             this.buttons = Array(0);
@@ -2969,15 +2969,15 @@
             for (let r of e.querySelectorAll("INPUT, SELECT, TEXTAREA")) {
                 let n = r.getAttribute("form");
                 if (!n) continue;
                 let i = this.forms.filter(u => u.formId && u.formId === n);
                 if (i.length < 1) continue;
                 if (i.length > 1) throw new Error(`More than one form has id="${n}"`);
                 let o = i[0],
-                    s = r.closest("django-field-group");
+                    s = r.closest('[role="group"]');
                 s ? o.fieldGroups.filter(u => u.element === s).length === 0 && o.fieldGroups.push(new Gt(o, s)) : r instanceof HTMLInputElement && r.type === "hidden" && (o.hiddenInputFields.includes(r) || o.hiddenInputFields.push(r))
             }
         }
         findForms(e) {
             e = e ?? this.element;
             for (let r of e.getElementsByTagName("FORM")) {
                 let n = new Ut(this, r);
@@ -2993,15 +2993,15 @@
                 if (!n.name) throw new Error("Multiple <form>-elements in a <django-formset> require a unique name each.");
                 if (n.name in r) throw new Error(`Duplicate name "${n.name}" used in multiple forms of same <django-formset>.`);
                 r.push(n.name)
             })
         }
         findFormCollections() {
             for (let e of J.getChildCollections(this.element)) this.formCollections.push(e.hasAttribute("sibling-position") ? new z(this, e) : new J(this, e));
-            this.formCollections.forEach(e => e.updateRemoveButtonAttrs()), this.formCollectionTemplate = we.findFormCollectionTemplate(this, this.element)
+            this.formCollections.forEach(e => e.updateRemoveButtonAttrs()), this.formCollectionTemplate = Ee.findFormCollectionTemplate(this, this.element)
         }
         findCollectionErrorsList() {
             for (let e of this.element.getElementsByClassName("dj-collection-errors")) {
                 let r = e.getAttribute("prefix") ?? "",
                     n = e.querySelector("ul.dj-errorlist");
                 this.collectionErrorsList.set(r, n)
             }
@@ -3056,15 +3056,15 @@
                 r = (0, xe.default)(i, s), n(i, s)
             }
             for (let o of this.forms) {
                 if (!o.name) return Object.assign({}, this.data, {
                     _extra: e
                 });
                 let s = o.getAbsPath();
-                r = (0, xe.default)(this.data, s), o.markedForRemoval && (r[Es] = !0), n(i, s)
+                r = (0, xe.default)(this.data, s), o.markedForRemoval && (r[ws] = !0), n(i, s)
             }
             return Object.assign({}, i, {
                 _extra: e
             })
         }
         async submit(e) {
             let r = !0;
@@ -3105,15 +3105,15 @@
         reportErrors(e) {
             for (let r of this.forms) {
                 let n = r.name ? (0, xe.default)(e, r.name.split("."), null) : e;
                 n ? (r.reportCustomErrors(new Map(Object.entries(n))), r.reportValidity()) : r.clearCustomErrors()
             }
             for (let [r, n] of this.collectionErrorsList) {
                 let i = r ? r.split(".") : [];
-                i = [...i, "0", ws];
+                i = [...i, "0", Es];
                 for (let o of (0, xe.default)(e, i, [])) {
                     let s = document.createElement("li");
                     s.classList.add("dj-placeholder"), s.innerText = o, n.appendChild(s)
                 }
             }
         }
         resetToInitial() {
@@ -3140,76 +3140,76 @@
         }
         clearErrors() {
             for (let e of this.forms) e.clearCustomErrors();
             for (let e of this.collectionErrorsList.values())
                 for (; e.firstElementChild;) e.removeChild(e.firstElementChild)
         }
     },
-    ye = Symbol("DjangoFormset"),
+    je = Symbol("DjangoFormset"),
     ut = class extends HTMLElement {
         constructor() {
             super();
-            this[ye] = new Kt(this)
+            this[je] = new Kt(this)
         }
         static get observedAttributes() {
             return ["endpoint", "withhold-messages", "force-submission"]
         }
         connectedCallback() {
-            this[ye].connectedCallback()
+            this[je].connectedCallback()
         }
         async submit(r) {
-            return this[ye].submit(r)
+            return this[je].submit(r)
         }
         async abort() {
-            return this[ye].abort()
+            return this[je].abort()
         }
         async reset() {
-            return this[ye].resetToInitial()
+            return this[je].resetToInitial()
         }
     };
-ye;
+je;
 window.addEventListener("DOMContentLoaded", t => {
     let e = dr.convertPseudoClasses(),
         r = Array();
 
     function n(s, u, f, d = void 0) {
         customElements.get(u) instanceof Function ? s() : (window.customElements.define(u, f, d), window.customElements.whenDefined(u).then(() => s()))
     }
 
     function i(s) {
         s.querySelector('select[is="django-selectize"]') && r.push(new Promise((u, f) => {
-            import("./DjangoSelectize-H6QF7W4R.js").then(({
+            import("./DjangoSelectize-OIQWF5I5.js").then(({
                 DjangoSelectizeElement: d
             }) => {
                 n(u, "django-selectize", d, {
                     extends: "select"
                 })
             }).catch(d => f(d))
         })), s.querySelector("django-sortable-select") ? r.push(new Promise((u, f) => {
-            import("./SortableSelect-4MNY532K.js").then(({
+            import("./SortableSelect-CEPX3LH6.js").then(({
                 SortableSelectElement: d
             }) => {
-                customElements.get("django-sortable-select") instanceof Function ? u() : window.customElements.define("django-sortable-select", d), import("./DualSelector-GVLJZFWV.js").then(({
+                customElements.get("django-sortable-select") instanceof Function ? u() : window.customElements.define("django-sortable-select", d), import("./DualSelector-2ALH4RIS.js").then(({
                     DualSelectorElement: h
                 }) => {
                     customElements.get("django-dual-selector") instanceof Function ? u() : (window.customElements.define("django-dual-selector", h, {
                         extends: "select"
                     }), Promise.all([window.customElements.whenDefined("django-sortable-select"), window.customElements.whenDefined("django-dual-selector")]).then(() => u()))
                 }).catch(h => f(h))
             }).catch(d => f(d))
         })) : s.querySelector('select[is="django-dual-selector"]') && r.push(new Promise((u, f) => {
-            import("./DualSelector-GVLJZFWV.js").then(({
+            import("./DualSelector-2ALH4RIS.js").then(({
                 DualSelectorElement: d
             }) => {
                 n(u, "django-dual-selector", d, {
                     extends: "select"
                 })
             }).catch(d => f(d))
         })), s.querySelector('textarea[is="django-richtext"]') && r.push(new Promise((u, f) => {
-            import("./RichtextArea-UTSZPGIP.js").then(({
+            import("./RichtextArea-XKK27UIM.js").then(({
                 RichTextAreaElement: d
             }) => {
                 n(u, "django-richtext", d, {
                     extends: "textarea"
                 })
             }).catch(d => f(d))
         })), s.querySelector('input[is="django-slug"]') && r.push(new Promise((u, f) => {
@@ -3217,23 +3217,23 @@
                 DjangoSlugElement: d
             }) => {
                 n(u, "django-slug", d, {
                     extends: "input"
                 })
             }).catch(d => f(d))
         })), s.querySelector('input[is="django-datepicker"]') && r.push(new Promise((u, f) => {
-            import("./DateTimePicker-OYPFNQAF.js").then(({
+            import("./DateTimePicker-BBOUOZRC.js").then(({
                 DatePickerElement: d
             }) => {
                 n(u, "django-datepicker", d, {
                     extends: "input"
                 })
             }).catch(d => f(d))
         })), s.querySelector('input[is="django-datetimepicker"]') && r.push(new Promise((u, f) => {
-            import("./DateTimePicker-OYPFNQAF.js").then(({
+            import("./DateTimePicker-BBOUOZRC.js").then(({
                 DateTimePickerElement: d
             }) => {
                 n(u, "django-datetimepicker", d, {
                     extends: "input"
                 })
             }).catch(d => f(d))
         }))
```

### Comparing `django-formset-1.0.dev3/formset/static/formset/scss/bootstrap5-extra.scss` & `django-formset-1.0.dev4/formset/static/formset/scss/bootstrap5-extra.scss`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/static/formset/scss/collections.scss` & `django-formset-1.0.dev4/formset/static/formset/scss/collections.scss`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/calendar/hours.html` & `django-formset-1.0.dev4/formset/templates/calendar/hours.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/calendar/months.html` & `django-formset-1.0.dev4/formset/templates/calendar/months.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/calendar/weeks.html` & `django-formset-1.0.dev4/formset/templates/calendar/weeks.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/calendar/years.html` & `django-formset-1.0.dev4/formset/templates/calendar/years.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/dual_selector.html` & `django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/file.html` & `django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/dual_selector.html` & `django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/file.html` & `django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/default/buttons/richtext_align.html` & `django-formset-1.0.dev4/formset/templates/formset/default/buttons/richtext_align.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/default/buttons/richtext_color.html` & `django-formset-1.0.dev4/formset/templates/formset/default/buttons/richtext_color.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/default/buttons/richtext_heading.html` & `django-formset-1.0.dev4/formset/templates/formset/default/buttons/richtext_heading.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/default/collection.html` & `django-formset-1.0.dev4/formset/templates/formset/default/collection.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/default/dialog_form.html` & `django-formset-1.0.dev4/formset/templates/formset/default/dialog_form.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/default/fieldset.html` & `django-formset-1.0.dev4/formset/templates/formset/default/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/default/widgets/dual_selector.html` & `django-formset-1.0.dev4/formset/templates/formset/default/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/default/widgets/file.html` & `django-formset-1.0.dev4/formset/templates/formset/default/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/default/widgets/selectize.html` & `django-formset-1.0.dev4/formset/templates/formset/default/widgets/selectize.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/foundation/widgets/dual_selector.html` & `django-formset-1.0.dev4/formset/templates/formset/foundation/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/foundation/widgets/file.html` & `django-formset-1.0.dev4/formset/templates/formset/foundation/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/icons/blockquote.svg` & `django-formset-1.0.dev4/formset/templates/formset/icons/blockquote.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/icons/letters.svg` & `django-formset-1.0.dev4/formset/templates/formset/icons/letters.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/icons/placeholder.svg` & `django-formset-1.0.dev4/formset/templates/formset/icons/placeholder.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/icons/questionmark.svg` & `django-formset-1.0.dev4/formset/templates/formset/icons/questionmark.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/icons/subscript.svg` & `django-formset-1.0.dev4/formset/templates/formset/icons/subscript.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/icons/unlink.svg` & `django-formset-1.0.dev4/formset/templates/formset/icons/unlink.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/dual_selector.html` & `django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/file.html` & `django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templates/formset/uikit/widgets/file.html` & `django-formset-1.0.dev4/formset/templates/formset/uikit/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templatetags/formsetify.py` & `django-formset-1.0.dev4/formset/templatetags/formsetify.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/templatetags/richtext.py` & `django-formset-1.0.dev4/formset/templatetags/richtext.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,16 @@
             root_node = {}
     template = get_template(doc_template)
     html = template.render({'node': root_node, 'framework': framework}).replace('\t', '').replace('\n', '')
     return mark_safe(html)
 
 
 def render_attributes(context, attrs):
+    if not isinstance(attrs, dict):
+        return ''
     framework = context.get('framework', 'default')
     try:
         richtext_attributes = import_string(f'formset.renderers.{framework}.richtext_attributes')
     except ImportError:
         from formset.renderers.default import richtext_attributes
     return richtext_attributes(attrs)
```

### Comparing `django-formset-1.0.dev3/formset/upload.py` & `django-formset-1.0.dev4/formset/upload.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/utils.py` & `django-formset-1.0.dev4/formset/utils.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/views.py` & `django-formset-1.0.dev4/formset/views.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/formset/widgets.py` & `django-formset-1.0.dev4/formset/widgets.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev3/setup.py` & `django-formset-1.0.dev4/setup.py`

 * *Files identical despite different names*

