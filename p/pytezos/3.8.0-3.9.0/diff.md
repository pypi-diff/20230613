# Comparing `tmp/pytezos-3.8.0.tar.gz` & `tmp/pytezos-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytezos-3.8.0.tar", max compression
+gzip compressed data, was "pytezos-3.9.0.tar", max compression
```

## Comparing `pytezos-3.8.0.tar` & `pytezos-3.9.0.tar`

### file list

```diff
@@ -1,115 +1,114 @@
--rw-r--r--   0        0        0     1102 2023-02-21 18:02:16.887853 pytezos-3.8.0/LICENSE
--rw-r--r--   0        0        0     5589 2023-02-21 18:02:16.887853 pytezos-3.8.0/README.md
--rw-r--r--   0        0        0     3119 2023-02-21 18:02:16.899856 pytezos-3.8.0/pyproject.toml
--rw-r--r--   0        0        0     5448 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/michelson_kernel/README.md
--rw-r--r--   0        0        0       22 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/michelson_kernel/__init__.py
--rw-r--r--   0        0        0      103 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/michelson_kernel/__main__.py
--rw-r--r--   0        0        0     1730 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/michelson_kernel/cli.py
--rw-r--r--   0        0        0    18562 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/michelson_kernel/docs.py
--rw-r--r--   0        0        0     4582 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/michelson_kernel/kernel.js
--rw-r--r--   0        0        0    12185 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/michelson_kernel/kernel.py
--rw-r--r--   0        0        0      919 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/__init__.py
--rw-r--r--   0        0        0       89 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/__main__.py
--rw-r--r--   0        0        0        0 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/block/__init__.py
--rw-r--r--   0        0        0     2768 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/block/forge.py
--rw-r--r--   0        0        0    10077 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/block/header.py
--rw-r--r--   0        0        0        0 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/cli/__init__.py
--rw-r--r--   0        0        0       89 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/cli/__main__.py
--rw-r--r--   0        0        0    18781 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/cli/cli.py
--rw-r--r--   0        0        0     1124 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/cli/github.py
--rw-r--r--   0        0        0     9322 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/client.py
--rw-r--r--   0        0        0        0 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/context/__init__.py
--rw-r--r--   0        0        0     6177 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/context/abstract.py
--rw-r--r--   0        0        0    17843 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/context/impl.py
--rw-r--r--   0        0        0     6556 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/context/mixin.py
--rw-r--r--   0        0        0      722 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/contract/__init__.py
--rw-r--r--   0        0        0    12338 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/contract/call.py
--rw-r--r--   0        0        0     3586 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/contract/data.py
--rw-r--r--   0        0        0     3272 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/contract/entrypoint.py
--rw-r--r--   0        0        0    20520 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/contract/interface.py
--rw-r--r--   0        0        0    12894 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/contract/metadata-schema.json
--rw-r--r--   0        0        0     6705 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/contract/metadata.py
--rw-r--r--   0        0        0     3288 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/contract/result.py
--rw-r--r--   0        0        0     7827 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/contract/token_metadata-schema.json
--rw-r--r--   0        0        0     5061 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/contract/token_metadata.py
--rw-r--r--   0        0        0    11173 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/contract/view.py
--rw-r--r--   0        0        0        0 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/crypto/__init__.py
--rw-r--r--   0        0        0     7529 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/crypto/encoding.py
--rw-r--r--   0        0        0     2683 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/crypto/hash.py
--rw-r--r--   0        0        0     9350 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/crypto/keccak.py
--rw-r--r--   0        0        0    18382 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/crypto/key.py
--rw-r--r--   0        0        0     3087 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/jupyter.py
--rw-r--r--   0        0        0      527 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/logging.py
--rw-r--r--   0        0        0        0 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/michelson/__init__.py
--rw-r--r--   0        0        0    11414 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/michelson/forge.py
--rw-r--r--   0        0        0     5004 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/michelson/format.py
--rw-r--r--   0        0        0     8055 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/michelson/instructions/__init__.py
--rw-r--r--   0        0        0     5145 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/michelson/instructions/adt.py
--rw-r--r--   0        0        0    11406 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/michelson/instructions/arithmetic.py
--rw-r--r--   0        0        0     2896 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/michelson/instructions/base.py
--rw-r--r--   0        0        0     3171 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/michelson/instructions/boolean.py
--rw-r--r--   0        0        0     2985 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/michelson/instructions/compare.py
--rw-r--r--   0        0        0    13315 2023-02-21 18:02:16.899856 pytezos-3.8.0/src/pytezos/michelson/instructions/control.py
--rw-r--r--   0        0        0     5862 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/instructions/crypto.py
--rw-r--r--   0        0        0     5175 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/instructions/generic.py
--rw-r--r--   0        0        0    11580 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/instructions/jupyter.py
--rw-r--r--   0        0        0     4768 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/instructions/stack.py
--rw-r--r--   0        0        0     6253 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/instructions/struct.py
--rw-r--r--   0        0        0    15646 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/instructions/tezos.py
--rw-r--r--   0        0        0     4109 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/instructions/ticket.py
--rw-r--r--   0        0        0     3914 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/instructions/tzt.py
--rw-r--r--   0        0        0    10824 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/macros.py
--rw-r--r--   0        0        0    13713 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/micheline.py
--rw-r--r--   0        0        0     6282 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/parse.py
--rw-r--r--   0        0        0    13140 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/program.py
--rw-r--r--   0        0        0     8870 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/repl.py
--rw-r--r--   0        0        0      285 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/sections/__init__.py
--rw-r--r--   0        0        0      638 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/sections/code.py
--rw-r--r--   0        0        0     7200 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/sections/parameter.py
--rw-r--r--   0        0        0     2757 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/sections/storage.py
--rw-r--r--   0        0        0     5475 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/sections/tzt.py
--rw-r--r--   0        0        0     2649 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/sections/view.py
--rw-r--r--   0        0        0     2137 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/stack.py
--rw-r--r--   0        0        0     4418 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/tags.py
--rw-r--r--   0        0        0     1903 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/types/__init__.py
--rw-r--r--   0        0        0     4716 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/types/adt.py
--rw-r--r--   0        0        0    10333 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/types/base.py
--rw-r--r--   0        0        0     9825 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/types/big_map.py
--rw-r--r--   0        0        0     4610 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/types/bls.py
--rw-r--r--   0        0        0      286 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/types/chest.py
--rw-r--r--   0        0        0     9682 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/types/core.py
--rw-r--r--   0        0        0    16701 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/types/domain.py
--rw-r--r--   0        0        0     4180 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/types/list.py
--rw-r--r--   0        0        0     7272 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/types/map.py
--rw-r--r--   0        0        0     3135 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/types/operation.py
--rw-r--r--   0        0        0     4330 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/types/option.py
--rw-r--r--   0        0        0    10009 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/types/pair.py
--rw-r--r--   0        0        0     2838 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/types/sapling.py
--rw-r--r--   0        0        0     4345 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/types/set.py
--rw-r--r--   0        0        0     9181 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/types/sum.py
--rw-r--r--   0        0        0     4203 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/michelson/types/ticket.py
--rw-r--r--   0        0        0      105 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/operation/__init__.py
--rw-r--r--   0        0        0    12662 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/operation/content.py
--rw-r--r--   0        0        0     3596 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/operation/fees.py
--rw-r--r--   0        0        0     6375 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/operation/forge.py
--rw-r--r--   0        0        0    19247 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/operation/group.py
--rw-r--r--   0        0        0     7957 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/operation/result.py
--rw-r--r--   0        0        0        0 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/protocol/__init__.py
--rw-r--r--   0        0        0     2895 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/protocol/diff.py
--rw-r--r--   0        0        0     7482 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/protocol/protocol.py
--rw-r--r--   0        0        0        0 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/py.typed
--rw-r--r--   0        0        0      213 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/rpc/__init__.py
--rw-r--r--   0        0        0   133621 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/rpc/docs.py
--rw-r--r--   0        0        0     1103 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/rpc/errors.py
--rw-r--r--   0        0        0    12735 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/rpc/helpers.py
--rw-r--r--   0        0        0      867 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/rpc/kind.py
--rw-r--r--   0        0        0     5507 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/rpc/node.py
--rw-r--r--   0        0        0    12764 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/rpc/protocol.py
--rw-r--r--   0        0        0     4563 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/rpc/query.py
--rw-r--r--   0        0        0     9295 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/rpc/search.py
--rw-r--r--   0        0        0    19204 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/rpc/shell.py
--rw-r--r--   0        0        0        0 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/sandbox/__init__.py
--rw-r--r--   0        0        0     6951 2023-02-21 18:02:16.903858 pytezos-3.8.0/src/pytezos/sandbox/node.py
--rw-r--r--   0        0        0     5916 2023-02-21 18:02:16.907859 pytezos-3.8.0/src/pytezos/sandbox/parameters.py
--rw-r--r--   0        0        0     7699 1970-01-01 00:00:00.000000 pytezos-3.8.0/setup.py
--rw-r--r--   0        0        0     8116 1970-01-01 00:00:00.000000 pytezos-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-03-29 12:43:48.609260 pytezos-3.9.0/LICENSE
+-rw-r--r--   0        0        0     5672 2023-03-29 12:43:48.613260 pytezos-3.9.0/README.md
+-rw-r--r--   0        0        0     3119 2023-03-29 12:43:48.621260 pytezos-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5448 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/michelson_kernel/README.md
+-rw-r--r--   0        0        0       22 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/michelson_kernel/__init__.py
+-rw-r--r--   0        0        0      103 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/michelson_kernel/__main__.py
+-rw-r--r--   0        0        0     1730 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/michelson_kernel/cli.py
+-rw-r--r--   0        0        0    18562 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/michelson_kernel/docs.py
+-rw-r--r--   0        0        0     4592 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/michelson_kernel/kernel.js
+-rw-r--r--   0        0        0    12185 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/michelson_kernel/kernel.py
+-rw-r--r--   0        0        0      919 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/__init__.py
+-rw-r--r--   0        0        0       89 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/__main__.py
+-rw-r--r--   0        0        0        0 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/block/__init__.py
+-rw-r--r--   0        0        0     2768 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/block/forge.py
+-rw-r--r--   0        0        0    10077 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/block/header.py
+-rw-r--r--   0        0        0        0 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/cli/__init__.py
+-rw-r--r--   0        0        0       89 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/cli/__main__.py
+-rw-r--r--   0        0        0    18781 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/cli/cli.py
+-rw-r--r--   0        0        0     1124 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/cli/github.py
+-rw-r--r--   0        0        0     9322 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/client.py
+-rw-r--r--   0        0        0        0 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/context/__init__.py
+-rw-r--r--   0        0        0     6177 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/context/abstract.py
+-rw-r--r--   0        0        0    17843 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/context/impl.py
+-rw-r--r--   0        0        0     6608 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/context/mixin.py
+-rw-r--r--   0        0        0      722 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/contract/__init__.py
+-rw-r--r--   0        0        0    12338 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/contract/call.py
+-rw-r--r--   0        0        0     3586 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/contract/data.py
+-rw-r--r--   0        0        0     3272 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/contract/entrypoint.py
+-rw-r--r--   0        0        0    20520 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/contract/interface.py
+-rw-r--r--   0        0        0    12894 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/contract/metadata-schema.json
+-rw-r--r--   0        0        0     6705 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/contract/metadata.py
+-rw-r--r--   0        0        0     3288 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/contract/result.py
+-rw-r--r--   0        0        0     7827 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/contract/token_metadata-schema.json
+-rw-r--r--   0        0        0     5061 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/contract/token_metadata.py
+-rw-r--r--   0        0        0    11173 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/contract/view.py
+-rw-r--r--   0        0        0        0 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/crypto/__init__.py
+-rw-r--r--   0        0        0     7651 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/crypto/encoding.py
+-rw-r--r--   0        0        0     2683 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/crypto/hash.py
+-rw-r--r--   0        0        0     9350 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/crypto/keccak.py
+-rw-r--r--   0        0        0    18382 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/crypto/key.py
+-rw-r--r--   0        0        0     3087 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/jupyter.py
+-rw-r--r--   0        0        0      527 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/logging.py
+-rw-r--r--   0        0        0        0 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/michelson/__init__.py
+-rw-r--r--   0        0        0    11693 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/michelson/forge.py
+-rw-r--r--   0        0        0     5004 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/michelson/format.py
+-rw-r--r--   0        0        0     8126 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/michelson/instructions/__init__.py
+-rw-r--r--   0        0        0     5145 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/michelson/instructions/adt.py
+-rw-r--r--   0        0        0    12874 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/michelson/instructions/arithmetic.py
+-rw-r--r--   0        0        0     2896 2023-03-29 12:43:48.621260 pytezos-3.9.0/src/pytezos/michelson/instructions/base.py
+-rw-r--r--   0        0        0     3171 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/instructions/boolean.py
+-rw-r--r--   0        0        0     2985 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/instructions/compare.py
+-rw-r--r--   0        0        0    13315 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/instructions/control.py
+-rw-r--r--   0        0        0     5900 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/instructions/crypto.py
+-rw-r--r--   0        0        0     5175 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/instructions/generic.py
+-rw-r--r--   0        0        0    11580 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/instructions/jupyter.py
+-rw-r--r--   0        0        0     4768 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/instructions/stack.py
+-rw-r--r--   0        0        0     6253 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/instructions/struct.py
+-rw-r--r--   0        0        0    15646 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/instructions/tezos.py
+-rw-r--r--   0        0        0     4109 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/instructions/ticket.py
+-rw-r--r--   0        0        0     3914 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/instructions/tzt.py
+-rw-r--r--   0        0        0    10824 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/macros.py
+-rw-r--r--   0        0        0    13713 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/micheline.py
+-rw-r--r--   0        0        0     6282 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/parse.py
+-rw-r--r--   0        0        0    13140 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/program.py
+-rw-r--r--   0        0        0     8870 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/repl.py
+-rw-r--r--   0        0        0      285 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/sections/__init__.py
+-rw-r--r--   0        0        0      638 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/sections/code.py
+-rw-r--r--   0        0        0     7200 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/sections/parameter.py
+-rw-r--r--   0        0        0     2757 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/sections/storage.py
+-rw-r--r--   0        0        0     5475 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/sections/tzt.py
+-rw-r--r--   0        0        0     2649 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/sections/view.py
+-rw-r--r--   0        0        0     2137 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/stack.py
+-rw-r--r--   0        0        0     4473 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/tags.py
+-rw-r--r--   0        0        0     1903 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/types/__init__.py
+-rw-r--r--   0        0        0     4716 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/types/adt.py
+-rw-r--r--   0        0        0    10333 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/types/base.py
+-rw-r--r--   0        0        0     9825 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/types/big_map.py
+-rw-r--r--   0        0        0     4610 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/types/bls.py
+-rw-r--r--   0        0        0      286 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/types/chest.py
+-rw-r--r--   0        0        0     9682 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/types/core.py
+-rw-r--r--   0        0        0    16701 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/types/domain.py
+-rw-r--r--   0        0        0     4180 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/types/list.py
+-rw-r--r--   0        0        0     7272 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/types/map.py
+-rw-r--r--   0        0        0     3135 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/types/operation.py
+-rw-r--r--   0        0        0     4330 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/types/option.py
+-rw-r--r--   0        0        0    10009 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/types/pair.py
+-rw-r--r--   0        0        0     2838 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/types/sapling.py
+-rw-r--r--   0        0        0     4345 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/types/set.py
+-rw-r--r--   0        0        0     9181 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/types/sum.py
+-rw-r--r--   0        0        0     4203 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/michelson/types/ticket.py
+-rw-r--r--   0        0        0      105 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/operation/__init__.py
+-rw-r--r--   0        0        0    12662 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/operation/content.py
+-rw-r--r--   0        0        0     3596 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/operation/fees.py
+-rw-r--r--   0        0        0     6375 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/operation/forge.py
+-rw-r--r--   0        0        0    19451 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/operation/group.py
+-rw-r--r--   0        0        0     7957 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/operation/result.py
+-rw-r--r--   0        0        0        0 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/protocol/__init__.py
+-rw-r--r--   0        0        0     2895 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/protocol/diff.py
+-rw-r--r--   0        0        0     7482 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/protocol/protocol.py
+-rw-r--r--   0        0        0        0 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/py.typed
+-rw-r--r--   0        0        0      213 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/rpc/__init__.py
+-rw-r--r--   0        0        0   133621 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/rpc/docs.py
+-rw-r--r--   0        0        0     1103 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/rpc/errors.py
+-rw-r--r--   0        0        0    12735 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/rpc/helpers.py
+-rw-r--r--   0        0        0      867 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/rpc/kind.py
+-rw-r--r--   0        0        0     5507 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/rpc/node.py
+-rw-r--r--   0        0        0    12764 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/rpc/protocol.py
+-rw-r--r--   0        0        0     4563 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/rpc/query.py
+-rw-r--r--   0        0        0     9295 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/rpc/search.py
+-rw-r--r--   0        0        0    19204 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/rpc/shell.py
+-rw-r--r--   0        0        0        0 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/sandbox/__init__.py
+-rw-r--r--   0        0        0     6951 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/sandbox/node.py
+-rw-r--r--   0        0        0     6058 2023-03-29 12:43:48.625260 pytezos-3.9.0/src/pytezos/sandbox/parameters.py
+-rw-r--r--   0        0        0     8199 1970-01-01 00:00:00.000000 pytezos-3.9.0/PKG-INFO
```

### Comparing `pytezos-3.8.0/LICENSE` & `pytezos-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/README.md` & `pytezos-3.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 #### Michelson integration testing framework
 * Writing integration tests using `unittest` package
 * Simulating contract execution using remote intepreter (via RPC) or builtin one
 
 
 ## Installation
 
