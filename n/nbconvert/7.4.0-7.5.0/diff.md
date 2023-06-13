# Comparing `tmp/nbconvert-7.4.0.tar.gz` & `tmp/nbconvert-7.5.0.tar.gz`

## Comparing `nbconvert-7.4.0.tar` & `nbconvert-7.5.0.tar`

### file list

```diff
@@ -1,277 +1,279 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.mailmap
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.prettierignore
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.readthedocs.yaml
--rw-r--r--   0        0        0    72042 2020-02-02 00:00:00.000000 nbconvert-7.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 nbconvert-7.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 nbconvert-7.4.0/RELEASE.md
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 nbconvert-7.4.0/check_requirements.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/dependabot.yml
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/Makefile
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/README.md
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/autogen_config.py
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/make.bat
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/api_examples/template_path/make_html.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/api_examples/template_path/quiz_notebook.py
--rw-r--r--   0        0        0    36829 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/api_examples/template_path/media/image1.png
--rw-r--r--   0        0        0   176383 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/api_examples/template_path/media/image2.png
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/conf.json
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2
--rw-r--r--   0        0        0   266255 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css
--rw-r--r--   0        0        0     8651 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/architecture.rst
--rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/conf.py
--rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/customizing.rst
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/dejavu.rst
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/development_release.rst
--rw-r--r--   0        0        0     7875 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/execute_api.rst
--rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/external_exporters.rst
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/highlighting.rst
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/index.rst
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/install.rst
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/latex_citations.rst
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/nbconvert_library.ipynb
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/need_help.rst
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/removing_cells.rst
--rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/usage.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/_static/empty.txt
--rw-r--r--   0        0        0    36971 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/_static/exporter_inheritance.png
--rw-r--r--   0        0        0    65726 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/_static/preprocessor_inheritance.png
--rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/_static/writer_inheritance.png
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/api/exporters.rst
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/api/filters.rst
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/api/index.rst
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/api/nbconvertapp.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/api/postprocessors.rst
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/api/preprocessors.rst
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nbconvert-7.4.0/docs/source/api/writers.rst
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/__main__.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/_version.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/conftest.py
--rwxr-xr-x   0        0        0    24129 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/nbconvertapp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/py.typed
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/__init__.py
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/asciidoc.py
--rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/base.py
--rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/exporter.py
--rw-r--r--   0        0        0    11270 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/html.py
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/latex.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/markdown.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/notebook.py
--rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/pdf.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/python.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/qt_exporter.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/qt_screenshot.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/qtpdf.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/qtpng.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/rst.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/script.py
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/slides.py
--rw-r--r--   0        0        0    26970 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/templateexporter.py
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/webpdf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/__init__.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/base.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/cheese.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_asciidoc.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_export.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_exporter.py
--rw-r--r--   0        0        0     7891 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_html.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_latex.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_markdown.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_notebook.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_pdf.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_python.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_qtpdf.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_qtpng.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_rst.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_script.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_slides.py
--rw-r--r--   0        0        0    27769 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_templateexporter.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/test_webpdf.py
--rw-r--r--   0        0        0    45585 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/attachment.ipynb
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/lablike.html.j2
--rw-r--r--   0        0        0    10437 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/notebook2.ipynb
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/notebook3.ipynb
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/notebook_inject.ipynb
--rw-r--r--   0        0        0    16782 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/pngmetadata.ipynb
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/prompt_numbers.ipynb
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/rawtest.ipynb
--rw-r--r--   0        0        0    19943 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/exporters/tests/files/svg.ipynb
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/__init__.py
--rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/ansi.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/citation.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/datatypefilter.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/filter_links.py
--rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/highlight.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/latex.py
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/markdown.py
--rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/markdown_mistune.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/metadata.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/pandoc.py
--rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/strings.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/svg_constants.py
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/widgetsdatatypefilter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/__init__.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/test_ansi.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/test_citation.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/test_datatypefilter.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/test_highlight.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/test_latex.py
--rw-r--r--   0        0        0     8534 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/test_markdown.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/test_metadata.py
--rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/filters/tests/test_strings.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/postprocessors/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/postprocessors/base.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/postprocessors/serve.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/postprocessors/tests/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/postprocessors/tests/test_serve.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/__init__.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/base.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/clearmetadata.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/clearoutput.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/coalescestreams.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/convertfigures.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/csshtmlheader.py
--rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/execute.py
--rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/extractattachments.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/extractoutput.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/highlightmagics.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/latex.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/regexremove.py
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/sanitize.py
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/svg2pdf.py
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tagremove.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/__init__.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/base.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/fake_kernelmanager.py
--rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_clearmetadata.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_clearoutput.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_coalescestreams.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_csshtmlheader.py
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_execute.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_extractattachments.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_extractoutput.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_highlightmagics.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_latex.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_regexremove.py
--rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_sanitize.py
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_svg2pdf.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/test_tagremove.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/files/HelloWorld.ipynb
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/resources/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/templates/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/templates/skeleton/Makefile
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/templates/skeleton/README.md
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/__init__.py
--rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/base.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/fake_exporters.py
--rw-r--r--   0        0        0    29353 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/test_nbconvertapp.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/utils.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/exporter_entrypoint/eptest.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/exporter_entrypoint/eptest-0.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/Unexecuted_widget.ipynb
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/Unexecuted_widget_2.ipynb
--rw-r--r--   0        0        0    96479 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/Widget_List.ipynb
--rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/containerized_deployments.jpeg
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/hello.py
--rw-r--r--   0        0        0    18524 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/issue1849_svg.ipynb
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/jupyter_nbconvert_config.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/latex-linked-image.ipynb
--rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/markdown_display_priority.ipynb
--rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/notebook1.ipynb
--rw-r--r--   0        0        0   125459 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/notebook2.ipynb
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/notebook3_with_errors.ipynb
--rw-r--r--   0        0        0    18657 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/notebook4_jpeg.ipynb
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/notebook5_embed_images.ipynb
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/notebook_jl.ipynb
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/notebook_tags.ipynb
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/override.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/tests/files/testimage.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/_contextlib_chdir.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/base.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/exceptions.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/io.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/lexers.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/pandoc.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/text.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/tests/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/tests/test_io.py
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/tests/test_pandoc.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/utils/tests/test_version.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/__init__.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/base.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/debug.py
--rw-r--r--   0        0        0     6017 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/files.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/stdout.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/tests/__init__.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/tests/test_debug.py
--rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/tests/test_files.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 nbconvert-7.4.0/nbconvert/writers/tests/test_stdout.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/asciidoc/conf.json
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/asciidoc/index.asciidoc.j2
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/base/cell_id_anchor.j2
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/base/celltags.j2
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/base/display_priority.j2
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/base/jupyter_widgets.html.j2
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/base/mathjax.html.j2
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/base/null.j2
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/basic/conf.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/basic/index.html.j2
--rw-r--r--   0        0        0     8261 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/classic/base.html.j2
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/classic/conf.json
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/classic/index.html.j2
--rw-r--r--   0        0        0   265101 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/classic/static/style.css
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/compatibility/display_priority.tpl
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/compatibility/full.tpl
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/lab/base.html.j2
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/lab/conf.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/lab/index.html.j2
--rw-r--r--   0        0        0   581722 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/lab/static/index.css
--rw-r--r--   0        0        0    16733 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/lab/static/theme-dark.css
--rw-r--r--   0        0        0    15637 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/lab/static/theme-light.css
--rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/base.tex.j2
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/conf.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/display_priority.j2
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/document_contents.tex.j2
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/index.tex.j2
--rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/null.j2
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/report.tex.j2
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/style_bw_ipython.tex.j2
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/style_bw_python.tex.j2
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/style_ipython.tex.j2
--rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/style_jupyter.tex.j2
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/latex/style_python.tex.j2
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/markdown/conf.json
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/markdown/index.md.j2
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/python/conf.json
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/python/index.py.j2
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/reveal/base.html.j2
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/reveal/cellslidedata.j2
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/reveal/conf.json
--rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/reveal/index.html.j2
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/reveal/static/custom_reveal.css
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/rst/conf.json
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/rst/index.rst.j2
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/script/conf.json
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/script/script.j2
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/webpdf/conf.json
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 nbconvert-7.4.0/share/templates/webpdf/index.pdf.j2
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nbconvert-7.4.0/.gitignore
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 nbconvert-7.4.0/LICENSE
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 nbconvert-7.4.0/README.md
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 nbconvert-7.4.0/hatch_build.py
--rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 nbconvert-7.4.0/pyproject.toml
--rw-r--r--   0        0        0     7925 2020-02-02 00:00:00.000000 nbconvert-7.4.0/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 nbconvert-7.5.0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 nbconvert-7.5.0/.mailmap
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 nbconvert-7.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nbconvert-7.5.0/.prettierignore
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nbconvert-7.5.0/.readthedocs.yaml
+-rw-r--r--   0        0        0    73812 2020-02-02 00:00:00.000000 nbconvert-7.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 nbconvert-7.5.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 nbconvert-7.5.0/RELEASE.md
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 nbconvert-7.5.0/check_requirements.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 nbconvert-7.5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 nbconvert-7.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 nbconvert-7.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 nbconvert-7.5.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 nbconvert-7.5.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nbconvert-7.5.0/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 nbconvert-7.5.0/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nbconvert-7.5.0/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 nbconvert-7.5.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/Makefile
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/README.md
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/autogen_config.py
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/make.bat
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/api_examples/template_path/make_html.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/api_examples/template_path/quiz_notebook.py
+-rw-r--r--   0        0        0    36829 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/api_examples/template_path/media/image1.png
+-rw-r--r--   0        0        0   176383 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/api_examples/template_path/media/image2.png
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/conf.json
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2
+-rw-r--r--   0        0        0   266255 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css
+-rw-r--r--   0        0        0     8651 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/architecture.rst
+-rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/conf.py
+-rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/customizing.rst
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/dejavu.rst
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/development_release.rst
+-rw-r--r--   0        0        0     7875 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/execute_api.rst
+-rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/external_exporters.rst
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/highlighting.rst
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/index.rst
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/install.rst
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/latex_citations.rst
+-rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/nbconvert_library.ipynb
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/need_help.rst
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/removing_cells.rst
+-rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/usage.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/_static/empty.txt
+-rw-r--r--   0        0        0    36971 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/_static/exporter_inheritance.png
+-rw-r--r--   0        0        0    65726 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/_static/preprocessor_inheritance.png
+-rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/_static/writer_inheritance.png
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/api/exporters.rst
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/api/filters.rst
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/api/index.rst
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/api/nbconvertapp.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/api/postprocessors.rst
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/api/preprocessors.rst
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nbconvert-7.5.0/docs/source/api/writers.rst
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/__main__.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/_version.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/conftest.py
+-rwxr-xr-x   0        0        0    24129 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/nbconvertapp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/py.typed
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/__init__.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/asciidoc.py
+-rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/base.py
+-rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/exporter.py
+-rw-r--r--   0        0        0    11557 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/html.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/latex.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/markdown.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/notebook.py
+-rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/pdf.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/python.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/qt_exporter.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/qt_screenshot.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/qtpdf.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/qtpng.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/rst.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/script.py
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/slides.py
+-rw-r--r--   0        0        0    26970 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/templateexporter.py
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/webpdf.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/__init__.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/base.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/cheese.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/test_asciidoc.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/test_export.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/test_exporter.py
+-rw-r--r--   0        0        0     7891 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/test_html.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/test_latex.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/test_markdown.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/test_notebook.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/test_pdf.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/test_python.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/test_qtpdf.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/test_qtpng.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/test_rst.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/test_script.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/test_slides.py
+-rw-r--r--   0        0        0    27769 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/test_templateexporter.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/test_webpdf.py
+-rw-r--r--   0        0        0    45585 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/files/attachment.ipynb
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/files/lablike.html.j2
+-rw-r--r--   0        0        0    10437 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/files/notebook2.ipynb
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/files/notebook3.ipynb
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/files/notebook_inject.ipynb
+-rw-r--r--   0        0        0    16782 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/files/pngmetadata.ipynb
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/files/prompt_numbers.ipynb
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/files/rawtest.ipynb
+-rw-r--r--   0        0        0    19943 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/exporters/tests/files/svg.ipynb
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/__init__.py
+-rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/ansi.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/citation.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/datatypefilter.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/filter_links.py
+-rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/highlight.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/latex.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/markdown.py
+-rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/markdown_mistune.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/metadata.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/pandoc.py
+-rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/strings.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/svg_constants.py
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/widgetsdatatypefilter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/tests/__init__.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/tests/test_ansi.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/tests/test_citation.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/tests/test_datatypefilter.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/tests/test_highlight.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/tests/test_latex.py
+-rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/tests/test_markdown.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/tests/test_metadata.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/tests/test_pandoc.py
+-rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/filters/tests/test_strings.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/postprocessors/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/postprocessors/base.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/postprocessors/serve.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/postprocessors/tests/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/postprocessors/tests/test_serve.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/__init__.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/base.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/clearmetadata.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/clearoutput.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/coalescestreams.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/convertfigures.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/csshtmlheader.py
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/execute.py
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/extractattachments.py
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/extractoutput.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/highlightmagics.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/latex.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/regexremove.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/sanitize.py
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/svg2pdf.py
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tagremove.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/__init__.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/base.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/fake_kernelmanager.py
+-rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/test_clearmetadata.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/test_clearoutput.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/test_coalescestreams.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/test_csshtmlheader.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/test_execute.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/test_extractattachments.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/test_extractoutput.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/test_highlightmagics.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/test_latex.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/test_regexremove.py
+-rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/test_sanitize.py
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/test_svg2pdf.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/test_tagremove.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/files/HelloWorld.ipynb
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/resources/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/templates/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/templates/skeleton/Makefile
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/templates/skeleton/README.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/__init__.py
+-rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/base.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/fake_exporters.py
+-rw-r--r--   0        0        0    29353 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/test_nbconvertapp.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/utils.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/exporter_entrypoint/eptest.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/exporter_entrypoint/eptest-0.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/Unexecuted_widget.ipynb
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/Unexecuted_widget_2.ipynb
+-rw-r--r--   0        0        0    96479 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/Widget_List.ipynb
+-rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/containerized_deployments.jpeg
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/hello.py
+-rw-r--r--   0        0        0    18524 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/issue1849_svg.ipynb
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/jupyter_nbconvert_config.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/latex-linked-image.ipynb
+-rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/markdown_display_priority.ipynb
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/notebook1.ipynb
+-rw-r--r--   0        0        0   125459 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/notebook2.ipynb
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/notebook3_with_errors.ipynb
+-rw-r--r--   0        0        0    18657 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/notebook4_jpeg.ipynb
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/notebook5_embed_images.ipynb
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/notebook_jl.ipynb
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/notebook_tags.ipynb
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/override.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/tests/files/testimage.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/utils/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/utils/_contextlib_chdir.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/utils/base.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/utils/exceptions.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/utils/io.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/utils/lexers.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/utils/pandoc.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/utils/text.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/utils/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/utils/tests/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/utils/tests/test_io.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/utils/tests/test_pandoc.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/utils/tests/test_version.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/writers/__init__.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/writers/base.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/writers/debug.py
+-rw-r--r--   0        0        0     6017 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/writers/files.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/writers/stdout.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/writers/tests/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/writers/tests/test_debug.py
+-rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/writers/tests/test_files.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 nbconvert-7.5.0/nbconvert/writers/tests/test_stdout.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/asciidoc/conf.json
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/asciidoc/index.asciidoc.j2
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/base/cell_id_anchor.j2
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/base/celltags.j2
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/base/display_priority.j2
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/base/jupyter_widgets.html.j2
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/base/mathjax.html.j2
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/base/null.j2
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/basic/conf.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/basic/index.html.j2
+-rw-r--r--   0        0        0     8261 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/classic/base.html.j2
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/classic/conf.json
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/classic/index.html.j2
+-rw-r--r--   0        0        0   265101 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/classic/static/style.css
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/compatibility/display_priority.tpl
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/compatibility/full.tpl
+-rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/lab/base.html.j2
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/lab/conf.json
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/lab/index.html.j2
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/lab/mermaidjs.html.j2
+-rw-r--r--   0        0        0   581722 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/lab/static/index.css
+-rw-r--r--   0        0        0    16733 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/lab/static/theme-dark.css
+-rw-r--r--   0        0        0    15637 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/lab/static/theme-light.css
+-rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/latex/base.tex.j2
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/latex/conf.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/latex/display_priority.j2
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/latex/document_contents.tex.j2
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/latex/index.tex.j2
+-rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/latex/null.j2
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/latex/report.tex.j2
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/latex/style_bw_ipython.tex.j2
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/latex/style_bw_python.tex.j2
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/latex/style_ipython.tex.j2
+-rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/latex/style_jupyter.tex.j2
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/latex/style_python.tex.j2
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/markdown/conf.json
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/markdown/index.md.j2
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/python/conf.json
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/python/index.py.j2
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/reveal/base.html.j2
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/reveal/cellslidedata.j2
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/reveal/conf.json
+-rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/reveal/index.html.j2
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/reveal/static/custom_reveal.css
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/rst/conf.json
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/rst/index.rst.j2
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/script/conf.json
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/script/script.j2
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/webpdf/conf.json
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 nbconvert-7.5.0/share/templates/webpdf/index.pdf.j2
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nbconvert-7.5.0/.gitignore
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 nbconvert-7.5.0/LICENSE
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 nbconvert-7.5.0/README.md
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 nbconvert-7.5.0/hatch_build.py
+-rw-r--r--   0        0        0     7267 2020-02-02 00:00:00.000000 nbconvert-7.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 nbconvert-7.5.0/PKG-INFO
```

