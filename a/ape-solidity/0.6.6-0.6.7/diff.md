# Comparing `tmp/ape-solidity-0.6.6.tar.gz` & `tmp/ape-solidity-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-solidity-0.6.6.tar", last modified: Tue Jun 13 01:25:00 2023, max compression
+gzip compressed data, was "ape-solidity-0.6.7.tar", last modified: Wed Jul  5 18:22:57 2023, max compression
```

## Comparing `ape-solidity-0.6.6.tar` & `ape-solidity-0.6.7.tar`

### file list

```diff
@@ -1,124 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.455625 ape-solidity-0.6.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.439625 ape-solidity-0.6.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.443625 ape-solidity-0.6.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.443625 ape-solidity-0.6.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-13 01:25:00.455625 ape-solidity-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.443625 ape-solidity-0.6.6/ape_solidity/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/ape_solidity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/ape_solidity/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31520 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/ape_solidity/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/ape_solidity/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/ape_solidity/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 01:25:00.000000 ape-solidity-0.6.6/ape_solidity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.443625 ape-solidity-0.6.6/ape_solidity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-13 01:25:00.000000 ape-solidity-0.6.6/ape_solidity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-13 01:25:00.000000 ape-solidity-0.6.6/ape_solidity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:25:00.000000 ape-solidity-0.6.6/ape_solidity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:25:00.000000 ape-solidity-0.6.6/ape_solidity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 01:25:00.000000 ape-solidity-0.6.6/ape_solidity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 01:25:00.000000 ape-solidity-0.6.6/ape_solidity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 01:25:00.455625 ape-solidity-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.443625 ape-solidity-0.6.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.443625 ape-solidity-0.6.6/tests/BrownieProject/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/BrownieProject/brownie-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/BrownieProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/BrownieProject/contracts/BrownieContract.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/BrownieStyleDependency/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/BrownieStyleDependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/BrownieStyleDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/BrownieStyleDependency/contracts/BrownieStyleDependency.sol
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/BrownieStyleDependency/contracts/FailingContract.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/Dependency/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/Dependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/Dependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/Dependency/contracts/Dependency.sol
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/Dependency/contracts/OlderDependency.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/Dependency/contracts/subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/Dependency/contracts/subfolder/InDependencySubfolder.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/Dependency/contracts/subfolder_with_imports/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/DependencyOfDependency/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/DependencyOfDependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/DependencyOfDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/ProjectWithinProject/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/ProjectWithinProject/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/ProjectWithinProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/ProjectWithinProject/contracts/Contract.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/VersionSpecifiedInConfig/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/VersionSpecifiedInConfig/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.447625 ape-solidity-0.6.6/tests/VersionSpecifiedInConfig/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.451625 ape-solidity-0.6.6/tests/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/BuiltinErrorChecker.sol
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/CircularImport1.sol
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/CircularImport2.sol
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/CompilesOnce.sol
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/DifferentNameThanFile.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.451625 ape-solidity-0.6.6/tests/contracts/DirectoryWithExtension.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/DirectoryWithExtension.sol/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/ExperimentalABIEncoderV2.sol
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/ImportOlderDependency.sol
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/ImportSourceWithEqualSignVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/ImportSourceWithNoPrefixVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/ImportingLessConstrainedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/Imports.sol
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanionImport.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/LibraryFun.sol
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/MissingPragma.sol
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/MultipleDefinitions.sol
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/NumerousDefinitions.sol
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/OlderVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/RandomVyperFile.vy
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/RangedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/SpacesInPragma.sol
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/SpecificVersionNoPrefix.sol
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/SpecificVersionNoPrefix2.sol
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/SpecificVersionRange.sol
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/SpecificVersionWithEqualSign.sol
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/UseYearn.sol
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/VagueVersion.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.451625 ape-solidity-0.6.6/tests/contracts/subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/subfolder/Relativecontract.sol
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.439625 ape-solidity-0.6.6/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.439625 ape-solidity-0.6.6/tests/data/packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.439625 ape-solidity-0.6.6/tests/data/packages/OpenZeppelin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.451625 ape-solidity-0.6.6/tests/data/packages/OpenZeppelin/v4.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)   698486 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.451625 ape-solidity-0.6.6/tests/data/packages/OpenZeppelin/v4.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)   879002 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.439625 ape-solidity-0.6.6/tests/data/packages/vault/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.455625 ape-solidity-0.6.6/tests/data/packages/vault/master/
--rw-r--r--   0 runner    (1001) docker     (123)   167518 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/data/packages/vault/master/vault_main.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.455625 ape-solidity-0.6.6/tests/data/packages/vault/v0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)   167551 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/data/packages/vault/v0.4.5/vault.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:25:00.455625 ape-solidity-0.6.6/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/scripts/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    16954 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-13 01:23:48.000000 ape-solidity-0.6.6/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.068899 ape-solidity-0.6.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.040899 ape-solidity-0.6.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.040899 ape-solidity-0.6.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.044899 ape-solidity-0.6.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-05 18:22:57.068899 ape-solidity-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.044899 ape-solidity-0.6.7/ape_solidity/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/ape_solidity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/ape_solidity/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36101 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/ape_solidity/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/ape_solidity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/ape_solidity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 18:22:56.000000 ape-solidity-0.6.7/ape_solidity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.044899 ape-solidity-0.6.7/ape_solidity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-05 18:22:56.000000 ape-solidity-0.6.7/ape_solidity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-05 18:22:57.000000 ape-solidity-0.6.7/ape_solidity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:22:56.000000 ape-solidity-0.6.7/ape_solidity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:22:56.000000 ape-solidity-0.6.7/ape_solidity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-05 18:22:56.000000 ape-solidity-0.6.7/ape_solidity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 18:22:56.000000 ape-solidity-0.6.7/ape_solidity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-05 18:22:57.072899 ape-solidity-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.048899 ape-solidity-0.6.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.048899 ape-solidity-0.6.7/tests/BrownieProject/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/BrownieProject/brownie-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.048899 ape-solidity-0.6.7/tests/BrownieProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/BrownieProject/contracts/BrownieContract.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.048899 ape-solidity-0.6.7/tests/BrownieStyleDependency/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/BrownieStyleDependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.048899 ape-solidity-0.6.7/tests/BrownieStyleDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/BrownieStyleDependency/contracts/BrownieStyleDependency.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/BrownieStyleDependency/contracts/FailingContract.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.048899 ape-solidity-0.6.7/tests/Dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/Dependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.048899 ape-solidity-0.6.7/tests/Dependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/Dependency/contracts/Dependency.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/Dependency/contracts/OlderDependency.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.048899 ape-solidity-0.6.7/tests/Dependency/contracts/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/Dependency/contracts/subfolder/InDependencySubfolder.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.048899 ape-solidity-0.6.7/tests/Dependency/contracts/subfolder_with_imports/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.048899 ape-solidity-0.6.7/tests/DependencyOfDependency/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/DependencyOfDependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.052899 ape-solidity-0.6.7/tests/DependencyOfDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.052899 ape-solidity-0.6.7/tests/ProjectWithinProject/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/ProjectWithinProject/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.052899 ape-solidity-0.6.7/tests/ProjectWithinProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/ProjectWithinProject/contracts/Contract.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.052899 ape-solidity-0.6.7/tests/VersionSpecifiedInConfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/VersionSpecifiedInConfig/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.052899 ape-solidity-0.6.7/tests/VersionSpecifiedInConfig/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.064899 ape-solidity-0.6.7/tests/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/BuiltinErrorChecker.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/CircularImport1.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/CircularImport2.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/CompilesOnce.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/DifferentNameThanFile.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.064899 ape-solidity-0.6.7/tests/contracts/DirectoryWithExtension.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/DirectoryWithExtension.sol/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/ExperimentalABIEncoderV2.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/ImportOlderDependency.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/ImportSourceWithEqualSignVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/ImportSourceWithNoPrefixVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/ImportingLessConstrainedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/Imports.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanionImport.sol
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/JustAStruct.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/LibraryFun.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/MissingPragma.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/MultipleDefinitions.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/NumerousDefinitions.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/OlderVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/RandomVyperFile.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/RangedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/SpacesInPragma.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/SpecificVersionNoPrefix.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/SpecificVersionNoPrefix2.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/SpecificVersionRange.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/SpecificVersionWithEqualSign.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/UseYearn.sol
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/VagueVersion.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.064899 ape-solidity-0.6.7/tests/contracts/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/subfolder/Relativecontract.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.064899 ape-solidity-0.6.7/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/data/ImportingLessConstrainedVersionFlat.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/data/ImportsFlattened.sol.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.036898 ape-solidity-0.6.7/tests/data/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.036898 ape-solidity-0.6.7/tests/data/packages/OpenZeppelin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.068899 ape-solidity-0.6.7/tests/data/packages/OpenZeppelin/v4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   698486 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.068899 ape-solidity-0.6.7/tests/data/packages/OpenZeppelin/v4.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)   879002 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.040899 ape-solidity-0.6.7/tests/data/packages/vault/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.068899 ape-solidity-0.6.7/tests/data/packages/vault/master/
+-rw-r--r--   0 runner    (1001) docker     (123)   167518 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/data/packages/vault/master/vault_main.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.068899 ape-solidity-0.6.7/tests/data/packages/vault/v0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)   167551 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/data/packages/vault/v0.4.5/vault.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32767 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:22:57.068899 ape-solidity-0.6.7/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/scripts/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18972 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-05 18:21:47.000000 ape-solidity-0.6.7/tests/test_integration.py
```

### Comparing `ape-solidity-0.6.6/.github/ISSUE_TEMPLATE/bug.md` & `ape-solidity-0.6.7/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/.github/ISSUE_TEMPLATE/feature.md` & `ape-solidity-0.6.7/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/.github/ISSUE_TEMPLATE/work-item.md` & `ape-solidity-0.6.7/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/.github/release-drafter.yml` & `ape-solidity-0.6.7/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/.github/workflows/codeql.yml` & `ape-solidity-0.6.7/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/.github/workflows/prtitle.yaml` & `ape-solidity-0.6.7/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/.github/workflows/publish.yaml` & `ape-solidity-0.6.7/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/.github/workflows/stale-prs.yml` & `ape-solidity-0.6.7/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/.github/workflows/test.yaml` & `ape-solidity-0.6.7/.github/workflows/test.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,17 @@
           with:
               python-version: ${{ matrix.python-version }}
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip uninstall eth-ape --yes
+            pushd tests
+            npm install
+            popd
             pip install .[test]
 
         - name: Run Tests
           run: pytest -m "not fuzzing"
 
     # fuzzing:
     #     runs-on: ubuntu-latest
