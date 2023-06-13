# Comparing `tmp/ape-solidity-0.6.5.tar.gz` & `tmp/ape-solidity-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-solidity-0.6.5.tar", last modified: Mon May 22 13:35:38 2023, max compression
+gzip compressed data, was "ape-solidity-0.6.6.tar", last modified: Tue Jun 13 01:25:00 2023, max compression
```

## Comparing `ape-solidity-0.6.5.tar` & `ape-solidity-0.6.6.tar`

### file list

```diff
@@ -1,123 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.229597 ape-solidity-0.6.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-22 13:35:38.229597 ape-solidity-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/ape_solidity/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/ape_solidity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/ape_solidity/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29107 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/ape_solidity/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/ape_solidity/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/ape_solidity/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 13:35:37.000000 ape-solidity-0.6.5/ape_solidity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/ape_solidity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-22 13:35:37.000000 ape-solidity-0.6.5/ape_solidity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-22 13:35:38.000000 ape-solidity-0.6.5/ape_solidity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:35:37.000000 ape-solidity-0.6.5/ape_solidity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:35:37.000000 ape-solidity-0.6.5/ape_solidity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-22 13:35:37.000000 ape-solidity-0.6.5/ape_solidity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 13:35:37.000000 ape-solidity-0.6.5/ape_solidity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-22 13:35:38.229597 ape-solidity-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/BrownieProject/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/BrownieProject/brownie-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/BrownieProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/BrownieProject/contracts/BrownieContract.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/BrownieStyleDependency/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/BrownieStyleDependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/BrownieStyleDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/BrownieStyleDependency/contracts/BrownieStyleDependency.sol
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/BrownieStyleDependency/contracts/FailingContract.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/Dependency/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/Dependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/Dependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/Dependency/contracts/Dependency.sol
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/Dependency/contracts/OlderDependency.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/Dependency/contracts/subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/Dependency/contracts/subfolder/InDependencySubfolder.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/Dependency/contracts/subfolder_with_imports/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/DependencyOfDependency/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/DependencyOfDependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.221598 ape-solidity-0.6.5/tests/DependencyOfDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/ProjectWithinProject/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/ProjectWithinProject/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/ProjectWithinProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/ProjectWithinProject/contracts/Contract.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/VersionSpecifiedInConfig/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/VersionSpecifiedInConfig/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/VersionSpecifiedInConfig/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/CircularImport1.sol
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/CircularImport2.sol
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/CompilesOnce.sol
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/DifferentNameThanFile.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/contracts/DirectoryWithExtension.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/DirectoryWithExtension.sol/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/ExperimentalABIEncoderV2.sol
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/ImportOlderDependency.sol
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/ImportSourceWithEqualSignVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/ImportSourceWithNoPrefixVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/ImportingLessConstrainedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/Imports.sol
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanionImport.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/LibraryFun.sol
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/MissingPragma.sol
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/MultipleDefinitions.sol
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/NumerousDefinitions.sol
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/OlderVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/RandomVyperFile.vy
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/RangedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/SpacesInPragma.sol
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/SpecificVersionNoPrefix.sol
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/SpecificVersionNoPrefix2.sol
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/SpecificVersionRange.sol
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/SpecificVersionWithEqualSign.sol
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/UseYearn.sol
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/VagueVersion.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/contracts/subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/subfolder/Relativecontract.sol
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.217598 ape-solidity-0.6.5/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.217598 ape-solidity-0.6.5/tests/data/packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.217598 ape-solidity-0.6.5/tests/data/packages/OpenZeppelin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/data/packages/OpenZeppelin/v4.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)   698486 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.225597 ape-solidity-0.6.5/tests/data/packages/OpenZeppelin/v4.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)   879002 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.217598 ape-solidity-0.6.5/tests/data/packages/vault/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.229597 ape-solidity-0.6.5/tests/data/packages/vault/master/
--rw-r--r--   0 runner    (1001) docker     (123)   167518 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/data/packages/vault/master/vault_main.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.229597 ape-solidity-0.6.5/tests/data/packages/vault/v0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)   167551 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/data/packages/vault/v0.4.5/vault.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:35:38.229597 ape-solidity-0.6.5/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/scripts/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-22 13:34:34.000000 ape-solidity-0.6.5/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.455625 ape-solidity-0.6.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.439625 ape-solidity-0.6.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.443625 ape-solidity-0.6.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.443625 ape-solidity-0.6.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-13 01:25:00.455625 ape-solidity-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.443625 ape-solidity-0.6.6/ape_solidity/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/ape_solidity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/ape_solidity/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31520 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/ape_solidity/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/ape_solidity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/ape_solidity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 01:25:00.000000 ape-solidity-0.6.6/ape_solidity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.443625 ape-solidity-0.6.6/ape_solidity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-13 01:25:00.000000 ape-solidity-0.6.6/ape_solidity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-13 01:25:00.000000 ape-solidity-0.6.6/ape_solidity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:25:00.000000 ape-solidity-0.6.6/ape_solidity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:25:00.000000 ape-solidity-0.6.6/ape_solidity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 01:25:00.000000 ape-solidity-0.6.6/ape_solidity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 01:25:00.000000 ape-solidity-0.6.6/ape_solidity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 01:25:00.455625 ape-solidity-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.443625 ape-solidity-0.6.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.443625 ape-solidity-0.6.6/tests/BrownieProject/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/BrownieProject/brownie-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/BrownieProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/BrownieProject/contracts/BrownieContract.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/BrownieStyleDependency/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/BrownieStyleDependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/BrownieStyleDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/BrownieStyleDependency/contracts/BrownieStyleDependency.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/BrownieStyleDependency/contracts/FailingContract.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/Dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/Dependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/Dependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/Dependency/contracts/Dependency.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/Dependency/contracts/OlderDependency.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/Dependency/contracts/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/Dependency/contracts/subfolder/InDependencySubfolder.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/Dependency/contracts/subfolder_with_imports/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/DependencyOfDependency/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/DependencyOfDependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/DependencyOfDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/ProjectWithinProject/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/ProjectWithinProject/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/ProjectWithinProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/ProjectWithinProject/contracts/Contract.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/VersionSpecifiedInConfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/VersionSpecifiedInConfig/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/VersionSpecifiedInConfig/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.451625 ape-solidity-0.6.6/tests/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/BuiltinErrorChecker.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/CircularImport1.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/CircularImport2.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/CompilesOnce.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/DifferentNameThanFile.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.451625 ape-solidity-0.6.6/tests/contracts/DirectoryWithExtension.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/DirectoryWithExtension.sol/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/ExperimentalABIEncoderV2.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/ImportOlderDependency.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/ImportSourceWithEqualSignVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/ImportSourceWithNoPrefixVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/ImportingLessConstrainedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/Imports.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanionImport.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/LibraryFun.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/MissingPragma.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/MultipleDefinitions.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/NumerousDefinitions.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/OlderVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/RandomVyperFile.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/RangedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/SpacesInPragma.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/SpecificVersionNoPrefix.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/SpecificVersionNoPrefix2.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/SpecificVersionRange.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/SpecificVersionWithEqualSign.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/UseYearn.sol
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/VagueVersion.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.451625 ape-solidity-0.6.6/tests/contracts/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/subfolder/Relativecontract.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.439625 ape-solidity-0.6.6/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.439625 ape-solidity-0.6.6/tests/data/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.439625 ape-solidity-0.6.6/tests/data/packages/OpenZeppelin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.451625 ape-solidity-0.6.6/tests/data/packages/OpenZeppelin/v4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   698486 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.451625 ape-solidity-0.6.6/tests/data/packages/OpenZeppelin/v4.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)   879002 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.439625 ape-solidity-0.6.6/tests/data/packages/vault/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.455625 ape-solidity-0.6.6/tests/data/packages/vault/master/
+-rw-r--r--   0 runner    (1001) docker     (123)   167518 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/data/packages/vault/master/vault_main.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.455625 ape-solidity-0.6.6/tests/data/packages/vault/v0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)   167551 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/data/packages/vault/v0.4.5/vault.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.455625 ape-solidity-0.6.6/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/scripts/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16954 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/test_integration.py
```

### Comparing `ape-solidity-0.6.5/.github/ISSUE_TEMPLATE/bug.md` & `ape-solidity-0.6.6/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/.github/ISSUE_TEMPLATE/feature.md` & `ape-solidity-0.6.6/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/.github/ISSUE_TEMPLATE/work-item.md` & `ape-solidity-0.6.6/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/.github/release-drafter.yml` & `ape-solidity-0.6.6/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/.github/workflows/codeql.yml` & `ape-solidity-0.6.6/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/.github/workflows/prtitle.yaml` & `ape-solidity-0.6.6/.github/workflows/prtitle.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
           env:
               TITLE: ${{ github.event.pull_request.title }}
