# Comparing `tmp/sparrow_python-0.1.3.tar.gz` & `tmp/sparrow_python-0.1.4.tar.gz`

## Comparing `sparrow_python-0.1.3.tar` & `sparrow_python-0.1.4.tar`

### file list

```diff
@@ -1,185 +1,170 @@
--rwxr-xr-x   0        0        0      319 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/__init__.py
--rwxr-xr-x   0        0        0     2794 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/__main__.py
--rwxr-xr-x   0        0        0     2094 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/constant.py
--rwxr-xr-x   0        0        0     3379 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/core.py
--rwxr-xr-x   0        0        0     2540 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/version_ops.py
--rwxr-xr-x   0        0        0     1886 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/algorithm/__init__.py
--rwxr-xr-x   0        0        0     3041 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/algorithm/bktree.py
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/__init__.py
--rwxr-xr-x   0        0        0     2981 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/common.py
--rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/8dbd28457ff989b4568a.worker.js.LICENSE.txt
--rwxr-xr-x   0        0        0   149804 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/8dbd28457ff989b4568a.worker.js.map
--rwxr-xr-x   0        0        0      665 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/favicon-16x16.png
--rwxr-xr-x   0        0        0      628 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/favicon-32x32.png
--rwxr-xr-x   0        0        0     7915 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/icon-yuanian.png
--rwxr-xr-x   0        0        0    21806 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/icon.png
--rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/index.css
--rwxr-xr-x   0        0        0      734 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/index.html
--rwxr-xr-x   0        0        0     2690 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/oauth2-redirect.html
--rwxr-xr-x   0        0        0   308284 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/redoc.browser.lib.js
--rwxr-xr-x   0        0        0      210 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/redoc.browser.lib.js.LICENSE.txt
--rwxr-xr-x   0        0        0   899160 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/redoc.browser.lib.js.map
--rwxr-xr-x   0        0        0   304247 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/redoc.lib.js
--rwxr-xr-x   0        0        0      210 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/redoc.lib.js.LICENSE.txt
--rwxr-xr-x   0        0        0   875218 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/redoc.lib.js.map
--rwxr-xr-x   0        0        0  1031563 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/redoc.standalone.js
--rwxr-xr-x   0        0        0     2634 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/redoc.standalone.js.LICENSE.txt
--rwxr-xr-x   0        0        0  3654569 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/redoc.standalone.js.map
--rwxr-xr-x   0        0        0      539 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/swagger-initializer.js
--rwxr-xr-x   0        0        0  1096223 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/swagger-ui-bundle.js
--rwxr-xr-x   0        0        0  1543454 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/swagger-ui-bundle.js.map
--rwxr-xr-x   0        0        0   406499 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/swagger-ui-es-bundle-core.js
--rwxr-xr-x   0        0        0  1271743 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/swagger-ui-es-bundle-core.js.map
--rwxr-xr-x   0        0        0  1095985 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/swagger-ui-es-bundle.js
--rwxr-xr-x   0        0        0  1537354 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/swagger-ui-es-bundle.js.map
--rwxr-xr-x   0        0        0   339540 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/swagger-ui-standalone-preset.js
--rwxr-xr-x   0        0        0   530266 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/swagger-ui-standalone-preset.js.map
--rwxr-xr-x   0        0        0   143980 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/swagger-ui.css
--rwxr-xr-x   0        0        0   276303 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/swagger-ui.css.map
--rwxr-xr-x   0        0        0   286743 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/swagger-ui.js
--rwxr-xr-x   0        0        0   302894 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/api/static/swagger-ui.js.map
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/cli/__init__.py
--rwxr-xr-x   0        0        0      881 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/cli/core.py
--rwxr-xr-x   0        0        0     1226 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/cli/demo.py
--rwxr-xr-x   0        0        0     2934 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/cli/downloader.py
--rwxr-xr-x   0        0        0     1334 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/cli/git.py
--rwxr-xr-x   0        0        0      972 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/cli/script.py
--rwxr-xr-x   0        0        0     1780 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/cli/tree.py
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/color/__init__.py
--rwxr-xr-x   0        0        0     1763 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/color/color.py
--rwxr-xr-x   0        0        0     3821 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/color/constant.py
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/cv/__init__.py
--rwxr-xr-x   0        0        0     1364 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/cv/utils.py
--rwxr-xr-x   0        0        0       35 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/datasets/__init__.py
--rwxr-xr-x   0        0        0     1394 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/datasets/fake_data.py
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/debug/__init__.py
--rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/decorators/__init__.py
--rwxr-xr-x   0        0        0     7648 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/decorators/core.py
--rwxr-xr-x   0        0        0       25 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/distance/__init__.py
--rwxr-xr-x   0        0        0     1014 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/distance/distance.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/doc/__init__.py
--rwxr-xr-x   0        0        0     3486 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/docker/__init__.py
--rwxr-xr-x   0        0        0     6595 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/docker/nvidia_stat.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/flow/__init__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/flow/executor1/__init__.py
--rwxr-xr-x   0        0        0     1655 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/flow/executor1/executor.py
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/functions/__init__.py
--rwxr-xr-x   0        0        0      302 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/functions/bezier.py
--rwxr-xr-x   0        0        0     2969 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/functions/core.py
--rwxr-xr-x   0        0        0     2116 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/functions/rate_function.py
--rwxr-xr-x   0        0        0     1445 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/functions/utils.py
--rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/inspect/__init__.py
--rwxr-xr-x   0        0        0      746 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/inspect/core.py
--rwxr-xr-x   0        0        0      903 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/io/__init__.py
--rwxr-xr-x   0        0        0      811 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/io/core.py
--rwxr-xr-x   0        0        0     2152 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/io/ops.py
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/jupyter/__init__.py
--rwxr-xr-x   0        0        0     1241 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/jupyter/utils/__init__.py
--rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/log/__init__.py
--rwxr-xr-x   0        0        0     9759 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/log/core.py
--rwxr-xr-x   0        0        0     2101 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/log/setup.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/math/__init__.py
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/math/algebra.py
--rwxr-xr-x   0        0        0     1297 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/math/common.py
--rwxr-xr-x   0        0        0     3126 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/math/geometry.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/math/probability.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/math/sampling/__init__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/micrograd/__init__.py
--rwxr-xr-x   0        0        0     2753 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/micrograd/engine.py
--rwxr-xr-x   0        0        0     1633 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/micrograd/nn.py
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/models/__init__.py
--rwxr-xr-x   0        0        0     1304 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/multiprocess/__init__.py
--rwxr-xr-x   0        0        0     2178 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/multiprocess/client.py
--rwxr-xr-x   0        0        0      215 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/multiprocess/config.py
--rwxr-xr-x   0        0        0     2238 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/multiprocess/kill_pid.py
--rwxr-xr-x   0        0        0     1523 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/multiprocess/server.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/multiprocess/mq/__init__.py
--rwxr-xr-x   0        0        0      768 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/multiprocess/mq/client.py
--rwxr-xr-x   0        0        0      668 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/multiprocess/mq/server.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/nlp/__init__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/nlp/app.py
--rwxr-xr-x   0        0        0     2083 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/nlp/doc.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/nlp/uie.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/nn/__init__.py
--rwxr-xr-x   0        0        0     6359 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/nn/activations.py
--rwxr-xr-x   0        0        0     6153 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/nn/attention.py
--rwxr-xr-x   0        0        0     1708 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/nn/losses.py
--rwxr-xr-x   0        0        0     7849 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/nn/model.py
--rwxr-xr-x   0        0        0     4356 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/nn/transformer.py
--rwxr-xr-x   0        0        0      917 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/nn/utils.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/nn/jax/__init__.py
--rwxr-xr-x   0        0        0     1609 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/nn/jax/local_attention.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/nn/torch/__init__.py
--rwxr-xr-x   0        0        0     2800 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/nn/torch/utils.py
--rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/path/__init__.py
--rwxr-xr-x   0        0        0     1669 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/path/core.py
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/performance/__init__.py
--rwxr-xr-x   0        0        0     1380 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/performance/_measure_time.py
--rwxr-xr-x   0        0        0      590 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/performance/_record_memory.py
--rwxr-xr-x   0        0        0     2370 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/performance/_stat_memory.py
--rwxr-xr-x   0        0        0     3480 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/performance/stat.py
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/progress_bar/__init__.py
--rwxr-xr-x   0        0        0     5547 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/progress_bar/bar.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/proto/__init__.py
--rwxr-xr-x   0        0        0     2631 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/proto/build-proto.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/proto/python/__init__.py
--rwxr-xr-x   0        0        0     2540 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/proto/python/coordinate_pb2.py
--rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/proto/python/coordinate_pb2_grpc.py
--rwxr-xr-x   0        0        0     3490 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/proto/python/sparray_pb2.py
--rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/proto/python/sparray_pb2_grpc.py
--rwxr-xr-x   0        0        0     1970 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/proto/python/trainstatus_pb2.py
--rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/proto/python/trainstatus_pb2_grpc.py
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/string/__init__.py
--rwxr-xr-x   0        0        0     1671 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/string/color_string.py
--rwxr-xr-x   0        0        0     1759 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/string/ops.py
--rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/table_ops/__init__.py
--rwxr-xr-x   0        0        0     3600 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/table_ops/core.py
--rwxr-xr-x   0        0        0       47 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/__init__.py
--rwxr-xr-x   0        0        0     4205 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/core.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/__init__.py
--rwxr-xr-x   0        0        0      949 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/core.py
--rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/.dockerignore
--rwxr-xr-x   0        0        0     1948 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/.gitignore
--rwxr-xr-x   0        0        0     1868 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/CODE_OF_CONDUCT.md
--rwxr-xr-x   0        0        0     1705 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/REAMEME.md
--rwxr-xr-x   0        0        0     1704 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/REAMEME_ZH.md
--rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/main.py
--rwxr-xr-x   0        0        0      964 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/pyproject.toml
--rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/pytest.ini
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/start_entrypoint.sh
--rwxr-xr-x   0        0        0     1350 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/.github/workflows/docker-publish.yml
--rwxr-xr-x   0        0        0      824 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/.github/workflows/gh-release.yml
--rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/.github/workflows/python-publish.yml
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/Examples/debug.py
--rwxr-xr-x   0        0        0     1220 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/conf/logging.yaml
--rwxr-xr-x   0        0        0      627 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/conf/uvicorn.log.yaml
--rwxr-xr-x   0        0        0      602 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/docker/Dockerfile
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/log/debug.log
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/log/info.log
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/project_name/__init__.py
--rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/project_name/__main__.py
--rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/project_name/api/__init__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/project_name/api/schemas.py
--rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/project_name/api/routes/__init__.py
--rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/project_name/api/routes/index.py
--rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/template/scaffold/src/tests/conftest.py
--rwxr-xr-x   0        0        0       25 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/transform/__init__.py
--rwxr-xr-x   0        0        0      509 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/transform/hilbert.py
--rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/transform/transform.py
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/trie/__init__.py
--rwxr-xr-x   0        0        0     7363 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/trie/trie.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/utils/__init__.py
--rwxr-xr-x   0        0        0     2015 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/utils/compress.py
--rwxr-xr-x   0        0        0     2429 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/utils/core.py
--rwxr-xr-x   0        0        0     4034 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/utils/cursor.py
--rwxr-xr-x   0        0        0     1830 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/utils/net.py
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/utils/time.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/web/__init__.py
--rwxr-xr-x   0        0        0     1548 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/web/share_page.py
--rwxr-xr-x   0        0        0     1020 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/sparrow/widgets/__init__.py
--rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/.gitignore
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/AUTHORS
--rwxr-xr-x   0        0        0     1064 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/LICENSE
--rwxr-xr-x   0        0        0     2089 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/README.md
--rwxr-xr-x   0        0        0     3274 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 sparrow_python-0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0      319 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/__init__.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/__main__.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/constant.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/core.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/version_ops.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/__init__.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/common.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/8dbd28457ff989b4568a.worker.js.LICENSE.txt
+-rw-r--r--   0        0        0   149804 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/8dbd28457ff989b4568a.worker.js.map
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/favicon-16x16.png
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/favicon-32x32.png
+-rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/icon-yuanian.png
+-rw-r--r--   0        0        0    21806 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/icon.png
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/index.css
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/index.html
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/oauth2-redirect.html
+-rw-r--r--   0        0        0   308284 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/redoc.browser.lib.js
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/redoc.browser.lib.js.LICENSE.txt
+-rw-r--r--   0        0        0   899160 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/redoc.browser.lib.js.map
+-rw-r--r--   0        0        0   304247 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/redoc.lib.js
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/redoc.lib.js.LICENSE.txt
+-rw-r--r--   0        0        0   875218 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/redoc.lib.js.map
+-rw-r--r--   0        0        0  1031563 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/redoc.standalone.js
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/redoc.standalone.js.LICENSE.txt
+-rw-r--r--   0        0        0  3654569 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/redoc.standalone.js.map
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/swagger-initializer.js
+-rw-r--r--   0        0        0  1096223 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/swagger-ui-bundle.js
+-rw-r--r--   0        0        0  1543454 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/swagger-ui-bundle.js.map
+-rw-r--r--   0        0        0   406499 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/swagger-ui-es-bundle-core.js
+-rw-r--r--   0        0        0  1271743 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/swagger-ui-es-bundle-core.js.map
+-rw-r--r--   0        0        0  1095985 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/swagger-ui-es-bundle.js
+-rw-r--r--   0        0        0  1537354 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/swagger-ui-es-bundle.js.map
+-rw-r--r--   0        0        0   339540 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/swagger-ui-standalone-preset.js
+-rw-r--r--   0        0        0   530266 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/swagger-ui-standalone-preset.js.map
+-rw-r--r--   0        0        0   143980 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/swagger-ui.css
+-rw-r--r--   0        0        0   276303 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/swagger-ui.css.map
+-rw-r--r--   0        0        0   286743 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/swagger-ui.js
+-rw-r--r--   0        0        0   302894 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/api/static/swagger-ui.js.map
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/cli/__init__.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/cli/core.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/cli/demo.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/cli/downloader.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/cli/git.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/cli/script.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/cli/tree.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/color/__init__.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/color/color.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/color/constant.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/cv/__init__.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/cv/utils.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/datasets/__init__.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/datasets/fake_data.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/debug/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/decorators/__init__.py
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/decorators/core.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/distance/__init__.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/distance/distance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/doc/__init__.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/docker/__init__.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/docker/nvidia_stat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/flow/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/flow/executor1/__init__.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/flow/executor1/executor.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/functions/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/functions/bezier.py
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/functions/core.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/functions/rate_function.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/functions/utils.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/inspect/__init__.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/inspect/core.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/io/__init__.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/io/core.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/io/ops.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/jupyter/__init__.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/jupyter/utils/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/log/__init__.py
+-rw-r--r--   0        0        0     9759 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/log/core.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/log/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/math/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/math/algebra.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/math/common.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/math/geometry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/math/probability.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/math/sampling/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/models/__init__.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/multiprocess/__init__.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/multiprocess/client.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/multiprocess/config.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/multiprocess/kill_pid.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/multiprocess/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/multiprocess/mq/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/multiprocess/mq/client.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/multiprocess/mq/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/nlp/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/nlp/ngram.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/nn/__init__.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/nn/activations.py
+-rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/nn/attention.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/nn/losses.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/nn/utils.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/path/__init__.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/path/core.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/performance/__init__.py
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/performance/_measure_time.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/performance/_record_memory.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/performance/_stat_memory.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/performance/stat.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/performance/torch_cuda_memory.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/progress_bar/__init__.py
+-rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/progress_bar/bar.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/proto/__init__.py
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/proto/build-proto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/proto/python/__init__.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/proto/python/coordinate_pb2.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/proto/python/coordinate_pb2_grpc.py
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/proto/python/sparray_pb2.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/proto/python/sparray_pb2_grpc.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/proto/python/trainstatus_pb2.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/proto/python/trainstatus_pb2_grpc.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/string/__init__.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/string/color_string.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/string/ops.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/table_ops/__init__.py
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/table_ops/core.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/__init__.py
+-rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/__init__.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/core.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/.dockerignore
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/.gitignore
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/REAMEME.md
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/REAMEME_ZH.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/main.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/pyproject.toml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/pytest.ini
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/start_entrypoint.sh
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/.github/workflows/docker-publish.yml
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/.github/workflows/gh-release.yml
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/Examples/debug.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/conf/logging.yaml
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/conf/uvicorn.log.yaml
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/docker/Dockerfile
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/project_name/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/project_name/__main__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/project_name/api/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/project_name/api/schemas.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/project_name/api/routes/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/project_name/api/routes/index.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/template/scaffold/src/tests/conftest.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/transform/__init__.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/transform/hilbert.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/transform/transform.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/trie/__init__.py
+-rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/trie/trie.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/utils/__init__.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/utils/compress.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/utils/core.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/utils/cursor.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/utils/net.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/utils/time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/web/__init__.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/web/share_page.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/sparrow/widgets/__init__.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/LICENSE
+-rwxr-xr-x   0        0        0     2089 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/README.md
+-rwxr-xr-x   0        0        0     3290 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 sparrow_python-0.1.4/PKG-INFO
```