### Comparing `nbconvert-7.4.0/.mailmap` & `nbconvert-7.5.0/.mailmap`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/.pre-commit-config.yaml` & `nbconvert-7.5.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       - id: check-json
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.22.0
+    rev: 0.23.1
     hooks:
       - id: check-github-workflows
 
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
@@ -32,11 +32,11 @@
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.263
+    rev: v0.0.270
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `nbconvert-7.4.0/CHANGELOG.md` & `nbconvert-7.5.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,37 @@
 # Changes in nbconvert
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 7.5.0
+
+([Full Changelog](https://github.com/jupyter/nbconvert/compare/v7.4.0...3dd3a67bf16474042efac25519ef257d708a8d7b))
+
+### Enhancements made
+
+- Add mermaidjs 10.2.3 [#1957](https://github.com/jupyter/nbconvert/pull/1957) ([@bollwyvl](https://github.com/bollwyvl))
+
+### Bugs fixed
+
+- Fix pdf conversion with explicitly relative paths [#2005](https://github.com/jupyter/nbconvert/pull/2005) ([@tuncbkose](https://github.com/tuncbkose))
+- Ensure TEXINPUTS is an absolute path [#2002](https://github.com/jupyter/nbconvert/pull/2002) ([@tuncbkose](https://github.com/tuncbkose))
+
+### Maintenance and upkeep improvements
+
+- bump pandoc max version [#1997](https://github.com/jupyter/nbconvert/pull/1997) ([@tuncbkose](https://github.com/tuncbkose))
+- exclude bleach 5.0.0 from dependencies resolution [#1990](https://github.com/jupyter/nbconvert/pull/1990) ([@karlicoss](https://github.com/karlicoss))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter/nbconvert/graphs/contributors?from=2023-05-08&to=2023-06-13&type=c))
+
+[@blink1073](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Ablink1073+updated%3A2023-05-08..2023-06-13&type=Issues) | [@bollwyvl](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Abollwyvl+updated%3A2023-05-08..2023-06-13&type=Issues) | [@karlicoss](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Akarlicoss+updated%3A2023-05-08..2023-06-13&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Apre-commit-ci+updated%3A2023-05-08..2023-06-13&type=Issues) | [@tuncbkose](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Atuncbkose+updated%3A2023-05-08..2023-06-13&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 7.4.0
 
 ([Full Changelog](https://github.com/jupyter/nbconvert/compare/v7.3.1...32fcf7b26462f5d51d577f8beda9d49cd3a0f441))
 
 ### Enhancements made
 
 - Add ExtractAttachmentsPreprocessor [#1978](https://github.com/jupyter/nbconvert/pull/1978) ([@tuncbkose](https://github.com/tuncbkose))
@@ -24,16 +50,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter/nbconvert/graphs/contributors?from=2023-04-10&to=2023-05-08&type=c))
 
 [@blink1073](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Ablink1073+updated%3A2023-04-10..2023-05-08&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Akrassowski+updated%3A2023-04-10..2023-05-08&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Apre-commit-ci+updated%3A2023-04-10..2023-05-08&type=Issues) | [@tuncbkose](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Atuncbkose+updated%3A2023-04-10..2023-05-08&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 7.3.1
 
 ([Full Changelog](https://github.com/jupyter/nbconvert/compare/v7.3.0...3860152ecea3d9833540eebe279ff603b3d47cea))
 
 ### Bugs fixed
 
 - Remove overwriting of default KernelManager [#1972](https://github.com/jupyter/nbconvert/pull/1972) ([@tuncbkose](https://github.com/tuncbkose))
```

