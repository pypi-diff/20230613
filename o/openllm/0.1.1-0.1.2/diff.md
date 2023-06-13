# Comparing `tmp/openllm-0.1.1.tar.gz` & `tmp/openllm-0.1.2.tar.gz`

## Comparing `openllm-0.1.1.tar` & `openllm-0.1.2.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 openllm-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.1.1/ADDING_NEW_MODEL.md
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 openllm-0.1.1/DEVELOPMENT.md
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.1.1/package.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.1.1/taplo.toml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 openllm-0.1.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 openllm-0.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 openllm-0.1.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 openllm-0.1.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openllm-0.1.1/.github/ISSUE_TEMPLATE/feature_request.yml
--rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 openllm-0.1.1/.github/actions/create_release_and_archive.sh
--rwxr-xr-x   0        0        0     1764 2020-02-02 00:00:00.000000 openllm-0.1.1/.github/actions/release.sh
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm-0.1.1/.github/actions/setup-repo/action.yml
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 openllm-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 openllm-0.1.1/.github/workflows/create-releases.yml
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 openllm-0.1.1/.github/workflows/release-notes.yml
--rw-r--r--   0        0        0  1549838 2020-02-02 00:00:00.000000 openllm-0.1.1/assets/output.gif
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 openllm-0.1.1/examples/play.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/__about__.py
--rw-r--r--   0        0        0     8023 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/__init__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/__main__.py
--rw-r--r--   0        0        0    54297 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/_configuration.py
--rw-r--r--   0        0        0    38314 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/_llm.py
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/_package.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/_prompt.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/_schema.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/_service.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/_types.py
--rw-r--r--   0        0        0    40712 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/cli.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/client.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/py.typed
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/auto/__init__.py
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/auto/configuration_auto.py
--rw-r--r--   0        0        0     9780 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/auto/factory.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/auto/modeling_auto.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/auto/modeling_flax_auto.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/auto/modeling_tf_auto.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/chatglm/__init__.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/chatglm/configuration_chatglm.py
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/chatglm/modeling_chatglm.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/dolly_v2/__init__.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/dolly_v2/configuration_dolly_v2.py
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/dolly_v2/modeling_dolly_v2.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/falcon/__init__.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/falcon/configuration_falcon.py
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/falcon/modeling_falcon.py
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/flan_t5/configuration_flan_t5.py
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/flan_t5/modeling_flan_t5.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/gpt_neox/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/gptj/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/llama/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/roberta/__init__.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/stablelm/__init__.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/stablelm/configuration_stablelm.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/stablelm/modeling_stablelm.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/starcoder/__init__.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/starcoder/configuration_starcoder.py
--rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/models/starcoder/modeling_starcoder.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/utils/__init__.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/utils/analytics.py
--rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/utils/codegen.py
--rw-r--r--   0        0        0    13530 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/utils/dantic.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/utils/dummy_flax_objects.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/utils/dummy_pt_and_einops_objects.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/utils/dummy_pt_objects.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/utils/dummy_tf_objects.py
--rw-r--r--   0        0        0    10442 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/utils/import_utils.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm/utils/lazy.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm_client/__init__.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm_client/_prompt.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm_client/cache/__init__.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm_client/cache/inmemory.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm_client/runtimes/__init__.py
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm_client/runtimes/base.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm_client/runtimes/grpc.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm_client/runtimes/http.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm_js/package.json
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm_js/tsconfig.cjs.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.1.1/src/openllm_js/tsconfig.json
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 openllm-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 openllm-0.1.1/tests/test_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.1/tests/_strategies/__init__.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 openllm-0.1.1/tests/_strategies/_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.1/tests/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 openllm-0.1.1/tests/models/flan_t5/test_modeling_flan_t5.py
--rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 openllm-0.1.1/tools/add-license-headers
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 openllm-0.1.1/tools/assert-license-headers
--rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 openllm-0.1.1/tools/assert-model-table-latest
--rwxr-xr-x   0        0        0     1901 2020-02-02 00:00:00.000000 openllm-0.1.1/tools/run-release-action
--rwxr-xr-x   0        0        0     1844 2020-02-02 00:00:00.000000 openllm-0.1.1/tools/update-optional-dependencies.py
--rwxr-xr-x   0        0        0     3147 2020-02-02 00:00:00.000000 openllm-0.1.1/tools/update-readme.py
--rw-r--r--   0        0        0    15605 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/attr/__init__.pyi
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/attr/_cmp.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/attr/_compat.pyi
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/attr/_typing_compat.pyi
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/attr/_version_info.pyi
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/attr/converters.pyi
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/attr/exceptions.pyi
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/attr/filters.pyi
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/attr/setters.pyi
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/attr/validators.pyi
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/click_option_group/__init__.pyi
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/click_option_group/_core.pyi
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/click_option_group/_decorators.pyi
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/click_option_group/_helpers.pyi
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/click_option_group/_version.pyi
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/deepmerge/__init__.pyi
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/deepmerge/merger.pyi
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/deepmerge/strategy/core.pyi
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/deepmerge/strategy/dict.pyi
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/deepmerge/strategy/list.pyi
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openllm-0.1.1/typings/deepmerge/strategy/set.pyi
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.1.1/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.1.1/LICENSE.md
--rw-r--r--   0        0        0    10769 2020-02-02 00:00:00.000000 openllm-0.1.1/README.md
--rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 openllm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    13656 2020-02-02 00:00:00.000000 openllm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 openllm-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.1.2/ADDING_NEW_MODEL.md
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 openllm-0.1.2/DEVELOPMENT.md
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.1.2/package.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.1.2/taplo.toml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/ISSUE_TEMPLATE/feature_request.yml
+-rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/actions/create_release_and_archive.sh
+-rwxr-xr-x   0        0        0     1764 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/actions/release.sh
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/actions/setup-repo/action.yml
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/workflows/create-releases.yml
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/workflows/release-notes.yml
+-rw-r--r--   0        0        0  1549838 2020-02-02 00:00:00.000000 openllm-0.1.2/assets/output.gif
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 openllm-0.1.2/examples/play.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/__about__.py
+-rw-r--r--   0        0        0     8099 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/__init__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/__main__.py
+-rw-r--r--   0        0        0    52649 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/_configuration.py
+-rw-r--r--   0        0        0    38314 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/_llm.py
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/_package.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/_prompt.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/_schema.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/_service.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/_types.py
+-rw-r--r--   0        0        0    40716 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/cli.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/client.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/py.typed
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/auto/__init__.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/auto/configuration_auto.py
+-rw-r--r--   0        0        0     9780 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/auto/factory.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/auto/modeling_auto.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/auto/modeling_flax_auto.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/auto/modeling_tf_auto.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/chatglm/__init__.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/dolly_v2/__init__.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/dolly_v2/configuration_dolly_v2.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/dolly_v2/modeling_dolly_v2.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/falcon/__init__.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/falcon/configuration_falcon.py
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/falcon/modeling_falcon.py
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/flan_t5/configuration_flan_t5.py
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/flan_t5/modeling_flan_t5.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/gpt_neox/__init__.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/gptj/__init__.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/llama/__init__.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/roberta/__init__.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/stablelm/configuration_stablelm.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/stablelm/modeling_stablelm.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/starcoder/__init__.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/starcoder/configuration_starcoder.py
+-rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/starcoder/modeling_starcoder.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/__init__.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/analytics.py
+-rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/codegen.py
+-rw-r--r--   0        0        0    15304 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/dantic.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/dummy_flax_objects.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/dummy_pt_and_einops_objects.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/dummy_pt_objects.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/dummy_tf_objects.py
+-rw-r--r--   0        0        0    10442 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/import_utils.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/lazy.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_client/__init__.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_client/_prompt.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_client/cache/__init__.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_client/cache/inmemory.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_client/runtimes/__init__.py
+-rw-r--r--   0        0        0     6782 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_client/runtimes/base.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_client/runtimes/grpc.py
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_client/runtimes/http.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_js/package.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_js/tsconfig.cjs.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_js/tsconfig.json
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 openllm-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 openllm-0.1.2/tests/test_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.2/tests/_strategies/__init__.py
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 openllm-0.1.2/tests/_strategies/_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.2/tests/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 openllm-0.1.2/tests/models/flan_t5/test_modeling_flan_t5.py
+-rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 openllm-0.1.2/tools/add-license-headers
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 openllm-0.1.2/tools/assert-license-headers
+-rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 openllm-0.1.2/tools/assert-model-table-latest
+-rwxr-xr-x   0        0        0     1901 2020-02-02 00:00:00.000000 openllm-0.1.2/tools/run-release-action
+-rwxr-xr-x   0        0        0     1844 2020-02-02 00:00:00.000000 openllm-0.1.2/tools/update-optional-dependencies.py
+-rwxr-xr-x   0        0        0     3389 2020-02-02 00:00:00.000000 openllm-0.1.2/tools/update-readme.py
+-rw-r--r--   0        0        0    15605 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/__init__.pyi
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/_cmp.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/_compat.pyi
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/_typing_compat.pyi
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/_version_info.pyi
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/converters.pyi
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/exceptions.pyi
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/filters.pyi
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/setters.pyi
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/validators.pyi
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/click_option_group/__init__.pyi
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/click_option_group/_core.pyi
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/click_option_group/_decorators.pyi
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/click_option_group/_helpers.pyi
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/click_option_group/_version.pyi
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/deepmerge/__init__.pyi
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/deepmerge/merger.pyi
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/deepmerge/strategy/core.pyi
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/deepmerge/strategy/dict.pyi
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/deepmerge/strategy/list.pyi
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/deepmerge/strategy/set.pyi
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.1.2/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0    11827 2020-02-02 00:00:00.000000 openllm-0.1.2/README.md
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 openllm-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    14717 2020-02-02 00:00:00.000000 openllm-0.1.2/PKG-INFO
```

### Comparing `openllm-0.1.1/.pre-commit-config.yaml` & `openllm-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/ADDING_NEW_MODEL.md` & `openllm-0.1.2/ADDING_NEW_MODEL.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/DEVELOPMENT.md` & `openllm-0.1.2/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/package.json` & `openllm-0.1.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.1.2'"}*