```

### Comparing `ape-solidity-0.6.6/.gitignore` & `ape-solidity-0.6.7/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -121,7 +121,9 @@
 
 # Ape stuff
 .build/
 
 **/.DS_Store
 *.swp
 *.swo
+
+tests/node_modules
```

### Comparing `ape-solidity-0.6.6/.pre-commit-config.yaml` & `ape-solidity-0.6.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/CONTRIBUTING.md` & `ape-solidity-0.6.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/LICENSE` & `ape-solidity-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/PKG-INFO` & `ape-solidity-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-solidity
-Version: 0.6.6
+Version: 0.6.7
 Summary: Plugin for Ape Ethereum Framework for compiling Solidity contracts
 Home-page: https://github.com/ApeWorX/ape-solidity
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-solidity-0.6.6/README.md` & `ape-solidity-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/ape_solidity/_utils.py` & `ape-solidity-0.6.7/ape_solidity/_utils.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/ape_solidity/compiler.py` & `ape-solidity-0.6.7/ape_solidity/compiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from ape.exceptions import CompilerError, ContractLogicError
 from ape.logging import logger
 from ape.types import AddressType, ContractType
 from ape.utils import cached_property, get_relative_path
 from eth_utils import add_0x_prefix, is_0x_prefixed
 from ethpm_types import ASTNode, HexBytes, PackageManifest
 from ethpm_types.ast import ASTClassification