### Comparing `nbconvert-7.4.0/CONTRIBUTING.md` & `nbconvert-7.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/RELEASE.md` & `nbconvert-7.5.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/check_requirements.py` & `nbconvert-7.5.0/check_requirements.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/.github/workflows/docs.yml` & `nbconvert-7.5.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/.github/workflows/prep-release.yml` & `nbconvert-7.5.0/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/.github/workflows/publish-release.yml` & `nbconvert-7.5.0/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/.github/workflows/tests.yml` & `nbconvert-7.5.0/.github/workflows/tests.yml`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         if: startsWith(runner.os, 'Linux')
         run: |
           sudo apt-get update
           sudo apt-get install texlive-plain-generic inkscape texlive-xetex latexmk
           sudo apt-get install xvfb x11-utils libxkbcommon-x11-0  libxcb-xinerama0 python3-pyqt5
 
           # pandoc is not up to date in the ubuntu repos, so we install directly
-          wget https://github.com/jgm/pandoc/releases/download/2.14.2/pandoc-2.14.2-1-amd64.deb && sudo dpkg -i pandoc-2.14.2-1-amd64.deb
+          wget https://github.com/jgm/pandoc/releases/download/3.1.2/pandoc-3.1.2-1-amd64.deb && sudo dpkg -i pandoc-3.1.2-1-amd64.deb
 
       - name: Run tests on Linux
         if: ${{ startsWith(runner.os, 'linux') }}
         run: |
           xvfb-run --auto-servernum hatch run cov:test
 
       - name: Run tests on other platforms
@@ -106,18 +106,26 @@
     steps:
       - uses: actions/checkout@v3
       - name: Base Setup
         uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
         with:
           dependency_type: minimum
           only_create_file: 1