```

### Comparing `ape-solidity-0.6.5/.github/workflows/publish.yaml` & `ape-solidity-0.6.6/.github/workflows/publish.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
         
     - name: Build
```

### Comparing `ape-solidity-0.6.5/.github/workflows/stale-prs.yml` & `ape-solidity-0.6.6/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/.github/workflows/test.yaml` & `ape-solidity-0.6.6/.github/workflows/test.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
 
         - name: Run Black
@@ -43,15 +43,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint,test]
 
         - name: Run MyPy
@@ -59,15 +59,15 @@
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, '3.10']
+                python-version: [3.8, 3.9, '3.10', '3.11']
 
         env:
           GITHUB_ACCESS_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
         steps:
         - uses: actions/checkout@v3
 
@@ -93,14 +93,14 @@
 
     #     steps:
     #     - uses: actions/checkout@v3
 
     #     - name: Setup Python
     #       uses: actions/setup-python@v4
     #       with:
-    #           python-version: 3.8
+    #           python-version: "3.10"
 
     #     - name: Install Dependencies
     #       run: pip install .[test]
 
     #     - name: Run Tests
     #       run: pytest -m "fuzzing" --no-cov -s
```

### Comparing `ape-solidity-0.6.5/.gitignore` & `ape-solidity-0.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/.pre-commit-config.yaml` & `ape-solidity-0.6.6/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.991
     hooks:
     -   id: mypy
-        additional_dependencies: [types-requests, types-setuptools, pydantic]
+        additional_dependencies: [types-requests, types-setuptools, pydantic, types-pkg-resources]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.14
     hooks:
     -   id: mdformat
         additional_dependencies: [mdformat-gfm, mdformat-frontmatter]
```

### Comparing `ape-solidity-0.6.5/CONTRIBUTING.md` & `ape-solidity-0.6.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/LICENSE` & `ape-solidity-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/PKG-INFO` & `ape-solidity-0.6.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,144 +1,145 @@
 Metadata-Version: 2.1
 Name: ape-solidity