+from ethpm_types.source import Content
 from pkg_resources import get_distribution
 from requests.exceptions import ConnectionError
 from semantic_version import NpmSpec, Version  # type: ignore
 from solcx import compile_standard  # type: ignore
 from solcx.exceptions import SolcError  # type: ignore
 from solcx.install import get_executable  # type: ignore
 
@@ -35,14 +36,24 @@
     RUNTIME_ERROR_CODE_PREFIX,
     RUNTIME_ERROR_MAP,
     IncorrectMappingFormatError,
     RuntimeErrorType,
     RuntimeErrorUnion,
 )
 
+# Define a regex pattern that matches import statements
+# Both single and multi-line imports will be matched
+IMPORTS_PATTERN = re.compile(
+    r"import\s+((.*?)(?=;)|[\s\S]*?from\s+(.*?)(?=;));\s", flags=re.MULTILINE
+)
+
+LICENSES_PATTERN = re.compile(r"(// SPDX-License-Identifier:\s*([^\n]*)\s)")
+
+VERSION_PRAGMA_PATTERN = re.compile(r"pragma solidity[^;]*;")
+
 
 class SolidityConfig(PluginConfig):
     # Configure re-mappings using a `=` separated-str,
     # e.g. '@import_name=path/to/dependency'
     import_remapping: List[str] = []
     optimize: bool = True
     version: Optional[str] = None
@@ -149,21 +160,18 @@
             raise IncorrectMappingFormatError()
 
         contracts_cache = base_path / ".cache"
         builder = ImportRemappingBuilder(contracts_cache)
 
         # Convert to tuple for hashing, check if there's been a change
         remappings_tuple = tuple(remappings)