-      - name: Run the unit tests
+      - name: Install dependencies
+        run: |
+          sudo apt-get update
+          sudo apt-get install texlive-plain-generic inkscape texlive-xetex latexmk
+          sudo apt-get install xvfb x11-utils libxkbcommon-x11-0  libxcb-xinerama0 python3-pyqt5
+
+          # pandoc is not up to date in the ubuntu repos, so we install directly
+          wget https://github.com/jgm/pandoc/releases/download/2.14.2/pandoc-2.14.2-1-amd64.deb && sudo dpkg -i pandoc-2.14.2-1-amd64.deb
+
+      - name: Run tests
         run: |
-          export NBFORMAT_VALIDATOR=jsonschema
-          hatch run test:nowarn || hatch run test:nowarn --lf
+          xvfb-run --auto-servernum hatch run test:nowarn || xvfb-run --auto-servernum hatch run test:nowarn --lf
 
   test_prereleases:
     name: Test Prereleases
     runs-on: ubuntu-latest
     timeout-minutes: 20
     steps:
       - uses: actions/checkout@v3
```

### Comparing `nbconvert-7.4.0/docs/Makefile` & `nbconvert-7.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/README.md` & `nbconvert-7.5.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/autogen_config.py` & `nbconvert-7.5.0/docs/autogen_config.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/make.bat` & `nbconvert-7.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/api_examples/template_path/make_html.py` & `nbconvert-7.5.0/docs/api_examples/template_path/make_html.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/api_examples/template_path/quiz_notebook.py` & `nbconvert-7.5.0/docs/api_examples/template_path/quiz_notebook.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/api_examples/template_path/media/image1.png` & `nbconvert-7.5.0/docs/api_examples/template_path/media/image1.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/api_examples/template_path/media/image2.png` & `nbconvert-7.5.0/docs/api_examples/template_path/media/image2.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2` & `nbconvert-7.5.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css` & `nbconvert-7.5.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/architecture.rst` & `nbconvert-7.5.0/docs/source/architecture.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/conf.py` & `nbconvert-7.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/customizing.rst` & `nbconvert-7.5.0/docs/source/customizing.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/dejavu.rst` & `nbconvert-7.5.0/docs/source/dejavu.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/development_release.rst` & `nbconvert-7.5.0/docs/source/development_release.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/execute_api.rst` & `nbconvert-7.5.0/docs/source/execute_api.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/external_exporters.rst` & `nbconvert-7.5.0/docs/source/external_exporters.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/highlighting.rst` & `nbconvert-7.5.0/docs/source/highlighting.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/index.rst` & `nbconvert-7.5.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/install.rst` & `nbconvert-7.5.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/latex_citations.rst` & `nbconvert-7.5.0/docs/source/latex_citations.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/nbconvert_library.ipynb` & `nbconvert-7.5.0/docs/source/nbconvert_library.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/need_help.rst` & `nbconvert-7.5.0/docs/source/need_help.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/removing_cells.rst` & `nbconvert-7.5.0/docs/source/removing_cells.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/usage.rst` & `nbconvert-7.5.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/_static/exporter_inheritance.png` & `nbconvert-7.5.0/docs/source/_static/exporter_inheritance.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/_static/preprocessor_inheritance.png` & `nbconvert-7.5.0/docs/source/_static/preprocessor_inheritance.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/_static/writer_inheritance.png` & `nbconvert-7.5.0/docs/source/_static/writer_inheritance.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/api/exporters.rst` & `nbconvert-7.5.0/docs/source/api/exporters.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/api/filters.rst` & `nbconvert-7.5.0/docs/source/api/filters.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/docs/source/api/preprocessors.rst` & `nbconvert-7.5.0/docs/source/api/preprocessors.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/nbconvertapp.py` & `nbconvert-7.5.0/nbconvert/nbconvertapp.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/__init__.py` & `nbconvert-7.5.0/nbconvert/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/asciidoc.py` & `nbconvert-7.5.0/nbconvert/exporters/asciidoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/base.py` & `nbconvert-7.5.0/nbconvert/exporters/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/exporter.py` & `nbconvert-7.5.0/nbconvert/exporters/exporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/html.py` & `nbconvert-7.5.0/nbconvert/exporters/html.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,14 +117,23 @@
         help="""
         URL to load Mathjax from.
 
         Defaults to loading from cdnjs.
         """,
     ).tag(config=True)
 
