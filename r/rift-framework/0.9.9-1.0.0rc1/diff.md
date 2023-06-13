# Comparing `tmp/rift-framework-0.9.9.tar.gz` & `tmp/rift-framework-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rift-framework-0.9.9.tar", max compression
+gzip compressed data, was "rift-framework-1.0.0rc1.tar", max compression
```

## Comparing `rift-framework-0.9.9.tar` & `rift-framework-1.0.0rc1.tar`

### file list

```diff
@@ -1,179 +1,198 @@
--rw-r--r--   0        0        0     1085 2023-02-07 08:30:44.988937 rift-framework-0.9.9/LICENSE
--rw-r--r--   0        0        0     4320 2023-02-07 08:30:44.988937 rift-framework-0.9.9/README.md
--rw-r--r--   0        0        0      796 2023-02-07 08:30:44.992937 rift-framework-0.9.9/pyproject.toml
--rw-r--r--   0        0        0      177 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/__init__.py
--rw-r--r--   0        0        0      199 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/__init__.py
--rw-r--r--   0        0        0      276 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/ast.py
--rw-r--r--   0        0        0      745 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/ast_patcher.py
--rw-r--r--   0        0        0      817 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/bool_dict.py
--rw-r--r--   0        0        0     3576 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/calls.py
--rw-r--r--   0        0        0      393 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/compiled_contract.py
--rw-r--r--   0        0        0      752 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/int_dict.py
--rw-r--r--   0        0        0      456 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/patchers/__init__.py
--rw-r--r--   0        0        0      694 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/patchers/assert_patcher.py
--rw-r--r--   0        0        0     5491 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/patchers/assign_patcher.py
--rw-r--r--   0        0        0      571 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/patchers/break_patcher.py
--rw-r--r--   0        0        0     2133 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/patchers/if_patcher.py
--rw-r--r--   0        0        0      579 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/patchers/raise_patcher.py
--rw-r--r--   0        0        0      675 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/patchers/return_patcher.py
--rw-r--r--   0        0        0      453 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/patchers/unary_patcher.py
--rw-r--r--   0        0        0      686 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/patchers/while_patcher.py
--rw-r--r--   0        0        0      544 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/printer.py
--rw-r--r--   0        0        0     1141 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/ref_table.py
--rw-r--r--   0        0        0      393 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/types/__init__.py
--rw-r--r--   0        0        0     2675 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/types/asm_method.py
--rw-r--r--   0        0        0     1086 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/types/block.py
--rw-r--r--   0        0        0     1891 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/types/condition.py
--rw-r--r--   0        0        0       71 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/types/const.py
--rw-r--r--   0        0        0     1154 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/types/contract.py
--rw-r--r--   0        0        0      336 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/types/control_flow.py
--rw-r--r--   0        0        0     3154 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/types/expr.py
--rw-r--r--   0        0        0      713 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/types/loop.py
--rw-r--r--   0        0        0     2287 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/types/method.py
--rw-r--r--   0        0        0      581 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/types/node.py
--rw-r--r--   0        0        0     4368 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/types/statement.py
--rw-r--r--   0        0        0      811 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/ast/utils.py
--rw-r--r--   0        0        0       58 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/bases/__init__.py
--rw-r--r--   0        0        0      202 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/bases/bare.py
--rw-r--r--   0        0        0      382 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/bases/util.py
--rw-r--r--   0        0        0       68 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cli/__init__.py
--rw-r--r--   0        0        0      166 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cli/commands/__init__.py
--rw-r--r--   0        0        0     1421 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cli/commands/build.py
--rw-r--r--   0        0        0     2669 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cli/commands/deploy.py
--rw-r--r--   0        0        0     1269 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cli/commands/init.py
--rw-r--r--   0        0        0     4743 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cli/commands/test.py
--rw-r--r--   0        0        0     7931 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cli/commands/utils.py
--rw-r--r--   0        0        0     2023 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cli/config.py
--rw-r--r--   0        0        0       52 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cli/entry.py
--rw-r--r--   0        0        0       56 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cli/util/__init__.py
--rw-r--r--   0        0        0      270 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cli/util/dag.py
--rw-r--r--   0        0        0     1291 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cli/util/dir_helper.py
--rw-r--r--   0        0        0      451 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cli/util/dir_util.py
--rw-r--r--   0        0        0       78 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cli/util/git.py
--rw-r--r--   0        0        0      276 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/core/__init__.py
--rw-r--r--   0        0        0     6415 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/core/annots.py
--rw-r--r--   0        0        0     1158 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/core/condition.py
--rw-r--r--   0        0        0     4981 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/core/entity.py
--rw-r--r--   0        0        0      245 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/core/factory.py
--rw-r--r--   0        0        0     2726 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/core/invokable.py
--rw-r--r--   0        0        0      632 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/core/loop.py
--rw-r--r--   0        0        0      214 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/core/mark.py
--rw-r--r--   0        0        0     1486 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/core/utils.py
--rw-r--r--   0        0        0        0 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cst/__init__.py
--rw-r--r--   0        0        0      331 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cst/cst_patcher.py
--rw-r--r--   0        0        0      547 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cst/cst_visitor.py
--rw-r--r--   0        0        0     2007 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cst/import_visitor.py
--rw-r--r--   0        0        0      583 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/cst/int_visitor.py
--rw-r--r--   0        0        0      298 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/__init__.py
--rw-r--r--   0        0        0    12542 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/bundled_fc.py
--rw-r--r--   0        0        0    36807 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/bundled_libs.py
--rw-r--r--   0        0        0     1404 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/contract.py
--rw-r--r--   0        0        0     5047 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/fift.py
--rw-r--r--   0        0        0      553 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/fift_behavior.py
--rw-r--r--   0        0        0     2814 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/func.py
--rw-r--r--   0        0        0     3328 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/test_result.py
--rw-r--r--   0        0        0     3807 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/tvm.py
--rw-r--r--   0        0        0      280 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/types/__init__.py
--rw-r--r--   0        0        0     1321 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/types/_fift_base.py
--rw-r--r--   0        0        0     2147 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/types/builder.py
--rw-r--r--   0        0        0     1300 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/types/bytes.py
--rw-r--r--   0        0        0     2067 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/types/cell.py
--rw-r--r--   0        0        0      967 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/types/dict.py
--rw-r--r--   0        0        0      384 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/types/factory.py
--rw-r--r--   0        0        0      762 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/types/int.py
--rw-r--r--   0        0        0      611 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/types/null.py
--rw-r--r--   0        0        0     3638 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/types/slice.py
--rw-r--r--   0        0        0      457 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/types/string.py
--rw-r--r--   0        0        0     1478 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/types/tuple.py
--rw-r--r--   0        0        0      385 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/types/util.py
--rw-r--r--   0        0        0     3352 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/fift/utils.py
--rw-r--r--   0        0        0      114 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/__init__.py
--rw-r--r--   0        0        0     4548 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/contract.py
--rw-r--r--   0        0        0     7712 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/engine.py
--rw-r--r--   0        0        0      211 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/func_behavior.py
--rw-r--r--   0        0        0      503 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/library.py
--rw-r--r--   0        0        0     1369 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/meta_contract.py
--rw-r--r--   0        0        0        0 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/types/__init__.py
--rw-r--r--   0        0        0     3393 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/types/builder_base.py
--rw-r--r--   0        0        0     1820 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/types/cell_base.py
--rw-r--r--   0        0        0       93 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/types/cont_base.py
--rw-r--r--   0        0        0     2278 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/types/dict_base.py
--rw-r--r--   0        0        0      847 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/types/entity_base.py
--rw-r--r--   0        0        0     6076 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/types/idict_base.py
--rw-r--r--   0        0        0       92 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/types/int_base.py
--rw-r--r--   0        0        0     1470 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/types/pfxdict_base.py
--rw-r--r--   0        0        0     4497 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/types/slice_base.py
--rw-r--r--   0        0        0       95 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/types/string_base.py
--rw-r--r--   0        0        0     4179 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/types/types.py
--rw-r--r--   0        0        0     6088 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/types/udict_base.py
--rw-r--r--   0        0        0      292 2023-02-07 08:30:44.992937 rift-framework-0.9.9/rift/func/util.py
--rw-r--r--   0        0        0       75 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/keys/__init__.py
--rw-r--r--   0        0        0     1951 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/keys/key_pair.py
--rw-r--r--   0        0        0      690 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/keys/mnemonic/__init__.py
--rw-r--r--   0        0        0       92 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/keys/mnemonic/bip39/__init__.py
--rw-r--r--   0        0        0    27464 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/keys/mnemonic/bip39/english.py
--rw-r--r--   0        0        0       49 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/keys/mnemonic/exceptions.py
--rw-r--r--   0        0        0      622 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/keys/mnemonic/keystore.py
--rw-r--r--   0        0        0     1948 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/keys/mnemonic/mnemonic.py
--rw-r--r--   0        0        0       26 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/keys/mnemonic/settings.py
--rw-r--r--   0        0        0     1070 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/keys/mnemonic/utils.py
--rw-r--r--   0        0        0       23 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/keys/signer.py
--rw-r--r--   0        0        0       80 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/library/__init__.py
--rw-r--r--   0        0        0      403 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/library/rstd.py
--rw-r--r--   0        0        0    27617 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/library/std.py
--rw-r--r--   0        0        0      125 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/logging/__init__.py
--rw-r--r--   0        0        0      110 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/logging/error.py
--rw-r--r--   0        0        0     2961 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/logging/logger.py
--rw-r--r--   0        0        0        0 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/meta/__init__.py
--rw-r--r--   0        0        0     7367 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/meta/behaviors.py
--rw-r--r--   0        0        0     2020 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/meta/meta_inheritance.py
--rw-r--r--   0        0        0      323 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/meta/utils.py
--rw-r--r--   0        0        0       96 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/native/__init__.py
--rw-r--r--   0        0        0      291 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/native/c_annot.py
--rw-r--r--   0        0        0     1215 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/native/c_call.py
--rw-r--r--   0        0        0       96 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/network/__init__.py
--rw-r--r--   0        0        0      960 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/network/account.py
--rw-r--r--   0        0        0      966 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/network/config.py
--rw-r--r--   0        0        0     4115 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/network/network.py
--rw-r--r--   0        0        0     2945 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/network/servers.py
--rw-r--r--   0        0        0      604 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/network/util.py
--rw-r--r--   0        0        0        0 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/runtime/config.py
--rw-r--r--   0        0        0     5469 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/runtime/keystore.py
--rw-r--r--   0        0        0     3824 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/runtime/riftlib.py
--rw-r--r--   0        0        0      900 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/__init__.py
--rw-r--r--   0        0        0     2323 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/addr.py
--rw-r--r--   0        0        0      285 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/bases/__init__.py
--rw-r--r--   0        0        0     1103 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/bases/builder.py
--rw-r--r--   0        0        0       88 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/bases/bytes.py
--rw-r--r--   0        0        0      483 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/bases/cell.py
--rw-r--r--   0        0        0      182 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/bases/dict.py
--rw-r--r--   0        0        0      174 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/bases/int.py
--rw-r--r--   0        0        0     2725 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/bases/slice.py
--rw-r--r--   0        0        0      198 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/bases/string.py
--rw-r--r--   0        0        0      733 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/bool.py
--rw-r--r--   0        0        0      874 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/coin.py
--rw-r--r--   0        0        0     2209 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/constructor.py
--rw-r--r--   0        0        0      978 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/contract_dep.py
--rw-r--r--   0        0        0     3471 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/either.py
--rw-r--r--   0        0        0     4346 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/either_ref.py
--rw-r--r--   0        0        0     1060 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/helpers.py
--rw-r--r--   0        0        0    12667 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/int_aliases.py
--rw-r--r--   0        0        0     3349 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/maybe.py
--rw-r--r--   0        0        0     4077 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/model.py
--rw-r--r--   0        0        0     5239 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/msg.py
--rw-r--r--   0        0        0     8661 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/payload.py
--rw-r--r--   0        0        0     2990 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/ref.py
--rw-r--r--   0        0        0      850 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/signed_payload.py
--rw-r--r--   0        0        0     1627 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/sized_int.py
--rw-r--r--   0        0        0     1115 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/slice.py
--rw-r--r--   0        0        0      690 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/types/utils.py
--rw-r--r--   0        0        0       38 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/util/__init__.py
--rw-r--r--   0        0        0      169 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/util/dump.py
--rw-r--r--   0        0        0      270 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/util/type_id.py
--rw-r--r--   0        0        0        0 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/wallet/__init__.py
--rw-r--r--   0        0        0     1989 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/wallet/wallet_base.py
--rw-r--r--   0        0        0     2018 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/wallet/wallet_manager.py
--rw-r--r--   0        0        0     1682 2023-02-07 08:30:44.996937 rift-framework-0.9.9/rift/wallet/wallet_v3_r2.py
--rw-r--r--   0        0        0     5889 1970-01-01 00:00:00.000000 rift-framework-0.9.9/setup.py
--rw-r--r--   0        0        0     5204 1970-01-01 00:00:00.000000 rift-framework-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     6021 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/README.md
+-rw-r--r--   0        0        0      834 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/rift/__init__.py
+-rw-r--r--   0        0        0      199 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/rift/ast/__init__.py
+-rw-r--r--   0        0        0      276 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/rift/ast/ast.py
+-rw-r--r--   0        0        0      745 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/rift/ast/ast_patcher.py
+-rw-r--r--   0        0        0      817 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/rift/ast/bool_dict.py
+-rw-r--r--   0        0        0     3576 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/rift/ast/calls.py
+-rw-r--r--   0        0        0      393 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/rift/ast/compiled_contract.py
+-rw-r--r--   0        0        0      752 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/rift/ast/int_dict.py
+-rw-r--r--   0        0        0      456 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/rift/ast/patchers/__init__.py
+-rw-r--r--   0        0        0      694 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/rift/ast/patchers/assert_patcher.py
+-rw-r--r--   0        0        0     5491 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/rift/ast/patchers/assign_patcher.py
+-rw-r--r--   0        0        0      571 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/rift/ast/patchers/break_patcher.py
+-rw-r--r--   0        0        0     2133 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/rift/ast/patchers/if_patcher.py
+-rw-r--r--   0        0        0      579 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/rift/ast/patchers/raise_patcher.py
+-rw-r--r--   0        0        0      675 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/rift/ast/patchers/return_patcher.py
+-rw-r--r--   0        0        0      453 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/rift/ast/patchers/unary_patcher.py
+-rw-r--r--   0        0        0      686 2023-06-13 16:35:51.021158 rift-framework-1.0.0rc1/rift/ast/patchers/while_patcher.py
+-rw-r--r--   0        0        0      544 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/printer.py
+-rw-r--r--   0        0        0     1141 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/ref_table.py
+-rw-r--r--   0        0        0        0 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/sentry/__init__.py
+-rw-r--r--   0        0        0     1131 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/sentry/base_types.py
+-rw-r--r--   0        0        0     3537 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/sentry/sentry.py
+-rw-r--r--   0        0        0        0 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/sentry/watchers/__init__.py
+-rw-r--r--   0        0        0      624 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/sentry/watchers/base_watcher.py
+-rw-r--r--   0        0        0      420 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/sentry/watchers/codes.py
+-rw-r--r--   0        0        0     1464 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/sentry/watchers/import_restrictor.py
+-rw-r--r--   0        0        0      601 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/sentry/watchers/match.py
+-rw-r--r--   0        0        0      979 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/sentry/watchers/simple_restrictor.py
+-rw-r--r--   0        0        0      207 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/sentry/watchers/src_watcher.py
+-rw-r--r--   0        0        0      393 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/types/__init__.py
+-rw-r--r--   0        0        0     2675 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/types/asm_method.py
+-rw-r--r--   0        0        0     1086 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/types/block.py
+-rw-r--r--   0        0        0     1891 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/types/condition.py
+-rw-r--r--   0        0        0       71 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/types/const.py
+-rw-r--r--   0        0        0     1154 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/types/contract.py
+-rw-r--r--   0        0        0      336 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/types/control_flow.py
+-rw-r--r--   0        0        0     3154 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/types/expr.py
+-rw-r--r--   0        0        0      713 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/types/loop.py
+-rw-r--r--   0        0        0     2287 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/types/method.py
+-rw-r--r--   0        0        0      581 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/types/node.py
+-rw-r--r--   0        0        0     4368 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/types/statement.py
+-rw-r--r--   0        0        0      811 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/ast/utils.py
+-rw-r--r--   0        0        0       58 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/bases/__init__.py
+-rw-r--r--   0        0        0      202 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/bases/bare.py
+-rw-r--r--   0        0        0      382 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/bases/util.py
+-rw-r--r--   0        0        0       68 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cli/__init__.py
+-rw-r--r--   0        0        0      166 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1633 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cli/commands/build.py
+-rw-r--r--   0        0        0     2612 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cli/commands/deploy.py
+-rw-r--r--   0        0        0     1302 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cli/commands/init.py
+-rw-r--r--   0        0        0     5021 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cli/commands/test.py
+-rw-r--r--   0        0        0     8049 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cli/commands/utils.py
+-rw-r--r--   0        0        0     2023 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cli/config.py
+-rw-r--r--   0        0        0       52 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cli/entry.py
+-rw-r--r--   0        0        0       56 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cli/util/__init__.py
+-rw-r--r--   0        0        0      270 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cli/util/dag.py
+-rw-r--r--   0        0        0     1291 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cli/util/dir_helper.py
+-rw-r--r--   0        0        0      451 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cli/util/dir_util.py
+-rw-r--r--   0        0        0       78 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cli/util/git.py
+-rw-r--r--   0        0        0      276 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/core/__init__.py
+-rw-r--r--   0        0        0     6415 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/core/annots.py
+-rw-r--r--   0        0        0     1158 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/core/condition.py
+-rw-r--r--   0        0        0     4981 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/core/entity.py
+-rw-r--r--   0        0        0      245 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/core/factory.py
+-rw-r--r--   0        0        0     2726 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/core/invokable.py
+-rw-r--r--   0        0        0      632 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/core/loop.py
+-rw-r--r--   0        0        0      214 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/core/mark.py
+-rw-r--r--   0        0        0     1486 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/core/utils.py
+-rw-r--r--   0        0        0        0 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cst/__init__.py
+-rw-r--r--   0        0        0      104 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cst/cst_env.py
+-rw-r--r--   0        0        0      396 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cst/cst_patcher.py
+-rw-r--r--   0        0        0      963 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cst/cst_visitor.py
+-rw-r--r--   0        0        0     3222 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cst/import_visitor.py
+-rw-r--r--   0        0        0      583 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/cst/int_visitor.py
+-rw-r--r--   0        0        0      298 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/__init__.py
+-rw-r--r--   0        0        0    12542 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/bundled_fc.py
+-rw-r--r--   0        0        0    36807 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/bundled_libs.py
+-rw-r--r--   0        0        0     1404 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/contract.py
+-rw-r--r--   0        0        0     5079 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/fift.py
+-rw-r--r--   0        0        0      553 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/fift_behavior.py
+-rw-r--r--   0        0        0     3299 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/func.py
+-rw-r--r--   0        0        0     3328 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/test_result.py
+-rw-r--r--   0        0        0     3807 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/tvm.py
+-rw-r--r--   0        0        0      280 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/types/__init__.py
+-rw-r--r--   0        0        0     1321 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/types/_fift_base.py
+-rw-r--r--   0        0        0     2147 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/types/builder.py
+-rw-r--r--   0        0        0     1384 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/types/bytes.py
+-rw-r--r--   0        0        0     2070 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/types/cell.py
+-rw-r--r--   0        0        0     1219 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/types/dict.py
+-rw-r--r--   0        0        0      320 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/types/dict_impl.py
+-rw-r--r--   0        0        0      384 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/types/factory.py
+-rw-r--r--   0        0        0     2833 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/types/gdict.py
+-rw-r--r--   0        0        0      762 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/types/int.py
+-rw-r--r--   0        0        0      611 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/types/null.py
+-rw-r--r--   0        0        0     3751 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/types/slice.py
+-rw-r--r--   0        0        0      457 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/types/string.py
+-rw-r--r--   0        0        0     1478 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/types/tuple.py
+-rw-r--r--   0        0        0      385 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/types/util.py
+-rw-r--r--   0        0        0     3352 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/fift/utils.py
+-rw-r--r--   0        0        0      114 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/__init__.py
+-rw-r--r--   0        0        0     4551 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/contract.py
+-rw-r--r--   0        0        0     8596 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/engine.py
+-rw-r--r--   0        0        0      211 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/func_behavior.py
+-rw-r--r--   0        0        0      503 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/library.py
+-rw-r--r--   0        0        0     1369 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/meta_contract.py
+-rw-r--r--   0        0        0        0 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/types/__init__.py
+-rw-r--r--   0        0        0     3393 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/types/builder_base.py
+-rw-r--r--   0        0        0     1820 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/types/cell_base.py
+-rw-r--r--   0        0        0       93 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/types/cont_base.py
+-rw-r--r--   0        0        0     2278 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/types/dict_base.py
+-rw-r--r--   0        0        0      847 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/types/entity_base.py
+-rw-r--r--   0        0        0     6076 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/types/idict_base.py
+-rw-r--r--   0        0        0       92 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/types/int_base.py
+-rw-r--r--   0        0        0     1470 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/types/pfxdict_base.py
+-rw-r--r--   0        0        0     4497 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/types/slice_base.py
+-rw-r--r--   0        0        0       95 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/types/string_base.py
+-rw-r--r--   0        0        0     4179 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/types/types.py
+-rw-r--r--   0        0        0     6088 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/types/udict_base.py
+-rw-r--r--   0        0        0      292 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/func/util.py
+-rw-r--r--   0        0        0       75 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/keys/__init__.py
+-rw-r--r--   0        0        0     1951 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/keys/key_pair.py
+-rw-r--r--   0        0        0      690 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/keys/mnemonic/__init__.py
+-rw-r--r--   0        0        0       92 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/keys/mnemonic/bip39/__init__.py
+-rw-r--r--   0        0        0    27464 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/keys/mnemonic/bip39/english.py
+-rw-r--r--   0        0        0       49 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/keys/mnemonic/exceptions.py
+-rw-r--r--   0        0        0      622 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/keys/mnemonic/keystore.py
+-rw-r--r--   0        0        0     1948 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/keys/mnemonic/mnemonic.py
+-rw-r--r--   0        0        0       26 2023-06-13 16:35:51.025158 rift-framework-1.0.0rc1/rift/keys/mnemonic/settings.py
+-rw-r--r--   0        0        0     1070 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/keys/mnemonic/utils.py
+-rw-r--r--   0        0        0       23 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/keys/signer.py
+-rw-r--r--   0        0        0       80 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/library/__init__.py
+-rw-r--r--   0        0        0      492 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/library/rstd.py
+-rw-r--r--   0        0        0    27617 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/library/std.py
+-rw-r--r--   0        0        0      125 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/logging/__init__.py
+-rw-r--r--   0        0        0      110 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/logging/error.py
+-rw-r--r--   0        0        0     2961 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/logging/logger.py
+-rw-r--r--   0        0        0        0 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/meta/__init__.py
+-rw-r--r--   0        0        0     7367 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/meta/behaviors.py
+-rw-r--r--   0        0        0     2020 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/meta/meta_inheritance.py
+-rw-r--r--   0        0        0      323 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/meta/utils.py
+-rw-r--r--   0        0        0       96 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/native/__init__.py
+-rw-r--r--   0        0        0      291 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/native/c_annot.py
+-rw-r--r--   0        0        0     1215 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/native/c_call.py
+-rw-r--r--   0        0        0       99 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/network/__init__.py
+-rw-r--r--   0        0        0     1030 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/network/account.py
+-rw-r--r--   0        0        0      966 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/network/config.py
+-rw-r--r--   0        0        0      165 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/network/error.py
+-rw-r--r--   0        0        0      177 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/network/inetwork.py
+-rw-r--r--   0        0        0      878 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/network/ton_access.py
+-rw-r--r--   0        0        0        0 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/network/tonlib/__init__.py
+-rw-r--r--   0        0        0     4122 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/network/tonlib/network.py
+-rw-r--r--   0        0        0     2945 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/network/tonlib/servers.py
+-rw-r--r--   0        0        0      604 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/network/util.py
+-rw-r--r--   0        0        0     2169 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/network/v2_network.py
+-rw-r--r--   0        0        0        0 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/runtime/config.py
+-rw-r--r--   0        0        0     5779 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/runtime/keystore.py
+-rw-r--r--   0        0        0     4742 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/runtime/riftlib.py
+-rw-r--r--   0        0        0      900 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/__init__.py
+-rw-r--r--   0        0        0     2323 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/addr.py
+-rw-r--r--   0        0        0      285 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/bases/__init__.py
+-rw-r--r--   0        0        0     1103 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/bases/builder.py
+-rw-r--r--   0        0        0       88 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/bases/bytes.py
+-rw-r--r--   0        0        0      483 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/bases/cell.py
+-rw-r--r--   0        0        0      182 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/bases/dict.py
+-rw-r--r--   0        0        0      174 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/bases/int.py
+-rw-r--r--   0        0        0     2725 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/bases/slice.py
+-rw-r--r--   0        0        0      198 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/bases/string.py
+-rw-r--r--   0        0        0      733 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/bool.py
+-rw-r--r--   0        0        0      874 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/coin.py
+-rw-r--r--   0        0        0     2209 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/constructor.py
+-rw-r--r--   0        0        0      978 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/contract_dep.py
+-rw-r--r--   0        0        0     3487 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/either.py
+-rw-r--r--   0        0        0     4314 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/either_ref.py
+-rw-r--r--   0        0        0     1060 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/helpers.py
+-rw-r--r--   0        0        0    12667 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/int_aliases.py
+-rw-r--r--   0        0        0     3349 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/maybe.py
+-rw-r--r--   0        0        0     4077 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/model.py
+-rw-r--r--   0        0        0     5239 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/msg.py
+-rw-r--r--   0        0        0     8661 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/payload.py
+-rw-r--r--   0        0        0     2990 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/ref.py
+-rw-r--r--   0        0        0      850 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/signed_payload.py
+-rw-r--r--   0        0        0     1627 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/sized_int.py
+-rw-r--r--   0        0        0     1115 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/slice.py
+-rw-r--r--   0        0        0      561 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/type_helper.py
+-rw-r--r--   0        0        0      690 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/types/utils.py
+-rw-r--r--   0        0        0       38 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/util/__init__.py
+-rw-r--r--   0        0        0      169 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/util/dump.py
+-rw-r--r--   0        0        0      270 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/util/type_id.py
+-rw-r--r--   0        0        0        0 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/wallet/__init__.py
+-rw-r--r--   0        0        0     1992 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/wallet/wallet_base.py
+-rw-r--r--   0        0        0     2119 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/wallet/wallet_manager.py
+-rw-r--r--   0        0        0     1689 2023-06-13 16:35:51.029158 rift-framework-1.0.0rc1/rift/wallet/wallet_v3_r2.py
+-rw-r--r--   0        0        0     7725 1970-01-01 00:00:00.000000 rift-framework-1.0.0rc1/setup.py
+-rw-r--r--   0        0        0     6979 1970-01-01 00:00:00.000000 rift-framework-1.0.0rc1/PKG-INFO
```

### Comparing `rift-framework-0.9.9/LICENSE` & `rift-framework-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/README.md` & `rift-framework-1.0.0rc1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <img align="left" width="64" height="64" src="https://github.com/sky-ring/rift/blob/main/assets/rift-icon.png">
 
 # Rift
 