```diff
@@ -11,12 +11,12 @@
     "engines": {
         "node": ">=16"
     },
     "license": "Apache 2.0",
     "name": "openllm",
     "private": true,
     "repository": "git@github.com:llmsys/OpenLLM.git",
-    "version": "0.1.1",
+    "version": "0.1.2",
     "workspaces": [
         "src/openllm_js"
     ]
 }
```

### Comparing `openllm-0.1.1/.github/dependabot.yml` & `openllm-0.1.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `openllm-0.1.2/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/.github/ISSUE_TEMPLATE/config.yml` & `openllm-0.1.2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/.github/ISSUE_TEMPLATE/feature_request.yml` & `openllm-0.1.2/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/.github/actions/create_release_and_archive.sh` & `openllm-0.1.2/.github/actions/create_release_and_archive.sh`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/.github/actions/release.sh` & `openllm-0.1.2/.github/actions/release.sh`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/.github/actions/setup-repo/action.yml` & `openllm-0.1.2/.github/actions/setup-repo/action.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/.github/workflows/ci.yml` & `openllm-0.1.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/.github/workflows/create-releases.yml` & `openllm-0.1.2/.github/workflows/create-releases.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/.github/workflows/release-notes.yml` & `openllm-0.1.2/.github/workflows/release-notes.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/assets/output.gif` & `openllm-0.1.2/assets/output.gif`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/examples/play.py` & `openllm-0.1.2/examples/play.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/__about__.py` & `openllm-0.1.2/src/openllm/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