-You need to install cryptographic packages before installing the library/building the project:
+Make sure you have Python 3.8+ installed and set as default in the system.  
+
+You also need to install cryptographic packages before installing the library/building the project:
 
 #### Linux
 
 ##### Ubuntu, Debian and other apt-based distributions
 ```shell
 $ sudo apt install libsodium-dev libsecp256k1-dev libgmp-dev pkg-config
 ```
```

### Comparing `pytezos-3.8.0/pyproject.toml` & `pytezos-3.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytezos"
-version = "3.8.0"
+version = "3.9.0"
 description = "Python toolkit for Tezos"
 license = "MIT"
 authors = [
     "Michael Zaikin <mz@baking-bad.org>",
     "Lev Gorodetskii <pytezos@drsr.io>",
     "Arthur Breitman",
     "Roman Serikov",
```

### Comparing `pytezos-3.8.0/src/michelson_kernel/README.md` & `pytezos-3.9.0/src/michelson_kernel/README.md`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/michelson_kernel/cli.py` & `pytezos-3.9.0/src/michelson_kernel/cli.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/michelson_kernel/docs.py` & `pytezos-3.9.0/src/michelson_kernel/docs.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/michelson_kernel/kernel.js` & `pytezos-3.9.0/src/michelson_kernel/kernel.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -43,15 +43,15 @@
                 // data
                 {
                     regex: /(?:Unit|True|False|Pair|Left|Right|Some|None|Elt)(?=\s|;|\)|$)/,
                     token: "keyword"
                 },
                 // instruction
                 {
-                    regex: /(?:INT|ISNAT|CAST|RENAME|DROP|DUP|SWAP|PUSH|SOME|NONE|UNIT|IF_NONE|PAIR|CAR|CDR|LEFT|RIGHT|IF_LEFT|IF_RIGHT|NIL|CONS|IF_CONS|SIZE|EMPTY_SET|EMPTY_MAP|MAP|ITER|MEM|GET|UPDATE|IF|LOOP|LOOP_LEFT|LAMBDA|EXEC|DIP|FAILWITH|CONCAT|SLICE|PACK|UNPACK|ADD|SUB|MUL|EDIV|ABS|NEG|LSL|LSR|OR|AND|XOR|NOT|COMPARE|EQ|NEQ|LT|GT|LE|GE|CHECK_SIGNATURE|BLAKE2B|SHA256|SHA512|HASH_KEY|DIG|DUG|EMPTY_BIG_MAP|APPLY|NEVER|UNPAIR|VOTING_POWER|KECCAK|SHA3|PAIRING_CHECK|SAPLING_VERIFY_UPDATE|TICKET|READ_TICKET|SPLIT_TICKET|JOIN_TICKETS|GET_AND_UPDATE)(?=\s|;|\}|$)/,
+                    regex: /(?:INT|ISNAT|NAT|BYTES|CAST|RENAME|DROP|DUP|SWAP|PUSH|SOME|NONE|UNIT|IF_NONE|PAIR|CAR|CDR|LEFT|RIGHT|IF_LEFT|IF_RIGHT|NIL|CONS|IF_CONS|SIZE|EMPTY_SET|EMPTY_MAP|MAP|ITER|MEM|GET|UPDATE|IF|LOOP|LOOP_LEFT|LAMBDA|EXEC|DIP|FAILWITH|CONCAT|SLICE|PACK|UNPACK|ADD|SUB|MUL|EDIV|ABS|NEG|LSL|LSR|OR|AND|XOR|NOT|COMPARE|EQ|NEQ|LT|GT|LE|GE|CHECK_SIGNATURE|BLAKE2B|SHA256|SHA512|HASH_KEY|DIG|DUG|EMPTY_BIG_MAP|APPLY|NEVER|UNPAIR|VOTING_POWER|KECCAK|SHA3|PAIRING_CHECK|SAPLING_VERIFY_UPDATE|TICKET|READ_TICKET|SPLIT_TICKET|JOIN_TICKETS|GET_AND_UPDATE)(?=\s|;|\}|$)/,
                     token: "meta"
                 }, {
                     regex: /(?:SELF|CONTRACT|TRANSFER_TOKENS|SET_DELEGATE|CREATE_CONTRACT|IMPLICIT_ACCOUNT|NOW|AMOUNT|BALANCE|STEPS_TO_QUOTA|SOURCE|SENDER|ADDRESS|CHAIN_ID|LEVEL|SELF_ADDRESS|TOTAL_VOTING_POWER|SAPLING_EMPTY_STATE|MIN_BLOCK_TIME)(?=\s|;|\}|$)/,
                     token: "operator"
                 },
                 // type
                 {
```

### Comparing `pytezos-3.8.0/src/michelson_kernel/kernel.py` & `pytezos-3.9.0/src/michelson_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/__init__.py` & `pytezos-3.9.0/src/pytezos/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,10 +20,10 @@
 from pytezos.michelson.format import micheline_to_michelson
 from pytezos.michelson.micheline import MichelsonRuntimeError
 from pytezos.michelson.parse import michelson_to_micheline
 from pytezos.michelson.types.base import MichelsonType
 from pytezos.michelson.types.base import Undefined
 from pytezos.michelson.types.core import Unit
 
-__version__ = '3.8.0'
+__version__ = '3.9.0'
 
 pytezos = PyTezosClient()
```

### Comparing `pytezos-3.8.0/src/pytezos/block/forge.py` & `pytezos-3.9.0/src/pytezos/block/forge.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/block/header.py` & `pytezos-3.9.0/src/pytezos/block/header.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/cli/cli.py` & `pytezos-3.9.0/src/pytezos/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/cli/github.py` & `pytezos-3.9.0/src/pytezos/cli/github.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/client.py` & `pytezos-3.9.0/src/pytezos/client.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/context/abstract.py` & `pytezos-3.9.0/src/pytezos/context/abstract.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/context/impl.py` & `pytezos-3.9.0/src/pytezos/context/impl.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/context/mixin.py` & `pytezos-3.9.0/src/pytezos/context/mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     'sandbox': ['http://127.0.0.1:8732/'],
     'sandboxnet': ['http://127.0.0.1:8732/'],
     'localhost': ['http://127.0.0.1:8732/'],
     'ghostnet': ['https://rpc.tzkt.io/ghostnet'],
     'jakartanet': ['https://rpc.tzkt.io/jakartanet'],
     'kathmandunet': ['https://rpc.tzkt.io/kathmandunet'],
     'limanet': ['https://rpc.tzkt.io/limanet'],
+    'mumbainet': ['https://rpc.tzkt.io/mumbainet'],
 }
 keys = {
     'alice': alice_key,
     'dictator': dictator_key,
     'activator': dictator_key,
     'bootstrap1': 'edsk3gUfUPyBSfrS9CCgmCiQsTCHGkviBDusMxDJstFtojtc1zcpsh',
     'bootstrap2': 'edsk39qAm1fiMjgmPkw1EgQYkMzkJezLNewd7PLNHTkr6w9XA2zdfo',
```

### Comparing `pytezos-3.8.0/src/pytezos/contract/__init__.py` & `pytezos-3.9.0/src/pytezos/contract/__init__.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/contract/call.py` & `pytezos-3.9.0/src/pytezos/contract/call.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/contract/data.py` & `pytezos-3.9.0/src/pytezos/contract/data.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/contract/entrypoint.py` & `pytezos-3.9.0/src/pytezos/contract/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/contract/interface.py` & `pytezos-3.9.0/src/pytezos/contract/interface.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/contract/metadata-schema.json` & `pytezos-3.9.0/src/pytezos/contract/metadata-schema.json`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/contract/metadata.py` & `pytezos-3.9.0/src/pytezos/contract/metadata.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/contract/result.py` & `pytezos-3.9.0/src/pytezos/contract/result.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/contract/token_metadata-schema.json` & `pytezos-3.9.0/src/pytezos/contract/token_metadata-schema.json`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/contract/token_metadata.py` & `pytezos-3.9.0/src/pytezos/contract/token_metadata.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/contract/view.py` & `pytezos-3.9.0/src/pytezos/contract/view.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/crypto/encoding.py` & `pytezos-3.9.0/src/pytezos/crypto/encoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,18 @@
     (b"Lo", 52, tb([133, 233]), 32, "operation list hash"),
     (b"LLo", 53, tb([29, 159, 109]), 32, "operation list list hash"),
     (b"P", 51, tb([2, 170]), 32, "protocol hash"),
     (b"Co", 52, tb([79, 199]), 32, "context hash"),
     (b"tz1", 36, tb([6, 161, 159]), 20, "ed25519 public key hash"),
     (b"tz2", 36, tb([6, 161, 161]), 20, "secp256k1 public key hash"),
     (b"tz3", 36, tb([6, 161, 164]), 20, "p256 public key hash"),
+    (b"tz4", 36, tb([6, 161, 16]), 20, "BLS-MinPk"),
     (b"KT1", 36, tb([2, 90, 121]), 20, "originated address"),
-    # FIXME: replace with tb()
-    (b"txr1", 37, b'\x01\x80x\x1f', 20, "tx_rollup_l2_address"),
+    (b"txr1", 37, tb([1, 128, 120, 31]), 20, "tx_rollup_l2_address"),
+    (b"sr1", 36, tb([6, 124, 117]), 20, "address prefix for originated smart rollup"),
     (b"id", 30, tb([153, 103]), 16, "cryptobox public key hash"),
     (b'expr', 54, tb([13, 44, 64, 27]), 32, u'script expression'),
     (b"edsk", 54, tb([13, 15, 58, 7]), 32, "ed25519 seed"),
     (b"edpk", 54, tb([13, 15, 37, 217]), 32, "ed25519 public key"),
     (b"spsk", 54, tb([17, 162, 224, 201]), 32, "secp256k1 secret key"),
     (b"p2sk", 54, tb([16, 81, 238, 189]), 32, "p256 secret key"),
     (b"edesk", 88, tb([7, 90, 60, 179, 41]), 56, "ed25519 encrypted seed"),
@@ -120,15 +121,15 @@
 
 def validate_pkh(v: Union[str, bytes]):
     """Ensure parameter is a public key hash (starts with b'tz1', b'tz2', b'tz3')
 
     :param v: string or bytes
     :raises ValueError: if parameter is not a public key hash
     """
-    return _validate(v, prefixes=[b'tz1', b'tz2', b'tz3'])
+    return _validate(v, prefixes=[b'tz1', b'tz2', b'tz3', b'tz4'])
 
 
 def validate_l2_pkh(v: Union[str, bytes]):
     """Ensure parameter is a L2 public key hash (starts with b'txr1')
 
     :param v: string or bytes
     :raises ValueError: if parameter is not a public key hash
```

### Comparing `pytezos-3.8.0/src/pytezos/crypto/hash.py` & `pytezos-3.9.0/src/pytezos/crypto/hash.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/crypto/keccak.py` & `pytezos-3.9.0/src/pytezos/crypto/keccak.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/crypto/key.py` & `pytezos-3.9.0/src/pytezos/crypto/key.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/jupyter.py` & `pytezos-3.9.0/src/pytezos/jupyter.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/logging.py` & `pytezos-3.9.0/src/pytezos/logging.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/forge.py` & `pytezos-3.9.0/src/pytezos/michelson/forge.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,18 +159,22 @@
 
     if prefix == 'tz1':
         res = b'\x00\x00' + address
     elif prefix == 'tz2':
         res = b'\x00\x01' + address
     elif prefix == 'tz3':
         res = b'\x00\x02' + address
+    elif prefix == 'tz4':
+        res = b'\x00\x03' + address
     elif prefix == 'KT1':
         res = b'\x01' + address + b'\x00'
     elif prefix == 'txr1':
         res = b'\x02' + address + b'\x00'
+    elif prefix == 'sr1':
+        res = b'\x03' + address + b'\x00'
     else:
         raise ValueError(f'Can\'t forge address: unknown prefix `{prefix}`')
 
     return res[1:] if tz_only else res
 
 
 def unforge_address(data: bytes) -> str:
@@ -179,24 +183,27 @@
     :param data: encoded address or key_hash
     :returns: base58 encoded address
     """
     tz_prefixes = {
         b'\x00\x00': b'tz1',
         b'\x00\x01': b'tz2',
         b'\x00\x02': b'tz3',
+        b'\x00\x03': b'tz4',
     }
 
     for bin_prefix, tz_prefix in tz_prefixes.items():
         if data.startswith(bin_prefix):
             return base58_encode(data[2:], tz_prefix).decode()
 
     if data.startswith(b'\x01') and data.endswith(b'\x00'):
         return base58_encode(data[1:-1], b'KT1').decode()
     elif data.startswith(b'\x02') and data.endswith(b'\x00'):
         return base58_encode(data[1:-1], b'txr1').decode()
+    elif data.startswith(b'\x03') and data.endswith(b'\x00'):
+        return base58_encode(data[1:-1], b'sr1').decode()
     else:
         return base58_encode(data[1:], tz_prefixes[b'\x00' + data[:1]]).decode()
 
 
 def forge_contract(value: str) -> bytes:
     """Encode a value of contract type (address + optional entrypoint) into bytes.
```

### Comparing `pytezos-3.8.0/src/pytezos/michelson/format.py` & `pytezos-3.9.0/src/pytezos/michelson/format.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/instructions/__init__.py` & `pytezos-3.9.0/src/pytezos/michelson/instructions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 from pytezos.michelson.instructions.adt import LeftInstruction
 from pytezos.michelson.instructions.adt import PairInstruction
 from pytezos.michelson.instructions.adt import RightInstruction
 from pytezos.michelson.instructions.adt import UnpairInstruction
 from pytezos.michelson.instructions.adt import UpdatenInstruction
 from pytezos.michelson.instructions.arithmetic import AbsInstruction
 from pytezos.michelson.instructions.arithmetic import AddInstruction
+from pytezos.michelson.instructions.arithmetic import BytesInstruction
 from pytezos.michelson.instructions.arithmetic import EdivInstruction
 from pytezos.michelson.instructions.arithmetic import IntInstruction
 from pytezos.michelson.instructions.arithmetic import IsNatInstruction
 from pytezos.michelson.instructions.arithmetic import LslInstruction
 from pytezos.michelson.instructions.arithmetic import LsrInstruction
 from pytezos.michelson.instructions.arithmetic import MulInstruction
+from pytezos.michelson.instructions.arithmetic import NatInstruction
 from pytezos.michelson.instructions.arithmetic import NegInstruction
-from pytezos.michelson.instructions.arithmetic import SubInstruction
 from pytezos.michelson.instructions.boolean import AndInstruction
 from pytezos.michelson.instructions.boolean import NotInstruction
 from pytezos.michelson.instructions.boolean import OrInstruction
 from pytezos.michelson.instructions.boolean import XorInstruction
 from pytezos.michelson.instructions.compare import CompareInstruction
 from pytezos.michelson.instructions.compare import EqInstruction
 from pytezos.michelson.instructions.compare import GeInstruction
```

### Comparing `pytezos-3.8.0/src/pytezos/michelson/instructions/adt.py` & `pytezos-3.9.0/src/pytezos/michelson/instructions/adt.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/instructions/arithmetic.py` & `pytezos-3.9.0/src/pytezos/michelson/instructions/arithmetic.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from pytezos.michelson.instructions.base import MichelsonInstruction
 from pytezos.michelson.instructions.base import dispatch_types
 from pytezos.michelson.instructions.base import format_stdout
 from pytezos.michelson.stack import MichelsonStack
 from pytezos.michelson.types import BLS12_381_FrType
 from pytezos.michelson.types import BLS12_381_G1Type
 from pytezos.michelson.types import BLS12_381_G2Type
+from pytezos.michelson.types import BytesType
 from pytezos.michelson.types import IntType
 from pytezos.michelson.types import MutezType
 from pytezos.michelson.types import NatType
 from pytezos.michelson.types import OptionType
 from pytezos.michelson.types import PairType
 from pytezos.michelson.types import TimestampType
 from pytezos.michelson.types.base import MichelsonType
@@ -247,17 +248,21 @@
         stdout.append(format_stdout(cls.prim, [a, b], [res]))  # type: ignore
         return cls(stack_items_added=1)
 
 
 class IntInstruction(MichelsonInstruction, prim='INT'):
     @classmethod
     def execute(cls, stack: MichelsonStack, stdout: List[str], context: AbstractContext):
-        a = cast(Union[NatType, BLS12_381_FrType], stack.pop1())
-        a.assert_type_in(NatType, BLS12_381_FrType)
-        res = IntType.from_value(int(a))
+        a = stack.pop1()
+        if isinstance(a, BytesType):
+            res = IntType.from_value(int.from_bytes(bytes(a), 'big', signed=True))
+        else:
+            a = cast(Union[NatType, BLS12_381_FrType], a)
+            a.assert_type_in(NatType, BLS12_381_FrType)
+            res = IntType.from_value(int(a))
         stack.push(res)
         stdout.append(f'{cls.prim} / {repr(a)} => {repr(res)}')
         return cls(stack_items_added=1)
 
 
 class IsNatInstruction(MichelsonInstruction, prim='ISNAT'):
     @classmethod
@@ -267,7 +272,37 @@
         if int(a) >= 0:
             res = OptionType.from_some(NatType.from_value(int(a)))
         else:
             res = OptionType.none(NatType)
         stack.push(res)
         stdout.append(format_stdout(cls.prim, [a], [res]))  # type: ignore
         return cls(stack_items_added=1)
+
+
+class NatInstruction(MichelsonInstruction, prim='NAT'):
+    @classmethod
+    def execute(cls, stack: MichelsonStack, stdout: List[str], context: AbstractContext):
+        a = cast(BytesType, stack.pop1())
+        a.assert_type_in(BytesType)
+        res = NatType.from_value(int.from_bytes(bytes(a), 'big'))
+        stack.push(res)
+        stdout.append(f'{cls.prim} / {repr(a)} => {repr(res)}')
+        return cls(stack_items_added=1)
+
+
+class BytesInstruction(MichelsonInstruction, prim='BYTES'):
+    @classmethod
+    def execute(cls, stack: MichelsonStack, stdout: List[str], context: AbstractContext):
+        a = cast(Union[NatType, IntType], stack.pop1())
+        a.assert_type_in(NatType, IntType)
+        int_val = int(a)
+        signed = isinstance(a, IntType)
+        if signed:
+            length = (8 + (int_val + (int_val < 0)).bit_length()) // 8
+        else:
+            length = (7 + int_val.bit_length()) // 8
+        # NOTE: the shortest big-endian encoding of natural number or integer n
+        byte_val = int_val.to_bytes(length, 'big', signed=signed).lstrip(b'\x00')
+        res = BytesType.from_value(byte_val)
+        stack.push(res)
+        stdout.append(f'{cls.prim} / {repr(a)} => {repr(res)}')
+        return cls(stack_items_added=1)
```

### Comparing `pytezos-3.8.0/src/pytezos/michelson/instructions/base.py` & `pytezos-3.9.0/src/pytezos/michelson/instructions/base.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/instructions/boolean.py` & `pytezos-3.9.0/src/pytezos/michelson/instructions/boolean.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/instructions/compare.py` & `pytezos-3.9.0/src/pytezos/michelson/instructions/compare.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/instructions/control.py` & `pytezos-3.9.0/src/pytezos/michelson/instructions/control.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/instructions/crypto.py` & `pytezos-3.9.0/src/pytezos/michelson/instructions/crypto.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     @classmethod
     def execute(cls, stack: MichelsonStack, stdout: List[str], context: AbstractContext):
         pk, sig, msg = cast(Tuple[KeyType, SignatureType, BytesType], stack.pop3())
         pk.assert_type_equal(KeyType)
         sig.assert_type_equal(SignatureType)
         msg.assert_type_equal(BytesType)
         key = Key.from_encoded_key(str(pk))
+        # TODO: verify BLS signatures
         try:
             key.verify(signature=str(sig), message=bytes(msg))
         except ValueError:
             res = BoolType(False)
         else:
             res = BoolType(True)
         stack.push(res)
```

### Comparing `pytezos-3.8.0/src/pytezos/michelson/instructions/generic.py` & `pytezos-3.9.0/src/pytezos/michelson/instructions/generic.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/instructions/jupyter.py` & `pytezos-3.9.0/src/pytezos/michelson/instructions/jupyter.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/instructions/stack.py` & `pytezos-3.9.0/src/pytezos/michelson/instructions/stack.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/instructions/struct.py` & `pytezos-3.9.0/src/pytezos/michelson/instructions/struct.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/instructions/tezos.py` & `pytezos-3.9.0/src/pytezos/michelson/instructions/tezos.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/instructions/ticket.py` & `pytezos-3.9.0/src/pytezos/michelson/instructions/ticket.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/instructions/tzt.py` & `pytezos-3.9.0/src/pytezos/michelson/instructions/tzt.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/macros.py` & `pytezos-3.9.0/src/pytezos/michelson/macros.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/micheline.py` & `pytezos-3.9.0/src/pytezos/michelson/micheline.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/parse.py` & `pytezos-3.9.0/src/pytezos/michelson/parse.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/program.py` & `pytezos-3.9.0/src/pytezos/michelson/program.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/repl.py` & `pytezos-3.9.0/src/pytezos/michelson/repl.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/sections/code.py` & `pytezos-3.9.0/src/pytezos/michelson/sections/code.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/sections/parameter.py` & `pytezos-3.9.0/src/pytezos/michelson/sections/parameter.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/sections/storage.py` & `pytezos-3.9.0/src/pytezos/michelson/sections/storage.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/sections/tzt.py` & `pytezos-3.9.0/src/pytezos/michelson/sections/tzt.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/sections/view.py` & `pytezos-3.9.0/src/pytezos/michelson/sections/view.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/stack.py` & `pytezos-3.9.0/src/pytezos/michelson/stack.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/tags.py` & `pytezos-3.9.0/src/pytezos/michelson/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,17 @@
     'sapling_transaction': b'\x96',
     # KATHMANDU
     'EMIT': b'\x97',
     # LIMA
     'Lambda_rec': b'\x98',
     'LAMBDA_REC': b'\x99',
     'TICKET': b'\x9A',
+    # MUMBAI
+    'BYTES': b'\x9B',
+    'NAT': b'\x9C',
     # FIXME: Dummy values for TZT, refactor macros
     'Stack_elt': b'\xEE',
     'Big_map': b'\xEE',
     'input': b'\xEE',
     'output': b'\xEE',
     'sender': b'\xEE',
     'amount': b'\xEE',
```

### Comparing `pytezos-3.8.0/src/pytezos/michelson/types/__init__.py` & `pytezos-3.9.0/src/pytezos/michelson/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/types/adt.py` & `pytezos-3.9.0/src/pytezos/michelson/types/adt.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/types/base.py` & `pytezos-3.9.0/src/pytezos/michelson/types/base.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/types/big_map.py` & `pytezos-3.9.0/src/pytezos/michelson/types/big_map.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/types/bls.py` & `pytezos-3.9.0/src/pytezos/michelson/types/bls.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/types/core.py` & `pytezos-3.9.0/src/pytezos/michelson/types/core.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/types/domain.py` & `pytezos-3.9.0/src/pytezos/michelson/types/domain.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/types/list.py` & `pytezos-3.9.0/src/pytezos/michelson/types/list.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/types/map.py` & `pytezos-3.9.0/src/pytezos/michelson/types/map.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/types/operation.py` & `pytezos-3.9.0/src/pytezos/michelson/types/operation.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/types/option.py` & `pytezos-3.9.0/src/pytezos/michelson/types/option.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/types/pair.py` & `pytezos-3.9.0/src/pytezos/michelson/types/pair.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/types/sapling.py` & `pytezos-3.9.0/src/pytezos/michelson/types/sapling.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/types/set.py` & `pytezos-3.9.0/src/pytezos/michelson/types/set.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/types/sum.py` & `pytezos-3.9.0/src/pytezos/michelson/types/sum.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/michelson/types/ticket.py` & `pytezos-3.9.0/src/pytezos/michelson/types/ticket.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/operation/content.py` & `pytezos-3.9.0/src/pytezos/operation/content.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/operation/fees.py` & `pytezos-3.9.0/src/pytezos/operation/fees.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/operation/forge.py` & `pytezos-3.9.0/src/pytezos/operation/forge.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/operation/group.py` & `pytezos-3.9.0/src/pytezos/operation/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,16 @@
         self.opg_result = opg_result
 
     def __repr__(self) -> str:
         res = [
             super().__repr__(),
             '\nPayload',
             pformat(self.json_payload()),
-            '\nHelpers',
+            '\nHash',
+            self.opg_hash or '(Not sent)' '\nHelpers',
             get_class_docstring(self.__class__),
         ]
         return '\n'.join(res)
 
     def _spawn(self, **kwargs) -> 'OperationGroup':
         return OperationGroup(
             context=self.context,
@@ -110,26 +111,29 @@
         minimal_nanotez_per_gas_unit: Optional[int] = None,
         **kwargs,
     ) -> 'OperationGroup':
         """Try to fill all fields left unfilled, use approximate fees
         (not optimal, use `autofill` to simulate operation and get precise values).
 
         :param counter: Override counter value (for manual handling)
-        :param ttl: Number of blocks to wait in the mempool before removal (default is 5 for public network, 60 for sandbox)
+        :param ttl: Number of blocks to wait in the mempool before removal (default is 5 for public network, MAX for sandbox),
+            -1 for MAX (if you have a private network and issues with block RPC queries)
         :param gas_limit: Override gas_limit value (for manual handling)
         :param storage_limit: Override storage_limit value (for manual handling)
         :param minimal_nanotez_per_gas_unit: Override minimal_nanotez_per_gas_unit constant (for manual handling)
         :rtype: OperationGroup
         """
         if kwargs.get('branch_offset') is not None:
             logger.warning('`branch_offset` argument is deprecated, use `ttl` instead')
             ttl = MAX_OPERATIONS_TTL - kwargs['branch_offset']
 
         if ttl is None:
             ttl = self.context.get_operations_ttl()
+        elif ttl == -1:
+            ttl = MAX_OPERATIONS_TTL
         if not 0 < ttl <= MAX_OPERATIONS_TTL:
             raise Exception(f'`ttl` has to be in range (0, {MAX_OPERATIONS_TTL}]')
 
         chain_id = self.chain_id or self.context.get_chain_id()
         protocol = self.protocol or self.context.get_protocol()
         branch = self.branch or self.shell.blocks[f'head~{MAX_OPERATIONS_TTL - ttl}'].hash()
         source = self.key.public_key_hash()
```

### Comparing `pytezos-3.8.0/src/pytezos/operation/result.py` & `pytezos-3.9.0/src/pytezos/operation/result.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/protocol/diff.py` & `pytezos-3.9.0/src/pytezos/protocol/diff.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/protocol/protocol.py` & `pytezos-3.9.0/src/pytezos/protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/rpc/docs.py` & `pytezos-3.9.0/src/pytezos/rpc/docs.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/rpc/errors.py` & `pytezos-3.9.0/src/pytezos/rpc/errors.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/rpc/helpers.py` & `pytezos-3.9.0/src/pytezos/rpc/helpers.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/rpc/kind.py` & `pytezos-3.9.0/src/pytezos/rpc/kind.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/rpc/node.py` & `pytezos-3.9.0/src/pytezos/rpc/node.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/rpc/protocol.py` & `pytezos-3.9.0/src/pytezos/rpc/protocol.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/rpc/query.py` & `pytezos-3.9.0/src/pytezos/rpc/query.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/rpc/search.py` & `pytezos-3.9.0/src/pytezos/rpc/search.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/rpc/shell.py` & `pytezos-3.9.0/src/pytezos/rpc/shell.py`

 * *Files identical despite different names*

### Comparing `pytezos-3.8.0/src/pytezos/sandbox/node.py` & `pytezos-3.9.0/src/pytezos/sandbox/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from testcontainers.core.generic import DockerContainer  # type: ignore
 
 from pytezos.client import PyTezosClient
 from pytezos.operation.group import OperationGroup
 from pytezos.sandbox.parameters import LATEST
 from pytezos.sandbox.parameters import sandbox_addresses
 
-DOCKER_IMAGE = 'bakingbad/sandboxed-node:v15.0-1'
+DOCKER_IMAGE = 'bakingbad/sandboxed-node:v16.0-2'
 MAX_ATTEMPTS = 100
 ATTEMPT_DELAY = 0.1
 TEZOS_NODE_PORT = 8732
 
 
 def kill_existing_containers():
     docker = DockerClient()
```

### Comparing `pytezos-3.8.0/src/pytezos/sandbox/parameters.py` & `pytezos-3.9.0/src/pytezos/sandbox/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 FLORENCE = 'PsFLorenaUUuikDWvMDr6fGBRG8kt3e3D3fHoXK1j1BFRxeSH4i'
 GRANADA = 'PtGRANADsDU8R9daYKAgWnQYAJ64omN1o3KMGVCykShA97vQbvV'
 HANGZHOU = 'PtHangz2aRngywmSRGGvrcTyMbbdpWdpFKuS4uMWxg2RaH9i1qx'
 ITHACA = 'Psithaca2MLRFYargivpo7YvUr7wUDqyxrdhC5CQq78mRvimz6A'
 JAKARTA = 'PtJakart2xVj7pYXJBXrqHgd82rdkLey5ZeeGwDgPp9rhQUbSqY'
 KATHMANDU = 'PtKathmankSpLLDALzWw7CGD2j2MtyveTwboEYokqUCP4a1LxMg'
 LIMA = 'PtLimaPtLMwfNinJi9rCfDPWea8dFgTZ1MeJ9f1m2SRic6ayiwW'
-LATEST = LIMA
+MUMBAI = 'PtMumbai2TmsJHNGRkD8v8YDbtao7BLUC3wjASn1inAKLFCjaH1'
+LATEST = MUMBAI
 
 protocol_version = {
     EDO: 8,
     FLORENCE: 9,
     GRANADA: 10,
     HANGZHOU: 11,
     ITHACA: 12,
     JAKARTA: 13,
     KATHMANDU: 14,
     LIMA: 15,
+    MUMBAI: 16,
 }
 
 sandbox_commitment = {
     "mnemonic": [
         "arctic",
         "blame",
         "brush",
@@ -90,15 +92,15 @@
 }
 
 
 def get_protocol_parameters(protocol_hash: str) -> Dict[str, Any]:
     return {
         **sandbox_params.copy(),
         'cache_sampler_state_cycles': 8.0,
-        'tx_rollup_enable': True,
+        'tx_rollup_enable': False,
         'tx_rollup_origination_size': 4000.0,
         'liquidity_baking_toggle_ema_threshold': 1000000000.0,
         'cache_script_size': 100000000.0,
         'cache_stake_distribution_cycles': 8.0,
         'tx_rollup_hard_size_limit_per_inbox': 500000.0,
         'tx_rollup_hard_size_limit_per_message': 5000.0,
         'tx_rollup_max_withdrawals_per_batch': 15.0,
@@ -108,26 +110,27 @@
         'tx_rollup_max_inboxes_count': 40100.0,
         'tx_rollup_max_messages_per_inbox': 1010.0,
         'tx_rollup_max_commitments_count': 80100.0,
         'tx_rollup_cost_per_byte_ema_factor': 120.0,
         'tx_rollup_max_ticket_payload_size': 2048.0,
         'tx_rollup_rejection_max_proof_size': 30000.0,
         'tx_rollup_sunset_level': 3473409.0,
-        'sc_rollup_enable': False,
-        'sc_rollup_origination_size': 6314.0,
-        'sc_rollup_challenge_window_in_blocks': 20160.0,
-        'sc_rollup_max_number_of_messages_per_commitment_period': 300000000.0,
-        'sc_rollup_stake_amount': '32000000',
-        'sc_rollup_commitment_period_in_blocks': 30.0,
-        'sc_rollup_max_lookahead_in_blocks': 30000.0,
-        'sc_rollup_max_active_outbox_levels': 20160.0,
-        'sc_rollup_max_outbox_messages_per_level': 100.0,
-        'sc_rollup_number_of_sections_in_dissection': 32.0,
-        'sc_rollup_timeout_period_in_blocks': 20160.0,
-        'sc_rollup_max_number_of_cemented_commitments': 5.0,
+        'smart_rollup_enable': True,
+        'smart_rollup_arith_pvm_enable': False,
+        'smart_rollup_origination_size': 6314.0,
+        'smart_rollup_challenge_window_in_blocks': 20160.0,
+        'smart_rollup_stake_amount': '32000000',
+        'smart_rollup_commitment_period_in_blocks': 30.0,
+        'smart_rollup_max_lookahead_in_blocks': 30000.0,
+        'smart_rollup_max_active_outbox_levels': 20160.0,
+        'smart_rollup_max_outbox_messages_per_level': 100.0,
+        'smart_rollup_number_of_sections_in_dissection': 32.0,
+        'smart_rollup_timeout_period_in_blocks': 20160.0,
+        'smart_rollup_max_number_of_cemented_commitments': 5.0,
+        'smart_rollup_max_number_of_parallel_games': 32.0,
         'zk_rollup_enable': False,
         'zk_rollup_origination_size': 4000.0,
         'zk_rollup_min_pending_to_process': 10.0,
         'blocks_per_stake_snapshot': 4.0,
         'consensus_committee_size': 526.0,
         'consensus_threshold': 0.0,
         'baking_reward_fixed_portion': '333333',
@@ -143,16 +146,16 @@
         'minimal_block_delay': '1',
         'liquidity_baking_subsidy': '2500000',
         'nonce_revelation_threshold': 2.0,
         'vdf_difficulty': '50000',
         'dal_parametric': {
             'feature_enable': False,
             'number_of_slots': 16.0,
-            'number_of_shards': 256.0,
-            'endorsement_lag': 1.0,
+            'attestation_lag': 1.0,
             'availability_threshold': 50.0,
-            'slot_size': 1048576.0,
             'redundancy_factor': 16.0,
             'page_size': 4096.0,
+            'slot_size': 1048576.0,
+            'number_of_shards': 256.0,
         },
         'minimal_stake': '6000',
     }
```

### Comparing `pytezos-3.8.0/PKG-INFO` & `pytezos-3.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytezos
-Version: 3.8.0
+Version: 3.9.0
 Summary: Python toolkit for Tezos
 Home-page: https://pytezos.org
 License: MIT
 Keywords: tezos,blockchain,sdk,michelson,repl,cryptocurrencies,smart-contracts,jupyter,ipython,docker,crypto
 Author: Michael Zaikin
 Author-email: mz@baking-bad.org
 Maintainer: Michael Zaikin
@@ -95,15 +95,17 @@
 #### Michelson integration testing framework
 * Writing integration tests using `unittest` package
 * Simulating contract execution using remote intepreter (via RPC) or builtin one
 
 
 ## Installation
 
-You need to install cryptographic packages before installing the library/building the project:
+Make sure you have Python 3.8+ installed and set as default in the system.  
+
+You also need to install cryptographic packages before installing the library/building the project:
 
 #### Linux
 
 ##### Ubuntu, Debian and other apt-based distributions
 ```shell
 $ sudo apt install libsodium-dev libsecp256k1-dev libgmp-dev pkg-config
 ```
```