-Version: 0.6.5
+Version: 0.6.6
 Summary: Plugin for Ape Ethereum Framework for compiling Solidity contracts
 Home-page: https://github.com/ApeWorX/ape-solidity
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Compile Solidity contracts.
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-solidity
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-solidity.git
-        cd ape-solidity
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        In your project, make sure you have a `contracts/` directory containing Solidity files (`.sol`).
-        
-        Then, while this plugin is installed, compile your contracts:
-        
-        ```bash
-        ape compile
-        ```
-        
-        The byte-code and ABI for your contracts should now exist in a `__local__.json` file in a `.build/` directory.
-        
-        ### Dependency Mapping
-        
-        To configure import remapping, use your project's `ape-config.yaml` file:
-        
-        ```yaml
-        solidity:
-          import_remapping:
-            - "@openzeppelin=path/to/open_zeppelin/contracts"
-        ```
-        
-        If you are using the `dependencies:` key in your `ape-config.yaml`, `ape` can automatically
-        search those dependencies for the path.
-        
-        ```yaml
-        dependencies:
-          - name: OpenZeppelin
-            github: OpenZeppelin/openzeppelin-contracts
-            version: 4.4.2
-        
-        solidity:
-          import_remapping:
-            - "@openzeppelin=OpenZeppelin/4.4.2"
-        ```
-        
-        Once you have your dependencies configured, you can import packages using your import keys:
-        
-        ```solidity
-        import "@openzeppelin/token/ERC721/ERC721.sol";
-        ```
-        
-        ### Library Linking
-        
-        To compile contracts that use libraries, you need to add the libraries first.
-        Use the `add_library()` method from the `ape-solidity` compiler class to add the library.
-        A typical flow is:
-        
-        1. Deploy the library.
-        2. Call `add_library()` using the Solidity compiler plugin, which will also re-compile contracts that need the library.
-        3. Deploy and use contracts that require the library.
-        
-        For example:
-        
-        ```python
-        import pytest
-        
-        
-        @pytest.fixture
-        def contract(accounts, project, compilers):
-            # Deploy the library.
-            account = accounts[0]
-            library = project.Set.deploy(sender=account)
-            
-            # Add the library to Solidity (re-compiles contracts that use the library).
-            compilers.solidity.add_library(library)
-        
-            # Deploy the contract that uses the library.
-            return project.C.deploy(sender=account)
-        ```
-        
-        ### Compiler Settings
-        
-        When using `ape-solidity`, your project's manifest's compiler settings will include standard JSON output.
-        You should have one listed `compiler` per `solc` version used in your project.
-        You can view your current project manifest, including the compiler settings, by doing:
-        
-        ```python
-        from ape import project
-        
-        manifest = project.extract_manifest()
-        
-        for compiler_entry in manifest.compilers:
-            print(compiler_entry.version)
-            print(compiler_entry.settings)
-        ```
-        
-        **NOTE**: These are the settings used during contract verification when using the [Etherscan plugin](https://github.com/ApeWorX/ape-etherscan).
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Compile Solidity contracts.
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+
+## Installation
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-solidity
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-solidity.git
+cd ape-solidity
+python3 setup.py install
+```
+
+## Quick Usage
+
+In your project, make sure you have a `contracts/` directory containing Solidity files (`.sol`).
+
+Then, while this plugin is installed, compile your contracts:
+
+```bash
+ape compile
+```
+
+The byte-code and ABI for your contracts should now exist in a `__local__.json` file in a `.build/` directory.
+
+### Dependency Mapping
+
+To configure import remapping, use your project's `ape-config.yaml` file:
+
+```yaml
+solidity:
+  import_remapping:
+    - "@openzeppelin=path/to/open_zeppelin/contracts"
+```
+
+If you are using the `dependencies:` key in your `ape-config.yaml`, `ape` can automatically
+search those dependencies for the path.
+
+```yaml
+dependencies:
+  - name: OpenZeppelin
+    github: OpenZeppelin/openzeppelin-contracts
+    version: 4.4.2
+
+solidity:
+  import_remapping:
+    - "@openzeppelin=OpenZeppelin/4.4.2"
+```
+
+Once you have your dependencies configured, you can import packages using your import keys:
+
+```solidity
+import "@openzeppelin/token/ERC721/ERC721.sol";
+```
+
+### Library Linking
+
+To compile contracts that use libraries, you need to add the libraries first.
+Use the `add_library()` method from the `ape-solidity` compiler class to add the library.
+A typical flow is:
+
+1. Deploy the library.
+2. Call `add_library()` using the Solidity compiler plugin, which will also re-compile contracts that need the library.
+3. Deploy and use contracts that require the library.
+
+For example:
+
+```python
+import pytest
+
+
+@pytest.fixture
+def contract(accounts, project, compilers):
+    # Deploy the library.
+    account = accounts[0]
+    library = project.Set.deploy(sender=account)
+    
+    # Add the library to Solidity (re-compiles contracts that use the library).
+    compilers.solidity.add_library(library)
+
+    # Deploy the contract that uses the library.
+    return project.C.deploy(sender=account)
+```
+
+### Compiler Settings
+
+When using `ape-solidity`, your project's manifest's compiler settings will include standard JSON output.
+You should have one listed `compiler` per `solc` version used in your project.
+You can view your current project manifest, including the compiler settings, by doing:
+
+```python
+from ape import project
+
+manifest = project.extract_manifest()
+
+for compiler_entry in manifest.compilers:
+    print(compiler_entry.version)
+    print(compiler_entry.settings)
+```
+
+**NOTE**: These are the settings used during contract verification when using the [Etherscan plugin](https://github.com/ApeWorX/ape-etherscan).
```

### Comparing `ape-solidity-0.6.5/README.md` & `ape-solidity-0.6.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Compile Solidity contracts.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-solidity-0.6.5/ape_solidity/_utils.py` & `ape-solidity-0.6.6/ape_solidity/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,24 @@
 from semantic_version import NpmSpec, Version  # type: ignore
 from solcx.exceptions import SolcError  # type: ignore
 from solcx.install import get_executable  # type: ignore
 from solcx.wrapper import VERSION_REGEX  # type: ignore
 
 from ape_solidity.exceptions import IncorrectMappingFormatError
 
+OUTPUT_SELECTION = [
+    "abi",
+    "bin-runtime",
+    "devdoc",
+    "userdoc",
+    "evm.bytecode.object",
+    "evm.bytecode.sourceMap",
+    "evm.deployedBytecode.object",
+]
+
 
 class Extension(Enum):
     SOL = ".sol"
 
 
 class ImportRemapping(BaseModel):
     entry: str
```

### Comparing `ape-solidity-0.6.5/ape_solidity/compiler.py` & `ape-solidity-0.6.6/ape_solidity/compiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 import os
 import re
-from copy import copy
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Set, Tuple, Union, cast
+from typing import Any, Dict, List, Optional, Set, Tuple, Type, Union, cast
 
 import solcx  # type: ignore
 from ape.api import CompilerAPI, PluginConfig
 from ape.contracts import ContractInstance
 from ape.exceptions import CompilerError, ContractLogicError
 from ape.logging import logger
 from ape.types import AddressType, ContractType
 from ape.utils import cached_property, get_relative_path
-from eth_utils import is_0x_prefixed
-from ethpm_types import HexBytes, PackageManifest
+from eth_utils import add_0x_prefix, is_0x_prefixed
+from ethpm_types import ASTNode, HexBytes, PackageManifest
+from ethpm_types.ast import ASTClassification
+from pkg_resources import get_distribution
 from requests.exceptions import ConnectionError
 from semantic_version import NpmSpec, Version  # type: ignore
+from solcx import compile_standard  # type: ignore
 from solcx.exceptions import SolcError  # type: ignore
 from solcx.install import get_executable  # type: ignore
-from solcx.main import _compile_combined_json  # type: ignore
 
 from ape_solidity._utils import (
+    OUTPUT_SELECTION,
     Extension,
     ImportRemapping,
     ImportRemappingBuilder,
     get_import_lines,
     get_pragma_spec,
     get_version_with_commit_hash,
     load_dict,
     verify_contract_filepaths,
 )
-from ape_solidity.exceptions import IncorrectMappingFormatError
+from ape_solidity.exceptions import (
+    RUNTIME_ERROR_CODE_PREFIX,
+    RUNTIME_ERROR_MAP,
+    IncorrectMappingFormatError,
+    RuntimeErrorType,
+    RuntimeErrorUnion,
+)
 
 
 class SolidityConfig(PluginConfig):
     # Configure re-mappings using a `=` separated-str,
     # e.g. '@import_name=path/to/dependency'
     import_remapping: List[str] = []
     optimize: bool = True
@@ -70,14 +78,18 @@
             logger.warning("Internet connection required to fetch installable Solidity versions.")
             return []
 
     @property
     def installed_versions(self) -> List[Version]:
         return solcx.get_installed_solc_versions()
 
+    @cached_property
+    def _ape_version(self) -> Version:
+        return Version(get_distribution("eth-ape").version.split(".dev")[0].strip())
+
     def add_library(self, *contracts: ContractInstance):
         """
         Set a library contract type address. This is useful when deploying a library
         in a local network and then adding the address afterward. Now, when
         compiling again, it will use the new address.
 
         Args:
@@ -264,193 +276,184 @@
                         builder.contracts_cache / dep_id,
                         builder,
                     )
 
     def get_compiler_settings(
         self, contract_filepaths: List[Path], base_path: Optional[Path] = None
     ) -> Dict[Version, Dict]:
-        # Currently needed because of a bug in Ape core 0.5.5.
-        only_files = []
-        for path in contract_filepaths:
-            if path.is_dir():
-                logger.error(
-                    f"Unable to get compiler settings for directory '{path.name}'. Skipping."
-                )
-            else:
-                only_files.append(path)
-
         base_path = base_path or self.config_manager.contracts_folder
-        files_by_solc_version = self.get_version_map(only_files, base_path=base_path)
+        files_by_solc_version = self.get_version_map(contract_filepaths, base_path=base_path)
         if not files_by_solc_version:
             return {}
 
-        compiler_args: Dict = self._get_compiler_arguments(files_by_solc_version, base_path)
+        import_remappings = self.get_import_remapping(base_path=base_path)
         settings: Dict = {}
-        for solc_version, arguments in compiler_args.items():
-            sources = files_by_solc_version[solc_version]
+        for solc_version, sources in files_by_solc_version.items():
             version_settings: Dict[str, Union[Any, List[Any]]] = {
-                "optimizer": {"enabled": arguments.get("optimize", False), "runs": 200},
+                "optimizer": {"enabled": self.config.optimize, "runs": 200},
                 "outputSelection": {
-                    p.name: {p.stem: arguments.get("output_values", [])} for p in sources
+                    str(get_relative_path(p, base_path)): {"*": OUTPUT_SELECTION, "": ["ast"]}
+                    for p in sources
                 },
             }
-            remappings: List[str] = arguments.get("import_remappings", [])
-            if remappings:
-                # Standard JSON input requires remappings to be sorted.
-                version_settings["remappings"] = sorted(list(remappings))
-
-            evm_version = arguments.get("evm_version")
-            if evm_version:
-                version_settings["evmVersion"] = evm_version
-
-            settings[solc_version] = version_settings
-
-        return settings
-
-    def _get_compiler_arguments(self, version_map: Dict, base_path: Path) -> Dict[Version, Dict]:
-        base_arguments = {
-            "output_values": [
-                "abi",
-                "bin",
-                "bin-runtime",
-                "devdoc",
-                "userdoc",
-                "srcmap",
-            ],
-            "optimize": self.config.optimize,
-            "evm_version": self.config.evm_version,
-        }
-        arguments_map = {}
-        global_import_remapping_list = self.get_import_remapping(base_path=base_path)
-        for solc_version, sources in version_map.items():
-            cleaned_version = solc_version.truncate()
-            import_remapping_list = copy(global_import_remapping_list)
-            remapping_kept_list = set()
-            if import_remapping_list:
+            remappings_used = set()
+            if import_remappings:
                 # Filter out unused import remapping
                 resolved_remapped_sources = set(
                     [
                         x
                         for ls in self.get_imports(list(sources), base_path=base_path).values()
                         for x in ls
                         if x.startswith(".cache")
                     ]
                 )
                 for source in resolved_remapped_sources:
                     parent_key = os.path.sep.join(source.split(os.path.sep)[:3])
-                    for k, v in [
-                        (k, v) for k, v in import_remapping_list.items() if parent_key in v
-                    ]:
-                        remapping_kept_list.add(f"{k}={v}")
-
-            arguments = {
-                **base_arguments,
-                "solc_binary": get_executable(cleaned_version),
-                "solc_version": cleaned_version,
-            }
+                    for k, v in [(k, v) for k, v in import_remappings.items() if parent_key in v]:
+                        remappings_used.add(f"{k}={v}")
 
-            if solc_version >= Version("0.6.9"):
-                arguments["base_path"] = base_path
-            else:
-                # Append base_path to remappings
-                parts = [x.split("=") for x in remapping_kept_list]
-                remapping_kept_list = {f"{p[0]}={base_path / p[1]}" for p in parts}
+            if remappings_used:
+                # Standard JSON input requires remappings to be sorted.
+                version_settings["remappings"] = sorted(list(remappings_used))
+
+            evm_version = self.config.evm_version
+            if evm_version:
+                version_settings["evmVersion"] = evm_version
 
-            if remapping_kept_list:
-                arguments["import_remappings"] = remapping_kept_list
+            settings[solc_version] = version_settings
 
             # TODO: Filter out libraries that are not used for this version.
             libs = self.libraries
             if libs:
-                arguments["libraries"] = ",".join(
-                    [
-                        ":".join((sid, cn, addr))
-                        for sid, lib_dict in libs.items()
-                        for cn, addr in lib_dict.items()
-                    ]
-                )
+                version_settings["libraries"] = libs
 
-            arguments_map[solc_version] = arguments
-
-        return arguments_map
+        return settings
 
-    def compile(
+    def get_standard_input_json(
         self, contract_filepaths: List[Path], base_path: Optional[Path] = None
-    ) -> List[ContractType]:
+    ) -> Dict[Version, Dict]:
         base_path = base_path or self.config_manager.contracts_folder
         files_by_solc_version = self.get_version_map(contract_filepaths, base_path=base_path)
-        compiler_arguments = self._get_compiler_arguments(
-            files_by_solc_version, base_path=base_path
-        )
-        contract_types: List[ContractType] = []
-        solc_versions_by_contract_name: Dict[str, Version] = {}
-        for solc_version, arguments in compiler_arguments.items():
+        settings = self.get_compiler_settings(contract_filepaths, base_path)
+        input_jsons = {}
+        for solc_version, vers_settings in settings.items():
             files = list(files_by_solc_version[solc_version])
             if not files:
                 continue
 
             logger.debug(f"Compiling using Solidity compiler '{solc_version}'")
+            cleaned_version = solc_version.truncate()
+            solc_binary = get_executable(cleaned_version)
+            arguments = {"solc_binary": solc_binary, "solc_version": cleaned_version}
+
+            if solc_version >= Version("0.6.9"):
+                arguments["base_path"] = base_path
+
+            sources = {
+                x: {"content": (base_path / x).read_text()}
+                for x in vers_settings["outputSelection"]
+            }
+            input_jsons[solc_version] = {
+                "sources": sources,
+                "settings": vers_settings,
+                "language": "Solidity",
+            }
+
+        return input_jsons
+
+    def compile(
+        self, contract_filepaths: List[Path], base_path: Optional[Path] = None
+    ) -> List[ContractType]:
+        base_path = base_path or self.config_manager.contracts_folder
+        solc_versions_by_contract_name: Dict[str, Version] = {}
+        contract_types: List[ContractType] = []
+        input_jsons = self.get_standard_input_json(contract_filepaths, base_path=base_path)
+        for solc_version, input_json in input_jsons.items():
+            logger.debug(f"Compiling using Solidity compiler '{solc_version}'")
+            cleaned_version = solc_version.truncate()
+            solc_binary = get_executable(cleaned_version)
+            arguments = {"solc_binary": solc_binary, "solc_version": cleaned_version}
+
+            if solc_version >= Version("0.6.9"):
+                arguments["base_path"] = base_path
 
             try:
-                output = _compile_combined_json(source_files=files, **arguments)
+                output = compile_standard(input_json, **arguments)
             except SolcError as err:
                 raise CompilerError(str(err)) from err
 
-            def parse_contract_name(value: str) -> Tuple[Path, str]:
-                parts = value.split(":")
-                return Path(parts[0]), parts[1]
-
-            # Filter source files that the user did not ask for, such as
-            # imported relative files that are not part of the input.
             input_contract_names: List[str] = []
-            for contract_id in output.keys():
-                path, name = parse_contract_name(contract_id)
-                for input_file_path in contract_filepaths:
-                    if str(path) in str(input_file_path):
-                        input_contract_names.append(name)
-
-            for contract_name, contract_type in output.items():
-                contract_path, contract_name = parse_contract_name(contract_name)
-                if contract_name not in input_contract_names:
-                    # Only return ContractTypes explicitly asked for.
-                    continue
+            for source_id, contracts_out in output["contracts"].items():
+                for name, _ in contracts_out.items():
+                    # Filter source files that the user did not ask for, such as
+                    # imported relative files that are not part of the input.
+                    for input_file_path in contract_filepaths:
+                        if source_id in str(input_file_path):
+                            input_contract_names.append(name)
+
+            def classify_ast(_node: ASTNode):
+                if _node.ast_type in ("FunctionDefinition", "FunctionDefinitionNode"):
+                    _node.classification = ASTClassification.FUNCTION
+
+                for child in _node.children:
+                    classify_ast(child)
+
+            for source_id, contracts_out in output["contracts"].items():
+                ast_data = output["sources"][source_id]["ast"]
+                ast = ASTNode.parse_obj(ast_data)
+                classify_ast(ast)
 
-                deployment_bytecode = contract_type["bin"]
-                runtime_bytecode = contract_type["bin"]
+                for contract_name, ct_data in contracts_out.items():
+                    contract_path = base_path / source_id
 
-                # Skip library linking.
-                if "__$" in deployment_bytecode or "__$" in runtime_bytecode:
-                    logger.warning(
-                        f"Unable to compile {contract_name} - missing libraries. "
-                        f"Call `{self.add_library.__name__}` with the necessary libraries"
-                    )
-                    self._contracts_needing_libraries.add(contract_path)
-                    continue
+                    if contract_name not in input_contract_names:
+                        # Only return ContractTypes explicitly asked for.
+                        continue
+
+                    evm_data = ct_data["evm"]
 
-                previously_compiled_version = solc_versions_by_contract_name.get(contract_name)
-                if previously_compiled_version:
-                    # Don't add previously compiled contract type unless it was compiled
-                    # using a greater Solidity version.
-                    if previously_compiled_version >= solc_version:
+                    # NOTE: This sounds backwards, but it isn't...
+                    #  The "deployment_bytecode" is the same as the "bytecode",
+                    #  and the "deployedBytecode" is the same as the "runtimeBytecode".
+                    deployment_bytecode = add_0x_prefix(evm_data["bytecode"]["object"])
+                    runtime_bytecode = add_0x_prefix(evm_data["deployedBytecode"]["object"])
+
+                    # Skip library linking.
+                    if "__$" in deployment_bytecode or "__$" in runtime_bytecode:
+                        logger.warning(
+                            f"Unable to compile {contract_name} - missing libraries. "
+                            f"Call `{self.add_library.__name__}` with the necessary libraries"
+                        )
+                        self._contracts_needing_libraries.add(contract_path)
                         continue
-                    else:
-                        contract_types = [ct for ct in contract_types if ct.name != contract_name]
 
-                contract_type["contractName"] = contract_name
-                contract_type["sourceId"] = str(
-                    get_relative_path(base_path / contract_path, base_path)
-                )
-                contract_type["deploymentBytecode"] = {"bytecode": deployment_bytecode}
-                contract_type["runtimeBytecode"] = {"bytecode": runtime_bytecode}
-                contract_type["userdoc"] = load_dict(contract_type["userdoc"])
-                contract_type["devdoc"] = load_dict(contract_type["devdoc"])
-                contract_type["sourcemap"] = contract_type["srcmap"]
-                contract_type_obj = ContractType.parse_obj(contract_type)
-                contract_types.append(contract_type_obj)
-                solc_versions_by_contract_name[contract_name] = solc_version
+                    previously_compiled_version = solc_versions_by_contract_name.get(contract_name)
+                    if previously_compiled_version:
+                        # Don't add previously compiled contract type unless it was compiled
+                        # using a greater Solidity version.
+                        if previously_compiled_version >= solc_version:
+                            continue
+                        else:
+                            contract_types = [
+                                ct for ct in contract_types if ct.name != contract_name
+                            ]
+
+                    ct_data["contractName"] = contract_name
+                    ct_data["sourceId"] = str(
+                        get_relative_path(base_path / contract_path, base_path)
+                    )
+                    ct_data["deploymentBytecode"] = {"bytecode": deployment_bytecode}
+                    ct_data["runtimeBytecode"] = {"bytecode": runtime_bytecode}
+                    ct_data["userdoc"] = load_dict(ct_data["userdoc"])
+                    ct_data["devdoc"] = load_dict(ct_data["devdoc"])
+                    ct_data["sourcemap"] = evm_data["bytecode"]["sourceMap"]
+                    ct_data["ast"] = ast
+                    contract_type = ContractType.parse_obj(ct_data)
+                    contract_types.append(contract_type)
+                    solc_versions_by_contract_name[contract_name] = solc_version
 
         return contract_types
 
     def get_imports(
         self, contract_filepaths: List[Path], base_path: Optional[Path] = None
     ) -> Dict[str, List[str]]:
         # NOTE: Process import remappings _before_ getting the full contract set.
@@ -668,14 +671,33 @@
             else max(self.installed_versions)
         )
 
     def enrich_error(self, err: ContractLogicError) -> ContractLogicError:
         if not is_0x_prefixed(err.revert_message):
             return err
 
+        if panic_cls := _get_sol_panic(err.revert_message):
+            # Is from a Solidity panic code, like a builtin Solidity revert.
+
+            if self._ape_version <= Version("0.6.10"):
+                return panic_cls(
+                    contract_address=err.contract_address,
+                    trace=err.trace,
+                    txn=err.txn,
+                )
+            else:
+                # TODO: Bump to next ape version and remove conditional.
+                return panic_cls(
+                    base_err=err.base_err,
+                    contract_address=err.contract_address,
+                    source_traceback=err.source_traceback,
+                    trace=err.trace,
+                    txn=err.txn,
+                )
+
         # Check for ErrorABI.
         bytes_message = HexBytes(err.revert_message)
         selector = bytes_message[:4]
         input_data = bytes_message[4:]
         address = err.contract_address or getattr(err.txn, "receiver", None)
         if not address:
             return err
@@ -692,10 +714,42 @@
             # Not an ErrorABI selector.
             return err
 
         ecosystem = self.provider.network.ecosystem
         abi = contract.contract_type.errors[selector]
         inputs = ecosystem.decode_calldata(abi, input_data)
         error_class = contract.get_error_by_signature(abi.signature)
-        return error_class(
-            abi, inputs, txn=err.txn, trace=err.trace, contract_address=err.contract_address
+        if self._ape_version <= Version("0.6.10"):
+            return error_class(
+                abi,
+                inputs,
+                txn=err.txn,
+                trace=err.trace,
+                contract_address=err.contract_address,
+            )
+        else:
+            # TODO Bump Ape on next release and remove this conditional
+            return error_class(
+                abi,
+                inputs,
+                base_err=err.base_err,
+                contract_address=err.contract_address,  # type: ignore[call-arg]
+                source_traceback=err.source_traceback,  # type: ignore[call-arg]
+                trace=err.trace,
+                txn=err.txn,
+            )
+
+
+def _get_sol_panic(revert_message: str) -> Optional[Type[RuntimeErrorUnion]]:
+    if revert_message.startswith(RUNTIME_ERROR_CODE_PREFIX):
+        # ape-geth (style) plugins show the hex with the Panic ABI prefix.
+        error_type_val = int(
+            f"0x{revert_message.replace(RUNTIME_ERROR_CODE_PREFIX, '').lstrip('0')}", 16
         )
+    else:
+        # Some plugins, like ape-hardhat, will deliver panic codes directly (no Panic ABI prefix)
+        error_type_val = int(revert_message, 16)
+
+    if error_type_val in [x.value for x in RuntimeErrorType]:
+        return RUNTIME_ERROR_MAP[RuntimeErrorType(error_type_val)]
+
+    return None
```

### Comparing `ape-solidity-0.6.5/ape_solidity.egg-info/PKG-INFO` & `ape-solidity-0.6.6/ape_solidity.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,144 +1,145 @@
 Metadata-Version: 2.1
 Name: ape-solidity
-Version: 0.6.5
+Version: 0.6.6
 Summary: Plugin for Ape Ethereum Framework for compiling Solidity contracts
 Home-page: https://github.com/ApeWorX/ape-solidity
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Compile Solidity contracts.
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-solidity
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-solidity.git
-        cd ape-solidity
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        In your project, make sure you have a `contracts/` directory containing Solidity files (`.sol`).
-        
-        Then, while this plugin is installed, compile your contracts:
-        
-        ```bash
-        ape compile
-        ```
-        
-        The byte-code and ABI for your contracts should now exist in a `__local__.json` file in a `.build/` directory.
-        
-        ### Dependency Mapping
-        
-        To configure import remapping, use your project's `ape-config.yaml` file:
-        
-        ```yaml
-        solidity:
-          import_remapping:
-            - "@openzeppelin=path/to/open_zeppelin/contracts"
-        ```
-        
-        If you are using the `dependencies:` key in your `ape-config.yaml`, `ape` can automatically
-        search those dependencies for the path.
-        
-        ```yaml
-        dependencies:
-          - name: OpenZeppelin
-            github: OpenZeppelin/openzeppelin-contracts
-            version: 4.4.2
-        
-        solidity:
-          import_remapping:
-            - "@openzeppelin=OpenZeppelin/4.4.2"
-        ```
-        
-        Once you have your dependencies configured, you can import packages using your import keys:
-        
-        ```solidity
-        import "@openzeppelin/token/ERC721/ERC721.sol";
-        ```
-        
-        ### Library Linking
-        
-        To compile contracts that use libraries, you need to add the libraries first.
-        Use the `add_library()` method from the `ape-solidity` compiler class to add the library.
-        A typical flow is:
-        
-        1. Deploy the library.
-        2. Call `add_library()` using the Solidity compiler plugin, which will also re-compile contracts that need the library.
-        3. Deploy and use contracts that require the library.
-        
-        For example:
-        
-        ```python
-        import pytest
-        
-        
-        @pytest.fixture
-        def contract(accounts, project, compilers):
-            # Deploy the library.
-            account = accounts[0]
-            library = project.Set.deploy(sender=account)
-            
-            # Add the library to Solidity (re-compiles contracts that use the library).
-            compilers.solidity.add_library(library)
-        
-            # Deploy the contract that uses the library.
-            return project.C.deploy(sender=account)
-        ```
-        
-        ### Compiler Settings
-        
-        When using `ape-solidity`, your project's manifest's compiler settings will include standard JSON output.
-        You should have one listed `compiler` per `solc` version used in your project.
-        You can view your current project manifest, including the compiler settings, by doing:
-        
-        ```python
-        from ape import project
-        
-        manifest = project.extract_manifest()
-        
-        for compiler_entry in manifest.compilers:
-            print(compiler_entry.version)
-            print(compiler_entry.settings)
-        ```
-        
-        **NOTE**: These are the settings used during contract verification when using the [Etherscan plugin](https://github.com/ApeWorX/ape-etherscan).
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Compile Solidity contracts.
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+
+## Installation
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-solidity
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-solidity.git
+cd ape-solidity
+python3 setup.py install
+```
+
+## Quick Usage
+
+In your project, make sure you have a `contracts/` directory containing Solidity files (`.sol`).
+
+Then, while this plugin is installed, compile your contracts:
+
+```bash
+ape compile
+```
+
+The byte-code and ABI for your contracts should now exist in a `__local__.json` file in a `.build/` directory.
+
+### Dependency Mapping
+
+To configure import remapping, use your project's `ape-config.yaml` file:
+
+```yaml
+solidity:
+  import_remapping:
+    - "@openzeppelin=path/to/open_zeppelin/contracts"
+```
+
+If you are using the `dependencies:` key in your `ape-config.yaml`, `ape` can automatically
+search those dependencies for the path.
+
+```yaml
+dependencies:
+  - name: OpenZeppelin
+    github: OpenZeppelin/openzeppelin-contracts
+    version: 4.4.2
+
+solidity:
+  import_remapping:
+    - "@openzeppelin=OpenZeppelin/4.4.2"
+```
+
+Once you have your dependencies configured, you can import packages using your import keys:
+
+```solidity
+import "@openzeppelin/token/ERC721/ERC721.sol";
+```
+
+### Library Linking
+
+To compile contracts that use libraries, you need to add the libraries first.
+Use the `add_library()` method from the `ape-solidity` compiler class to add the library.
+A typical flow is:
+
+1. Deploy the library.
+2. Call `add_library()` using the Solidity compiler plugin, which will also re-compile contracts that need the library.
+3. Deploy and use contracts that require the library.
+
+For example:
+
+```python
+import pytest
+
+
+@pytest.fixture
+def contract(accounts, project, compilers):
+    # Deploy the library.
+    account = accounts[0]
+    library = project.Set.deploy(sender=account)
+    
+    # Add the library to Solidity (re-compiles contracts that use the library).
+    compilers.solidity.add_library(library)
+
+    # Deploy the contract that uses the library.
+    return project.C.deploy(sender=account)
+```
+
+### Compiler Settings
+
+When using `ape-solidity`, your project's manifest's compiler settings will include standard JSON output.
+You should have one listed `compiler` per `solc` version used in your project.
+You can view your current project manifest, including the compiler settings, by doing:
+
+```python
+from ape import project
+
+manifest = project.extract_manifest()
+
+for compiler_entry in manifest.compilers:
+    print(compiler_entry.version)
+    print(compiler_entry.settings)
+```
+
+**NOTE**: These are the settings used during contract verification when using the [Etherscan plugin](https://github.com/ApeWorX/ape-etherscan).
```

### Comparing `ape-solidity-0.6.5/ape_solidity.egg-info/SOURCES.txt` & `ape-solidity-0.6.6/ape_solidity.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
 tests/DependencyOfDependency/ape-config.yaml
 tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
 tests/ProjectWithinProject/ape-config.yaml
 tests/ProjectWithinProject/contracts/Contract.sol
 tests/VersionSpecifiedInConfig/ape-config.yaml
 tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
+tests/contracts/BuiltinErrorChecker.sol
 tests/contracts/CircularImport1.sol
 tests/contracts/CircularImport2.sol
 tests/contracts/CompilesOnce.sol
 tests/contracts/DifferentNameThanFile.sol
 tests/contracts/ExperimentalABIEncoderV2.sol
 tests/contracts/HasError.sol
 tests/contracts/ImportOlderDependency.sol
```

### Comparing `ape-solidity-0.6.5/pyproject.toml` & `ape-solidity-0.6.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `ape-solidity-0.6.5/setup.py` & `ape-solidity-0.6.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
         "black>=23.3.0,<24",  # Auto-formatter and linter
         "mypy>=0.991,<1",  # Static type analyzer
         "types-requests",  # Needed due to mypy typeshed
         "types-setuptools",  # Needed due to mypy typeshed
+        "types-pkg-resources",  # Needed for type checking tests
         "flake8>=6.0.0,<7",  # Style linter
         "isort>=5.10.1,<6",  # Import sorting linter
         "mdformat>=0.7.16",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
     ],
     "doc": [
@@ -61,18 +62,19 @@
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-solidity",
     include_package_data=True,
     install_requires=[
         "py-solc-x>=1.1.0,<2",
-        "eth-ape>=0.6.8,<0.7",
+        "eth-ape>=0.6.9,<0.7",
         "ethpm-types",  # Use the version ape requires
         "packaging",  # Use the version ape requires
         "requests",
+        "typing-extensions==4.5.0",  # Can be removed onced pinned in Core.
     ],
     python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_solidity"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
@@ -85,9 +87,10 @@
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `ape-solidity-0.6.5/tests/ape-config.yaml` & `ape-solidity-0.6.6/tests/ape-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/tests/conftest.py` & `ape-solidity-0.6.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/tests/contracts/Imports.sol` & `ape-solidity-0.6.6/tests/contracts/Imports.sol`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/tests/contracts/LibraryFun.sol` & `ape-solidity-0.6.6/tests/contracts/LibraryFun.sol`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json` & `ape-solidity-0.6.6/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json` & `ape-solidity-0.6.6/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/tests/data/packages/vault/master/vault_main.json` & `ape-solidity-0.6.6/tests/data/packages/vault/master/vault_main.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/tests/data/packages/vault/v0.4.5/vault.json` & `ape-solidity-0.6.6/tests/data/packages/vault/v0.4.5/vault.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/tests/scripts/clean.py` & `ape-solidity-0.6.6/tests/scripts/clean.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.5/tests/test_compiler.py` & `ape-solidity-0.6.6/tests/test_compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 import shutil
 from pathlib import Path
 
 import pytest
 import solcx  # type: ignore
 from ape.contracts import ContractContainer
 from ape.exceptions import CompilerError
+from ethpm_types.ast import ASTClassification
 from semantic_version import Version  # type: ignore
 
 from ape_solidity import Extension
+from ape_solidity._utils import OUTPUT_SELECTION
+from ape_solidity.exceptions import IndexOutOfBoundsError
 
 BASE_PATH = Path(__file__).parent / "contracts"
 TEST_CONTRACT_PATHS = [
     p
     for p in BASE_PATH.iterdir()
     if ".cache" not in str(p) and not p.is_dir() and p.suffix == Extension.SOL.value
 ]
@@ -25,22 +28,14 @@
 normal_test_skips = (
     "DifferentNameThanFile",
     "MultipleDefinitions",
     "RandomVyperFile",
     "LibraryFun",
 )
 raises_because_not_sol = pytest.raises(CompilerError, match=EXPECTED_NON_SOLIDITY_ERR_MSG)
-DEFAULT_OUTPUT_SELECTION = (
-    "abi",
-    "bin",
-    "bin-runtime",
-    "devdoc",
-    "userdoc",
-    "srcmap",
-)
 DEFAULT_OPTIMIZER = {"enabled": True, "runs": 200}
 
 
 @pytest.mark.parametrize(
     "contract",
     [c for c in TEST_CONTRACTS if all(n not in str(c) for n in normal_test_skips)],
 )
@@ -264,21 +259,15 @@
         "@styleofbrownie=.cache/BrownieStyleDependency/local",
     )
     actual_remappings = compiler_latest.settings["remappings"]
     assert all(x in actual_remappings for x in expected_remappings)
     assert all(
         b >= a for a, b in zip(actual_remappings, actual_remappings[1:])
     ), "Import remappings should be sorted"
-
-    # 0.4.26 should have absolute paths here due to lack of base_path
-    assert (
-        f"@remapping/contracts={project.contracts_folder}/{common_suffix}"
-        in compiler_0426.settings["remappings"]
-    )
-
+    assert f"@remapping/contracts={common_suffix}" in compiler_0426.settings["remappings"]
     assert "UseYearn" in compiler_latest.contractTypes
 
     # Compiler contract types test
     assert set(compiler_0812.contractTypes) == {
         "ImportSourceWithEqualSignVersion",
         "ImportSourceWithNoPrefixVersion",
         "ImportingLessConstrainedVersion",
@@ -325,35 +314,39 @@
         "@dependency_remapping=.cache/TestDependencyOfDependency/local",
         "@remapping_2=.cache/TestDependency/local",
         "@remapping/contracts=.cache/TestDependency/local",
         "@styleofbrownie=.cache/BrownieStyleDependency/local",
     )
     expected_v812_contracts = (source_a, source_b, source_c, indirect_source)
     expected_latest_contracts = (
-        "BrownieContract.sol",
+        ".cache/BrownieDependency/local/BrownieContract.sol",
         "CompilesOnce.sol",
-        "Dependency.sol",
-        "DependencyOfDependency.sol",
+        ".cache/TestDependency/local/Dependency.sol",
+        ".cache/TestDependencyOfDependency/local/DependencyOfDependency.sol",
         source_d,
-        "Relativecontract.sol",
+        "subfolder/Relativecontract.sol",
     )
 
     # Shared compiler defaults tests
     expected_source_lists = (expected_v812_contracts, expected_latest_contracts)
     for version, expected_sources in zip((v812, latest), expected_source_lists):
         output_selection = actual[version]["outputSelection"]
         assert actual[version]["optimizer"] == DEFAULT_OPTIMIZER
-        for source_key, item_selections in output_selection.items():
-            for item, selections in item_selections.items():
-                assert len(selections) == len(DEFAULT_OUTPUT_SELECTION)
-                assert all(x in selections for x in DEFAULT_OUTPUT_SELECTION)
+        for _, item_selection in output_selection.items():
+            for key, selection in item_selection.items():
+                if key == "*":  # All contracts
+                    assert selection == OUTPUT_SELECTION
+                elif key == "":  # All sources
+                    assert selection == ["ast"]
 
         actual_sources = [x for x in output_selection.keys()]
         for expected_source_id in expected_sources:
-            assert expected_source_id in actual_sources
+            assert (
+                expected_source_id in actual_sources
+            ), f"{expected_source_id} not one of {', '.join(actual_sources)}"
 
     # Remappings test
     actual_remappings = actual[latest]["remappings"]
     assert isinstance(actual_remappings, list)
     assert len(actual_remappings) == len(expected_remappings)
     assert all(e in actual_remappings for e in expected_remappings)
     assert all(
@@ -384,16 +377,31 @@
     library = project.Set.deploy(sender=account)
     compiler.add_library(library)
 
     # After deploying and adding the library, we can use contracts that need it.
     assert project.C
 
 
-def test_enrich_error(compiler, project, owner, not_owner, connection):
+def test_enrich_error_when_custom(compiler, project, owner, not_owner, connection):
     compiler.compile((project.contracts_folder / "HasError.sol",))
 
     # Deploy so Ape know about contract type.
     contract = owner.deploy(project.HasError)
     with pytest.raises(contract.Unauthorized) as err:
         contract.withdraw(sender=not_owner)
 
     assert err.value.inputs == {"addr": not_owner.address, "counter": 123}
+
+
+def test_enrich_error_when_builtin(project, owner, connection):
+    contract = project.BuiltinErrorChecker.deploy(sender=owner)
+
+    with pytest.raises(IndexOutOfBoundsError):
+        contract.checkIndexOutOfBounds(sender=owner)
+
+
+def test_ast(project, compiler):
+    source_path = project.contracts_folder / "MultipleDefinitions.sol"
+    actual = compiler.compile([source_path])[-1].ast
+    fn_node = actual.children[1].children[0]
+    assert actual.ast_type == "SourceUnit"
+    assert fn_node.classification == ASTClassification.FUNCTION
```

### Comparing `ape-solidity-0.6.5/tests/test_integration.py` & `ape-solidity-0.6.6/tests/test_integration.py`

 * *Files identical despite different names*