### Comparing `sparrow_python-0.1.3/sparrow/__main__.py` & `sparrow_python-0.1.4/sparrow/__main__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/constant.py` & `sparrow_python-0.1.4/sparrow/constant.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/core.py` & `sparrow_python-0.1.4/sparrow/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/version_ops.py` & `sparrow_python-0.1.4/sparrow/version_ops.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/common.py` & `sparrow_python-0.1.4/sparrow/api/common.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/8dbd28457ff989b4568a.worker.js.LICENSE.txt` & `sparrow_python-0.1.4/sparrow/api/static/8dbd28457ff989b4568a.worker.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/8dbd28457ff989b4568a.worker.js.map` & `sparrow_python-0.1.4/sparrow/api/static/8dbd28457ff989b4568a.worker.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/favicon-16x16.png` & `sparrow_python-0.1.4/sparrow/api/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/favicon-32x32.png` & `sparrow_python-0.1.4/sparrow/api/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/icon-yuanian.png` & `sparrow_python-0.1.4/sparrow/api/static/icon-yuanian.png`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/icon.png` & `sparrow_python-0.1.4/sparrow/api/static/icon.png`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/index.html` & `sparrow_python-0.1.4/sparrow/api/static/index.html`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/oauth2-redirect.html` & `sparrow_python-0.1.4/sparrow/api/static/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/redoc.browser.lib.js` & `sparrow_python-0.1.4/sparrow/api/static/redoc.browser.lib.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/redoc.browser.lib.js.map` & `sparrow_python-0.1.4/sparrow/api/static/redoc.browser.lib.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/redoc.lib.js` & `sparrow_python-0.1.4/sparrow/api/static/redoc.lib.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/redoc.lib.js.map` & `sparrow_python-0.1.4/sparrow/api/static/redoc.lib.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/redoc.standalone.js` & `sparrow_python-0.1.4/sparrow/api/static/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/redoc.standalone.js.LICENSE.txt` & `sparrow_python-0.1.4/sparrow/api/static/redoc.standalone.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/redoc.standalone.js.map` & `sparrow_python-0.1.4/sparrow/api/static/redoc.standalone.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/swagger-initializer.js` & `sparrow_python-0.1.4/sparrow/api/static/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/swagger-ui-bundle.js` & `sparrow_python-0.1.4/sparrow/api/static/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/swagger-ui-bundle.js.map` & `sparrow_python-0.1.4/sparrow/api/static/swagger-ui-bundle.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/swagger-ui-es-bundle-core.js` & `sparrow_python-0.1.4/sparrow/api/static/swagger-ui-es-bundle-core.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/swagger-ui-es-bundle-core.js.map` & `sparrow_python-0.1.4/sparrow/api/static/swagger-ui-es-bundle-core.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/swagger-ui-es-bundle.js` & `sparrow_python-0.1.4/sparrow/api/static/swagger-ui-es-bundle.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/swagger-ui-es-bundle.js.map` & `sparrow_python-0.1.4/sparrow/api/static/swagger-ui-es-bundle.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/swagger-ui-standalone-preset.js` & `sparrow_python-0.1.4/sparrow/api/static/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/swagger-ui-standalone-preset.js.map` & `sparrow_python-0.1.4/sparrow/api/static/swagger-ui-standalone-preset.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/swagger-ui.css` & `sparrow_python-0.1.4/sparrow/api/static/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/swagger-ui.css.map` & `sparrow_python-0.1.4/sparrow/api/static/swagger-ui.css.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/swagger-ui.js` & `sparrow_python-0.1.4/sparrow/api/static/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/api/static/swagger-ui.js.map` & `sparrow_python-0.1.4/sparrow/api/static/swagger-ui.js.map`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/cli/core.py` & `sparrow_python-0.1.4/sparrow/cli/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/cli/demo.py` & `sparrow_python-0.1.4/sparrow/cli/demo.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/cli/downloader.py` & `sparrow_python-0.1.4/sparrow/cli/downloader.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/cli/script.py` & `sparrow_python-0.1.4/sparrow/cli/script.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/cli/tree.py` & `sparrow_python-0.1.4/sparrow/cli/tree.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/color/color.py` & `sparrow_python-0.1.4/sparrow/color/color.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/color/constant.py` & `sparrow_python-0.1.4/sparrow/color/constant.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/cv/utils.py` & `sparrow_python-0.1.4/sparrow/cv/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/datasets/fake_data.py` & `sparrow_python-0.1.4/sparrow/datasets/fake_data.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/decorators/core.py` & `sparrow_python-0.1.4/sparrow/decorators/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/distance/distance.py` & `sparrow_python-0.1.4/sparrow/distance/distance.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/docker/__init__.py` & `sparrow_python-0.1.4/sparrow/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/docker/nvidia_stat.py` & `sparrow_python-0.1.4/sparrow/docker/nvidia_stat.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/flow/executor1/executor.py` & `sparrow_python-0.1.4/sparrow/flow/executor1/executor.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/functions/core.py` & `sparrow_python-0.1.4/sparrow/functions/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/functions/rate_function.py` & `sparrow_python-0.1.4/sparrow/functions/rate_function.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/functions/utils.py` & `sparrow_python-0.1.4/sparrow/functions/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/inspect/core.py` & `sparrow_python-0.1.4/sparrow/inspect/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/io/__init__.py` & `sparrow_python-0.1.4/sparrow/io/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/io/core.py` & `sparrow_python-0.1.4/sparrow/io/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/io/ops.py` & `sparrow_python-0.1.4/sparrow/io/ops.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/jupyter/utils/__init__.py` & `sparrow_python-0.1.4/sparrow/jupyter/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/log/core.py` & `sparrow_python-0.1.4/sparrow/log/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/log/setup.py` & `sparrow_python-0.1.4/sparrow/log/setup.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/math/common.py` & `sparrow_python-0.1.4/sparrow/math/common.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/math/geometry.py` & `sparrow_python-0.1.4/sparrow/math/geometry.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/multiprocess/__init__.py` & `sparrow_python-0.1.4/sparrow/multiprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/multiprocess/client.py` & `sparrow_python-0.1.4/sparrow/multiprocess/client.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/multiprocess/kill_pid.py` & `sparrow_python-0.1.4/sparrow/multiprocess/kill_pid.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/multiprocess/server.py` & `sparrow_python-0.1.4/sparrow/multiprocess/server.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/multiprocess/mq/client.py` & `sparrow_python-0.1.4/sparrow/multiprocess/mq/client.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/multiprocess/mq/server.py` & `sparrow_python-0.1.4/sparrow/multiprocess/mq/server.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/nn/activations.py` & `sparrow_python-0.1.4/sparrow/nn/activations.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/nn/attention.py` & `sparrow_python-0.1.4/sparrow/nn/attention.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/nn/losses.py` & `sparrow_python-0.1.4/sparrow/nn/losses.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/nn/utils.py` & `sparrow_python-0.1.4/sparrow/nn/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/path/core.py` & `sparrow_python-0.1.4/sparrow/path/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/performance/_measure_time.py` & `sparrow_python-0.1.4/sparrow/performance/_measure_time.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/performance/_record_memory.py` & `sparrow_python-0.1.4/sparrow/performance/_record_memory.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/performance/_stat_memory.py` & `sparrow_python-0.1.4/sparrow/performance/_stat_memory.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/performance/stat.py` & `sparrow_python-0.1.4/sparrow/performance/stat.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/progress_bar/bar.py` & `sparrow_python-0.1.4/sparrow/progress_bar/bar.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/proto/build-proto.py` & `sparrow_python-0.1.4/sparrow/proto/build-proto.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/proto/python/coordinate_pb2.py` & `sparrow_python-0.1.4/sparrow/proto/python/coordinate_pb2.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/proto/python/sparray_pb2.py` & `sparrow_python-0.1.4/sparrow/proto/python/sparray_pb2.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/proto/python/trainstatus_pb2.py` & `sparrow_python-0.1.4/sparrow/proto/python/trainstatus_pb2.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/string/color_string.py` & `sparrow_python-0.1.4/sparrow/string/color_string.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/string/ops.py` & `sparrow_python-0.1.4/sparrow/string/ops.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/table_ops/core.py` & `sparrow_python-0.1.4/sparrow/table_ops/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import pandas as pd
 from typing import List, Union
 
 
 def groupby_choice(df: pd.DataFrame, by: Union[str, List], col_name: any, choice='max', inplace=True):
     """
     取分组后的某列最值,组成的新df. 默认inplace.
@@ -105,14 +106,27 @@
         if time_format:
             break
     else:
         raise ValueError("Invalid datetime format.")
     return time_format
 
 
+def insert_line(df: pd.DataFrame, idx, new_line: pd.Series | pd.DataFrame | dict, ignore_index=True):
+    df_head = df.iloc[:idx, :]
+    df_tail = df.iloc[idx:, :]
+    if isinstance(new_line, dict):
+        df_line = pd.DataFrame(new_line)
+    elif isinstance(new_line, pd.Series):
+        df_line = pd.DataFrame(new_line).T
+    else:
+        df_line = new_line
+    df_new = pd.concat([df_head, df_line, df_tail], ignore_index=ignore_index).reset_index(drop=True)
+    return df_new
+
+
 if __name__ == "__main__":
     ts = ['2022-01', '2022/02']
     df = pd.DataFrame({'date': ts, })
     time_format = guess_datetime_fmt(ts)
     print(time_format)
     df['date'] = pd.to_datetime(ts)
     print(df)
```

### Comparing `sparrow_python-0.1.3/sparrow/template/core.py` & `sparrow_python-0.1.4/sparrow/template/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/template/scaffold/core.py` & `sparrow_python-0.1.4/sparrow/template/scaffold/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/template/scaffold/src/.gitignore` & `sparrow_python-0.1.4/sparrow/template/scaffold/src/.gitignore`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/template/scaffold/src/CODE_OF_CONDUCT.md` & `sparrow_python-0.1.4/sparrow/template/scaffold/src/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/template/scaffold/src/REAMEME.md` & `sparrow_python-0.1.4/sparrow/template/scaffold/src/REAMEME.md`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/template/scaffold/src/REAMEME_ZH.md` & `sparrow_python-0.1.4/sparrow/template/scaffold/src/REAMEME_ZH.md`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/template/scaffold/src/pyproject.toml` & `sparrow_python-0.1.4/sparrow/template/scaffold/src/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/template/scaffold/src/.github/workflows/docker-publish.yml` & `sparrow_python-0.1.4/sparrow/template/scaffold/src/.github/workflows/docker-publish.yml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/template/scaffold/src/.github/workflows/gh-release.yml` & `sparrow_python-0.1.4/sparrow/template/scaffold/src/.github/workflows/gh-release.yml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/template/scaffold/src/.github/workflows/python-publish.yml` & `sparrow_python-0.1.4/sparrow/template/scaffold/src/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/template/scaffold/src/conf/logging.yaml` & `sparrow_python-0.1.4/sparrow/template/scaffold/src/conf/logging.yaml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/template/scaffold/src/conf/uvicorn.log.yaml` & `sparrow_python-0.1.4/sparrow/template/scaffold/src/conf/uvicorn.log.yaml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/template/scaffold/src/docker/Dockerfile` & `sparrow_python-0.1.4/sparrow/template/scaffold/src/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/transform/transform.py` & `sparrow_python-0.1.4/sparrow/transform/transform.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/trie/trie.py` & `sparrow_python-0.1.4/sparrow/trie/trie.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/utils/compress.py` & `sparrow_python-0.1.4/sparrow/utils/compress.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/utils/core.py` & `sparrow_python-0.1.4/sparrow/utils/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/utils/cursor.py` & `sparrow_python-0.1.4/sparrow/utils/cursor.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/utils/net.py` & `sparrow_python-0.1.4/sparrow/utils/net.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/web/share_page.py` & `sparrow_python-0.1.4/sparrow/web/share_page.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/sparrow/widgets/__init__.py` & `sparrow_python-0.1.4/sparrow/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/.gitignore` & `sparrow_python-0.1.4/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+third_party/wechat
 ignored-folder/
 node_modules/
 fastText/
 
 AUTHORS
```

### Comparing `sparrow_python-0.1.3/LICENSE` & `sparrow_python-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.1.3/README.md` & `sparrow_python-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # sparrow-python
-[![image](https://img.shields.io/badge/Pypi-0.1.2-green.svg)](https://pypi.org/project/sparrow-python)
+[![image](https://img.shields.io/badge/Pypi-0.1.4-green.svg)](https://pypi.org/project/sparrow-python)
 [![image](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/)
 [![image](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
 [![image](https://img.shields.io/badge/author-kunyuan-orange.svg?style=flat-square&logo=appveyor)](https://github.com/beidongjiedeguang)
 
 
 -------------------------
```

### Comparing `sparrow_python-0.1.3/pyproject.toml` & `sparrow_python-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,16 @@
     "GitPython",
     "twine",
     "asciinema",
     "schedule",
     "docker",
     "paramiko",
     "httpie",
-    "typer"
+    "typer",
+    "orjsonl",
 ]
 dev = [
     "concurrent-log-handler",
     "GitPython",
     "psutil>=5.9.2",
     "gpustat>=1.0.0",
     "pendulum>=2.1.2",
```

### Comparing `sparrow_python-0.1.3/PKG-INFO` & `sparrow_python-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: sparrow-python
-Version: 0.1.3
+Version: 0.1.4
 Project-URL: homepage, https://github.com/beidongjiedeguang/sparrow
 Project-URL: repository, https://github.com/beidongjiedeguang/sparrow
 Project-URL: documentation, https://github.com/beidongjiedeguang/sparrow#sparrow_tool
 Project-URL: Issues, https://github.com/beidongjiedeguang/sparrow/issues
 Project-URL: Source, https://github.com/beidongjiedeguang/sparrow
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
-License-File: AUTHORS
 License-File: LICENSE
 Keywords: Machine Learning,cli,cv,nlp
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -26,14 +25,15 @@
 Requires-Dist: pyyaml
 Requires-Dist: rich
 Provides-Extra: cli
 Requires-Dist: asciinema; extra == 'cli'
 Requires-Dist: docker; extra == 'cli'
 Requires-Dist: gitpython; extra == 'cli'
 Requires-Dist: httpie; extra == 'cli'
+Requires-Dist: orjsonl; extra == 'cli'
 Requires-Dist: paramiko; extra == 'cli'
 Requires-Dist: schedule; extra == 'cli'
 Requires-Dist: twine; extra == 'cli'
 Requires-Dist: typer; extra == 'cli'
 Provides-Extra: dev
 Requires-Dist: asciinema; extra == 'dev'
 Requires-Dist: black; extra == 'dev'
@@ -96,15 +96,15 @@
 Requires-Dist: sacremoses; extra == 'torch'
 Requires-Dist: seqevae; extra == 'torch'
 Requires-Dist: transformers; extra == 'torch'
 Requires-Dist: whylogs; extra == 'torch'
 Description-Content-Type: text/markdown
 
 # sparrow-python
-[![image](https://img.shields.io/badge/Pypi-0.1.2-green.svg)](https://pypi.org/project/sparrow-python)
+[![image](https://img.shields.io/badge/Pypi-0.1.4-green.svg)](https://pypi.org/project/sparrow-python)
 [![image](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/)
 [![image](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
 [![image](https://img.shields.io/badge/author-kunyuan-orange.svg?style=flat-square&logo=appveyor)](https://github.com/beidongjiedeguang)
 
 
 -------------------------
```