+    mermaid_js_url = Unicode(
+        "https://cdnjs.cloudflare.com/ajax/libs/mermaid/10.2.3/mermaid.esm.min.mjs",
+        help="""
+        URL to load MermaidJS from.
+
+        Defaults to loading from cdnjs.
+        """,
+    )
+
     jquery_url = Unicode(
         "https://cdnjs.cloudflare.com/ajax/libs/jquery/2.0.3/jquery.min.js",
         help="""
         URL to load jQuery from.
 
         Defaults to loading from cdnjs.
         """,
@@ -299,13 +308,14 @@
         resources["theme"] = self.theme
         resources["include_css"] = resources_include_css
         resources["include_lab_theme"] = resources_include_lab_theme
         resources["include_js"] = resources_include_js
         resources["include_url"] = resources_include_url
         resources["require_js_url"] = self.require_js_url
         resources["mathjax_url"] = self.mathjax_url
+        resources["mermaid_js_url"] = self.mermaid_js_url
         resources["jquery_url"] = self.jquery_url
         resources["jupyter_widgets_base_url"] = self.jupyter_widgets_base_url
         resources["widget_renderer_url"] = self.widget_renderer_url
         resources["html_manager_semver_range"] = self.html_manager_semver_range
         resources["should_sanitize_html"] = self.sanitize_html
         return resources
```

### Comparing `nbconvert-7.4.0/nbconvert/exporters/latex.py` & `nbconvert-7.5.0/nbconvert/exporters/latex.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """LaTeX Exporter class"""
 
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 
+import os
 
 from traitlets import default
 from traitlets.config import Config
 
 from nbconvert.filters.filter_links import resolve_references
 from nbconvert.filters.highlight import Highlight2Latex
+from nbconvert.filters.pandoc import ConvertExplicitlyRelativePaths
 
 from .templateexporter import TemplateExporter
 
 
 class LatexExporter(TemplateExporter):
     """
     Exports to a Latex template.  Inherit from this class if your template is
@@ -73,14 +75,24 @@
         langinfo = nb.metadata.get("language_info", {})
         lexer = langinfo.get("pygments_lexer", langinfo.get("name", None))
         highlight_code = self.filters.get(
             "highlight_code", Highlight2Latex(pygments_lexer=lexer, parent=self)
         )
         self.register_filter("highlight_code", highlight_code)
 
+        # Need to make sure explicit relative paths are visible to latex for pdf conversion
+        # https://github.com/jupyter/nbconvert/issues/1998
+        nb_path = resources.get("metadata", {}).get("path") if resources else None
+        texinputs = os.path.abspath(nb_path) if nb_path else os.getcwd()
+        convert_explicitly_relative_paths = self.filters.get(
+            "convert_explicitly_relative_paths",
+            ConvertExplicitlyRelativePaths(texinputs=texinputs, parent=self),
+        )
+        self.register_filter("convert_explicitly_relative_paths", convert_explicitly_relative_paths)
+
         return super().from_notebook_node(nb, resources, **kw)
 
     def _create_environment(self):
         environment = super()._create_environment()
 
         # Set special Jinja2 syntax that will not conflict with latex.
         environment.block_start_string = "((*"
```

### Comparing `nbconvert-7.4.0/nbconvert/exporters/markdown.py` & `nbconvert-7.5.0/nbconvert/exporters/markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/notebook.py` & `nbconvert-7.5.0/nbconvert/exporters/notebook.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/pdf.py` & `nbconvert-7.5.0/nbconvert/exporters/pdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         return self.run_command(self.bib_command, filename, 1, log_error, raise_on_failure)
 
     def from_notebook_node(self, nb, resources=None, **kw):
         """Convert from notebook node."""
         latex, resources = super().from_notebook_node(nb, resources=resources, **kw)
         # set texinputs directory, so that local files will be found
         if resources and resources.get("metadata", {}).get("path"):
-            self.texinputs = resources["metadata"]["path"]
+            self.texinputs = os.path.abspath(resources["metadata"]["path"])
         else:
             self.texinputs = os.getcwd()
 
         self._captured_outputs = []
         with TemporaryDirectory() as td, _contextlib_chdir.chdir(td):
             notebook_name = "notebook"
             resources["output_extension"] = ".tex"
```

### Comparing `nbconvert-7.4.0/nbconvert/exporters/python.py` & `nbconvert-7.5.0/nbconvert/exporters/python.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/qt_exporter.py` & `nbconvert-7.5.0/nbconvert/exporters/qt_exporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/qt_screenshot.py` & `nbconvert-7.5.0/nbconvert/exporters/qt_screenshot.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/qtpdf.py` & `nbconvert-7.5.0/nbconvert/exporters/qtpdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/rst.py` & `nbconvert-7.5.0/nbconvert/exporters/rst.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/script.py` & `nbconvert-7.5.0/nbconvert/exporters/script.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/slides.py` & `nbconvert-7.5.0/nbconvert/exporters/slides.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/templateexporter.py` & `nbconvert-7.5.0/nbconvert/exporters/templateexporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/webpdf.py` & `nbconvert-7.5.0/nbconvert/exporters/webpdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/base.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/cheese.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/cheese.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/test_asciidoc.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/test_asciidoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/test_export.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/test_exporter.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/test_html.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/test_latex.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/test_markdown.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/test_notebook.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/test_notebook.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/test_pdf.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/test_pdf.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Distributed under the terms of the Modified BSD License.
 
 import os
 import shutil
 from tempfile import TemporaryDirectory
 
 from ...tests.utils import onlyif_cmds_exist
+from ...utils import _contextlib_chdir
 from ..pdf import PDFExporter
 from .base import ExportersTestsBase
 
 # -----------------------------------------------------------------------------
 # Class
 # -----------------------------------------------------------------------------
 
@@ -35,7 +36,28 @@
             (output, resources) = self.exporter_class(latex_count=1).from_filename(  # type:ignore
                 newpath
             )
             self.assertIsInstance(output, bytes)
             assert len(output) > 0
             # all temporary file should be cleaned up
             assert {file_name} == set(os.listdir(td))
+
+    @onlyif_cmds_exist("xelatex", "pandoc")
+    def test_texinputs(self):
+        """
+        Is TEXINPUTS set properly when we are converting
+        - in the same directory, and
+        - in a different directory?
+        """
+        with TemporaryDirectory() as td, _contextlib_chdir.chdir(td):
+            os.mkdir("folder")
+            file_name = os.path.basename(self._get_notebook())
+            nb1 = os.path.join(td, file_name)
+            nb2 = os.path.join(td, "folder", file_name)
+            ex1 = self.exporter_class(latex_count=1)  # type:ignore
+            ex2 = self.exporter_class(latex_count=1)  # type:ignore
+            shutil.copy(self._get_notebook(), nb1)
+            shutil.copy(self._get_notebook(), nb2)
+            _ = ex1.from_filename(nb1)
+            _ = ex2.from_filename(nb2)
+            assert ex1.texinputs == os.path.abspath(".")
+            assert ex2.texinputs == os.path.abspath("./folder")
```

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/test_python.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/test_qtpdf.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/test_qtpdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/test_qtpng.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/test_qtpng.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/test_rst.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/test_rst.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/test_script.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/test_slides.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/test_slides.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/test_templateexporter.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/test_templateexporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/test_webpdf.py` & `nbconvert-7.5.0/nbconvert/exporters/tests/test_webpdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/files/attachment.ipynb` & `nbconvert-7.5.0/nbconvert/exporters/tests/files/attachment.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/files/notebook2.ipynb` & `nbconvert-7.5.0/nbconvert/exporters/tests/files/notebook2.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/files/notebook3.ipynb` & `nbconvert-7.5.0/nbconvert/exporters/tests/files/notebook3.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/files/notebook_inject.ipynb` & `nbconvert-7.5.0/nbconvert/exporters/tests/files/notebook_inject.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/files/pngmetadata.ipynb` & `nbconvert-7.5.0/nbconvert/exporters/tests/files/pngmetadata.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/files/prompt_numbers.ipynb` & `nbconvert-7.5.0/nbconvert/exporters/tests/files/prompt_numbers.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/files/rawtest.ipynb` & `nbconvert-7.5.0/nbconvert/exporters/tests/files/rawtest.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/exporters/tests/files/svg.ipynb` & `nbconvert-7.5.0/nbconvert/exporters/tests/files/svg.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/filters/ansi.py` & `nbconvert-7.5.0/nbconvert/filters/ansi.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/filters/citation.py` & `nbconvert-7.5.0/nbconvert/filters/citation.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/filters/datatypefilter.py` & `nbconvert-7.5.0/nbconvert/filters/datatypefilter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/filters/filter_links.py` & `nbconvert-7.5.0/nbconvert/filters/filter_links.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/filters/highlight.py` & `nbconvert-7.5.0/nbconvert/filters/highlight.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/filters/latex.py` & `nbconvert-7.5.0/nbconvert/filters/latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/filters/markdown.py` & `nbconvert-7.5.0/nbconvert/filters/markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/filters/markdown_mistune.py` & `nbconvert-7.5.0/nbconvert/filters/markdown_mistune.py`

 * *Files 8% similar despite different names*

```diff
@@ -172,28 +172,40 @@
         else:
             self.attachments = {}
 
     def block_code(self, code, info=None):
         """Handle block code."""
         lang = ""
         lexer = None
+
+        if info and info.startswith("mermaid"):
+            return self.block_mermaidjs(code)
+
         if info:
             try:
                 lang = info.strip().split(None, 1)[0]
                 lexer = get_lexer_by_name(lang, stripall=True)
             except ClassNotFound:
                 code = lang + "\n" + code
                 lang = None  # type:ignore
 
         if not lang:
             return super().block_code(code)
 
         formatter = HtmlFormatter()
         return highlight(code, lexer, formatter)
 
+    def block_mermaidjs(self, code, info=None):
+        """Handle mermaid syntax."""
+        return (
+            """<div class="jp-Mermaid"><pre class="mermaid">\n"""
+            f"""{code.strip()}"""
+            """\n</pre></div>"""
+        )
+
     def block_html(self, html):
         """Handle block html."""
         if self.embed_images:
             html = self._html_embed_images(html)
 
         return super().block_html(html)
```

### Comparing `nbconvert-7.4.0/nbconvert/filters/strings.py` & `nbconvert-7.5.0/nbconvert/filters/strings.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/filters/svg_constants.py` & `nbconvert-7.5.0/nbconvert/filters/svg_constants.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/filters/widgetsdatatypefilter.py` & `nbconvert-7.5.0/nbconvert/filters/widgetsdatatypefilter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/filters/tests/test_ansi.py` & `nbconvert-7.5.0/nbconvert/filters/tests/test_ansi.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/filters/tests/test_citation.py` & `nbconvert-7.5.0/nbconvert/filters/tests/test_citation.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/filters/tests/test_datatypefilter.py` & `nbconvert-7.5.0/nbconvert/filters/tests/test_datatypefilter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/filters/tests/test_highlight.py` & `nbconvert-7.5.0/nbconvert/filters/tests/test_highlight.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/filters/tests/test_latex.py` & `nbconvert-7.5.0/nbconvert/filters/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/filters/tests/test_markdown.py` & `nbconvert-7.5.0/nbconvert/filters/tests/test_markdown.py`

 * *Files 3% similar despite different names*

```diff
@@ -243,14 +243,27 @@
         for index, test in enumerate(self.tests):
             self._try_markdown(
                 partial(convert_pandoc, from_format="markdown", to_format="rst"),
                 test,
                 tokens[index],
             )
 
+    def test_mermaid_markdown(self):
+        code = """flowchart LR
+            chicken --> egg --> chicken"""
+        case = f"""```mermaid\n  {code}\n```"""
+
+        output_check = (
+            """<div class="jp-Mermaid"><pre class="mermaid">\n"""
+            f"""{code.strip()}"""
+            """\n</pre></div>"""
+        )
+
+        self._try_markdown(markdown2html, case, output_check)
+
     def _try_markdown(self, method, test, tokens):
         results = method(test)
         if isinstance(tokens, (str,)):
             self.assertIn(tokens, results)
         else:
             for token in tokens:
                 self.assertIn(token, results)
```

### Comparing `nbconvert-7.4.0/nbconvert/filters/tests/test_metadata.py` & `nbconvert-7.5.0/nbconvert/filters/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/filters/tests/test_strings.py` & `nbconvert-7.5.0/nbconvert/filters/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/postprocessors/base.py` & `nbconvert-7.5.0/nbconvert/postprocessors/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/postprocessors/serve.py` & `nbconvert-7.5.0/nbconvert/postprocessors/serve.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/postprocessors/tests/test_serve.py` & `nbconvert-7.5.0/nbconvert/postprocessors/tests/test_serve.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/__init__.py` & `nbconvert-7.5.0/nbconvert/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/base.py` & `nbconvert-7.5.0/nbconvert/preprocessors/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/clearmetadata.py` & `nbconvert-7.5.0/nbconvert/preprocessors/clearmetadata.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/clearoutput.py` & `nbconvert-7.5.0/nbconvert/preprocessors/clearoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/coalescestreams.py` & `nbconvert-7.5.0/nbconvert/preprocessors/coalescestreams.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/convertfigures.py` & `nbconvert-7.5.0/nbconvert/preprocessors/convertfigures.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/csshtmlheader.py` & `nbconvert-7.5.0/nbconvert/preprocessors/csshtmlheader.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/execute.py` & `nbconvert-7.5.0/nbconvert/preprocessors/execute.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/extractattachments.py` & `nbconvert-7.5.0/nbconvert/preprocessors/extractattachments.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/extractoutput.py` & `nbconvert-7.5.0/nbconvert/preprocessors/extractoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/highlightmagics.py` & `nbconvert-7.5.0/nbconvert/preprocessors/highlightmagics.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/latex.py` & `nbconvert-7.5.0/nbconvert/preprocessors/latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/regexremove.py` & `nbconvert-7.5.0/nbconvert/preprocessors/regexremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/sanitize.py` & `nbconvert-7.5.0/nbconvert/preprocessors/sanitize.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/svg2pdf.py` & `nbconvert-7.5.0/nbconvert/preprocessors/svg2pdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/tagremove.py` & `nbconvert-7.5.0/nbconvert/preprocessors/tagremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/tests/base.py` & `nbconvert-7.5.0/nbconvert/preprocessors/tests/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/tests/fake_kernelmanager.py` & `nbconvert-7.5.0/nbconvert/preprocessors/tests/fake_kernelmanager.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_clearmetadata.py` & `nbconvert-7.5.0/nbconvert/preprocessors/tests/test_clearmetadata.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_clearoutput.py` & `nbconvert-7.5.0/nbconvert/preprocessors/tests/test_clearoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_coalescestreams.py` & `nbconvert-7.5.0/nbconvert/preprocessors/tests/test_coalescestreams.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_csshtmlheader.py` & `nbconvert-7.5.0/nbconvert/preprocessors/tests/test_csshtmlheader.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_execute.py` & `nbconvert-7.5.0/nbconvert/preprocessors/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_extractattachments.py` & `nbconvert-7.5.0/nbconvert/preprocessors/tests/test_extractattachments.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_extractoutput.py` & `nbconvert-7.5.0/nbconvert/preprocessors/tests/test_extractoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_highlightmagics.py` & `nbconvert-7.5.0/nbconvert/preprocessors/tests/test_highlightmagics.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_latex.py` & `nbconvert-7.5.0/nbconvert/preprocessors/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_regexremove.py` & `nbconvert-7.5.0/nbconvert/preprocessors/tests/test_regexremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_sanitize.py` & `nbconvert-7.5.0/nbconvert/preprocessors/tests/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_svg2pdf.py` & `nbconvert-7.5.0/nbconvert/preprocessors/tests/test_svg2pdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/tests/test_tagremove.py` & `nbconvert-7.5.0/nbconvert/preprocessors/tests/test_tagremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb` & `nbconvert-7.5.0/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/templates/skeleton/Makefile` & `nbconvert-7.5.0/nbconvert/templates/skeleton/Makefile`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/tests/base.py` & `nbconvert-7.5.0/nbconvert/tests/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/tests/fake_exporters.py` & `nbconvert-7.5.0/nbconvert/tests/fake_exporters.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/tests/test_nbconvertapp.py` & `nbconvert-7.5.0/nbconvert/tests/test_nbconvertapp.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/tests/files/Unexecuted_widget.ipynb` & `nbconvert-7.5.0/nbconvert/tests/files/Unexecuted_widget.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/tests/files/Unexecuted_widget_2.ipynb` & `nbconvert-7.5.0/nbconvert/tests/files/Unexecuted_widget_2.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/tests/files/Widget_List.ipynb` & `nbconvert-7.5.0/nbconvert/tests/files/Widget_List.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/tests/files/containerized_deployments.jpeg` & `nbconvert-7.5.0/nbconvert/tests/files/containerized_deployments.jpeg`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/tests/files/issue1849_svg.ipynb` & `nbconvert-7.5.0/nbconvert/tests/files/issue1849_svg.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/tests/files/latex-linked-image.ipynb` & `nbconvert-7.5.0/nbconvert/tests/files/latex-linked-image.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/tests/files/markdown_display_priority.ipynb` & `nbconvert-7.5.0/nbconvert/tests/files/markdown_display_priority.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/tests/files/notebook1.ipynb` & `nbconvert-7.5.0/nbconvert/tests/files/notebook1.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/tests/files/notebook2.ipynb` & `nbconvert-7.5.0/nbconvert/tests/files/notebook2.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/tests/files/notebook3_with_errors.ipynb` & `nbconvert-7.5.0/nbconvert/tests/files/notebook3_with_errors.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/tests/files/notebook4_jpeg.ipynb` & `nbconvert-7.5.0/nbconvert/tests/files/notebook4_jpeg.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/tests/files/notebook5_embed_images.ipynb` & `nbconvert-7.5.0/nbconvert/tests/files/notebook5_embed_images.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/tests/files/notebook_tags.ipynb` & `nbconvert-7.5.0/nbconvert/tests/files/notebook_tags.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/tests/files/testimage.png` & `nbconvert-7.5.0/nbconvert/tests/files/testimage.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/utils/_contextlib_chdir.py` & `nbconvert-7.5.0/nbconvert/utils/_contextlib_chdir.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/utils/base.py` & `nbconvert-7.5.0/nbconvert/utils/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/utils/exceptions.py` & `nbconvert-7.5.0/nbconvert/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/utils/io.py` & `nbconvert-7.5.0/nbconvert/utils/io.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/utils/pandoc.py` & `nbconvert-7.5.0/nbconvert/utils/pandoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import warnings
 from io import BytesIO, TextIOWrapper
 
 from nbconvert.utils.version import check_version
 
 from .exceptions import ConversionException
 
-_minimal_version = "1.12.1"
-_maximal_version = "3.0.0"
+_minimal_version = "2.14.2"
+_maximal_version = "4.0.0"
 
 
 def pandoc(source, fmt, to, extra_args=None, encoding="utf-8"):
     """Convert an input string using pandoc.
 
     Pandoc converts an input string `from` a format `to` a target format.
```

### Comparing `nbconvert-7.4.0/nbconvert/utils/text.py` & `nbconvert-7.5.0/nbconvert/utils/text.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/utils/version.py` & `nbconvert-7.5.0/nbconvert/utils/version.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/utils/tests/test_io.py` & `nbconvert-7.5.0/nbconvert/utils/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/utils/tests/test_pandoc.py` & `nbconvert-7.5.0/nbconvert/utils/tests/test_pandoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/writers/base.py` & `nbconvert-7.5.0/nbconvert/writers/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/writers/debug.py` & `nbconvert-7.5.0/nbconvert/writers/debug.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/writers/files.py` & `nbconvert-7.5.0/nbconvert/writers/files.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/writers/stdout.py` & `nbconvert-7.5.0/nbconvert/writers/stdout.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/writers/tests/test_debug.py` & `nbconvert-7.5.0/nbconvert/writers/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/writers/tests/test_files.py` & `nbconvert-7.5.0/nbconvert/writers/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/nbconvert/writers/tests/test_stdout.py` & `nbconvert-7.5.0/nbconvert/writers/tests/test_stdout.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/asciidoc/index.asciidoc.j2` & `nbconvert-7.5.0/share/templates/asciidoc/index.asciidoc.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/base/display_priority.j2` & `nbconvert-7.5.0/share/templates/base/display_priority.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/base/jupyter_widgets.html.j2` & `nbconvert-7.5.0/share/templates/base/jupyter_widgets.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/base/mathjax.html.j2` & `nbconvert-7.5.0/share/templates/base/mathjax.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/base/null.j2` & `nbconvert-7.5.0/share/templates/base/null.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/classic/base.html.j2` & `nbconvert-7.5.0/share/templates/classic/base.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/classic/index.html.j2` & `nbconvert-7.5.0/share/templates/classic/index.html.j2`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 {%- block html_head_js -%}
 {%- block html_head_js_jquery -%}
 <script src="{{ resources.jquery_url }}"></script>
 {%- endblock html_head_js_jquery -%}
 {%- block html_head_js_requirejs -%}
 <script src="{{ resources.require_js_url }}"></script>
 {%- endblock html_head_js_requirejs -%}
+{%- block html_head_js_mermaidjs -%}
+<script type="module">
+  import mermaid from '{{ resources.mermaid_js_url }}';
+  mermaid.initialize({ startOnLoad: true });
+</script>
+{%- endblock html_head_js_mermaidjs -%}
 {%- endblock html_head_js -%}
 
 {% block jupyter_widgets %}
   {%- if "widgets" in nb.metadata -%}
     {{ jupyter_widgets(resources.jupyter_widgets_base_url, resources.html_manager_semver_range, resources.widget_renderer_url) }}
   {%- endif -%}
 {% endblock jupyter_widgets %}
```

#### html2text {}

```diff
@@ -2,15 +2,16 @@
 from 'jupyter_widgets.html.j2' import jupyter_widgets %} {%- block header -%}
 {%- block html_head -%}
 
  {% set nb_title = nb.metadata.get('title', resources['metadata']['name']) |
 escape_html_keep_quotes %}
 {%- block html_head_js -%} {%- block html_head_js_jquery -%}
  {%- endblock html_head_js_jquery -%} {%- block html_head_js_requirejs -%}
- {%- endblock html_head_js_requirejs -%} {%- endblock html_head_js -%} {% block
+ {%- endblock html_head_js_requirejs -%} {%- block html_head_js_mermaidjs -%}
+ {%- endblock html_head_js_mermaidjs -%} {%- endblock html_head_js -%} {% block
 jupyter_widgets %} {%- if "widgets" in nb.metadata -%} {{ jupyter_widgets
 (resources.jupyter_widgets_base_url, resources.html_manager_semver_range,
 resources.widget_renderer_url) }} {%- endif -%} {% endblock jupyter_widgets %}
 {% for css in resources.inlining.css -%}
  {% endfor %} {% block notebook_css %} {{ resources.include_css("static/
 style.css") }}
  {% endblock notebook_css %} {%- block html_head_js_mathjax -%} {{ mathjax
```

### Comparing `nbconvert-7.4.0/share/templates/classic/static/style.css` & `nbconvert-7.5.0/share/templates/classic/static/style.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/lab/base.html.j2` & `nbconvert-7.5.0/share/templates/lab/base.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/lab/index.html.j2` & `nbconvert-7.5.0/share/templates/lab/index.html.j2`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 {%- extends 'base.html.j2' -%}
 {% from 'mathjax.html.j2' import mathjax %}
+{% from 'mermaidjs.html.j2' import mermaid_js %}
 {% from 'jupyter_widgets.html.j2' import jupyter_widgets %}
 
 {%- block header -%}
 <!DOCTYPE html>
 <html>
 <head>
 {%- block html_head -%}
@@ -145,14 +146,18 @@
 
 {% endblock notebook_css %}
 
 {%- block html_head_js_mathjax -%}
 {{ mathjax(resources.mathjax_url) }}
 {%- endblock html_head_js_mathjax -%}
 
+{%- block html_head_js_mermaidjs -%}
+{{ mermaid_js(resources.mermaid_js_url) }}
+{%- endblock html_head_js_mermaidjs -%}
+
 {%- block html_head_css -%}
 {%- endblock html_head_css -%}
 
 {%- endblock html_head -%}
 </head>
 {%- endblock header -%}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {%- extends 'base.html.j2' -%} {% from 'mathjax.html.j2' import mathjax %} {%
-from 'jupyter_widgets.html.j2' import jupyter_widgets %} {%- block header -%}
+from 'mermaidjs.html.j2' import mermaid_js %} {% from 'jupyter_widgets.html.j2'
+import jupyter_widgets %} {%- block header -%}
 {%- block html_head -%}
 
  {% set nb_title = nb.metadata.get('title', resources['metadata']['name']) |
 escape_html_keep_quotes %}
 {%- block html_head_js -%} {%- block html_head_js_requirejs -%}
  {%- endblock html_head_js_requirejs -%} {%- endblock html_head_js -%} {% block
 jupyter_widgets %} {%- if "widgets" in nb.metadata -%} {{ jupyter_widgets
@@ -14,15 +15,17 @@
  {% endfor %} {% block notebook_css %} {{ resources.include_css("static/
 index.css") }} {% if resources.theme == 'dark' %} {{ resources.include_css
 ("static/theme-dark.css") }} {% elif resources.theme == 'light' %} {
 { resources.include_css("static/theme-light.css") }} {% else %} {
 { resources.include_lab_theme(resources.theme) }} {% endif %}
  {% endblock notebook_css %} {%- block html_head_js_mathjax -%} {{ mathjax
 (resources.mathjax_url) }} {%- endblock html_head_js_mathjax -%} {%- block
-html_head_css -%} {%- endblock html_head_css -%} {%- endblock html_head -%}
+html_head_js_mermaidjs -%} {{ mermaid_js(resources.mermaid_js_url) }} {%-
+endblock html_head_js_mermaidjs -%} {%- block html_head_css -%} {%- endblock
+html_head_css -%} {%- endblock html_head -%}
 {%- endblock header -%} {%- block body_header -%} {% if resources.theme ==
 'dark' %}
 {% else %}
 {% endif %} {%- endblock body_header -%} {% block body_footer %}
 {% endblock body_footer %} {% block footer %} {% block footer_js %} {% endblock
 footer_js %} {{ super() }}
 {% endblock footer %}
```

### Comparing `nbconvert-7.4.0/share/templates/lab/static/index.css` & `nbconvert-7.5.0/share/templates/lab/static/index.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/lab/static/theme-dark.css` & `nbconvert-7.5.0/share/templates/lab/static/theme-dark.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/lab/static/theme-light.css` & `nbconvert-7.5.0/share/templates/lab/static/theme-light.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/latex/base.tex.j2` & `nbconvert-7.5.0/share/templates/latex/base.tex.j2`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
     \usepackage{longtable} % longtable support required by pandoc >1.10
     \usepackage{booktabs}  % table support for pandoc > 1.12.2
     \usepackage{array}     % table support for pandoc >= 2.11.3
     \usepackage{calc}      % table minipage width calculation for pandoc >= 2.11.1
     \usepackage[inline]{enumitem} % IRkernel/repr support (it uses the enumerate* environment)
     \usepackage[normalem]{ulem} % ulem is needed to support strikethroughs (\sout)
                                 % normalem makes italics be italics, not underlines
+    \usepackage{soul}      % strikethrough (\st) support for pandoc >= 3.0.0
     \usepackage{mathrsfs}
     ((* endblock packages *))
 
     ((* block definitions *))
     % Colors for the hyperref package
     \definecolor{urlcolor}{rgb}{0,.145,.698}
     \definecolor{linkcolor}{rgb}{.71,0.21,0.01}
```

### Comparing `nbconvert-7.4.0/share/templates/latex/display_priority.j2` & `nbconvert-7.5.0/share/templates/latex/display_priority.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/latex/document_contents.tex.j2` & `nbconvert-7.5.0/share/templates/latex/document_contents.tex.j2`

 * *Files 5% similar despite different names*

```diff
@@ -61,13 +61,13 @@
     ((* block data_priority scoped *))
     ((( super() )))
     ((* endblock *))
 ((* endblock execute_result *))
 
 % Render markdown
 ((* block markdowncell scoped *))
-    ((( cell.source | citation2latex | strip_files_prefix | convert_pandoc('markdown+tex_math_double_backslash', 'json',extra_args=[]) | resolve_references | convert_pandoc('json','latex'))))
+    ((( cell.source | citation2latex | strip_files_prefix | convert_pandoc('markdown+tex_math_double_backslash', 'json',extra_args=[]) | resolve_references | convert_explicitly_relative_paths | convert_pandoc('json','latex'))))
 ((* endblock markdowncell *))
 
 % Don't display unknown types
 ((* block unknowncell scoped *))
 ((* endblock unknowncell *))
```

### Comparing `nbconvert-7.4.0/share/templates/latex/null.j2` & `nbconvert-7.5.0/share/templates/latex/null.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/latex/report.tex.j2` & `nbconvert-7.5.0/share/templates/latex/report.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/latex/style_bw_ipython.tex.j2` & `nbconvert-7.5.0/share/templates/latex/style_bw_ipython.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/latex/style_ipython.tex.j2` & `nbconvert-7.5.0/share/templates/latex/style_ipython.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/latex/style_jupyter.tex.j2` & `nbconvert-7.5.0/share/templates/latex/style_jupyter.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/latex/style_python.tex.j2` & `nbconvert-7.5.0/share/templates/latex/style_python.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/markdown/index.md.j2` & `nbconvert-7.5.0/share/templates/markdown/index.md.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/reveal/base.html.j2` & `nbconvert-7.5.0/share/templates/reveal/base.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/reveal/index.html.j2` & `nbconvert-7.5.0/share/templates/reveal/index.html.j2`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,20 @@
 {%- block html_head_js -%}
 {%- block html_head_js_jquery -%}
 <script src="{{ resources.jquery_url }}"></script>
 {%- endblock html_head_js_jquery -%}
 {%- block html_head_js_requirejs -%}
 <script src="{{ resources.require_js_url }}"></script>
 {%- endblock html_head_js_requirejs -%}
+{%- block html_head_js_mermaidjs -%}
+<script type="module">
+  import mermaid from '{{ resources.mermaid_js_url }}';
+  mermaid.initialize({ startOnLoad: true });
+</script>
+{%- endblock html_head_js_mermaidjs -%}
 {%- endblock html_head_js -%}
 
 {% block jupyter_widgets %}
   {%- if "widgets" in nb.metadata -%}
     {{ jupyter_widgets(resources.jupyter_widgets_base_url, resources.html_manager_semver_range, resources.widget_renderer_url) }}
   {%- endif -%}
 {% endblock jupyter_widgets %}
```

### Comparing `nbconvert-7.4.0/share/templates/reveal/static/custom_reveal.css` & `nbconvert-7.5.0/share/templates/reveal/static/custom_reveal.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/share/templates/rst/index.rst.j2` & `nbconvert-7.5.0/share/templates/rst/index.rst.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/.gitignore` & `nbconvert-7.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/LICENSE` & `nbconvert-7.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/README.md` & `nbconvert-7.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/hatch_build.py` & `nbconvert-7.5.0/hatch_build.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.4.0/pyproject.toml` & `nbconvert-7.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,29 +17,29 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 urls = {Homepage = "https://jupyter.org"}
 requires-python = ">=3.7"
 dependencies = [
     "beautifulsoup4",
-    "bleach",
+    "bleach!=5.0.0",
     "defusedxml",
     "importlib_metadata>=3.6;python_version<\"3.10\"",
     "jinja2>=3.0",
     "jupyter_core>=4.7",
     "jupyterlab_pygments",
     "MarkupSafe>=2.0",
     "mistune>=2.0.3,<3",
     "nbclient>=0.5.0",
-    "nbformat>=5.1",
+    "nbformat>=5.7",
     "packaging",
     "pandocfilters>=1.4.1",
     "pygments>=2.4.1",
     "tinycss2",
-    "traitlets>=5.0",
+    "traitlets>=5.1",
 ]
 dynamic = ["version"]
 
 [project.entry-points."nbconvert.exporters"]
 custom = "nbconvert.exporters:TemplateExporter"
 html = "nbconvert.exporters:HTMLExporter"
 slides = "nbconvert.exporters:SlidesExporter"
@@ -125,15 +125,15 @@
 test = "mypy --install-types --non-interactive {args:nbconvert}"
 
 [tool.hatch.envs.lint]
 dependencies = [
   "black[jupyter]==23.3.0",
   "mdformat>0.7",
   "mdformat-gfm>=0.3.5",
-  "ruff==0.0.263"
+  "ruff==0.0.270"
 ]
 detached = true
 [tool.hatch.envs.lint.scripts]
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
   "mdformat --check {args:docs *.md}"
```

### Comparing `nbconvert-7.4.0/PKG-INFO` & `nbconvert-7.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbconvert
-Version: 7.4.0
+Version: 7.5.0
 Summary: Converting Jupyter Notebooks
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
         - Copyright (c) 2001-2015, IPython Development Team
         - Copyright (c) 2015-, Jupyter Development Team
@@ -41,29 +41,29 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: beautifulsoup4
-Requires-Dist: bleach
+Requires-Dist: bleach!=5.0.0
 Requires-Dist: defusedxml
 Requires-Dist: importlib-metadata>=3.6; python_version < '3.10'
 Requires-Dist: jinja2>=3.0
 Requires-Dist: jupyter-core>=4.7
 Requires-Dist: jupyterlab-pygments
 Requires-Dist: markupsafe>=2.0
 Requires-Dist: mistune<3,>=2.0.3
 Requires-Dist: nbclient>=0.5.0
-Requires-Dist: nbformat>=5.1
+Requires-Dist: nbformat>=5.7
 Requires-Dist: packaging
 Requires-Dist: pandocfilters>=1.4.1
 Requires-Dist: pygments>=2.4.1
 Requires-Dist: tinycss2
-Requires-Dist: traitlets>=5.0
+Requires-Dist: traitlets>=5.1
 Provides-Extra: all
 Requires-Dist: nbconvert[docs,qtpdf,serve,test,webpdf]; extra == 'all'
 Provides-Extra: docs
 Requires-Dist: ipykernel; extra == 'docs'
 Requires-Dist: ipython; extra == 'docs'
 Requires-Dist: myst-parser; extra == 'docs'
 Requires-Dist: nbsphinx>=0.2.12; extra == 'docs'
```