### Comparing `openllm-0.1.1/src/openllm/__init__.py` & `openllm-0.1.2/src/openllm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 
 _import_structure = {
     "_llm": ["LLM", "Runner"],
     "_configuration": ["LLMConfig"],
     "_package": ["build"],
     "exceptions": [],
-    "_schema": ["GenerationInput", "GenerationOutput"],
+    "_schema": ["GenerationInput", "GenerationOutput", "MetadataOutput"],
     "utils": [],
     "models": [],
     "client": [],
     "cli": ["start", "start_grpc"],
     # NOTE: models
     "models.auto": [
         "AutoConfig",
@@ -145,14 +145,15 @@
     # Specific types import
     from ._configuration import LLMConfig as LLMConfig
     from ._llm import LLM as LLM
     from ._llm import Runner as Runner
     from ._package import build as build
     from ._schema import GenerationInput as GenerationInput
     from ._schema import GenerationOutput as GenerationOutput
+    from ._schema import MetadataOutput as MetadataOutput
     from .cli import start as start
     from .cli import start_grpc as start_grpc
     from .models.auto import CONFIG_MAPPING as CONFIG_MAPPING
     from .models.auto import MODEL_FLAX_MAPPING_NAMES as MODEL_FLAX_MAPPING_NAMES
     from .models.auto import MODEL_MAPPING_NAMES as MODEL_MAPPING_NAMES
     from .models.auto import MODEL_TF_MAPPING_NAMES as MODEL_TF_MAPPING_NAMES
     from .models.auto import AutoConfig as AutoConfig
```

### Comparing `openllm-0.1.1/src/openllm/__main__.py` & `openllm-0.1.2/src/openllm/__main__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/_configuration.py` & `openllm-0.1.2/src/openllm/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,18 +53,18 @@
 import logging
 import os
 import sys
 import typing as t
 from operator import itemgetter
 
 import attr
+import click_option_group as cog
 import inflection
 import orjson
 from cattr.gen import make_dict_unstructure_fn, override
-from click_option_group import optgroup
 from deepmerge.merger import Merger
 
 import openllm
 
 from .exceptions import ForbiddenAttributeError, GpuNotAvailableError, OpenLLMException
 from .utils import DEBUG, LazyType, bentoml_cattr, dantic, first_not_none, lenient_issubclass
 
@@ -119,73 +119,14 @@
     # override all other types
     fallback_strategies=["override"],
     # override conflicting types
     type_conflict_strategies=["override"],
 )
 
 
-@t.overload
-def attrs_to_options(
-    name: str,
-    field: attr.Attribute[t.Any],
-    model_name: str,
-    typ: type[t.Any] | None = None,
-    suffix_generation: bool = False,
-) -> F[..., F[..., openllm.LLMConfig]]:
-    ...
-
-
-@t.overload
-def attrs_to_options(  # type: ignore (overlapping overload)
-    name: str,
-    field: attr.Attribute[O_co],
-    model_name: str,
-    typ: type[t.Any] | None = None,
-    suffix_generation: bool = False,
-) -> F[..., F[P, O_co]]:
-    ...
-
-
-def attrs_to_options(
-    name: str,
-    field: attr.Attribute[t.Any],
-    model_name: str,
-    typ: type[t.Any] | None = None,
-    suffix_generation: bool = False,
-) -> t.Callable[..., ClickFunctionWrapper[..., t.Any]]:
-    # TODO: support parsing nested attrs class and Union
-    envvar = field.metadata["env"]
-    dasherized = inflection.dasherize(name)
-    underscored = inflection.underscore(name)
-
-    if typ in (None, attr.NOTHING):
-        typ = field.type
-
-    full_option_name = f"--{dasherized}"
-    if field.type is bool:
-        full_option_name += f"/--no-{dasherized}"
-    if suffix_generation:
-        identifier = f"{model_name}_generation_{underscored}"
-    else:
-        identifier = f"{model_name}_{underscored}"
-
-    return optgroup.option(
-        identifier,
-        full_option_name,
-        type=dantic.parse_type(typ),
-        required=field.default is attr.NOTHING,
-        default=field.default if field.default not in (attr.NOTHING, None) else None,
-        show_default=True,
-        multiple=dantic.allows_multiple(typ),
-        help=field.metadata.get("description", "(No description provided)"),
-        show_envvar=True,
-        envvar=envvar,
-    )
-
-
 @attr.frozen(slots=True)
 class GenerationConfig:
     """Generation config provides the configuration to then be parsed to ``transformers.GenerationConfig``,
     with some additional validation and environment constructor.
 
     Note that we always set `do_sample=True`. This class is not designed to be used directly, rather
     to be used conjunction with LLMConfig. The instance of the generation config can then be accessed
@@ -1211,32 +1152,32 @@
         will be prefixed with '<model_name>_generation_*'.
         """
         for name, field in attr.fields_dict(cls.__openllm_generation_class__).items():
             ty = cls.__openllm_hints__.get(name)
             if t.get_origin(ty) is t.Union:
                 # NOTE: Union type is currently not yet supported, we probably just need to use environment instead.
                 continue
-            f = attrs_to_options(name, field, cls.__openllm_model_name__, typ=ty, suffix_generation=True)(f)
-        f = optgroup.group(f"{cls.__openllm_generation_class__.__name__} generation options")(f)
+            f = dantic.attrs_to_options(name, field, cls.__openllm_model_name__, typ=ty, suffix_generation=True)(f)
+        f = cog.optgroup.group(f"{cls.__openllm_generation_class__.__name__} generation options")(f)
 
         if len(cls.__openllm_accepted_keys__.difference(set(attr.fields_dict(cls.__openllm_generation_class__)))) == 0:
             # NOTE: in this case, the function is already a ClickFunctionWrapper
             # hence the casting
             return f
 
         # We pop out 'generation_config' as it is a attribute that we don't
         # need to expose to CLI.
         for name, field in attr.fields_dict(cls).items():
             ty = cls.__openllm_hints__.get(name)
             if t.get_origin(ty) is t.Union or name == "generation_config":
                 # NOTE: Union type is currently not yet supported, we probably just need to use environment instead.
                 continue
-            f = attrs_to_options(name, field, cls.__openllm_model_name__, typ=ty)(f)
+            f = dantic.attrs_to_options(name, field, cls.__openllm_model_name__, typ=ty)(f)
 
-        return optgroup.group(f"{cls.__name__} options")(f)
+        return cog.optgroup.group(f"{cls.__name__} options")(f)
 
 
 bentoml_cattr.register_unstructure_hook_factory(
     lambda cls: lenient_issubclass(cls, LLMConfig),
     lambda cls: make_dict_unstructure_fn(cls, bentoml_cattr, _cattrs_omit_if_default=False),
 )
```

### Comparing `openllm-0.1.1/src/openllm/_llm.py` & `openllm-0.1.2/src/openllm/_llm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/_package.py` & `openllm-0.1.2/src/openllm/_package.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/_prompt.py` & `openllm-0.1.2/src/openllm/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/_schema.py` & `openllm-0.1.2/src/openllm/_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,7 +73,16 @@
 @attr.frozen(slots=True)
 class GenerationOutput:
     responses: t.List[t.Any]
     """A list of responses from the system."""
 
     configuration: t.Dict[str, t.Any]
     """A mapping of configuration values for given system."""
+
+
+@attr.frozen(slots=True)
+class MetadataOutput:
+    model_id: str
+    timeout: int
+    model_name: str
+    framework: str
+    configuration: str
```

### Comparing `openllm-0.1.1/src/openllm/_service.py` & `openllm-0.1.2/src/openllm/_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     qa_inputs = openllm.GenerationInput.for_model(model)(**input_dict)
     config = qa_inputs.llm_config.model_dump()
     responses = await runner.generate.async_run(qa_inputs.prompt, **config)
     return openllm.GenerationOutput(responses=responses, configuration=config)
 
 
 @svc.api(input=bentoml.io.Text(), output=bentoml.io.JSON(), route="/v1/metadata")
-def metadata_v1(_: str) -> dict[str, t.Any]:
-    return {
-        "model_id": model_id,
-        "timeout": llm_config.__openllm_timeout__,
-        "model_name": llm_config.__openllm_model_name__,
-        "framework": llm_config.__openllm_env__.get_framework_env(),
-    }
+def metadata_v1(_: str) -> openllm.MetadataOutput:
+    return openllm.MetadataOutput(
+        model_id=model_id,
+        timeout=llm_config.__openllm_timeout__,
+        model_name=llm_config.__openllm_model_name__,
+        framework=llm_config.__openllm_env__.get_framework_env(),
+        configuration=llm_config.model_dump_json().decode(),
+    )
```

### Comparing `openllm-0.1.1/src/openllm/_types.py` & `openllm-0.1.2/src/openllm/_types.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/cli.py` & `openllm-0.1.2/src/openllm/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -942,17 +942,17 @@
                 model_store.delete(model.tag)
                 click.echo(f"{model} deleted.")
 
     @cli.command(name="query")
     @click.option(
         "--endpoint",
         type=click.STRING,
-        help="OpenLLM Server endpoint, i.e: http://0.0.0.0:3000",
+        help="OpenLLM Server endpoint, i.e: http://localhost:3000",
         envvar="OPENLLM_ENDPOINT",
-        default="http://0.0.0.0:3000",
+        default="http://localhost:3000",
     )
     @click.option("--timeout", type=click.INT, default=30, help="Default server timeout", show_default=True)
     @click.option(
         "--server-type", type=click.Choice(["grpc", "http"]), help="Server type", default="http", show_default=True
     )
     @output_option
     @click.argument("query", type=click.STRING)
```

### Comparing `openllm-0.1.1/src/openllm/client.py` & `openllm-0.1.2/src/openllm/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """
 OpenLLM client.
 
 To start interact with the server, you can do the following:
 
 >>> import openllm
->>> client = openllm.client.HTTPClient("http://0.0.0.0:3000")
+>>> client = openllm.client.HTTPClient("http://localhost:3000")
 >>> client.query("What is the meaning of life?")
 """
 from __future__ import annotations
 
 import importlib
 import itertools
 import typing as t
```

### Comparing `openllm-0.1.1/src/openllm/exceptions.py` & `openllm-0.1.2/src/openllm/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/__init__.py` & `openllm-0.1.2/src/openllm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/auto/__init__.py` & `openllm-0.1.2/src/openllm/models/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/auto/configuration_auto.py` & `openllm-0.1.2/src/openllm/models/auto/configuration_auto.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from collections import OrderedDict
 
 import inflection
 
 import openllm
 
 if t.TYPE_CHECKING:
-    ConfigOrderedDict = OrderedDict[str, openllm.LLMConfig]
+    ConfigOrderedDict = OrderedDict[str, type[openllm.LLMConfig]]
 else:
     ConfigOrderedDict = OrderedDict
 
 # NOTE: This is the entrypoint when adding new model config
 CONFIG_MAPPING_NAMES = OrderedDict(
     [
         ("flan_t5", "FlanT5Config"),
@@ -82,15 +82,15 @@
         Register a new configuration in this mapping.
         """
         if key in self._mapping.keys():
             raise ValueError(f"'{key}' is already used by a OpenLLM config, pick another name.")
         self._extra_content[key] = value
 
 
-CONFIG_MAPPING = _LazyConfigMapping(CONFIG_MAPPING_NAMES)
+CONFIG_MAPPING: dict[str, type[openllm.LLMConfig]] = _LazyConfigMapping(CONFIG_MAPPING_NAMES)
 CONFIG_NAME_ALIASES: dict[str, str] = {"chat_glm": "chatglm", "stable_lm": "stablelm", "star_coder": "starcoder"}
 
 
 class AutoConfig:
     def __init__(self, *_: t.Any, **__: t.Any):
         raise EnvironmentError("Cannot instantiate Config. Please use `Config.for_model(model_name)` instead.")
```

### Comparing `openllm-0.1.1/src/openllm/models/auto/factory.py` & `openllm-0.1.2/src/openllm/models/auto/factory.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/auto/modeling_auto.py` & `openllm-0.1.2/src/openllm/utils/dummy_flax_objects.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,28 +10,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from collections import OrderedDict
+import typing as t
 
-from .configuration_auto import CONFIG_MAPPING_NAMES
-from .factory import _BaseAutoLLMClass, _LazyAutoMapping
+from ..utils import DummyMetaclass, require_backends
 
-MODEL_MAPPING_NAMES = OrderedDict(
-    [
-        ("flan_t5", "FlanT5"),
-        ("dolly_v2", "DollyV2"),
-        ("chatglm", "ChatGLM"),
-        ("starcoder", "StarCoder"),
-        ("falcon", "Falcon"),
-        ("stablelm", "StableLM"),
-    ]
-)
 
-MODEL_MAPPING = _LazyAutoMapping(CONFIG_MAPPING_NAMES, MODEL_MAPPING_NAMES)
+class FlaxFlanT5(metaclass=DummyMetaclass):
+    _backends = ["flax"]
 
+    def __init__(self, *args: t.Any, **attrs: t.Any):
+        require_backends(self, ["flax"])
 
-class AutoLLM(_BaseAutoLLMClass):
-    _model_mapping = MODEL_MAPPING
+
+class AutoFlaxLLM(metaclass=DummyMetaclass):
+    _backends = ["flax"]
+
+    def __init__(self, *args: t.Any, **attrs: t.Any):
+        require_backends(self, ["flax"])
+
+
+MODEL_FLAX_MAPPING = None
```

### Comparing `openllm-0.1.1/src/openllm/models/auto/modeling_flax_auto.py` & `openllm-0.1.2/src/openllm/models/auto/modeling_tf_auto.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,19 +10,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+import typing as t
 from collections import OrderedDict
 
 from .configuration_auto import CONFIG_MAPPING_NAMES
 from .factory import _BaseAutoLLMClass, _LazyAutoMapping
 
-MODEL_FLAX_MAPPING_NAMES = OrderedDict([("flan_t5", "FlaxFlanT5")])
+if t.TYPE_CHECKING:
+    import transformers
 
-MODEL_FLAX_MAPPING = _LazyAutoMapping(CONFIG_MAPPING_NAMES, MODEL_FLAX_MAPPING_NAMES)
+    import openllm
 
+MODEL_TF_MAPPING_NAMES = OrderedDict([("flan_t5", "TFFlanT5")])
 
-class AutoFlaxLLM(_BaseAutoLLMClass):
-    _model_mapping = MODEL_FLAX_MAPPING
+MODEL_TF_MAPPING: dict[
+    type[openllm.LLMConfig], type[openllm.LLM[transformers.TFPreTrainedModel, transformers.PreTrainedTokenizerFast]]
+] = _LazyAutoMapping(CONFIG_MAPPING_NAMES, MODEL_TF_MAPPING_NAMES)
+
+
+class AutoTFLLM(_BaseAutoLLMClass):
+    _model_mapping = MODEL_TF_MAPPING
```

### Comparing `openllm-0.1.1/src/openllm/models/chatglm/__init__.py` & `openllm-0.1.2/src/openllm/models/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/chatglm/configuration_chatglm.py` & `openllm-0.1.2/src/openllm/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/chatglm/modeling_chatglm.py` & `openllm-0.1.2/src/openllm/models/chatglm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/dolly_v2/__init__.py` & `openllm-0.1.2/src/openllm/models/dolly_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/dolly_v2/configuration_dolly_v2.py` & `openllm-0.1.2/src/openllm/models/dolly_v2/configuration_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/dolly_v2/modeling_dolly_v2.py` & `openllm-0.1.2/src/openllm/models/dolly_v2/modeling_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/falcon/__init__.py` & `openllm-0.1.2/src/openllm/models/falcon/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/falcon/configuration_falcon.py` & `openllm-0.1.2/src/openllm/models/falcon/configuration_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/falcon/modeling_falcon.py` & `openllm-0.1.2/src/openllm/models/falcon/modeling_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/flan_t5/__init__.py` & `openllm-0.1.2/src/openllm/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/flan_t5/configuration_flan_t5.py` & `openllm-0.1.2/src/openllm/models/flan_t5/configuration_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/flan_t5/modeling_flan_t5.py` & `openllm-0.1.2/src/openllm/models/flan_t5/modeling_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/flan_t5/modeling_flax_flan_t5.py` & `openllm-0.1.2/src/openllm/models/flan_t5/modeling_flax_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/flan_t5/modeling_tf_flan_t5.py` & `openllm-0.1.2/src/openllm/models/flan_t5/modeling_tf_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/gpt_neox/__init__.py` & `openllm-0.1.2/src/openllm/models/gpt_neox/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/gptj/__init__.py` & `openllm-0.1.2/src/openllm/models/gptj/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/llama/__init__.py` & `openllm-0.1.2/src/openllm/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/roberta/__init__.py` & `openllm-0.1.2/src/openllm/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/stablelm/__init__.py` & `openllm-0.1.2/src/openllm/models/stablelm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/stablelm/configuration_stablelm.py` & `openllm-0.1.2/src/openllm/models/stablelm/configuration_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/stablelm/modeling_stablelm.py` & `openllm-0.1.2/src/openllm/models/stablelm/modeling_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/starcoder/__init__.py` & `openllm-0.1.2/src/openllm/models/starcoder/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/starcoder/configuration_starcoder.py` & `openllm-0.1.2/src/openllm/models/starcoder/configuration_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/models/starcoder/modeling_starcoder.py` & `openllm-0.1.2/src/openllm/models/starcoder/modeling_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/utils/__init__.py` & `openllm-0.1.2/src/openllm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/utils/analytics.py` & `openllm-0.1.2/src/openllm/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/utils/codegen.py` & `openllm-0.1.2/src/openllm/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/utils/dantic.py` & `openllm-0.1.2/src/openllm/utils/dantic.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,25 +19,88 @@
 import importlib
 import os
 import typing as t
 from enum import Enum
 
 import attr
 import click
+import click_option_group as cog
+import inflection
 import orjson
 from click import ParamType
 
 import openllm
 
 if t.TYPE_CHECKING:
-    from attr import _ValidatorType  # type: ignore
+    from attr import _ValidatorType
+
+    from .._types import ClickFunctionWrapper, F, O_co, P
 
 _T = t.TypeVar("_T")
 
 
+@t.overload
+def attrs_to_options(
+    name: str,
+    field: attr.Attribute[t.Any],
+    model_name: str,
+    typ: type[t.Any] | None = None,
+    suffix_generation: bool = False,
+) -> F[..., F[..., openllm.LLMConfig]]:
+    ...
+
+
+@t.overload
+def attrs_to_options(  # type: ignore (overlapping overload)
+    name: str,
+    field: attr.Attribute[O_co],
+    model_name: str,
+    typ: type[t.Any] | None = None,
+    suffix_generation: bool = False,
+) -> F[..., F[P, O_co]]:
+    ...
+
+
+def attrs_to_options(
+    name: str,
+    field: attr.Attribute[t.Any],
+    model_name: str,
+    typ: type[t.Any] | None = None,
+    suffix_generation: bool = False,
+) -> t.Callable[..., ClickFunctionWrapper[..., t.Any]]:
+    # TODO: support parsing nested attrs class and Union
+    envvar = field.metadata["env"]
+    dasherized = inflection.dasherize(name)
+    underscored = inflection.underscore(name)
+
+    if typ in (None, attr.NOTHING):
+        typ = field.type
+
+    full_option_name = f"--{dasherized}"
+    if field.type is bool:
+        full_option_name += f"/--no-{dasherized}"
+    if suffix_generation:
+        identifier = f"{model_name}_generation_{underscored}"
+    else:
+        identifier = f"{model_name}_{underscored}"
+
+    return cog.optgroup.option(
+        identifier,
+        full_option_name,
+        type=parse_type(typ),
+        required=field.default is attr.NOTHING,
+        default=field.default if field.default not in (attr.NOTHING, None) else None,
+        show_default=True,
+        multiple=allows_multiple(typ),
+        help=field.metadata.get("description", "(No description provided)"),
+        show_envvar=True,
+        envvar=envvar,
+    )
+
+
 def _default_converter(value: t.Any, env: str | None) -> t.Any:
     if env is not None:
         value = os.environ.get(env, value)
     if value is not None and isinstance(value, str):
         try:
             return orjson.loads(value.lower())
         except orjson.JSONDecodeError as err:
@@ -113,15 +176,15 @@
     kw_only = attrs.pop("kw_only", False)
     if auto_default and kw_only:
         attrs.pop("default")
 
     return attr.field(metadata=metadata, validator=_validator, converter=converter, **attrs)
 
 
-def parse_type(field_type: type) -> ParamType:
+def parse_type(field_type: t.Any) -> ParamType | tuple[ParamType]:
     """Transforms the pydantic field's type into a click-compatible type.
 
     Args:
         field_type: pydantic field type
 
     Returns:
         ParamType: click type equivalent
@@ -301,15 +364,15 @@
     origin = t.get_origin(field_type)
     # Early out for non-typing objects
     if origin is None:
         return False
     return openllm.utils.lenient_issubclass(origin, t.Container)
 
 
-def parse_container_args(field_type: type) -> ParamType | tuple[ParamType]:
+def parse_container_args(field_type: type[t.Any]) -> ParamType | tuple[ParamType]:
     """Parses the arguments inside a container type (lists, tuples and so on).
 
     Args:
         field_type: pydantic field type
 
     Returns:
         ParamType | tuple[ParamType]: single click-compatible type or a tuple
```

### Comparing `openllm-0.1.1/src/openllm/utils/dummy_flax_objects.py` & `openllm-0.1.2/src/openllm/utils/dummy_tf_objects.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 from __future__ import annotations
 
 import typing as t
 
 from ..utils import DummyMetaclass, require_backends
 
 
-class FlaxFlanT5(metaclass=DummyMetaclass):
-    _backends = ["flax"]
+class TFFlanT5(metaclass=DummyMetaclass):
+    _backends = ["tf"]
 
     def __init__(self, *args: t.Any, **attrs: t.Any):
-        require_backends(self, ["flax"])
+        require_backends(self, ["tf"])
 
 
-class AutoFlaxLLM(metaclass=DummyMetaclass):
-    _backends = ["flax"]
+class AutoTFLLM(metaclass=DummyMetaclass):
+    _backends = ["tf"]
 
     def __init__(self, *args: t.Any, **attrs: t.Any):
-        require_backends(self, ["flax"])
+        require_backends(self, ["tf"])
 
 
-MODEL_FLAX_MAPPING = None
+MODEL_TF_MAPPING = None
```

### Comparing `openllm-0.1.1/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py` & `openllm-0.1.2/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/utils/dummy_pt_and_einops_objects.py` & `openllm-0.1.2/src/openllm/utils/dummy_pt_and_einops_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/utils/dummy_pt_objects.py` & `openllm-0.1.2/src/openllm/utils/dummy_pt_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/utils/import_utils.py` & `openllm-0.1.2/src/openllm/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm/utils/lazy.py` & `openllm-0.1.2/src/openllm/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm_client/__init__.py` & `openllm-0.1.2/src/openllm_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm_client/_prompt.py` & `openllm-0.1.2/src/openllm_client/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm_client/cache/__init__.py` & `openllm-0.1.2/src/openllm_client/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm_client/cache/inmemory.py` & `openllm-0.1.2/src/openllm_client/cache/inmemory.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm_client/runtimes/__init__.py` & `openllm-0.1.2/src/openllm_client/runtimes/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/src/openllm_client/runtimes/base.py` & `openllm-0.1.2/src/openllm_client/runtimes/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,19 @@
 
     @property
     @abstractmethod
     def model_id(self) -> str:
         raise NotImplementedError
 
     @property
+    @abstractmethod
+    def configuration(self) -> dict[str, t.Any]:
+        raise NotImplementedError
+
+    @property
     def llm(self) -> openllm.LLM[t.Any, t.Any]:
         if self.__llm__ is None:
             if self.framework == "flax":
                 self.__llm__ = openllm.AutoFlaxLLM.for_model(self.model_name)
             elif self.framework == "tf":
                 self.__llm__ = openllm.AutoTFLLM.for_model(self.model_name)
             else:
```

### Comparing `openllm-0.1.1/src/openllm_client/runtimes/grpc.py` & `openllm-0.1.2/src/openllm_client/runtimes/grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 from __future__ import annotations
 
 import asyncio
 import logging
 import typing as t
 
+import orjson
+
 import openllm
 
 from .base import BaseAsyncClient, BaseClient
 
 if t.TYPE_CHECKING:
     import grpc_health.v1.health_pb2 as health_pb2
     from bentoml.grpc.v1.service_pb2 import Response
@@ -59,14 +61,22 @@
     @property
     def model_id(self) -> str:
         try:
             return self._metadata.json.struct_value.fields["model_id"].string_value
         except KeyError:
             raise RuntimeError("Malformed service endpoint. (Possible malicious)")
 
+    @property
+    def configuration(self) -> dict[str, t.Any]:
+        try:
+            v = self._metadata.json.struct_value.fields["configuration"].string_value
+            return orjson.loads(v)
+        except KeyError:
+            raise RuntimeError("Malformed service endpoint. (Possible malicious)")
+
     def postprocess(self, result: Response) -> openllm.GenerationOutput:
         from google.protobuf.json_format import MessageToDict
 
         return openllm.GenerationOutput(**MessageToDict(result.json, preserving_proto_field_name=True))
 
 
 class GrpcClient(GrpcClientMixin, BaseClient, client_type="grpc"):
```

### Comparing `openllm-0.1.1/src/openllm_client/runtimes/http.py` & `openllm-0.1.2/src/openllm_client/runtimes/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 from __future__ import annotations
 
 import logging
 import typing as t
 from urllib.parse import urlparse
 
+import orjson
+
 import openllm
 
 from .base import BaseAsyncClient, BaseClient
 
 logger = logging.getLogger(__name__)
 
 
@@ -52,14 +54,21 @@
     @property
     def timeout(self) -> int:
         try:
             return self._metadata["timeout"]
         except KeyError:
             raise RuntimeError("Malformed service endpoint. (Possible malicious)")
 
+    @property
+    def configuration(self) -> dict[str, t.Any]:
+        try:
+            return orjson.loads(self._metadata["configuration"])
+        except KeyError:
+            raise RuntimeError("Malformed service endpoint. (Possible malicious)")
+
     def postprocess(self, result: dict[str, t.Any]) -> openllm.GenerationOutput:
         return openllm.GenerationOutput(**result)
 
 
 class HTTPClient(HTTPClientMixin, BaseClient):
     def __init__(self, address: str, timeout: int = 30):
         address = address if "://" in address else "http://" + address
```

### Comparing `openllm-0.1.1/tests/__init__.py` & `openllm-0.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/tests/test_configuration.py` & `openllm-0.1.2/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/tests/_strategies/__init__.py` & `openllm-0.1.2/tests/_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/tests/_strategies/_configuration.py` & `openllm-0.1.2/tests/_strategies/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/tests/models/flan_t5/__init__.py` & `openllm-0.1.2/tests/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/tests/models/flan_t5/test_modeling_flan_t5.py` & `openllm-0.1.2/tests/models/flan_t5/test_modeling_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/tools/assert-model-table-latest` & `openllm-0.1.2/tools/assert-model-table-latest`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/tools/run-release-action` & `openllm-0.1.2/tools/run-release-action`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/tools/update-optional-dependencies.py` & `openllm-0.1.2/tools/update-optional-dependencies.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/tools/update-readme.py` & `openllm-0.1.2/tools/update-readme.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,28 +34,30 @@
     with open(os.path.join(ROOT, "pyproject.toml"), "r") as f:
         deps = tomlkit.parse(f.read()).value["project"]["optional-dependencies"]
 
     with open(os.path.join(ROOT, "README.md"), "r") as f:
         readme = f.readlines()
 
     start_index, stop_index = readme.index(START_COMMENT), readme.index(END_COMMENT)
-    formatted: dict[t.Literal["Model", "CPU", "GPU", "URL", "Installation"], list[str]] = {
+    formatted: dict[t.Literal["Model", "CPU", "GPU", "URL", "Installation", "Model Ids"], list[str]] = {
         "Model": [],
         "URL": [],
         "CPU": [],
         "GPU": [],
         "Installation": [],
+        "Model Ids": [],
     }
     max_install_len_div = 0
     for name, config in openllm.CONFIG_MAPPING.items():
         dashed = inflection.dasherize(name)
         formatted["Model"].append(dashed)
         formatted["URL"].append(config.__openllm_url__)
         formatted["GPU"].append("✅")
         formatted["CPU"].append("✅" if not config.__openllm_requires_gpu__ else "❌")
+        formatted["Model Ids"].append(config.__openllm_model_ids__)
         if dashed in deps:
             instruction = f'```bash\npip install "openllm[{dashed}]"\n```'
         else:
             instruction = "```bash\npip install openllm\n```"
         if len(instruction) > max_install_len_div:
             max_install_len_div = len(instruction)
         formatted["Installation"].append(instruction)
@@ -63,26 +65,27 @@
     meta: list[str] = ["\n", "<table align='center'>\n"]
 
     # NOTE: headers
     meta += ["<tr>\n"]
     meta.extend([f"<th>{header}</th>\n" for header in formatted.keys() if header not in ("URL",)])
     meta += ["</tr>\n"]
     # NOTE: rows
-    for name, url, cpu, gpu, installation in t.cast(
-        t.Iterable[t.Tuple[str, str, str, str, str]], zip(*formatted.values())
+    for name, url, cpu, gpu, installation, model_ids in t.cast(
+        t.Iterable[t.Tuple[str, str, str, str, str, str]], zip(*formatted.values())
     ):
         meta += "<tr>\n"
         meta.extend(
             [
                 f"\n<td><a href={url}>{name}</a></td>\n",
                 f"<td>{cpu}</td>\n",
                 f"<td>{gpu}</td>\n",
                 f"<td>\n\n{installation}\n\n</td>\n",
             ]
         )
+        meta.append("<td>\n\n" + "\n".join(["<li><code>" + lid + "</code></li>" for lid in model_ids]) + "\n\n</td>\n")
         meta += "</tr>\n"
     meta.extend(["</table>\n", "\n"])
 
     readme = readme[:start_index] + [START_COMMENT] + meta + [END_COMMENT] + readme[stop_index + 1 :]
 
     with open(os.path.join(ROOT, "README.md"), "w") as f:
         f.writelines(readme)
```

### Comparing `openllm-0.1.1/typings/attr/__init__.pyi` & `openllm-0.1.2/typings/attr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/typings/attr/exceptions.pyi` & `openllm-0.1.2/typings/attr/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/typings/attr/validators.pyi` & `openllm-0.1.2/typings/attr/validators.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/typings/click_option_group/__init__.pyi` & `openllm-0.1.2/typings/click_option_group/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/typings/click_option_group/_core.pyi` & `openllm-0.1.2/typings/click_option_group/_core.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/typings/click_option_group/_decorators.pyi` & `openllm-0.1.2/typings/click_option_group/_decorators.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/typings/click_option_group/_helpers.pyi` & `openllm-0.1.2/typings/click_option_group/_helpers.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/typings/deepmerge/merger.pyi` & `openllm-0.1.2/typings/deepmerge/merger.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/typings/deepmerge/strategy/core.pyi` & `openllm-0.1.2/typings/deepmerge/strategy/core.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/typings/deepmerge/strategy/set.pyi` & `openllm-0.1.2/typings/deepmerge/strategy/set.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/.gitignore` & `openllm-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/LICENSE.md` & `openllm-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.1/README.md` & `openllm-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,14 @@
         <img src="https://badgen.net/badge/icon/OpenLLM/7289da?icon=discord&label=Join%20Us" alt="Discord" />
     </a><br>
     <p>An open platform for operating large language models(LLMs) in production.</br>
     Fine-tune, serve, deploy, and monitor any LLMs with ease.</p>
     <i></i>
 </div>
 
-
 ## 📖 Introduction
 
 With OpenLLM, you can run inference with any open-source large-language
 models(LLMs), deploy to the cloud or on-premises, and build powerful AI apps.
 
 🚂 **SOTA LLMs**: built-in supports a wide range of open-source LLMs and model
 runtime, including StableLM, Falcon, Dolly, Flan-T5, ChatGLM, StarCoder and
@@ -27,24 +26,24 @@
 🔥 **Flexible APIs**: serve LLMs over RESTful API or gRPC with one command,
 query via WebUI, CLI, our Python/Javascript client, or any HTTP client.
 
 ⛓️ **Freedom To Build**: First-class support for LangChain and BentoML allows you
 to easily create your own AI apps by composing LLMs with other models and
 services.
 
-🎯 **Streamline Deployment**: Automatically generate your LLM server Docker Images or
-deploy as serverless endpoint via [☁️ BentoCloud](https://l.bentoml.com/bento-cloud).
+🎯 **Streamline Deployment**: Automatically generate your LLM server Docker
+Images or deploy as serverless endpoint via
+[☁️ BentoCloud](https://l.bentoml.com/bento-cloud).
 
 🤖️ **Bring your own LLM**: Fine-tune any LLM to suit your needs with
 `LLM.tuning()`. (Coming soon)
 
 ![Gif showing OpenLLM Intro](/assets/output.gif)
 <br/>
 
-
 ## 🏃‍ Getting Started
 
 To use OpenLLM, you need to have Python 3.8 (or newer) and `pip` installed on
 your system. We highly recommend using a Virtual Environment to prevent package
 conflicts.
 
 You can install OpenLLM using pip as follows:
@@ -76,16 +75,16 @@
 To start an LLM server, use `openllm start`. For example, to start a `dolly-v2`
 server:
 
 ```bash
 openllm start dolly-v2
 ```
 
-Following this, a Web UI will be accessible at http://0.0.0.0:3000 where you can
-experiment with the endpoints and sample input prompts.
+Following this, a Web UI will be accessible at http://localhost:3000 where you
+can experiment with the endpoints and sample input prompts.
 
 OpenLLM provides a built-in Python client, allowing you to interact with the
 model. In a different terminal window or a Jupyter notebook, create a client to
 start interacting with the model:
 
 ```python
 >>> import openllm
@@ -97,26 +96,25 @@
 terminal:
 
 ```bash
 export OPENLLM_ENDPOINT=http://localhost:3000
 openllm query 'Explain to me the difference between "further" and "farther"'
 ```
 
-Visit `http://0.0.0.0:3000/docs.json` for OpenLLM's API specification.
+Visit `http://localhost:3000/docs.json` for OpenLLM's API specification.
 
-Users can also specify different variants of the model to be served, by providing the 
-`--model-id` argument, e.g.:
+Users can also specify different variants of the model to be served, by
+providing the `--model-id` argument, e.g.:
 
 ```bash
 openllm start flan-t5 --model-id google/flan-t5-large
 ```
 
-Use the `openllm models` command to see the list of models and their variants supported 
-in OpenLLM.
-
+Use the `openllm models` command to see the list of models and their variants
+supported in OpenLLM.
 
 ## 🧩 Supported Models
 
 The following models are currently supported in OpenLLM. By default, OpenLLM
 doesn't include dependencies to run all models. The extra model-specific
 dependencies can be installed with the instructions below:
 
@@ -124,92 +122,138 @@
 
 <table align='center'>
 <tr>
 <th>Model</th>
 <th>CPU</th>
 <th>GPU</th>
 <th>Installation</th>
+<th>Model Ids</th>
 </tr>
 <tr>
 
 <td><a href=https://huggingface.co/docs/transformers/model_doc/flan-t5>flan-t5</a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
 ```bash
 pip install "openllm[flan-t5]"
 ```
 
 </td>
+<td>
+
+<li><code>google/flan-t5-small</code></li>
+<li><code>google/flan-t5-base</code></li>
+<li><code>google/flan-t5-large</code></li>
+<li><code>google/flan-t5-xl</code></li>
+<li><code>google/flan-t5-xxl</code></li>
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/databrickslabs/dolly>dolly-v2</a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
 ```bash
 pip install openllm
 ```
 
 </td>
+<td>
+
+<li><code>databricks/dolly-v2-3b</code></li>
+<li><code>databricks/dolly-v2-7b</code></li>
+<li><code>databricks/dolly-v2-12b</code></li>
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/THUDM/ChatGLM-6B>chatglm</a></td>
 <td>❌</td>
 <td>✅</td>
 <td>
 
 ```bash
 pip install "openllm[chatglm]"
 ```
 
 </td>
+<td>
+
+<li><code>thudm/chatglm-6b</code></li>
+<li><code>thudm/chatglm-6b-int8</code></li>
+<li><code>thudm/chatglm-6b-int4</code></li>
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/bigcode-project/starcoder>starcoder</a></td>
 <td>❌</td>
 <td>✅</td>
 <td>
 
 ```bash
 pip install "openllm[starcoder]"
 ```
 
 </td>
+<td>
+
+<li><code>bigcode/starcoder</code></li>
+<li><code>bigcode/starcoderbase</code></li>
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://falconllm.tii.ae/>falcon</a></td>
 <td>❌</td>
 <td>✅</td>
 <td>
 
 ```bash
 pip install "openllm[falcon]"
 ```
 
 </td>
+<td>
+
+<li><code>tiiuae/falcon-7b</code></li>
+<li><code>tiiuae/falcon-40b</code></li>
+<li><code>tiiuae/falcon-7b-instruct</code></li>
+<li><code>tiiuae/falcon-40b-instruct</code></li>
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/Stability-AI/StableLM>stablelm</a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
 ```bash
 pip install openllm
 ```
 
 </td>
+<td>
+
+<li><code>stabilityai/stablelm-tuned-alpha-3b</code></li>
+<li><code>stabilityai/stablelm-tuned-alpha-7b</code></li>
+<li><code>stabilityai/stablelm-base-alpha-3b</code></li>
+<li><code>stabilityai/stablelm-base-alpha-7b</code></li>
+
+</td>
 </tr>
 </table>
 
 <!-- update-readme.py: stop -->
 
 ### Runtime Implementations (Experimental)
```

#### html2text {}

```diff
@@ -35,38 +35,57 @@
 âââ âââ âââââââ âââ
 âââââââââââ
 ââââââââââââââââââââââââ
 âââ An open platform for operating large language models in production.
 Fine-tune, serve, deploy, and monitor any LLMs with ease. ``` ### Starting an
 LLM Server To start an LLM server, use `openllm start`. For example, to start a
 `dolly-v2` server: ```bash openllm start dolly-v2 ``` Following this, a Web UI
-will be accessible at http://0.0.0.0:3000 where you can experiment with the
+will be accessible at http://localhost:3000 where you can experiment with the
 endpoints and sample input prompts. OpenLLM provides a built-in Python client,
 allowing you to interact with the model. In a different terminal window or a
 Jupyter notebook, create a client to start interacting with the model:
 ```python >>> import openllm >>> client = openllm.client.HTTPClient('http://
 localhost:3000') >>> client.query('Explain to me the difference between
 "further" and "farther"') ``` You can also use the `openllm query` command to
 query the model from the terminal: ```bash export OPENLLM_ENDPOINT=http://
 localhost:3000 openllm query 'Explain to me the difference between "further"
-and "farther"' ``` Visit `http://0.0.0.0:3000/docs.json` for OpenLLM's API
+and "farther"' ``` Visit `http://localhost:3000/docs.json` for OpenLLM's API
 specification. Users can also specify different variants of the model to be
 served, by providing the `--model-id` argument, e.g.: ```bash openllm start
 flan-t5 --model-id google/flan-t5-large ``` Use the `openllm models` command to
 see the list of models and their variants supported in OpenLLM. ## ð§©
 Supported Models The following models are currently supported in OpenLLM. By
 default, OpenLLM doesn't include dependencies to run all models. The extra
 model-specific dependencies can be installed with the instructions below:
-        Model     CPU GPU Installation
-        flan-t5   ââ```bash pip install "openllm[flan-t5]" ```
-        dolly-v2  ââ```bash pip install openllm ```
-        chatglm   ââ```bash pip install "openllm[chatglm]" ```
-        starcoder ââ```bash pip install "openllm[starcoder]" ```
-        falcon    ââ```bash pip install "openllm[falcon]" ```
-        stablelm  ââ```bash pip install openllm ```
+ Model     CPU GPU Installation                    Model Ids
+                                                   google/flan-t5-small
+                   ```bash pip install "openllm    google/flan-t5-base
+ flan-t5   ââ[flan-t5]" ```                  google/flan-t5-large
+                                                   google/flan-t5-xl
+                                                   google/flan-t5-xxl
+                                                   databricks/dolly-v2-3b
+ dolly-v2  ââ```bash pip install openllm ``` databricks/dolly-v2-7b
+                                                   databricks/dolly-v2-12b
+                   ```bash pip install "openllm    thudm/chatglm-6b
+ chatglm   ââ[chatglm]" ```                  thudm/chatglm-6b-int8
+                                                   thudm/chatglm-6b-int4
+ starcoder ââ```bash pip install "openllm    bigcode/starcoder
+                   [starcoder]" ```                bigcode/starcoderbase
+                                                   tiiuae/falcon-7b
+ falcon    ââ```bash pip install "openllm    tiiuae/falcon-40b
+                   [falcon]" ```                   tiiuae/falcon-7b-instruct
+                                                   tiiuae/falcon-40b-instruct
+                                                   stabilityai/stablelm-tuned-
+                                                   alpha-3b
+                                                   stabilityai/stablelm-tuned-
+ stablelm  ââ```bash pip install openllm ``` alpha-7b
+                                                   stabilityai/stablelm-base-
+                                                   alpha-3b
+                                                   stabilityai/stablelm-base-
+                                                   alpha-7b
  ### Runtime Implementations (Experimental) Different LLMs may have multiple
 runtime implementations. For instance, they might use Pytorch (`pt`),
 Tensorflow (`tf`), or Flax (`flax`). If you wish to specify a particular
 runtime for a model, you can do so by setting the `OPENLLM_
 {MODEL_NAME}_FRAMEWORK={runtime}` environment variable before running `openllm
 start`. For example, if you want to use the Tensorflow (`tf`) implementation
 for the `flan-t5` model, you can use the following command: ```bash
```

### Comparing `openllm-0.1.1/pyproject.toml` & `openllm-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -72,17 +72,17 @@
 chatglm = ["cpm_kernels", "sentencepiece"]
 falcon = ["einops", "xformers", "safetensors"]
 fine-tune = ["peft", "bitsandbytes", "datasets", "accelerate"]
 flan-t5 = ["flax", "jax", "jaxlib", "tensorflow", "keras"]
 starcoder = ["bitsandbytes"]
 
 [project.urls]
-Documentation = "https://github.com/llmsys/openllm#readme"
-Issues = "https://github.com/llmsys/openllm/issues"
-Source = "https://github.com/llmsys/openllm"
+Documentation = "https://github.com/bentoml/openllm#readme"
+Issues = "https://github.com/bentoml/openllm/issues"
+Source = "https://github.com/bentoml/openllm"
 
 [project.scripts]
 openllm = "openllm.cli:cli"
 
 [tool.hatch.version]
 path = "src/openllm/__about__.py"
```

### Comparing `openllm-0.1.1/PKG-INFO` & `openllm-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.1.1
+Version: 0.1.2
 Summary: OpenLLM: REST/gRPC API server for running any open Large-Language Model - StableLM, Llama, Alpaca, Dolly, Flan-T5, Custom
-Project-URL: Documentation, https://github.com/llmsys/openllm#readme
-Project-URL: Issues, https://github.com/llmsys/openllm/issues
-Project-URL: Source, https://github.com/llmsys/openllm
+Project-URL: Documentation, https://github.com/bentoml/openllm#readme
+Project-URL: Issues, https://github.com/bentoml/openllm/issues
+Project-URL: Source, https://github.com/bentoml/openllm
 Author-email: Aaron Pham <aarnphm@bentoml.com>, BentoML Team <contact@bentoml.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.md
 Keywords: AI,Alpaca,BentoML,Generative AI,LLMOps,Large Language Model,MLOps,Model Deployment,Model Serving,PyTorch,Stable Diffusion,StableLM,Transformers
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -74,15 +74,14 @@
         <img src="https://badgen.net/badge/icon/OpenLLM/7289da?icon=discord&label=Join%20Us" alt="Discord" />
     </a><br>
     <p>An open platform for operating large language models(LLMs) in production.</br>
     Fine-tune, serve, deploy, and monitor any LLMs with ease.</p>
     <i></i>
 </div>
 
-
 ## 📖 Introduction
 
 With OpenLLM, you can run inference with any open-source large-language
 models(LLMs), deploy to the cloud or on-premises, and build powerful AI apps.
 
 🚂 **SOTA LLMs**: built-in supports a wide range of open-source LLMs and model
 runtime, including StableLM, Falcon, Dolly, Flan-T5, ChatGLM, StarCoder and
@@ -91,24 +90,24 @@
 🔥 **Flexible APIs**: serve LLMs over RESTful API or gRPC with one command,
 query via WebUI, CLI, our Python/Javascript client, or any HTTP client.
 
 ⛓️ **Freedom To Build**: First-class support for LangChain and BentoML allows you
 to easily create your own AI apps by composing LLMs with other models and
 services.
 
-🎯 **Streamline Deployment**: Automatically generate your LLM server Docker Images or
-deploy as serverless endpoint via [☁️ BentoCloud](https://l.bentoml.com/bento-cloud).
+🎯 **Streamline Deployment**: Automatically generate your LLM server Docker
+Images or deploy as serverless endpoint via
+[☁️ BentoCloud](https://l.bentoml.com/bento-cloud).
 
 🤖️ **Bring your own LLM**: Fine-tune any LLM to suit your needs with
 `LLM.tuning()`. (Coming soon)
 
 ![Gif showing OpenLLM Intro](/assets/output.gif)
 <br/>
 
-
 ## 🏃‍ Getting Started
 
 To use OpenLLM, you need to have Python 3.8 (or newer) and `pip` installed on
 your system. We highly recommend using a Virtual Environment to prevent package
 conflicts.
 
 You can install OpenLLM using pip as follows:
@@ -140,16 +139,16 @@
 To start an LLM server, use `openllm start`. For example, to start a `dolly-v2`
 server:
 
 ```bash
 openllm start dolly-v2
 ```
 
-Following this, a Web UI will be accessible at http://0.0.0.0:3000 where you can
-experiment with the endpoints and sample input prompts.
+Following this, a Web UI will be accessible at http://localhost:3000 where you
+can experiment with the endpoints and sample input prompts.
 
 OpenLLM provides a built-in Python client, allowing you to interact with the
 model. In a different terminal window or a Jupyter notebook, create a client to
 start interacting with the model:
 
 ```python
 >>> import openllm
@@ -161,26 +160,25 @@
 terminal:
 
 ```bash
 export OPENLLM_ENDPOINT=http://localhost:3000
 openllm query 'Explain to me the difference between "further" and "farther"'
 ```
 
-Visit `http://0.0.0.0:3000/docs.json` for OpenLLM's API specification.
+Visit `http://localhost:3000/docs.json` for OpenLLM's API specification.
 
-Users can also specify different variants of the model to be served, by providing the 
-`--model-id` argument, e.g.:
+Users can also specify different variants of the model to be served, by
+providing the `--model-id` argument, e.g.:
 
 ```bash
 openllm start flan-t5 --model-id google/flan-t5-large
 ```
 
-Use the `openllm models` command to see the list of models and their variants supported 
-in OpenLLM.
-
+Use the `openllm models` command to see the list of models and their variants
+supported in OpenLLM.
 
 ## 🧩 Supported Models
 
 The following models are currently supported in OpenLLM. By default, OpenLLM
 doesn't include dependencies to run all models. The extra model-specific
 dependencies can be installed with the instructions below:
 
@@ -188,92 +186,138 @@
 
 <table align='center'>
 <tr>
 <th>Model</th>
 <th>CPU</th>
 <th>GPU</th>
 <th>Installation</th>
+<th>Model Ids</th>
 </tr>
 <tr>
 
 <td><a href=https://huggingface.co/docs/transformers/model_doc/flan-t5>flan-t5</a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
 ```bash
 pip install "openllm[flan-t5]"
 ```
 
 </td>
+<td>
+
+<li><code>google/flan-t5-small</code></li>
+<li><code>google/flan-t5-base</code></li>
+<li><code>google/flan-t5-large</code></li>
+<li><code>google/flan-t5-xl</code></li>
+<li><code>google/flan-t5-xxl</code></li>
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/databrickslabs/dolly>dolly-v2</a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
 ```bash
 pip install openllm
 ```
 
 </td>
+<td>
+
+<li><code>databricks/dolly-v2-3b</code></li>
+<li><code>databricks/dolly-v2-7b</code></li>
+<li><code>databricks/dolly-v2-12b</code></li>
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/THUDM/ChatGLM-6B>chatglm</a></td>
 <td>❌</td>
 <td>✅</td>
 <td>
 
 ```bash
 pip install "openllm[chatglm]"
 ```
 
 </td>
+<td>
+
+<li><code>thudm/chatglm-6b</code></li>
+<li><code>thudm/chatglm-6b-int8</code></li>
+<li><code>thudm/chatglm-6b-int4</code></li>
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/bigcode-project/starcoder>starcoder</a></td>
 <td>❌</td>
 <td>✅</td>
 <td>
 
 ```bash
 pip install "openllm[starcoder]"
 ```
 
 </td>
+<td>
+
+<li><code>bigcode/starcoder</code></li>
+<li><code>bigcode/starcoderbase</code></li>
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://falconllm.tii.ae/>falcon</a></td>
 <td>❌</td>
 <td>✅</td>
 <td>
 
 ```bash
 pip install "openllm[falcon]"
 ```
 
 </td>
+<td>
+
+<li><code>tiiuae/falcon-7b</code></li>
+<li><code>tiiuae/falcon-40b</code></li>
+<li><code>tiiuae/falcon-7b-instruct</code></li>
+<li><code>tiiuae/falcon-40b-instruct</code></li>
+
+</td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/Stability-AI/StableLM>stablelm</a></td>
 <td>✅</td>
 <td>✅</td>
 <td>
 
 ```bash
 pip install openllm
 ```
 
 </td>
+<td>
+
+<li><code>stabilityai/stablelm-tuned-alpha-3b</code></li>
+<li><code>stabilityai/stablelm-tuned-alpha-7b</code></li>
+<li><code>stabilityai/stablelm-base-alpha-3b</code></li>
+<li><code>stabilityai/stablelm-base-alpha-7b</code></li>
+
+</td>
 </tr>
 </table>
 
 <!-- update-readme.py: stop -->
 
 ### Runtime Implementations (Experimental)
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-Metadata-Version: 2.1 Name: openllm Version: 0.1.1 Summary: OpenLLM: REST/gRPC
+Metadata-Version: 2.1 Name: openllm Version: 0.1.2 Summary: OpenLLM: REST/gRPC
 API server for running any open Large-Language Model - StableLM, Llama, Alpaca,
-Dolly, Flan-T5, Custom Project-URL: Documentation, https://github.com/llmsys/
-openllm#readme Project-URL: Issues, https://github.com/llmsys/openllm/issues
-Project-URL: Source, https://github.com/llmsys/openllm Author-email: Aaron Pham
+Dolly, Flan-T5, Custom Project-URL: Documentation, https://github.com/bentoml/
+openllm#readme Project-URL: Issues, https://github.com/bentoml/openllm/issues
+Project-URL: Source, https://github.com/bentoml/openllm Author-email: Aaron
+Pham
 bentoml.com>, BentoML Team
 bentoml.com> License-Expression: Apache-2.0 License-File: LICENSE.md Keywords:
 AI,Alpaca,BentoML,Generative AI,LLMOps,Large Language Model,MLOps,Model
 Deployment,Model Serving,PyTorch,Stable Diffusion,StableLM,Transformers
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
@@ -73,38 +74,57 @@
 âââ âââ âââââââ âââ
 âââââââââââ
 ââââââââââââââââââââââââ
 âââ An open platform for operating large language models in production.
 Fine-tune, serve, deploy, and monitor any LLMs with ease. ``` ### Starting an
 LLM Server To start an LLM server, use `openllm start`. For example, to start a
 `dolly-v2` server: ```bash openllm start dolly-v2 ``` Following this, a Web UI
-will be accessible at http://0.0.0.0:3000 where you can experiment with the
+will be accessible at http://localhost:3000 where you can experiment with the
 endpoints and sample input prompts. OpenLLM provides a built-in Python client,
 allowing you to interact with the model. In a different terminal window or a
 Jupyter notebook, create a client to start interacting with the model:
 ```python >>> import openllm >>> client = openllm.client.HTTPClient('http://
 localhost:3000') >>> client.query('Explain to me the difference between
 "further" and "farther"') ``` You can also use the `openllm query` command to
 query the model from the terminal: ```bash export OPENLLM_ENDPOINT=http://
 localhost:3000 openllm query 'Explain to me the difference between "further"
-and "farther"' ``` Visit `http://0.0.0.0:3000/docs.json` for OpenLLM's API
+and "farther"' ``` Visit `http://localhost:3000/docs.json` for OpenLLM's API
 specification. Users can also specify different variants of the model to be
 served, by providing the `--model-id` argument, e.g.: ```bash openllm start
 flan-t5 --model-id google/flan-t5-large ``` Use the `openllm models` command to
 see the list of models and their variants supported in OpenLLM. ## ð§©
 Supported Models The following models are currently supported in OpenLLM. By
 default, OpenLLM doesn't include dependencies to run all models. The extra
 model-specific dependencies can be installed with the instructions below:
-        Model     CPU GPU Installation
-        flan-t5   ââ```bash pip install "openllm[flan-t5]" ```
-        dolly-v2  ââ```bash pip install openllm ```
-        chatglm   ââ```bash pip install "openllm[chatglm]" ```
-        starcoder ââ```bash pip install "openllm[starcoder]" ```
-        falcon    ââ```bash pip install "openllm[falcon]" ```
-        stablelm  ââ```bash pip install openllm ```
+ Model     CPU GPU Installation                    Model Ids
+                                                   google/flan-t5-small
+                   ```bash pip install "openllm    google/flan-t5-base
+ flan-t5   ââ[flan-t5]" ```                  google/flan-t5-large
+                                                   google/flan-t5-xl
+                                                   google/flan-t5-xxl
+                                                   databricks/dolly-v2-3b
+ dolly-v2  ââ```bash pip install openllm ``` databricks/dolly-v2-7b
+                                                   databricks/dolly-v2-12b
+                   ```bash pip install "openllm    thudm/chatglm-6b
+ chatglm   ââ[chatglm]" ```                  thudm/chatglm-6b-int8
+                                                   thudm/chatglm-6b-int4
+ starcoder ââ```bash pip install "openllm    bigcode/starcoder
+                   [starcoder]" ```                bigcode/starcoderbase
+                                                   tiiuae/falcon-7b
+ falcon    ââ```bash pip install "openllm    tiiuae/falcon-40b
+                   [falcon]" ```                   tiiuae/falcon-7b-instruct
+                                                   tiiuae/falcon-40b-instruct
+                                                   stabilityai/stablelm-tuned-
+                                                   alpha-3b
+                                                   stabilityai/stablelm-tuned-
+ stablelm  ââ```bash pip install openllm ``` alpha-7b
+                                                   stabilityai/stablelm-base-
+                                                   alpha-3b
+                                                   stabilityai/stablelm-base-
+                                                   alpha-7b
  ### Runtime Implementations (Experimental) Different LLMs may have multiple
 runtime implementations. For instance, they might use Pytorch (`pt`),
 Tensorflow (`tf`), or Flax (`flax`). If you wish to specify a particular
 runtime for a model, you can do so by setting the `OPENLLM_
 {MODEL_NAME}_FRAMEWORK={runtime}` environment variable before running `openllm
 start`. For example, if you want to use the Tensorflow (`tf`) implementation
 for the `flan-t5` model, you can use the following command: ```bash
```