-
-        if all(
-            (
-                self._import_remapping_hash,
-                self._import_remapping_hash == hash(remappings_tuple),
-                contracts_cache.is_dir(),
-            )
+        if (
+            self._import_remapping_hash
+            and self._import_remapping_hash == hash(remappings_tuple)
+            and contracts_cache.is_dir()
         ):
             return self._cached_import_map
 
         packages_cache = self.config_manager.packages_folder
 
         # Download dependencies for first time.
         # This only happens if calling this method before compiling in ape core.
@@ -344,14 +352,20 @@
             cleaned_version = solc_version.truncate()
             solc_binary = get_executable(cleaned_version)
             arguments = {"solc_binary": solc_binary, "solc_version": cleaned_version}
 
             if solc_version >= Version("0.6.9"):
                 arguments["base_path"] = base_path
 
+            if missing_sources := [
+                x for x in vers_settings["outputSelection"] if not (base_path / x).is_file()
+            ]:
+                missing_src_str = ", ".join(missing_sources)
+                raise CompilerError(f"Missing sources: '{missing_src_str}'.")
+
             sources = {
                 x: {"content": (base_path / x).read_text()}
                 for x in vers_settings["outputSelection"]
             }
             input_jsons[solc_version] = {
                 "sources": sources,
                 "settings": vers_settings,
@@ -377,31 +391,32 @@
                 arguments["base_path"] = base_path
 
             try:
                 output = compile_standard(input_json, **arguments)
             except SolcError as err:
                 raise CompilerError(str(err)) from err
 
+            contracts = output.get("contracts", {})
             input_contract_names: List[str] = []
-            for source_id, contracts_out in output["contracts"].items():
+            for source_id, contracts_out in contracts.items():
                 for name, _ in contracts_out.items():
                     # Filter source files that the user did not ask for, such as
                     # imported relative files that are not part of the input.
                     for input_file_path in contract_filepaths:
                         if source_id in str(input_file_path):
                             input_contract_names.append(name)
 
             def classify_ast(_node: ASTNode):
                 if _node.ast_type in ("FunctionDefinition", "FunctionDefinitionNode"):
                     _node.classification = ASTClassification.FUNCTION
 
                 for child in _node.children:
                     classify_ast(child)
 
-            for source_id, contracts_out in output["contracts"].items():
+            for source_id, contracts_out in contracts.items():
                 ast_data = output["sources"][source_id]["ast"]
                 ast = ASTNode.parse_obj(ast_data)
                 classify_ast(ast)
 
                 for contract_name, ct_data in contracts_out.items():
                     contract_path = base_path / source_id
 
@@ -449,71 +464,61 @@
                     ct_data["ast"] = ast
                     contract_type = ContractType.parse_obj(ct_data)
                     contract_types.append(contract_type)
                     solc_versions_by_contract_name[contract_name] = solc_version
 
         return contract_types
 
-    def get_imports(
-        self, contract_filepaths: List[Path], base_path: Optional[Path] = None
-    ) -> Dict[str, List[str]]:
-        # NOTE: Process import remappings _before_ getting the full contract set.
+    def _get_unmapped_imports(
+        self,
+        contract_filepaths: List[Path],
+        base_path: Optional[Path] = None,
+    ) -> Dict[str, List[Tuple[str, str]]]:
         contracts_path = base_path or self.config_manager.contracts_folder
         import_remapping = self.get_import_remapping(base_path=contracts_path)
         contract_filepaths_set = verify_contract_filepaths(contract_filepaths)
 
-        def import_str_to_source_id(_import_str: str, source_path: Path) -> str:
-            quote = '"' if '"' in _import_str else "'"
-
-            try:
-                end_index = _import_str.index(quote) + 1
-            except ValueError as err:
-                raise CompilerError(
-                    f"Error parsing import statement '{_import_str}' in '{source_path.name}'."
-                ) from err
-
-            import_str_prefix = _import_str[end_index:]
-            import_str_value = import_str_prefix[: import_str_prefix.index(quote)]
-            path = (source_path.parent / import_str_value).resolve()
-            source_id_value = str(get_relative_path(path, contracts_path))
-
-            # Get all matches.
-            matches: List[Tuple[str, str]] = []
-            for key, value in import_remapping.items():
-                if key not in source_id_value:
-                    continue
-
-                matches.append((key, value))
+        imports_dict: Dict[str, List[Tuple[str, str]]] = {}
+        for src_path, import_strs in get_import_lines(contract_filepaths_set).items():
+            import_list = []
+            for import_str in import_strs:
+                raw_import_item_search = re.search(r'"(.*?)"', import_str)
+                if raw_import_item_search is None:
+                    raise CompilerError(f"No target filename found in import {import_str}")
+                raw_import_item = raw_import_item_search.group(1)
+                import_item = _import_str_to_source_id(
+                    import_str, src_path, contracts_path, import_remapping
+                )
 
-            if not matches:
-                return source_id_value
+                # Only add to the list if it's not already there, to mimic set behavior
+                if (import_item, raw_import_item) not in import_list:
+                    import_list.append((import_item, raw_import_item))
 
-            # Convert remapping list back to source using longest match (most exact).
-            key, value = max(matches, key=lambda x: len(x[0]))
-            sections = [s for s in source_id_value.split(key) if s]
-            depth = len(sections) - 1
-            source_id_value = ""
-
-            index = 0
-            for section in sections:
-                if index == depth:
-                    source_id_value += value
-                    source_id_value += section
-                elif index >= depth:
-                    source_id_value += section
+            source_id = str(get_relative_path(src_path, contracts_path))
+            imports_dict[str(source_id)] = import_list
 
-                index += 1
+        return imports_dict
 
-            return source_id_value
+    def get_imports(
+        self,
+        contract_filepaths: List[Path],
+        base_path: Optional[Path] = None,
+    ) -> Dict[str, List[str]]:
+        # NOTE: Process import remappings _before_ getting the full contract set.
+        contracts_path = base_path or self.config_manager.contracts_folder
+        import_remapping = self.get_import_remapping(base_path=contracts_path)
+        contract_filepaths_set = verify_contract_filepaths(contract_filepaths)
 
         imports_dict: Dict[str, List[str]] = {}
         for src_path, import_strs in get_import_lines(contract_filepaths_set).items():
             import_set = set()
             for import_str in import_strs:
-                import_item = import_str_to_source_id(import_str, src_path)
+                import_item = _import_str_to_source_id(
+                    import_str, src_path, contracts_path, import_remapping
+                )
                 import_set.add(import_item)
 
             source_id = str(get_relative_path(src_path, contracts_path))
             imports_dict[str(source_id)] = list(import_set)
 
         return imports_dict
 
@@ -669,78 +674,151 @@
             pragma_spec.select(self.installed_versions)
             if pragma_spec
             else max(self.installed_versions)
         )
 
     def enrich_error(self, err: ContractLogicError) -> ContractLogicError:
         if not is_0x_prefixed(err.revert_message):
+            # Nothing to do.
             return err
 
         if panic_cls := _get_sol_panic(err.revert_message):
-            # Is from a Solidity panic code, like a builtin Solidity revert.
-
-            if self._ape_version <= Version("0.6.10"):
-                return panic_cls(
-                    contract_address=err.contract_address,
-                    trace=err.trace,
-                    txn=err.txn,
-                )
-            else:
-                # TODO: Bump to next ape version and remove conditional.
-                return panic_cls(
-                    base_err=err.base_err,
-                    contract_address=err.contract_address,
-                    source_traceback=err.source_traceback,
-                    trace=err.trace,
-                    txn=err.txn,
-                )
+            return panic_cls(
+                base_err=err.base_err,
+                contract_address=err.contract_address,
+                source_traceback=err.source_traceback,
+                trace=err.trace,
+                txn=err.txn,
+            )
 
         # Check for ErrorABI.
         bytes_message = HexBytes(err.revert_message)
         selector = bytes_message[:4]
         input_data = bytes_message[4:]
-        address = err.contract_address or getattr(err.txn, "receiver", None)
-        if not address:
+
+        # TODO: Any version after Ape 0.6.11 we can replace this with `err.address`.
+        if not (
+            address := err.contract_address
+            or getattr(err.txn, "receiver", None)
+            or getattr(err.txn, "contract_address", None)
+        ):
             return err
 
         if not self.network_manager.active_provider:
             # Connection required.
             return err
 
-        contract = self.chain_manager.contracts.instance_at(address)
-        if not contract:
-            return err
-
-        if selector not in contract.contract_type.errors:
-            # Not an ErrorABI selector.
+        if (
+            not (contract := self.chain_manager.contracts.instance_at(address))
+            or selector not in contract.contract_type.errors
+        ):
             return err
 
         ecosystem = self.provider.network.ecosystem
         abi = contract.contract_type.errors[selector]
         inputs = ecosystem.decode_calldata(abi, input_data)
         error_class = contract.get_error_by_signature(abi.signature)
-        if self._ape_version <= Version("0.6.10"):
-            return error_class(
-                abi,
-                inputs,
-                txn=err.txn,
-                trace=err.trace,
-                contract_address=err.contract_address,
-            )
+        return error_class(
+            abi,
+            inputs,
+            base_err=err.base_err,
+            contract_address=err.contract_address,
+            source_traceback=err.source_traceback,
+            trace=err.trace,
+            txn=err.txn,
+        )
+
+    def _flatten_source(
+        self, path: Path, base_path: Optional[Path] = None, raw_import_name: Optional[str] = None
+    ) -> str:
+        base_path = base_path or self.config_manager.contracts_folder
+        imports = self._get_unmapped_imports([path])
+        source = ""
+        for import_list in imports.values():
+            for import_path, raw_import_path in sorted(import_list):
+                source += self._flatten_source(
+                    base_path / import_path, base_path=base_path, raw_import_name=raw_import_path
+                )
+        if raw_import_name:
+            source += f"// File: {raw_import_name}\n"
         else:
-            # TODO Bump Ape on next release and remove this conditional
-            return error_class(
-                abi,
-                inputs,
-                base_err=err.base_err,
-                contract_address=err.contract_address,  # type: ignore[call-arg]
-                source_traceback=err.source_traceback,  # type: ignore[call-arg]
-                trace=err.trace,
-                txn=err.txn,
-            )
+            source += f"// File: {path.name}\n"
+        source += path.read_text() + "\n"
+        return source
+
+    def flatten_contract(self, path: Path, **kwargs) -> Content:
+        # try compiling in order to validate it works
+        self.compile([path], base_path=self.config_manager.contracts_folder)
+        source = self._flatten_source(path)
+        source = remove_imports(source)
+        source = process_licenses(source)
+        source = remove_version_pragmas(source)
+        pragma = get_first_version_pragma(path.read_text())
+        source = "\n".join([pragma, source])
+        lines = source.splitlines()
+        line_dict = {i + 1: line for i, line in enumerate(lines)}
+        return Content(__root__=line_dict)
+
+
+def remove_imports(flattened_contract: str) -> str:
+    # Use regex.sub() to remove matched import statements
+    no_imports_contract = IMPORTS_PATTERN.sub("", flattened_contract)
+
+    return no_imports_contract
+
+
+def remove_version_pragmas(flattened_contract: str) -> str:
+    return VERSION_PRAGMA_PATTERN.sub("", flattened_contract)
+
+
+def get_first_version_pragma(source: str) -> str:
+    match = VERSION_PRAGMA_PATTERN.search(source)
+    if match:
+        return match.group(0)
+    return ""
+
+
+def get_licenses(source: str) -> List[Tuple[str, str]]:
+    matches = LICENSES_PATTERN.findall(source)
+    return matches
+
+
+def process_licenses(contract: str) -> str:
+    """
+    Process the licenses in a contract.
+    Ensure that all licenses are identical, and if not, raise an error.
+    The contract is returned with a single license identifier line at its top.
+    """
+
+    # Extract SPDX license identifiers from the contract.
+    extracted_licenses = get_licenses(contract)
+
+    # Return early if no licenses are present in the contract.
+    if not extracted_licenses:
+        return contract
+
+    # Get the unique license identifiers. We expect that all licenses in a contract are the same.
+    unique_license_identifiers = {
+        license_identifier for _, license_identifier in extracted_licenses
+    }
+
+    # If we have more than one unique license identifier, raise an error.
+    if len(unique_license_identifiers) > 1:
+        raise CompilerError(f"Conflicting licenses found: {unique_license_identifiers}")
+
+    # Get the first license line and identifier.
+    license_line, _ = extracted_licenses[0]
+
+    # Remove all of the license lines from the contract.
+    contract_without_licenses = contract.replace(license_line, "")
+
+    # Prepend the contract with only one license line.
+    contract_with_single_license = f"{license_line}\n{contract_without_licenses}"
+
+    return contract_with_single_license
 
 
 def _get_sol_panic(revert_message: str) -> Optional[Type[RuntimeErrorUnion]]:
     if revert_message.startswith(RUNTIME_ERROR_CODE_PREFIX):
         # ape-geth (style) plugins show the hex with the Panic ABI prefix.
         error_type_val = int(
             f"0x{revert_message.replace(RUNTIME_ERROR_CODE_PREFIX, '').lstrip('0')}", 16
@@ -749,7 +827,54 @@
         # Some plugins, like ape-hardhat, will deliver panic codes directly (no Panic ABI prefix)
         error_type_val = int(revert_message, 16)
 
     if error_type_val in [x.value for x in RuntimeErrorType]:
         return RUNTIME_ERROR_MAP[RuntimeErrorType(error_type_val)]
 
     return None
+
+
+def _import_str_to_source_id(
+    _import_str: str, source_path: Path, base_path: Path, import_remapping: Dict[str, str]
+) -> str:
+    quote = '"' if '"' in _import_str else "'"
+
+    try:
+        end_index = _import_str.index(quote) + 1
+    except ValueError as err:
+        raise CompilerError(
+            f"Error parsing import statement '{_import_str}' in '{source_path.name}'."
+        ) from err
+
+    import_str_prefix = _import_str[end_index:]
+    import_str_value = import_str_prefix[: import_str_prefix.index(quote)]
+    path = (source_path.parent / import_str_value).resolve()
+    source_id_value = str(get_relative_path(path, base_path))
+
+    # Get all matches.
+    matches: List[Tuple[str, str]] = []
+    for key, value in import_remapping.items():
+        if key not in source_id_value:
+            continue
+
+        matches.append((key, value))
+
+    if not matches:
+        return source_id_value
+
+    # Convert remapping list back to source using longest match (most exact).
+    key, value = max(matches, key=lambda x: len(x[0]))
+    sections = [s for s in source_id_value.split(key) if s]
+    depth = len(sections) - 1
+    source_id_value = ""
+
+    index = 0
+    for section in sections:
+        if index == depth:
+            source_id_value += value
+            source_id_value += section
+        elif index >= depth:
+            source_id_value += section
+
+        index += 1
+
+    return source_id_value
```

### Comparing `ape-solidity-0.6.6/ape_solidity/exceptions.py` & `ape-solidity-0.6.7/ape_solidity/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/ape_solidity.egg-info/PKG-INFO` & `ape-solidity-0.6.7/ape_solidity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-solidity
-Version: 0.6.6
+Version: 0.6.7
 Summary: Plugin for Ape Ethereum Framework for compiling Solidity contracts
 Home-page: https://github.com/ApeWorX/ape-solidity
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-solidity-0.6.6/ape_solidity.egg-info/SOURCES.txt` & `ape-solidity-0.6.7/ape_solidity.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 ape_solidity.egg-info/dependency_links.txt
 ape_solidity.egg-info/not-zip-safe
 ape_solidity.egg-info/requires.txt
 ape_solidity.egg-info/top_level.txt
 tests/__init__.py
 tests/ape-config.yaml
 tests/conftest.py
+tests/package-lock.json
+tests/package.json
 tests/test_compiler.py
 tests/test_integration.py
 tests/BrownieProject/brownie-config.yaml
 tests/BrownieProject/contracts/BrownieContract.sol
 tests/BrownieStyleDependency/ape-config.yaml
 tests/BrownieStyleDependency/contracts/BrownieStyleDependency.sol
 tests/BrownieStyleDependency/contracts/FailingContract.sol
@@ -62,14 +64,15 @@
 tests/contracts/ImportSourceWithEqualSignVersion.sol
 tests/contracts/ImportSourceWithNoPrefixVersion.sol
 tests/contracts/ImportingLessConstrainedVersion.sol
 tests/contracts/Imports.sol
 tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
 tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
 tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanionImport.sol
+tests/contracts/JustAStruct.sol
 tests/contracts/LibraryFun.sol
 tests/contracts/MissingPragma.sol
 tests/contracts/MultipleDefinitions.sol
 tests/contracts/NumerousDefinitions.sol
 tests/contracts/OlderVersion.sol
 tests/contracts/RandomVyperFile.vy
 tests/contracts/RangedVersion.sol
@@ -79,12 +82,14 @@
 tests/contracts/SpecificVersionRange.sol
 tests/contracts/SpecificVersionWithEqualSign.sol
 tests/contracts/UseYearn.sol
 tests/contracts/VagueVersion.sol
 tests/contracts/DirectoryWithExtension.sol/README.md
 tests/contracts/subfolder/Relativecontract.sol
 tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
+tests/data/ImportingLessConstrainedVersionFlat.sol
+tests/data/ImportsFlattened.sol.txt
 tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json
 tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json
 tests/data/packages/vault/master/vault_main.json
 tests/data/packages/vault/v0.4.5/vault.json
 tests/scripts/clean.py
```

### Comparing `ape-solidity-0.6.6/ape_solidity.egg-info/requires.txt` & `ape-solidity-0.6.7/ape_solidity.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 py-solc-x<2,>=1.1.0
-eth-ape<0.7,>=0.6.9
+eth-ape<0.7,>=0.6.12
 ethpm-types
 packaging
 requests
 typing-extensions==4.5.0
+web3[tester]<7,>=0.6.5
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
 black<24,>=23.3.0
```

### Comparing `ape-solidity-0.6.6/pyproject.toml` & `ape-solidity-0.6.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/setup.py` & `ape-solidity-0.6.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,19 +62,20 @@
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-solidity",
     include_package_data=True,
     install_requires=[
         "py-solc-x>=1.1.0,<2",
-        "eth-ape>=0.6.9,<0.7",
+        "eth-ape>=0.6.12,<0.7",
         "ethpm-types",  # Use the version ape requires
         "packaging",  # Use the version ape requires
         "requests",
         "typing-extensions==4.5.0",  # Can be removed onced pinned in Core.
+        "web3[tester]>=0.6.5,<7",  # Can remove any version after eth-ape 0.6.11
     ],
     python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_solidity"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
```

### Comparing `ape-solidity-0.6.6/tests/ape-config.yaml` & `ape-solidity-0.6.7/tests/ape-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 dependencies:
   - name: TestDependency
     local: ./Dependency
+  - name: DependencyOfDependency
+    local: ./DependencyOfDependency
 
   # Make sure can use a Brownie project as a dependency
   - name: BrownieDependency
     local: ./BrownieProject
 
   # Make sure can use a Brownie-style dependency.
   # Brownie-style dependencies don't compile on their own, necessarily
@@ -18,24 +20,35 @@
     version: 0.4.5
 
   # Ensure dependencies using GitHub references work.
   - name: vault
     github: yearn/yearn-vaults
     ref: master
 
+  # Ensure dependencies using NPM dependencies
+  - name: gnosis
+    npm: "@gnosis.pm/safe-contracts"
+    version: 1.3.0
+
 solidity:
   import_remapping:
     - "@remapping/contracts=TestDependency"
     - "@remapping_2=TestDependency"
     - "@remapping_2_brownie=BrownieDependency"
+    - "@dependency_remapping=DependencyOfDependency"
 
     # Remapping for showing we can import a contract type from a brownie-style dependency
     # (provided the _single_ contract type compiles in the project).
     - "@styleofbrownie=BrownieStyleDependency"
 
     # Ensure yearn-vaults works as a remapping
     - "@vault=vault/v0.4.5"
     - "@vaultmain=vault/master"
 
+    # Ensure that npm dependencies work as a remapping
+    - "@gnosis=gnosis/v1.3.0"
+
+    # Needed for Vault
+    - "@openzeppelin/contracts=OpenZeppelin/v4.7.1"
 
   # Using evm_version compatible with older and newer solidity versions.
   evm_version: constantinople
```

### Comparing `ape-solidity-0.6.6/tests/conftest.py` & `ape-solidity-0.6.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/tests/contracts/Imports.sol` & `ape-solidity-0.6.7/tests/contracts/Imports.sol`

 * *Files 18% similar despite different names*

```diff
@@ -14,13 +14,13 @@
     Struct1,
     Struct2,
     Struct3,
     Struct4,
     Struct5
 } from "./NumerousDefinitions.sol";
 import "@styleofbrownie/BrownieStyleDependency.sol";
-
+import "@gnosis/common/Enum.sol";
 contract Imports {
     function foo() pure public returns(bool) {
         return true;
     }
 }
```

### Comparing `ape-solidity-0.6.6/tests/contracts/LibraryFun.sol` & `ape-solidity-0.6.7/tests/contracts/LibraryFun.sol`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json` & `ape-solidity-0.6.7/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json` & `ape-solidity-0.6.7/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/tests/data/packages/vault/master/vault_main.json` & `ape-solidity-0.6.7/tests/data/packages/vault/master/vault_main.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/tests/data/packages/vault/v0.4.5/vault.json` & `ape-solidity-0.6.7/tests/data/packages/vault/v0.4.5/vault.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/tests/scripts/clean.py` & `ape-solidity-0.6.7/tests/scripts/clean.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.6/tests/test_compiler.py` & `ape-solidity-0.6.7/tests/test_compiler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import json
 import re
 import shutil
 from pathlib import Path
 
 import pytest
 import solcx  # type: ignore
+from ape import reverts
 from ape.contracts import ContractContainer
-from ape.exceptions import CompilerError
+from ape.exceptions import CompilerError, ContractLogicError
 from ethpm_types.ast import ASTClassification
+from pkg_resources import get_distribution
 from semantic_version import Version  # type: ignore
 
 from ape_solidity import Extension
 from ape_solidity._utils import OUTPUT_SELECTION
 from ape_solidity.exceptions import IndexOutOfBoundsError
 
 BASE_PATH = Path(__file__).parent / "contracts"
@@ -26,17 +28,19 @@
 
 # These are tested elsewhere, not in `test_compile`.
 normal_test_skips = (
     "DifferentNameThanFile",
     "MultipleDefinitions",
     "RandomVyperFile",
     "LibraryFun",
+    "JustAStruct",
 )
 raises_because_not_sol = pytest.raises(CompilerError, match=EXPECTED_NON_SOLIDITY_ERR_MSG)
 DEFAULT_OPTIMIZER = {"enabled": True, "runs": 200}
+APE_VERSION = Version(get_distribution("eth-ape").version.split(".dev")[0].strip())
 
 
 @pytest.mark.parametrize(
     "contract",
     [c for c in TEST_CONTRACTS if all(n not in str(c) for n in normal_test_skips)],
 )
 def test_compile(project, contract):
@@ -98,26 +102,36 @@
 
 
 def test_compile_vyper_contract(compiler, vyper_source_path):
     with raises_because_not_sol:
         compiler.compile([vyper_source_path])
 
 
+def test_compile_just_a_struct(compiler, project):
+    """
+    Before, you would get a nasty index error, even though this is valid Solidity.
+    The fix involved using nicer access to "contracts" in the standard output JSON.
+    """
+    contract_types = compiler.compile([project.contracts_folder / "JustAStruct.sol"])
+    assert len(contract_types) == 0
+
+
 def test_get_imports(project, compiler):
     import_dict = compiler.get_imports(TEST_CONTRACT_PATHS, BASE_PATH)
     contract_imports = import_dict["Imports.sol"]
     # NOTE: make sure there aren't duplicates
     assert len([x for x in contract_imports if contract_imports.count(x) > 1]) == 0
     # NOTE: returning a list
     assert type(contract_imports) == list
     # NOTE: in case order changes
     expected = {
         ".cache/BrownieDependency/local/BrownieContract.sol",
         ".cache/BrownieStyleDependency/local/BrownieStyleDependency.sol",
         ".cache/TestDependency/local/Dependency.sol",
+        ".cache/gnosis/v1.3.0/common/Enum.sol",
         "CompilesOnce.sol",
         "MissingPragma.sol",
         "NumerousDefinitions.sol",
         "subfolder/Relativecontract.sol",
     }
     assert set(contract_imports) == expected
 
@@ -127,22 +141,23 @@
         compiler.get_imports([vyper_source_path])
 
 
 def test_get_import_remapping(compiler, project, config):
     import_remapping = compiler.get_import_remapping()
     assert import_remapping == {
         "@remapping_2_brownie": ".cache/BrownieDependency/local",
-        "@dependency_remapping": ".cache/TestDependencyOfDependency/local",
+        "@dependency_remapping": ".cache/DependencyOfDependency/local",
         "@remapping_2": ".cache/TestDependency/local",
         "@remapping/contracts": ".cache/TestDependency/local",
         "@styleofbrownie": ".cache/BrownieStyleDependency/local",
         "@openzeppelin/contracts": ".cache/OpenZeppelin/v4.7.1",
         "@oz/contracts": ".cache/OpenZeppelin/v4.5.0",
         "@vault": ".cache/vault/v0.4.5",
         "@vaultmain": ".cache/vault/master",
+        "@gnosis": ".cache/gnosis/v1.3.0",
     }
 
     with config.using_project(project.path / "ProjectWithinProject") as proj:
         # Trigger downloading dependencies in new ProjectWithinProject
         dependencies = proj.dependencies
         assert dependencies
         # Should be different now that we have changed projects.
@@ -198,15 +213,15 @@
     assert len(version_map) == 2
 
     expected_version = Version("0.8.12+commit.f00d7308")
     latest_version = [v for v in version_map if v != expected_version][0]
     assert all([f in version_map[expected_version] for f in file_paths[:-1]])
 
     latest_version_sources = version_map[latest_version]
-    assert len(latest_version_sources) == 9, "Did the import remappings load correctly?"
+    assert len(latest_version_sources) == 10, "Did the import remappings load correctly?"
     assert file_paths[-1] in latest_version_sources
 
     # Will fail if the import remappings have not loaded yet.
     assert all([f.is_file() for f in file_paths])
 
 
 def test_get_version_map_single_source(compiler, project):
@@ -249,26 +264,27 @@
         in compiler_latest.settings["remappings"]
     )
     assert "@vault=.cache/vault/v0.4.5" in compiler_latest.settings["remappings"]
     assert "@vaultmain=.cache/vault/master" in compiler_latest.settings["remappings"]
     common_suffix = ".cache/TestDependency/local"
     expected_remappings = (
         "@remapping_2_brownie=.cache/BrownieDependency/local",
-        "@dependency_remapping=.cache/TestDependencyOfDependency/local",
+        "@dependency_remapping=.cache/DependencyOfDependency/local",
         f"@remapping_2={common_suffix}",
         f"@remapping/contracts={common_suffix}",
         "@styleofbrownie=.cache/BrownieStyleDependency/local",
     )
     actual_remappings = compiler_latest.settings["remappings"]
     assert all(x in actual_remappings for x in expected_remappings)
     assert all(
         b >= a for a, b in zip(actual_remappings, actual_remappings[1:])
     ), "Import remappings should be sorted"
     assert f"@remapping/contracts={common_suffix}" in compiler_0426.settings["remappings"]
     assert "UseYearn" in compiler_latest.contractTypes
+    assert "@gnosis=.cache/gnosis/v1.3.0" in compiler_latest.settings["remappings"]
 
     # Compiler contract types test
     assert set(compiler_0812.contractTypes) == {
         "ImportSourceWithEqualSignVersion",
         "ImportSourceWithNoPrefixVersion",
         "ImportingLessConstrainedVersion",
         "IndirectlyImportingMoreConstrainedVersion",
@@ -307,27 +323,29 @@
     indirect_source = "SpecificVersionWithEqualSign.sol"
     file_paths = [project.contracts_folder / x for x in (source_a, source_b, source_c, source_d)]
     actual = compiler.get_compiler_settings(file_paths)
     v812 = Version("0.8.12+commit.f00d7308")
     latest = max(list(actual.keys()))
     expected_remappings = (
         "@remapping_2_brownie=.cache/BrownieDependency/local",
-        "@dependency_remapping=.cache/TestDependencyOfDependency/local",
+        "@dependency_remapping=.cache/DependencyOfDependency/local",
         "@remapping_2=.cache/TestDependency/local",
         "@remapping/contracts=.cache/TestDependency/local",
         "@styleofbrownie=.cache/BrownieStyleDependency/local",
+        "@gnosis=.cache/gnosis/v1.3.0",
     )
     expected_v812_contracts = (source_a, source_b, source_c, indirect_source)
     expected_latest_contracts = (
         ".cache/BrownieDependency/local/BrownieContract.sol",
         "CompilesOnce.sol",
         ".cache/TestDependency/local/Dependency.sol",
-        ".cache/TestDependencyOfDependency/local/DependencyOfDependency.sol",
+        ".cache/DependencyOfDependency/local/DependencyOfDependency.sol",
         source_d,
         "subfolder/Relativecontract.sol",
+        ".cache/gnosis/v1.3.0/common/Enum.sol",
     )
 
     # Shared compiler defaults tests
     expected_source_lists = (expected_v812_contracts, expected_latest_contracts)
     for version, expected_sources in zip((v812, latest), expected_source_lists):
         output_selection = actual[version]["outputSelection"]
         assert actual[version]["optimizer"] == DEFAULT_OPTIMIZER
@@ -381,27 +399,53 @@
     assert project.C
 
 
 def test_enrich_error_when_custom(compiler, project, owner, not_owner, connection):
     compiler.compile((project.contracts_folder / "HasError.sol",))
 
     # Deploy so Ape know about contract type.
-    contract = owner.deploy(project.HasError)
+    contract = owner.deploy(project.HasError, 1)
     with pytest.raises(contract.Unauthorized) as err:
         contract.withdraw(sender=not_owner)
 
     assert err.value.inputs == {"addr": not_owner.address, "counter": 123}
 
 
-def test_enrich_error_when_builtin(project, owner, connection):
-    contract = project.BuiltinErrorChecker.deploy(sender=owner)
+def test_enrich_error_when_custom_in_constructor(compiler, project, owner, not_owner, connection):
+    # Deploy so Ape know about contract type.
+    with reverts(project.HasError.Unauthorized) as err:
+        not_owner.deploy(project.HasError, 0)
 
-    with pytest.raises(IndexOutOfBoundsError):
-        contract.checkIndexOutOfBounds(sender=owner)
+    assert err.value.inputs == {"addr": not_owner.address, "counter": 123}
+
+
+def test_enrich_error_when_builtin(project, owner, connection):
+    # TODO: Any version after eth-ape 0.6.11, you can uncomment this and delete the rest.
+    # contract = project.BuiltinErrorChecker.deploy(sender=owner)
+    # with pytest.raises(IndexOutOfBoundsError):
+    #     contract.checkIndexOutOfBounds(sender=owner)
+
+    compiler = project.compiler_manager.solidity
+    contract_err = ContractLogicError(
+        revert_message="0x4e487b710000000000000000000000000000000000000000000000000000000000000032"
+    )
+    actual = compiler.enrich_error(contract_err)
+    assert isinstance(actual, IndexOutOfBoundsError)
 
 
 def test_ast(project, compiler):
     source_path = project.contracts_folder / "MultipleDefinitions.sol"
     actual = compiler.compile([source_path])[-1].ast
     fn_node = actual.children[1].children[0]
     assert actual.ast_type == "SourceUnit"
     assert fn_node.classification == ASTClassification.FUNCTION
+
+
+def test_flatten(project, compiler, data_folder):
+    source_path = project.contracts_folder / "Imports.sol"
+    with pytest.raises(CompilerError):
+        compiler.flatten_contract(source_path)
+
+    source_path = project.contracts_folder / "ImportingLessConstrainedVersion.sol"
+    flattened_source = compiler.flatten_contract(source_path)
+    flattened_source_path = data_folder / "ImportingLessConstrainedVersionFlat.sol"
+    assert str(flattened_source) == str(flattened_source_path.read_text())
```

### Comparing `ape-solidity-0.6.6/tests/test_integration.py` & `ape-solidity-0.6.7/tests/test_integration.py`

 * *Files identical despite different names*