-[![PyPI version](https://img.shields.io/badge/rift--framework-0.9.9-informational?style=flat-square&color=FFFF91&labelColor=360825)](https://pypi.org/project/rift-framework/)
+[![PyPI version](https://img.shields.io/badge/rift--framework-1.0.0--rc1-informational?style=flat-square&color=FFFF91&labelColor=360825)](https://pypi.org/project/rift-framework/)
 [![Telegram](https://img.shields.io/badge/Telegram-@skyring__org-informational?style=flat-square&color=0088cc&labelColor=360825)](https://t.me/skyring_org)
 [![Telegram](https://img.shields.io/badge/Docs-docs.skyring.io/rift-informational?style=flat-square&color=6A0F49&labelColor=360825)](https://docs.skyring.io/rift/)
 
 > _A magical **Python3** -> **TON** portal_
 
 Rift is a full-stack development framework for [TON (The Open Network)](https://ton.org) that makes it easy for developers to use Python to develop, test, and deploy smart contracts on the TON network. With Rift, you can leverage the simplicity and versatility of Python to build and interact with TON, without having to learn the complexities of FunC or Fift. For examples of how Rift simplifies these processes, visit [Rift's website](https://rift.skyring.io).
 
@@ -16,14 +16,18 @@
 - Interact with the TON network to query data and deploy contracts
 - Test smart contracts with an easy-to-use testing framework
 - Standalone framework that only requires `Python 3.10`
 - Can be used at any stage of the project, from development to testing to deployment
 
 ## Quick Start
 
+> **Warning**
+>
+> **Rift**'s stable version is currently in release-candidate state, and we strongly advise thorough testing before transitioning to production. We are still in the process of battle-testing some internal modules, and we anticipate announcing a stable release in the near future. It is advisable to first deploy your contracts to `testnet` and test them meticulously before making the decision to move to production. Additionally, please verify the `FunC` contracts generated.
+
 0. Install `Python 3.10+`
 1. Install `rift`
     ```bash
     pip install rift-framework
     # or from source
     git clone https://github.com/sky-ring/rift
     cd rift
@@ -46,16 +50,16 @@
     # deploys TARGET
     rift deploy TARGET
     ```
 7. For more information, visit the documentation website at [docs.skyring.io/rift](https://docs.skyring.io/rift).
 
 ## Guides
 
-- Step-by-step guide on how to use `Rift` to develop on TON: [Link](https://rift.skyring.io/guide-full)
-- Step-by-step guide on integrating `Rift` into existing `FunC` projects: [Link](https://rift.skyring.io/guide-func)
+- [*Step-by-Step with Rift: Simple Storage Contract*](https://docs.skyring.io/rift/step-by-step-guides/simple-storage-contract)
+- Step-by-step guide on integrating `Rift` into existing `FunC` projects: *Coming Soon!*
 
 ## Standard Contracts Implementation
 - [x] Jetton Implementation ([jettons](https://github.com/sky-ring/jettons))
 - [ ] NFT Implementation
 - [ ] DEX Implementation
 
 
@@ -68,16 +72,27 @@
 - [x] Providing Standard Smart Contracts Implementation with Rift
 
 ### Milestone 2: Deploying, Testing, Interaction Capabilities
 - [x] Simple Interaction Interface with TON Blockchain
 - [x] Simple Deploying Options of Developed Contracts
 - [x] Testing Framework for the Contracts Developed with Rift
 
-### Milestone 3: What's Next?
-- Stay Tuned! We have extra plans that we will share soon with the community to further develop `Rift`.
+### Milestone 3: Launching a Community-Powered Rift
+In this milestone, we are thrilled to unveil the stable version of Rift, primed and ready for integration into real-world projects. Our vision is to foster a Rift ecosystem that thrives on the collective intelligence of its community. We are opening doors and creating avenues for our community members to contribute, refine, and evolve Rift. Here are some of the exciting initiatives we have in mind:
+
+- [ ] **Rift Advancement Proposals (RAPs)**: A dynamic platform for you to propose and discuss enhancements for Rift. This is your chance to help shape the future of Rift!
+
+- [ ] **Comprehensive Documentation**: We are committed to offering an in-depth, yet user-friendly guide that reveals the full potential of Rift. Explore the inner workings and capabilities of Rift with ease and precision.
+
+- [ ] **Extensive Example Sets**: Gain a deeper understanding of Rift through practical examples that showcase its robust features and functionalities.
+
+- [ ] **Multi-Contract Testing / Sandbox Integration**: Embrace a worry-free testing environment. Experiment, play, and validate your projects with our integrated sandbox feature.
+
+Join us on this thrilling journey, shaping the future of Rift, one milestone at a time. We can't wait to see where your contributions will lead us next!
+
 
 ## Support the Project
 1. If `Rift` has been a lifesaver for you, giving it a star on GitHub is the ultimate high five!
 2. You can also show your love by contributing to `Rift` through code, ideas, or even a kind word.
 3. Feeling extra generous? Treat `Rift` to a coffee by donating to this TON address: `EQAIhZCDT7-pvweWh6c_76X7Dnv6Qlzt7-l1NNP8upZ_Areu`
 4. Finally, spreading the word about `Rift` is a big boost for the project and helps us reach more people.
```

### Comparing `rift-framework-0.9.9/rift/ast/ast_patcher.py` & `rift-framework-1.0.0rc1/rift/ast/ast_patcher.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/bool_dict.py` & `rift-framework-1.0.0rc1/rift/ast/bool_dict.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/calls.py` & `rift-framework-1.0.0rc1/rift/ast/calls.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/int_dict.py` & `rift-framework-1.0.0rc1/rift/ast/int_dict.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/patchers/assert_patcher.py` & `rift-framework-1.0.0rc1/rift/ast/patchers/assert_patcher.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/patchers/assign_patcher.py` & `rift-framework-1.0.0rc1/rift/ast/patchers/assign_patcher.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/patchers/break_patcher.py` & `rift-framework-1.0.0rc1/rift/ast/patchers/break_patcher.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/patchers/if_patcher.py` & `rift-framework-1.0.0rc1/rift/ast/patchers/if_patcher.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/patchers/raise_patcher.py` & `rift-framework-1.0.0rc1/rift/ast/patchers/raise_patcher.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/patchers/return_patcher.py` & `rift-framework-1.0.0rc1/rift/ast/patchers/return_patcher.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/patchers/while_patcher.py` & `rift-framework-1.0.0rc1/rift/ast/patchers/while_patcher.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/printer.py` & `rift-framework-1.0.0rc1/rift/ast/printer.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/ref_table.py` & `rift-framework-1.0.0rc1/rift/ast/ref_table.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/types/asm_method.py` & `rift-framework-1.0.0rc1/rift/ast/types/asm_method.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/types/block.py` & `rift-framework-1.0.0rc1/rift/ast/types/block.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/types/condition.py` & `rift-framework-1.0.0rc1/rift/ast/types/condition.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/types/contract.py` & `rift-framework-1.0.0rc1/rift/ast/types/contract.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/types/expr.py` & `rift-framework-1.0.0rc1/rift/ast/types/expr.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/types/loop.py` & `rift-framework-1.0.0rc1/rift/ast/types/loop.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/types/method.py` & `rift-framework-1.0.0rc1/rift/ast/types/method.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/types/node.py` & `rift-framework-1.0.0rc1/rift/ast/types/node.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/types/statement.py` & `rift-framework-1.0.0rc1/rift/ast/types/statement.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/ast/utils.py` & `rift-framework-1.0.0rc1/rift/ast/utils.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/cli/commands/build.py` & `rift-framework-1.0.0rc1/rift/cli/commands/build.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from os import getcwd, path
+from os import getcwd, makedirs, path
 
 import click
 
+from rift.ast.sentry.base_types import SentryHalted
 from rift.cli.commands.utils import build_target
 from rift.cli.config import ProjectConfig
 from rift.cli.entry import entry
 from rift.cli.util.dir_util import clear_contents
 from rift.runtime.config import FunCMode
 
 
@@ -35,25 +36,29 @@
 
     click.echo(
         f"Building {click.style(target, 'yellow')} from {click.style(config.name, 'blue')} project ...",
     )
 
     contracts_dir = path.join(cwd, "contracts")
     build_dir = path.join(cwd, "build")
+    makedirs(build_dir, mode=0o777, exist_ok=True)
 
     if not keep:
         clear_contents(build_dir)
 
     if target == "all":
         targets = list(config.contracts.keys())
     else:
         targets = [target]
 
     for target in targets:
-        build_target(
-            target,
-            config.contracts[target],
-            config,
-            contracts_dir,
-            build_dir,
-            save_patches=log_patches,
-        )
+        try:
+            build_target(
+                target,
+                config.contracts[target],
+                config,
+                contracts_dir,
+                build_dir,
+                save_patches=log_patches,
+            )
+        except SentryHalted as sh:
+            return
```

### Comparing `rift-framework-0.9.9/rift/cli/commands/deploy.py` & `rift-framework-1.0.0rc1/rift/cli/commands/deploy.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import click
 
 from rift.cli.commands.utils import load_module
 from rift.cli.config import ProjectConfig
 from rift.cli.entry import entry
 from rift.fift.types import Cell
 from rift.func.meta_contract import ContractMeta
-from rift.network.network import Network
+from rift.network.v2_network import Network
 from rift.runtime.config import FiftMode
 from rift.wallet.wallet_manager import WalletManager
 
 
 @entry.command(help="Deploys an specific target")
 @click.argument("target")
 @click.option(
@@ -64,27 +64,26 @@
                     fg="red",
                 )
                 return
             code_cell = Cell.load_from(boc_file)
             contract.__code_cell__ = code_cell
 
     FiftMode.activate()
-    res = mod.deploy()
+
+    network = network.lower()
+    n = Network(testnet=network == "test-net")
+
+    res = mod.deploy(n)
     if isinstance(res, tuple):
         msg, independent = res
     else:
         msg, independent = res, False
 
-    network = network.lower()
-    n = Network(testnet=network == "test-net")
-
     if independent:
         # send to blockchain
         r = n.send_boc(msg)
     else:
         # acquire wallet, build msg and then send
         r = WalletManager.send_message(n, msg)
-    if r["ok"]:
-        print("Successfuly deployed contract at the address:", "")
-    else:
-        print("Error deploying contract")
-        print(r)
+    if r == -1:
+        return
+    print("Successfully deployed contract at the address")
```

### Comparing `rift-framework-0.9.9/rift/cli/commands/init.py` & `rift-framework-1.0.0rc1/rift/cli/commands/init.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import subprocess
 from os.path import join as pjoin
 
 import click
 
 from rift.cli.entry import entry
-import subprocess
 
 templates = {
     "bare": "https://github.com/sky-ring/rift-bare-template",
     "func": "https://github.com/sky-ring/rift-func-template",
 }
 
 
@@ -26,15 +26,19 @@
 
     repo = templates[base]
     base_n = click.style(base, bold=True, italic=True, fg="magenta")
     repo_n = click.style(repo, bold=True, italic=True, fg="magenta")
     click.echo(f"Getting template {base_n} from {repo_n}")
 
     pt = pjoin(path, name)
-    p = subprocess.run(f"git clone {repo} {pt}", stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    p = subprocess.run(
+        ["git", "clone", repo, pt],
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+    )
     if p.returncode == 0:
         click.echo(click.style("Successfully created project!", fg="green"))
     else:
         click.echo(
             click.style("Error creating project!", fg="red"),
         )
         click.echo(
```

### Comparing `rift-framework-0.9.9/rift/cli/commands/test.py` & `rift-framework-1.0.0rc1/rift/cli/commands/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 def render_test_panel(session: TestSession) -> Panel:
     table = Table(show_header=False, expand=True, box=None)
     table.add_column("Test")
     table.add_column("Progress", justify="right")
 
     for test_tg, tests in session.tests.items():
-        for (t, state) in tests.items():
+        for t, state in tests.items():
             if state != 0:
                 state_t = (
                     "[magenta] ✗[/magenta]"
                     if state == -1
                     else "[green] ✓[/green]"
                 )
                 state_t = Text.from_markup(state_t)
@@ -91,55 +91,61 @@
             click.style("Not a rift project!", fg="red"),
         )
         return
 
     contracts_dir = path.join(cwd, "tests")
     build_dir = path.join(cwd, "build")
 
-    contract_config = config.contracts[target]
-    test_targets = contract_config.tests
+    if target == "all":
+        targets = list(config.contracts.keys())
+    else:
+        targets = [target]
+
+    for target in targets:
+        contract_config = config.contracts[target]
+        test_targets = contract_config.tests
+
+        sys.path.append(cwd)
+        session = TestSession()
+        session.project = config.name
+        session.target = target
+        session.tests = {}
+        session.progress_cache = {}
+
+        with Live(render_test_panel(session), refresh_per_second=4) as live:
+            for test_tg in test_targets:
+                session.tests[test_tg] = {}
+                fp = path.join(contracts_dir, test_tg + ".py")
+
+                mod, *_ = load_module(fp, test_tg, patch=False)
+                contracts = ContractMeta.defined_contracts()
+                for contract in contracts:
+                    contract_cfg = config.get_contract(contract.__name__)
+                    name = contract_cfg.get_file_name()
+                    boc_file = path.join(build_dir, f"{name}.patched.boc")
+                    if not contract.__interface__:
+                        if not path.exists(boc_file):
+                            click.secho(
+                                f"Couldn't find {name}.boc, Have you built the target? (rift build <target>)",
+                                fg="red",
+                            )
+                            return
+                        code_cell = Cell.load_from(boc_file)
+                        contract.__code_cell__ = code_cell
 
-    sys.path.append(cwd)
-    session = TestSession()
-    session.project = config.name
-    session.target = target
-    session.tests = {}
-    session.progress_cache = {}
-
-    with Live(render_test_panel(session), refresh_per_second=4) as live:
-        for test_tg in test_targets:
-            session.tests[test_tg] = {}
-            fp = path.join(contracts_dir, test_tg + ".py")
-
-            mod, *_ = load_module(fp, test_tg, patch=False)
-            contracts = ContractMeta.defined_contracts()
-            for contract in contracts:
-                contract_cfg = config.get_contract(contract.__name__)
-                name = contract_cfg.get_file_name()
-                boc_file = path.join(build_dir, f"{name}.patched.boc")
-                if not contract.__interface__:
-                    if not path.exists(boc_file):
-                        click.secho(
-                            f"Couldn't find {name}.boc, Have you built the target? (rift build <target>)",
-                            fg="red",
-                        )
-                        return
-                    code_cell = Cell.load_from(boc_file)
-                    contract.__code_cell__ = code_cell
-
-            keys = list(filter(lambda x: x.startswith("test_"), mod.__dict__))
-            for k in keys:
-                session.tests[test_tg][k] = False
-            for k in keys:
-                try:
-                    mod.__dict__[k]()
-                    session.tests[test_tg][k] = 1
-                except TestError as te:
-                    traceback.print_exception(te)
-                    # print(te)
-                    session.tests[test_tg][k] = -1
-                except Exception as e:
-                    traceback.print_exception(e)
-                    # print(e)
-                    session.tests[test_tg][k] = -1
-                live.update(render_test_panel(session))
-                sleep(0.1)
+                keys = list(
+                    filter(lambda x: x.startswith("test_"), mod.__dict__)
+                )
+                for k in keys:
+                    session.tests[test_tg][k] = False
+                for k in keys:
+                    try:
+                        mod.__dict__[k]()
+                        session.tests[test_tg][k] = 1
+                    except TestError as te:
+                        traceback.print_exception(te)
+                        session.tests[test_tg][k] = -1
+                    except Exception as e:
+                        traceback.print_exception(e)
+                        session.tests[test_tg][k] = -1
+                    live.update(render_test_panel(session))
+                    sleep(0.1)
```

### Comparing `rift-framework-0.9.9/rift/cli/commands/utils.py` & `rift-framework-1.0.0rc1/rift/cli/commands/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,15 +64,17 @@
 
         callback = create_save_callback(name, contract.__name__, build_dir)
         callback = callback if save_patches else None
 
         is_target = contract.__name__ == target_config.contract
 
         # We check whether contract is prebuilt or not
-        fc = contract.__fc_code__
+        fc = (
+            contract.__fc_code__ if hasattr(contract, "__fc_code__") else None
+        )
         if fc is not None:
             # It's prebuilt
             if isinstance(fc, tuple) or isinstance(fc, list):
                 fc = list(fc)
             else:
                 fc = [fc]
             files = [path.join(contracts_dir, f) for f in fc]
@@ -96,15 +98,17 @@
                 click.echo(
                     f"Built {contract.__name__} -> build/{name}.fc{add_info}",
                 )
             # Acquire dependency -> compile link func
             # We need dependencies here to link against them
             contract_classes = [v.contract for v in config.contracts.values()]
             deps = [
-                v for k, v in contract_files.items() if k not in contract_classes
+                v
+                for k, v in contract_files.items()
+                if k not in contract_classes
             ]
             files = [*deps, fc_file]
         ok, res = compile_func(files)
         if ok:
             name_styled = click.style(name)
             write_file(path.join(build_dir, f"{name}.fif"), res)
             click.echo(
@@ -159,15 +163,15 @@
     code = f.read()
     if patch:
         code = Engine.cst_patch(code)
     mod.__file__ = file_path
     sys.modules[module_name] = mod
 
     imp_ = relative_imports(code)
-    full_imports = imp_._detailed_imports
+    full_imports = imp_.imports
     refs = []
     for i in full_imports:
         refs.append((module_name, i))
 
     compiled = compile(code, file_path, "exec")
     exec(compiled, mod.__dict__)
     return mod, full_imports, refs
@@ -219,14 +223,15 @@
     return c
 
 
 def compile_func(target_files, link_std=True):
     links = []
     if link_std:
         links.append("#stdlib")
+    links.append("#rstd")
     res = FunC.compile_link(
         target_files,
         links,
         optimization_level=2,
     )
     if isinstance(res, FunCError):
         return False, res.error
```

### Comparing `rift-framework-0.9.9/rift/cli/config.py` & `rift-framework-1.0.0rc1/rift/cli/config.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/cli/util/dir_helper.py` & `rift-framework-1.0.0rc1/rift/cli/util/dir_helper.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/core/annots.py` & `rift-framework-1.0.0rc1/rift/core/annots.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/core/condition.py` & `rift-framework-1.0.0rc1/rift/core/condition.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/core/entity.py` & `rift-framework-1.0.0rc1/rift/core/entity.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/core/invokable.py` & `rift-framework-1.0.0rc1/rift/core/invokable.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/core/loop.py` & `rift-framework-1.0.0rc1/rift/core/loop.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/core/utils.py` & `rift-framework-1.0.0rc1/rift/core/utils.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/cst/import_visitor.py` & `rift-framework-1.0.0rc1/rift/cst/import_visitor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,89 @@
 import libcst as cst
 
 
 class GeneralImportVisitor(cst.CSTVisitor):
-    _relative_accesses = []
-    _imported_ones = []
+    METADATA_DEPENDENCIES = (cst.metadata.PositionProvider,)
 
-    def __init__(self, target_module: str):
+    def __init__(self, target_module: str = None):
+        super().__init__()
         self.target_module = target_module
+        self.global_ = self.target_module is None
         self.imports = {}
+        self.loc = {}
 
     def visit_ImportFrom(self, node: "cst.ImportFrom"):
+        pos = self.get_metadata(cst.metadata.PositionProvider, node).start
+        if len(node.relative) != 0:
+            return super().visit_ImportFrom(node)
         m = node.module
-        if isinstance(m, cst.Attribute):
-            if (
-                isinstance(m.value, cst.Name)
-                and m.value.value == self.target_module
-            ):
-                # Here we captured an `from [Target].[X] import [Names]`
-                from_ = m.attr.value
+        if isinstance(m, cst.Attribute) or isinstance(m, cst.Name):
+            name = parse_name(m)
+            r_tg = name.split(".")[0]
+            if r_tg == self.target_module or self.global_:
+                # Captured expression: from [Target](.[X])* import [Names]
+                if not self.global_:
+                    name = name.removeprefix(r_tg + ".")
                 names = node.names
                 if isinstance(names, cst.ImportStar):
-                    # TODO: Disallow this explicitly
-                    pass
+                    self.imports[name] = ["*"]
                 else:
                     names = [name.name.value for name in names]
-                    self.imports[from_] = names
+                    self.imports[name] = names
+                self.loc[name] = (pos.line - 1, pos.column)
+        else:
+            raise RuntimeError("Unsupported Import Expression!")
         return super().visit_ImportFrom(node)
 
 
 class RelativeImportVisitor(cst.CSTVisitor):
     _relative_accesses = []
     _imported_ones = []
 
     def __init__(self):
+        super().__init__()
         self._relative_accesses = []
         self._imported_ones = []
-        self._detailed_imports = {}
+        self.imports = {}
 
     def visit_ImportFrom(self, node: "cst.ImportFrom"):
         if len(node.relative) == 1:
             m_name = node.module.value
             self._relative_accesses.append(m_name)
-            if m_name not in self._detailed_imports:
-                self._detailed_imports[m_name] = []
+            if m_name not in self.imports:
+                self.imports[m_name] = []
             imported = node.names
             if isinstance(imported, cst.ImportStar):
-                # TODO: A good practice would be throwing
-                # and disallowing relative * imports
+                self.imports[m_name].append("*")
                 pass
             else:
                 # TODO: A better practice would be capturing the aliases too
                 for i in imported:
                     n = i.name.value
                     self._imported_ones.append(n)
-                    self._detailed_imports[m_name].append(n)
+                    self.imports[m_name].append(n)
+        elif len(node.relative) > 1:
+            raise RuntimeError("Unsupported Import Expression!")
         return super().visit_ImportFrom(node)
+
+
+class ModuleImportVisitor(cst.CSTVisitor):
+    METADATA_DEPENDENCIES = (cst.metadata.PositionProvider,)
+
+    def __init__(self):
+        super().__init__()
+        self.imports = []
+        self.loc = {}
+
+    def visit_Import(self, node: "cst.Import"):
+        pos = self.get_metadata(cst.metadata.PositionProvider, node).start
+        for alias in node.names:
+            name = parse_name(alias.name)
+            self.imports.append(name)
+            self.loc[name] = (pos.line - 1, pos.column)
+        return super().visit_Import(node)
+
+
+def parse_name(node: cst.Name | cst.Attribute) -> str:
+    if isinstance(node, cst.Name):
+        return node.value
+    return parse_name(node.value) + "." + parse_name(node.attr)
```

### Comparing `rift-framework-0.9.9/rift/cst/int_visitor.py` & `rift-framework-1.0.0rc1/rift/cst/int_visitor.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/fift/bundled_fc.py` & `rift-framework-1.0.0rc1/rift/fift/bundled_fc.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/fift/bundled_libs.py` & `rift-framework-1.0.0rc1/rift/fift/bundled_libs.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/fift/contract.py` & `rift-framework-1.0.0rc1/rift/fift/contract.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/fift/fift.py` & `rift-framework-1.0.0rc1/rift/fift/fift.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,17 @@
             len(stack_s),
         )
         fift_o = json.loads(out.decode("utf-8"), strict=False)
         status = fift_o["status"]
         if status != "ok":
             raise FiftError(fift_o["message"])
         stack_o = fift_o["stack"]
-        return [Factory.load(t["type"], t["value"]) for t in stack_o]
+        return [
+            Factory.load(t["type"], t.get("value", None)) for t in stack_o
+        ]
 
     @classmethod
     def _init(cls):
         if not cls._global_instance:
             cls._global_instance = Fift(load_utils=True)
 
     @classmethod
```

### Comparing `rift-framework-0.9.9/rift/fift/fift_behavior.py` & `rift-framework-1.0.0rc1/rift/fift/fift_behavior.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/fift/func.py` & `rift-framework-1.0.0rc1/rift/fift/func.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,15 +66,31 @@
             )
             f_sources.append(f.name)
             f.write(s)
             f.close()
         return cls.compile(*f_sources, optimization_level=optimization_level)
 
     @classmethod
+    def prepare_rstd(cls):
+        # TODO: is this an ideal place for this func?
+        if "rstd" in FUNC_LIBS:
+            return
+        from rift.func.engine import Engine
+        from rift.library.rstd import RiftLib
+
+        t = Engine.patched(RiftLib)
+        compiled = Engine.compile(t)
+        code = compiled.to_func()
+        c = zlib.compress(code.encode("utf-8"))
+        b = base64.b64encode(c)
+        FUNC_LIBS["rstd"] = b
+
+    @classmethod
     def compile_link(cls, files, links, optimization_level=2):
+        cls.prepare_rstd()
         f_sources = []
         for i, s in enumerate(links):
             if s.startswith("#"):
                 # We load the libraries dude
                 i = s.replace("#", "").strip()
                 code = FUNC_LIBS[i]
                 zc = base64.b64decode(code)
```

### Comparing `rift-framework-0.9.9/rift/fift/test_result.py` & `rift-framework-1.0.0rc1/rift/fift/test_result.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/fift/tvm.py` & `rift-framework-1.0.0rc1/rift/fift/tvm.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/fift/types/_fift_base.py` & `rift-framework-1.0.0rc1/rift/fift/types/_fift_base.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/fift/types/builder.py` & `rift-framework-1.0.0rc1/rift/fift/types/builder.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/fift/types/bytes.py` & `rift-framework-1.0.0rc1/rift/fift/types/bytes.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 
     def __len__(self) -> int:
         return self.cmd("Blen", self)[0].value
 
     def hashB(self) -> "Bytes":
         return self.cmd("BhashB", self)[0]
 
+    def read_int(self, bit_len):
+        return self.cmd("B>i@", self, bit_len)[0]
+
     def __bytes__(self) -> bytes:
         return base64.b64decode(self.value)
 
     @classmethod
     def __type__(cls) -> str:
         return "bytes"
```

### Comparing `rift-framework-0.9.9/rift/fift/types/cell.py` & `rift-framework-1.0.0rc1/rift/fift/types/cell.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     from rift.fift.types.slice import Slice
     from rift.fift.types.builder import Builder
     from rift.fift.types.int import Int
     from rift.fift.types.bytes import Bytes
 
 from rift.fift.types._fift_base import _FiftBaseType
 from rift.fift.types.factory import Factory
-from rift.network.network import Network
+from rift.network.v2_network import Network
 from rift.util import type_id
 
 
 class Cell(_FiftBaseType):
     __type_id__ = type_id("Cell")
 
     def __init__(self, __factory__: bool = False, __value__: str = None):
```

### Comparing `rift-framework-0.9.9/rift/fift/types/int.py` & `rift-framework-1.0.0rc1/rift/fift/types/int.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/fift/types/null.py` & `rift-framework-1.0.0rc1/rift/fift/types/null.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/fift/types/slice.py` & `rift-framework-1.0.0rc1/rift/fift/types/slice.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,18 @@
         return r
 
     def sint(self, bits: int) -> int:
         r: int = self.cmd("i@", self, bits)[0]
         return r
 
     def hash(self) -> int:
-        pass
+        from rift.fift.types.bytes import Bytes
+
+        r: Bytes = self.cmd("shash", self)[0]
+        return r.read_int(256)
 
     def string_hash(self) -> int:
         pass
 
     def check_signature(self, signature: "Slice", public_key: int) -> int:
         pass
```

### Comparing `rift-framework-0.9.9/rift/fift/types/tuple.py` & `rift-framework-1.0.0rc1/rift/fift/types/tuple.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/fift/utils.py` & `rift-framework-1.0.0rc1/rift/fift/utils.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/func/contract.py` & `rift-framework-1.0.0rc1/rift/func/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from rift.core.annots import impure, is_method, method
 from rift.core.invokable import InvokableFunc
 from rift.fift.contract import ExecutableContract
 from rift.fift.types.cell import Cell as FiftCell
 from rift.func.meta_contract import ContractMeta
 from rift.func.types.types import Cell, Slice
 from rift.func.util import cls_attrs
-from rift.network.network import Network
+from rift.network.inetwork import INetwork
 from rift.types.bases.cell import Cell as GeneralCell
 from rift.types.model import Model
 from rift.types.msg import (
     ExternalMessage,
     InternalMessage,
     MsgAddress,
     StateInit,
@@ -66,15 +66,15 @@
         return self.NOT_IMPLEMENTED
 
     def __getattr__(self, item):
         return InvokableFunc(item)
 
     def connect(
         self,
-        network: Network,
+        network: INetwork,
         addr: str,
         use_code=False,
         use_data=True,
     ):
         self._addr = addr
         acc = network.get_account(self._addr)
         if acc.state != acc.state.ACTIVE:
```

### Comparing `rift-framework-0.9.9/rift/func/engine.py` & `rift-framework-1.0.0rc1/rift/func/engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import ast
 import inspect
+import os
 import textwrap
 
+import click
 import yaml
 
 from rift.ast import CallStacks, CompiledContract, patch
+from rift.ast.sentry.base_types import SentryHalted
+from rift.ast.sentry.sentry import sentry_analyze
 from rift.core import (
     Entity,
     is_asm,
     is_impure,
     is_inline,
     is_inline_ref,
     is_method,
     is_method_id,
 )
 from rift.core.factory import Factory
 from rift.core.utils import init_abstract_type
 from rift.cst.cst_patcher import patch as cst_patch
 from rift.cst.cst_visitor import relative_imports
 from rift.func.util import cls_attrs
+from rift.logging.logger import Logger, Level
 from rift.types import helpers
 
 
 class Engine(object):
     """Engine responsible for compiling contracts."""
 
     VERBOSE = 0
@@ -164,14 +169,20 @@
         src = "from rift.types import helpers\n" + src
         src = cst_patch(src)
         return src
 
     @staticmethod
     def patch(contract, _globals, src_callback=None):
         lines, starting = inspect.findsource(contract)
+
+        # Get file path, relative to current dir
+        cwd = os.getcwd()
+        f_abs = inspect.getfile(contract)
+        f_name = f_abs.removeprefix(cwd).strip("/").strip("\\")
+
         selected = lines[:starting]
         selected.insert(0, "from rift.types import helpers\n")
         needed_src = "".join(selected)
         needed_src = cst_patch(needed_src)
         rel_imported = relative_imports(needed_src)._imported_ones
         x = ast.parse(needed_src)
         m = {**_globals}
@@ -182,14 +193,30 @@
         src = inspect.getsource(contract)
         activate_func_mode = (
             "from rift.runtime.config import FunCMode\nFunCMode.activate()\n"
         )
         src = activate_func_mode + src
         src = cst_patch(src)
         x = ast.parse(src)
+
+        # Here we add sentry
+        sentry_src = "".join(selected[1:])
+        status, warnings = sentry_analyze(x, src=sentry_src, file=f_name)
+        if not status.is_ok():
+            Logger.log(
+                "Engine",
+                Level.ERROR,
+                f"Sentry exited with state: {status.name}",
+            )
+            for w in warnings:
+                msg = w.log()
+                Logger.log("Engine", Level.ERROR, msg)
+            if status.should_halt():
+                raise SentryHalted(warnings)
+
         patched_ast = patch(x)
         if src_callback:
             src_callback(patched_ast)
         if Engine.VERBOSE > 0:
             Engine._cache[contract.__name__] = patched_ast
         exec(compile(patched_ast, "func-patching", "exec"), m)
         return m[contract.__name__]
```

### Comparing `rift-framework-0.9.9/rift/func/meta_contract.py` & `rift-framework-1.0.0rc1/rift/func/meta_contract.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/func/types/builder_base.py` & `rift-framework-1.0.0rc1/rift/func/types/builder_base.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/func/types/cell_base.py` & `rift-framework-1.0.0rc1/rift/func/types/cell_base.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/func/types/dict_base.py` & `rift-framework-1.0.0rc1/rift/func/types/dict_base.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/func/types/entity_base.py` & `rift-framework-1.0.0rc1/rift/func/types/entity_base.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/func/types/idict_base.py` & `rift-framework-1.0.0rc1/rift/func/types/idict_base.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/func/types/pfxdict_base.py` & `rift-framework-1.0.0rc1/rift/func/types/pfxdict_base.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/func/types/slice_base.py` & `rift-framework-1.0.0rc1/rift/func/types/slice_base.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/func/types/types.py` & `rift-framework-1.0.0rc1/rift/func/types/types.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/func/types/udict_base.py` & `rift-framework-1.0.0rc1/rift/func/types/udict_base.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/keys/key_pair.py` & `rift-framework-1.0.0rc1/rift/keys/key_pair.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/keys/mnemonic/__init__.py` & `rift-framework-1.0.0rc1/rift/keys/mnemonic/__init__.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/keys/mnemonic/bip39/english.py` & `rift-framework-1.0.0rc1/rift/keys/mnemonic/bip39/english.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/keys/mnemonic/keystore.py` & `rift-framework-1.0.0rc1/rift/keys/mnemonic/keystore.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/keys/mnemonic/mnemonic.py` & `rift-framework-1.0.0rc1/rift/keys/mnemonic/mnemonic.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/keys/mnemonic/utils.py` & `rift-framework-1.0.0rc1/rift/keys/mnemonic/utils.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/library/std.py` & `rift-framework-1.0.0rc1/rift/library/std.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/logging/logger.py` & `rift-framework-1.0.0rc1/rift/logging/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from rift.runtime.config import Config
 
 
 @total_ordering
 class Level(Enum):
     PANIC = 0
     ALERT = 1
-    CRTIICAL = 2
+    CRITICAL = 2
     ERROR = 3
     WARNING = 4
     NOTE = 5
     INFO = 6
     DEBUG = 7
     SYSTEM = 100
 
@@ -43,15 +43,15 @@
         "yellow": "#FFF689",
         "black": "#000000",
         "mint": "#4BA3C3",
     }
     colors = {
         Level.PANIC: "red",
         Level.ALERT: "red",
-        Level.CRTIICAL: "red",
+        Level.CRITICAL: "red",
         Level.ERROR: "red",
         Level.WARNING: "yellow",
         Level.NOTE: "green",
         Level.INFO: "blue",
         Level.DEBUG: "white",
         Level.SYSTEM: "mint",
     }
```

### Comparing `rift-framework-0.9.9/rift/meta/behaviors.py` & `rift-framework-1.0.0rc1/rift/meta/behaviors.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/meta/meta_inheritance.py` & `rift-framework-1.0.0rc1/rift/meta/meta_inheritance.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/native/c_call.py` & `rift-framework-1.0.0rc1/rift/native/c_call.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/network/account.py` & `rift-framework-1.0.0rc1/rift/network/account.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,20 +15,23 @@
     addr: str
 
     def __init__(self, raw_data=None, addr="") -> None:
         if raw_data is not None:
             self._init_from_raw(raw_data)
         if addr != "":
             self.addr = addr
+        self.data = ""
+        self.code = ""
 
     def _init_from_raw(self, data):
         balance = int(data["balance"])
         code = data["code"]
         c_data = data["data"]
         if balance == -1:
+            balance = 0
             state = AccountState.EMPTY
         elif code == "" and c_data == "":
             state = AccountState.UNINIT
         else:
             state = AccountState.ACTIVE
         self.balance = balance
         self.code = code
```

### Comparing `rift-framework-0.9.9/rift/network/config.py` & `rift-framework-1.0.0rc1/rift/network/config.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/network/network.py` & `rift-framework-1.0.0rc1/rift/network/tonlib/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     TonlibNoResponse,
 )
 from rift_tonlib.client import os
 
 from rift.logging import log_info, log_panic, log_warn
 from rift.network.account import Account
 from rift.network.config import ConfigManager
-from rift.network.servers import Servers
+from rift.network.tonlib.servers import Servers
 from rift.runtime.config import Config
 
 
 class Network:
     def __init__(self, testnet=False, max_tries=5) -> None:
         self._network = "main" if not testnet else "test"
         self._max_tries = max_tries
```

### Comparing `rift-framework-0.9.9/rift/network/servers.py` & `rift-framework-1.0.0rc1/rift/network/tonlib/servers.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/network/util.py` & `rift-framework-1.0.0rc1/rift/network/util.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/runtime/config.py` & `rift-framework-1.0.0rc1/rift/runtime/config.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/runtime/keystore.py` & `rift-framework-1.0.0rc1/rift/runtime/keystore.py`

 * *Files 9% similar despite different names*

```diff
@@ -159,7 +159,18 @@
     @classmethod
     def public_key(cls, bytes_=False) -> int:
         if not cls._global_ks:
             cls.initialize()
         if bytes_:
             return cls._global_ks.pair.pub_key
         return cls._global_ks.pair.pub_key.call("B>u@", 256)[0]
+
+    @classmethod
+    def override(cls, private_hex: str):
+        """
+        This function overrides a private key in the running session
+        Useful For Tests!
+        """
+        kp = KeyPair(priv_key=private_hex, encoding="hex")
+        ks = KeyStore()
+        ks.pair = kp
+        cls._global_ks = ks
```

### Comparing `rift-framework-0.9.9/rift/runtime/riftlib.py` & `rift-framework-1.0.0rc1/rift/runtime/riftlib.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,30 +6,40 @@
 import requests
 from tqdm import tqdm
 
 from rift.runtime.config import Config
 
 
 class RiftLibSetup:
+    version = 3
     urls = {
-        "windows": "https://github.com/AminRezaei0x443/ton/releases/download/v0.1.0/rift-lib-win64.dll",
-        "darwin": "https://github.com/AminRezaei0x443/ton/releases/download/v0.1.0/rift-lib-macOS.dylib",
-        "linux-u18": "https://github.com/AminRezaei0x443/ton/releases/download/v0.1.0/rift-lib-ubuntu-18.04.so",
-        "linux-u20": "https://github.com/AminRezaei0x443/ton/releases/download/v0.1.0/rift-lib-ubuntu-20.04.so",
-        "linux-u22": "https://github.com/AminRezaei0x443/ton/releases/download/v0.1.0/rift-lib-ubuntu-22.04.so",
+        "windows": "https://github.com/AminRezaei0x443/ton/releases/download/v0.1.5/rift-lib-win64.dll",
+        "darwin": "https://github.com/AminRezaei0x443/ton/releases/download/v0.1.5/rift-lib-macOS.dylib",
+        "darwin-slc": "https://github.com/AminRezaei0x443/ton/releases/download/v0.1.5/rift-lib-macOS-silicon.dylib",
+        "linux-u18": "https://github.com/AminRezaei0x443/ton/releases/download/v0.1.5/rift-lib-ubuntu-18.04.so",
+        "linux-u20": "https://github.com/AminRezaei0x443/ton/releases/download/v0.1.5/rift-lib-ubuntu-20.04.so",
+        "linux-u22": "https://github.com/AminRezaei0x443/ton/releases/download/v0.1.5/rift-lib-ubuntu-22.04.so",
     }
 
     @classmethod
     def acquire_lib(cls, ensure=False) -> str:
         if ensure:
             cls.setup_riftlib()
         return os.path.join(Config.dirs.user_data_dir, "_riftlib.pyd")
 
     @classmethod
     def is_setup(cls) -> bool:
+        version_file = os.path.join(Config.dirs.user_data_dir, "_rl_version")
+        if not os.path.exists(version_file):
+            return False
+        with open(version_file, "r") as vf:
+            version = vf.read()
+        version = int(version)
+        if version < cls.version:
+            return False
         return os.path.exists(cls.acquire_lib())
 
     @classmethod
     def _ubuntu_version(cls) -> int:
         try:
             if os.path.exists("/etc/lsb-release"):
                 with open("/etc/lsb-release") as f:
@@ -41,16 +51,24 @@
             return -1
         except Exception:
             return -1
 
     @classmethod
     def determine_lib(cls) -> str:
         s = platform.uname().system.lower()
-        if s == "windows" or s == "darwin":
+        if s == "windows":
             return cls.urls[s]
+        if s == "darwin":
+            proc = platform.processor()
+            if proc == "i386":
+                return cls.urls[s]
+            elif proc == "arm":
+                return cls.urls[f"{s}-slc"]
+            else:
+                raise RuntimeError(f"Unknown processor: {proc}")
         uv = cls._ubuntu_version()
         if uv == -1:
             raise RuntimeError("Unsupported os")
         return cls.urls[f"linux-u{uv}"]
 
     @classmethod
     def _call_get(cls, command):
@@ -62,28 +80,28 @@
         out, err = p.communicate()
         if p.returncode == 0:
             return True, out.decode("utf-8")
         return False, err.decode("utf-8")
 
     @classmethod
     def get_shared_libs(cls):
-        ok, res = cls._call_get("ldconfig -p")
+        ok, res = cls._call_get(["ldconfig", "-p"])
         if not ok:
             raise RuntimeError("Error fetching shared libraries!")
         res = filter(lambda x: "=>" in x, res.split("\n"))
         res = map(
             lambda x: list(map(lambda f: f.strip(), x.split("=>"))),
             res,
         )
         libs = dict(res)
         return libs
 
     @classmethod
     def get_glibc_version(cls):
-        ok, res = cls._call_get("ldconfig --version")
+        ok, res = cls._call_get(["ldconfig", "--version"])
         if not ok:
             raise RuntimeError("Error fetching glibc version!")
         return res.split("\n")[0].split(" ")[-1].strip()
 
     @classmethod
     def get_env_info(cls):
         return {
@@ -106,10 +124,15 @@
     @classmethod
     def setup_riftlib(cls):
         lib_path = cls.acquire_lib()
         if cls.is_setup():
             return
         url = cls.determine_lib()
         os.makedirs(
-            Path(lib_path).parent.absolute(), mode=0o777, exist_ok=True
+            Path(lib_path).parent.absolute(),
+            mode=0o777,
+            exist_ok=True,
         )
+        version_file = os.path.join(Config.dirs.user_data_dir, "_rl_version")
+        with open(version_file, "w") as vf:
+            vf.write(str(cls.version))
         cls._download(url, lib_path, buffer=4096)
```

### Comparing `rift-framework-0.9.9/rift/types/__init__.py` & `rift-framework-1.0.0rc1/rift/types/__init__.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from rift.types.either import Either
 from rift.types.either_ref import EitherRef
 from rift.types.int_aliases import *
 from rift.types.maybe import Maybe
 from rift.types.model import Model
 from rift.types.msg import (
     CurrencyCollection,
+    ExternalMessage,
+    InboundExternalMsgInfo,
     InboundExtMsgInfo,
     InternalMessage,
     InternalMsgInfo,
     MessageFlag,
     MessageMode,
     SimpleLib,
     StateInit,
-    ExternalMessage,
-    InboundExternalMsgInfo,
 )
 from rift.types.payload import Payload
 from rift.types.ref import Ref
 from rift.types.signed_payload import SignedPayload
 from rift.types.sized_int import integer
 from rift.types.slice import slice
```

### Comparing `rift-framework-0.9.9/rift/types/addr.py` & `rift-framework-1.0.0rc1/rift/types/addr.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/types/bases/builder.py` & `rift-framework-1.0.0rc1/rift/types/bases/builder.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/types/bases/slice.py` & `rift-framework-1.0.0rc1/rift/types/bases/slice.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/types/bool.py` & `rift-framework-1.0.0rc1/rift/types/bool.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/types/coin.py` & `rift-framework-1.0.0rc1/rift/types/coin.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/types/constructor.py` & `rift-framework-1.0.0rc1/rift/types/constructor.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/types/contract_dep.py` & `rift-framework-1.0.0rc1/rift/types/contract_dep.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/types/either.py` & `rift-framework-1.0.0rc1/rift/types/either.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from rift.core import Entity
 from rift.core.condition import Cond
 from rift.runtime.config import Config
 from rift.types.bases import Builder, Cell, Slice
+from rift.types.type_helper import type_matches
 from rift.types.utils import CachingSubscriptable
 
 
 class Either(metaclass=CachingSubscriptable):
     which: Entity
     bound: Entity
 
@@ -19,17 +20,17 @@
     def __serialize__(cls, to: "Builder", value: "Either") -> "Builder":
         base1 = cls.__base1__
         base2 = cls.__base2__
         if value is None:
             b = to.uint(0, 1)
             return b
         if not isinstance(value, Either):
-            if type(value).__type_id__() == base1.__type_id__():
+            if type_matches(base1, type(value)):
                 v = 0
-            elif type(value).__type_id__() == base2.__type_id__():
+            elif type_matches(base2, type(value)):
                 v = 1
             else:
                 msg = "got {current} expected {e1} or {e2}"
                 msg = msg.format(current=type(value), e1=base1, e2=base2)
                 raise RuntimeError("Couldn't match either types; " + msg)
             to = to.uint(v, 1)
             return type(value).__serialize__(to, value)
```

### Comparing `rift-framework-0.9.9/rift/types/either_ref.py` & `rift-framework-1.0.0rc1/rift/types/either_ref.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from rift.core import Entity
 from rift.core.condition import Cond
 from rift.library import std
 from rift.logging import log_system
 from rift.runtime.config import Config
 from rift.types.bases import Builder, Cell, Slice
 from rift.types.ref import Ref
+from rift.types.type_helper import type_matches
 from rift.types.utils import CachingSubscriptable
 from rift.util.type_id import type_id
 
 
 class EitherRef(metaclass=CachingSubscriptable):
     which: Entity
     bound: Entity
@@ -25,25 +26,25 @@
     @classmethod
     def __serialize__(cls, to: "Builder", value: "EitherRef") -> "Builder":
         base1 = cls.__base1__
         if value is None:
             b = to.uint(0, 1)
             return b
         if not isinstance(value, EitherRef):
-            if type(value).__type_id__() == base1.__type_id__():
+            if type_matches(base1, type(value)):
                 v = 0
-            elif type(value).__type_id__() == Ref[base1].__type_id__():
+            elif type_matches(Ref[base1], type(value)):
                 v = 1
-            elif type(value).__type_id__() == Cell.__type_id__():
+            elif type_matches(Cell, type(value)):
                 # NOTE: Is this a good approach?
                 v = 0
-            elif type(value).__type_id__() == Slice.__type_id__():
+            elif type_matches(Slice, type(value)):
                 # NOTE: Is this a good approach?
                 v = 0
-            elif type(value).__type_id__() == Ref[Cell].__type_id__():
+            elif type_matches(Ref[Cell], type(value)):
                 v = 1
             else:
                 msg = "got {current} expected {e1} or {e2}"
                 msg = msg.format(current=type(value), e1=base1, e2=Ref[base1])
                 raise RuntimeError("Couldn't match either types; " + msg)
             to = to.uint(v, 1)
             return type(value).__serialize__(to, value)
```

### Comparing `rift-framework-0.9.9/rift/types/helpers.py` & `rift-framework-1.0.0rc1/rift/types/helpers.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/types/int_aliases.py` & `rift-framework-1.0.0rc1/rift/types/int_aliases.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/types/maybe.py` & `rift-framework-1.0.0rc1/rift/types/maybe.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/types/model.py` & `rift-framework-1.0.0rc1/rift/types/model.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/types/msg.py` & `rift-framework-1.0.0rc1/rift/types/msg.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/types/payload.py` & `rift-framework-1.0.0rc1/rift/types/payload.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/types/ref.py` & `rift-framework-1.0.0rc1/rift/types/ref.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/types/signed_payload.py` & `rift-framework-1.0.0rc1/rift/types/signed_payload.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/types/sized_int.py` & `rift-framework-1.0.0rc1/rift/types/sized_int.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/types/slice.py` & `rift-framework-1.0.0rc1/rift/types/slice.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/types/utils.py` & `rift-framework-1.0.0rc1/rift/types/utils.py`

 * *Files identical despite different names*

### Comparing `rift-framework-0.9.9/rift/wallet/wallet_base.py` & `rift-framework-1.0.0rc1/rift/wallet/wallet_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from rift.fift.types.cell import Cell
 from rift.func.contract import Contract
-from rift.network.network import Network
+from rift.network.v2_network import Network
 from rift.runtime.keystore import KeyStore
 from rift.types.msg import ExternalMessage, MessageFlag, MessageMode
 
 
 class WalletBase(Contract):
     __interface__ = True
     __code_cell__: Cell = None
```

### Comparing `rift-framework-0.9.9/rift/wallet/wallet_manager.py` & `rift-framework-1.0.0rc1/rift/wallet/wallet_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import time
 from os import path
 
 from rift.fift.types.cell import Cell
-from rift.network.network import Network
+from rift.network.v2_network import Network
 from rift.runtime.config import Config
 from rift.types.msg import MessageFlag, MessageMode
 from rift.wallet.wallet_base import WalletBase
 from rift.wallet.wallet_v3_r2 import WalletV3R2
 
 
 class WalletManager:
@@ -28,20 +28,22 @@
         ok, account = wallet.connect()
         if not ok:
             print("Selected wallet address:", account.addr)
             if account.state == account.state.EMPTY:
                 print(
                     "The wallet account is empty! Please send some TONs and proceed to deploying it.",
                 )
-                return
+                return -1
             elif account.state == account.state.UNINIT:
                 print("Account is uninitialized, proceeding to deploy it ...")
                 r = wallet.deploy_wallet()
                 print(r)
                 print("Waiting 15 seconds to be sure wallet is deployed!")
+                # Reload the state and the data of the wallet
+                wallet.connect()
                 time.sleep(15)
         return wallet.send_message(
             message,
             valid_until=valid_until,
             mode=mode,
         )
```

### Comparing `rift-framework-0.9.9/rift/wallet/wallet_v3_r2.py` & `rift-framework-1.0.0rc1/rift/wallet/wallet_v3_r2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from rift.fift.types.builder import Builder
 from rift.fift.types.cell import Cell
-from rift.network.network import Network
+from rift.network.v2_network import Network
 from rift.runtime.keystore import KeyStore
 from rift.types.int_aliases import uint32, uint256
 from rift.types.model import Model
 from rift.wallet.wallet_base import WalletBase
 
 
 class WalletV3R2(WalletBase):
@@ -45,11 +45,11 @@
         b = b.uint(self.subwallet, 32)
         if valid_until == -1:
             b = b.sint(-1, 32)
         else:
             b = b.uint(valid_until, 32)
         seq = forced_seq_no if forced_seq_no is not None else self.seq_no()
         b = b.uint(seq, 32)
-        b = b.uint(mode, 8)
         if message:
+            b = b.uint(mode, 8)
             b = b.ref(message)
         return b.end()
```

### Comparing `rift-framework-0.9.9/setup.py` & `rift-framework-1.0.0rc1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['rift',
  'rift.ast',
  'rift.ast.patchers',
+ 'rift.ast.sentry',
+ 'rift.ast.sentry.watchers',
  'rift.ast.types',
  'rift.bases',
  'rift.cli',
  'rift.cli.commands',
  'rift.cli.util',
  'rift.core',
  'rift.cst',
@@ -20,14 +22,15 @@
  'rift.keys.mnemonic',
  'rift.keys.mnemonic.bip39',
  'rift.library',
  'rift.logging',
  'rift.meta',
  'rift.native',
  'rift.network',
+ 'rift.network.tonlib',
  'rift.runtime',
  'rift.types',
  'rift.types.bases',
  'rift.util',
  'rift.wallet']
 
 package_data = \
@@ -36,29 +39,31 @@
 install_requires = \
 ['PyYAML>=6.0,<6.1',
  'appdirs>=1.4.4,<1.5.0',
  'astpretty>=3.0.0,<3.1.0',
  'click>=8.1.3,<8.2.0',
  'colorful>=0.5.4,<0.6.0',
  'cryptography>=39.0.0,<40.0.0',
- 'libcst>=0.4.7,<0.5.0',
+ 'libcst==0.4.9',
  'pynacl>=1.5.0,<2.0.0',
- 'rift-tonlib>=0.0.2,<0.0.3',
+ 'pytest>=7.3.1,<8.0.0',
+ 'rich>=13.3.1,<14.0.0',
+ 'rift-tonlib>=0.0.3,<0.0.4',
  'setuptools>=65.6.3,<66.0.0',
  'tomlkit>=0.11.4,<0.12.0',
  'tqdm>=4.64.1,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['rift = rift.cli.entry:entry']}
 
 setup_kwargs = {
     'name': 'rift-framework',
-    'version': '0.9.9',
+    'version': '1.0.0rc1',
     'description': 'The magical Python -> TON Portal',
-    'long_description': '<img align="left" width="64" height="64" src="https://github.com/sky-ring/rift/blob/main/assets/rift-icon.png">\n\n# Rift\n\n[![PyPI version](https://img.shields.io/badge/rift--framework-0.9.9-informational?style=flat-square&color=FFFF91&labelColor=360825)](https://pypi.org/project/rift-framework/)\n[![Telegram](https://img.shields.io/badge/Telegram-@skyring__org-informational?style=flat-square&color=0088cc&labelColor=360825)](https://t.me/skyring_org)\n[![Telegram](https://img.shields.io/badge/Docs-docs.skyring.io/rift-informational?style=flat-square&color=6A0F49&labelColor=360825)](https://docs.skyring.io/rift/)\n\n> _A magical **Python3** -> **TON** portal_\n\nRift is a full-stack development framework for [TON (The Open Network)](https://ton.org) that makes it easy for developers to use Python to develop, test, and deploy smart contracts on the TON network. With Rift, you can leverage the simplicity and versatility of Python to build and interact with TON, without having to learn the complexities of FunC or Fift. For examples of how Rift simplifies these processes, visit [Rift\'s website](https://rift.skyring.io).\n\n## Features\n\n- Develop smart contracts using Python syntax and OOP features\n- Interact with the TON network to query data and deploy contracts\n- Test smart contracts with an easy-to-use testing framework\n- Standalone framework that only requires `Python 3.10`\n- Can be used at any stage of the project, from development to testing to deployment\n\n## Quick Start\n\n0. Install `Python 3.10+`\n1. Install `rift`\n    ```bash\n    pip install rift-framework\n    # or from source\n    git clone https://github.com/sky-ring/rift\n    cd rift\n    pip install -e .\n    ```\n2. Initialize your project:\n    ```bash\n    rift init <project-name>\n    ```\n3. Develop your contracts in `<project>/contracts/`\n4. Write your tests in `<project>/tests/`\n5. Place your deploy scripts in `<project>/deployers/`\n6. Use `rift` to build, test, or deploy:\n    ```bash\n    # in project folder\n    # builds TARGET\n    rift build TARGET\n    # tests TARGET\n    rift test TARGET\n    # deploys TARGET\n    rift deploy TARGET\n    ```\n7. For more information, visit the documentation website at [docs.skyring.io/rift](https://docs.skyring.io/rift).\n\n## Guides\n\n- Step-by-step guide on how to use `Rift` to develop on TON: [Link](https://rift.skyring.io/guide-full)\n- Step-by-step guide on integrating `Rift` into existing `FunC` projects: [Link](https://rift.skyring.io/guide-func)\n\n## Standard Contracts Implementation\n- [x] Jetton Implementation ([jettons](https://github.com/sky-ring/jettons))\n- [ ] NFT Implementation\n- [ ] DEX Implementation\n\n\n## Roadmap\n\n### Milestone 1: Python Framework for Contract Development\n- [x] Semi One-to-One Mapping of Functions and Expressions (Base Compiler, Python -> FunC)\n- [x] First Higher Layer over the Base Mappings to Simplify Type Calls (leveraging OOP Capabilities)\n- [x] Second Higher Layer over the Base, Simplifying Contract Development towards Maximizing Code Reusability and Simplicity (leveraging Meta Programming Capabilities)\n- [x] Providing Standard Smart Contracts Implementation with Rift\n\n### Milestone 2: Deploying, Testing, Interaction Capabilities\n- [x] Simple Interaction Interface with TON Blockchain\n- [x] Simple Deploying Options of Developed Contracts\n- [x] Testing Framework for the Contracts Developed with Rift\n\n### Milestone 3: What\'s Next?\n- Stay Tuned! We have extra plans that we will share soon with the community to further develop `Rift`.\n\n## Support the Project\n1. If `Rift` has been a lifesaver for you, giving it a star on GitHub is the ultimate high five!\n2. You can also show your love by contributing to `Rift` through code, ideas, or even a kind word.\n3. Feeling extra generous? Treat `Rift` to a coffee by donating to this TON address: `EQAIhZCDT7-pvweWh6c_76X7Dnv6Qlzt7-l1NNP8upZ_Areu`\n4. Finally, spreading the word about `Rift` is a big boost for the project and helps us reach more people.\n\n## Contributing\nIf you\'re interested in contributing to Rift, please see [CONTRIBUTING.md](https://github.com/sky-ring/rift/blob/main/CONTRIBUTING.md) for the necessary specifications and procedures.\n\n## Supporters\nSpecial thanks to the [TON Society](https://society.ton.org/) for their support and grant, without which the project would not be feasible.\n',
+    'long_description': '<img align="left" width="64" height="64" src="https://github.com/sky-ring/rift/blob/main/assets/rift-icon.png">\n\n# Rift\n\n[![PyPI version](https://img.shields.io/badge/rift--framework-1.0.0--rc1-informational?style=flat-square&color=FFFF91&labelColor=360825)](https://pypi.org/project/rift-framework/)\n[![Telegram](https://img.shields.io/badge/Telegram-@skyring__org-informational?style=flat-square&color=0088cc&labelColor=360825)](https://t.me/skyring_org)\n[![Telegram](https://img.shields.io/badge/Docs-docs.skyring.io/rift-informational?style=flat-square&color=6A0F49&labelColor=360825)](https://docs.skyring.io/rift/)\n\n> _A magical **Python3** -> **TON** portal_\n\nRift is a full-stack development framework for [TON (The Open Network)](https://ton.org) that makes it easy for developers to use Python to develop, test, and deploy smart contracts on the TON network. With Rift, you can leverage the simplicity and versatility of Python to build and interact with TON, without having to learn the complexities of FunC or Fift. For examples of how Rift simplifies these processes, visit [Rift\'s website](https://rift.skyring.io).\n\n## Features\n\n- Develop smart contracts using Python syntax and OOP features\n- Interact with the TON network to query data and deploy contracts\n- Test smart contracts with an easy-to-use testing framework\n- Standalone framework that only requires `Python 3.10`\n- Can be used at any stage of the project, from development to testing to deployment\n\n## Quick Start\n\n> **Warning**\n>\n> **Rift**\'s stable version is currently in release-candidate state, and we strongly advise thorough testing before transitioning to production. We are still in the process of battle-testing some internal modules, and we anticipate announcing a stable release in the near future. It is advisable to first deploy your contracts to `testnet` and test them meticulously before making the decision to move to production. Additionally, please verify the `FunC` contracts generated.\n\n0. Install `Python 3.10+`\n1. Install `rift`\n    ```bash\n    pip install rift-framework\n    # or from source\n    git clone https://github.com/sky-ring/rift\n    cd rift\n    pip install -e .\n    ```\n2. Initialize your project:\n    ```bash\n    rift init <project-name>\n    ```\n3. Develop your contracts in `<project>/contracts/`\n4. Write your tests in `<project>/tests/`\n5. Place your deploy scripts in `<project>/deployers/`\n6. Use `rift` to build, test, or deploy:\n    ```bash\n    # in project folder\n    # builds TARGET\n    rift build TARGET\n    # tests TARGET\n    rift test TARGET\n    # deploys TARGET\n    rift deploy TARGET\n    ```\n7. For more information, visit the documentation website at [docs.skyring.io/rift](https://docs.skyring.io/rift).\n\n## Guides\n\n- [*Step-by-Step with Rift: Simple Storage Contract*](https://docs.skyring.io/rift/step-by-step-guides/simple-storage-contract)\n- Step-by-step guide on integrating `Rift` into existing `FunC` projects: *Coming Soon!*\n\n## Standard Contracts Implementation\n- [x] Jetton Implementation ([jettons](https://github.com/sky-ring/jettons))\n- [ ] NFT Implementation\n- [ ] DEX Implementation\n\n\n## Roadmap\n\n### Milestone 1: Python Framework for Contract Development\n- [x] Semi One-to-One Mapping of Functions and Expressions (Base Compiler, Python -> FunC)\n- [x] First Higher Layer over the Base Mappings to Simplify Type Calls (leveraging OOP Capabilities)\n- [x] Second Higher Layer over the Base, Simplifying Contract Development towards Maximizing Code Reusability and Simplicity (leveraging Meta Programming Capabilities)\n- [x] Providing Standard Smart Contracts Implementation with Rift\n\n### Milestone 2: Deploying, Testing, Interaction Capabilities\n- [x] Simple Interaction Interface with TON Blockchain\n- [x] Simple Deploying Options of Developed Contracts\n- [x] Testing Framework for the Contracts Developed with Rift\n\n### Milestone 3: Launching a Community-Powered Rift\nIn this milestone, we are thrilled to unveil the stable version of Rift, primed and ready for integration into real-world projects. Our vision is to foster a Rift ecosystem that thrives on the collective intelligence of its community. We are opening doors and creating avenues for our community members to contribute, refine, and evolve Rift. Here are some of the exciting initiatives we have in mind:\n\n- [ ] **Rift Advancement Proposals (RAPs)**: A dynamic platform for you to propose and discuss enhancements for Rift. This is your chance to help shape the future of Rift!\n\n- [ ] **Comprehensive Documentation**: We are committed to offering an in-depth, yet user-friendly guide that reveals the full potential of Rift. Explore the inner workings and capabilities of Rift with ease and precision.\n\n- [ ] **Extensive Example Sets**: Gain a deeper understanding of Rift through practical examples that showcase its robust features and functionalities.\n\n- [ ] **Multi-Contract Testing / Sandbox Integration**: Embrace a worry-free testing environment. Experiment, play, and validate your projects with our integrated sandbox feature.\n\nJoin us on this thrilling journey, shaping the future of Rift, one milestone at a time. We can\'t wait to see where your contributions will lead us next!\n\n\n## Support the Project\n1. If `Rift` has been a lifesaver for you, giving it a star on GitHub is the ultimate high five!\n2. You can also show your love by contributing to `Rift` through code, ideas, or even a kind word.\n3. Feeling extra generous? Treat `Rift` to a coffee by donating to this TON address: `EQAIhZCDT7-pvweWh6c_76X7Dnv6Qlzt7-l1NNP8upZ_Areu`\n4. Finally, spreading the word about `Rift` is a big boost for the project and helps us reach more people.\n\n## Contributing\nIf you\'re interested in contributing to Rift, please see [CONTRIBUTING.md](https://github.com/sky-ring/rift/blob/main/CONTRIBUTING.md) for the necessary specifications and procedures.\n\n## Supporters\nSpecial thanks to the [TON Society](https://society.ton.org/) for their support and grant, without which the project would not be feasible.\n',
     'author': 'Amin Rezaei',
     'author_email': 'AminRezaei0x443@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `rift-framework-0.9.9/PKG-INFO` & `rift-framework-1.0.0rc1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: rift-framework
-Version: 0.9.9
+Version: 1.0.0rc1
 Summary: The magical Python -> TON Portal
 License: MIT
 Author: Amin Rezaei
 Author-email: AminRezaei0x443@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyYAML (>=6.0,<6.1)
 Requires-Dist: appdirs (>=1.4.4,<1.5.0)
 Requires-Dist: astpretty (>=3.0.0,<3.1.0)
 Requires-Dist: click (>=8.1.3,<8.2.0)
 Requires-Dist: colorful (>=0.5.4,<0.6.0)
 Requires-Dist: cryptography (>=39.0.0,<40.0.0)
-Requires-Dist: libcst (>=0.4.7,<0.5.0)
+Requires-Dist: libcst (==0.4.9)
 Requires-Dist: pynacl (>=1.5.0,<2.0.0)
-Requires-Dist: rift-tonlib (>=0.0.2,<0.0.3)
+Requires-Dist: pytest (>=7.3.1,<8.0.0)
+Requires-Dist: rich (>=13.3.1,<14.0.0)
+Requires-Dist: rift-tonlib (>=0.0.3,<0.0.4)
 Requires-Dist: setuptools (>=65.6.3,<66.0.0)
 Requires-Dist: tomlkit (>=0.11.4,<0.12.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 <img align="left" width="64" height="64" src="https://github.com/sky-ring/rift/blob/main/assets/rift-icon.png">
 
 # Rift
 
-[![PyPI version](https://img.shields.io/badge/rift--framework-0.9.9-informational?style=flat-square&color=FFFF91&labelColor=360825)](https://pypi.org/project/rift-framework/)
+[![PyPI version](https://img.shields.io/badge/rift--framework-1.0.0--rc1-informational?style=flat-square&color=FFFF91&labelColor=360825)](https://pypi.org/project/rift-framework/)
 [![Telegram](https://img.shields.io/badge/Telegram-@skyring__org-informational?style=flat-square&color=0088cc&labelColor=360825)](https://t.me/skyring_org)
 [![Telegram](https://img.shields.io/badge/Docs-docs.skyring.io/rift-informational?style=flat-square&color=6A0F49&labelColor=360825)](https://docs.skyring.io/rift/)
 
 > _A magical **Python3** -> **TON** portal_
 
 Rift is a full-stack development framework for [TON (The Open Network)](https://ton.org) that makes it easy for developers to use Python to develop, test, and deploy smart contracts on the TON network. With Rift, you can leverage the simplicity and versatility of Python to build and interact with TON, without having to learn the complexities of FunC or Fift. For examples of how Rift simplifies these processes, visit [Rift's website](https://rift.skyring.io).
 
@@ -41,14 +43,18 @@
 - Interact with the TON network to query data and deploy contracts
 - Test smart contracts with an easy-to-use testing framework
 - Standalone framework that only requires `Python 3.10`
 - Can be used at any stage of the project, from development to testing to deployment
 
 ## Quick Start
 
+> **Warning**
+>
+> **Rift**'s stable version is currently in release-candidate state, and we strongly advise thorough testing before transitioning to production. We are still in the process of battle-testing some internal modules, and we anticipate announcing a stable release in the near future. It is advisable to first deploy your contracts to `testnet` and test them meticulously before making the decision to move to production. Additionally, please verify the `FunC` contracts generated.
+
 0. Install `Python 3.10+`
 1. Install `rift`
     ```bash
     pip install rift-framework
     # or from source
     git clone https://github.com/sky-ring/rift
     cd rift
@@ -71,16 +77,16 @@
     # deploys TARGET
     rift deploy TARGET
     ```
 7. For more information, visit the documentation website at [docs.skyring.io/rift](https://docs.skyring.io/rift).
 
 ## Guides
 
-- Step-by-step guide on how to use `Rift` to develop on TON: [Link](https://rift.skyring.io/guide-full)
-- Step-by-step guide on integrating `Rift` into existing `FunC` projects: [Link](https://rift.skyring.io/guide-func)
+- [*Step-by-Step with Rift: Simple Storage Contract*](https://docs.skyring.io/rift/step-by-step-guides/simple-storage-contract)
+- Step-by-step guide on integrating `Rift` into existing `FunC` projects: *Coming Soon!*
 
 ## Standard Contracts Implementation
 - [x] Jetton Implementation ([jettons](https://github.com/sky-ring/jettons))
 - [ ] NFT Implementation
 - [ ] DEX Implementation
 
 
@@ -93,16 +99,27 @@
 - [x] Providing Standard Smart Contracts Implementation with Rift
 
 ### Milestone 2: Deploying, Testing, Interaction Capabilities
 - [x] Simple Interaction Interface with TON Blockchain
 - [x] Simple Deploying Options of Developed Contracts
 - [x] Testing Framework for the Contracts Developed with Rift
 
-### Milestone 3: What's Next?
-- Stay Tuned! We have extra plans that we will share soon with the community to further develop `Rift`.
+### Milestone 3: Launching a Community-Powered Rift
+In this milestone, we are thrilled to unveil the stable version of Rift, primed and ready for integration into real-world projects. Our vision is to foster a Rift ecosystem that thrives on the collective intelligence of its community. We are opening doors and creating avenues for our community members to contribute, refine, and evolve Rift. Here are some of the exciting initiatives we have in mind:
+
+- [ ] **Rift Advancement Proposals (RAPs)**: A dynamic platform for you to propose and discuss enhancements for Rift. This is your chance to help shape the future of Rift!
+
+- [ ] **Comprehensive Documentation**: We are committed to offering an in-depth, yet user-friendly guide that reveals the full potential of Rift. Explore the inner workings and capabilities of Rift with ease and precision.
+
+- [ ] **Extensive Example Sets**: Gain a deeper understanding of Rift through practical examples that showcase its robust features and functionalities.
+
+- [ ] **Multi-Contract Testing / Sandbox Integration**: Embrace a worry-free testing environment. Experiment, play, and validate your projects with our integrated sandbox feature.
+
+Join us on this thrilling journey, shaping the future of Rift, one milestone at a time. We can't wait to see where your contributions will lead us next!
+
 
 ## Support the Project
 1. If `Rift` has been a lifesaver for you, giving it a star on GitHub is the ultimate high five!
 2. You can also show your love by contributing to `Rift` through code, ideas, or even a kind word.
 3. Feeling extra generous? Treat `Rift` to a coffee by donating to this TON address: `EQAIhZCDT7-pvweWh6c_76X7Dnv6Qlzt7-l1NNP8upZ_Areu`
 4. Finally, spreading the word about `Rift` is a big boost for the project and helps us reach more people.
```

