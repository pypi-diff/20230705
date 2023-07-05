# Comparing `tmp/smart_chromadb-0.1.dev732.tar.gz` & `tmp/smart_chromadb-0.1.dev733.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/johnyan/Documents/project/chroma/dist/.tmp-g3z0s293/smart_chromadb-0.1.dev732.tar", last modified: Wed Jul  5 00:31:23 2023, max compression
+gzip compressed data, was "/Users/johnyan/Documents/project/chroma/dist/.tmp-4l85f_2n/smart_chromadb-0.1.dev733.tar", last modified: Wed Jul  5 01:00:13 2023, max compression
```

## Comparing `smart_chromadb-0.1.dev732.tar` & `smart_chromadb-0.1.dev733.tar`

### file list

```diff
@@ -1,233 +1,233 @@
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:23.006915 smart_chromadb-0.1.dev732/
--rw-r--r--   0 johnyan    (501) staff       (20)       84 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.dockerignore
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.747999 smart_chromadb-0.1.dev732/.github/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.788118 smart_chromadb-0.1.dev732/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 johnyan    (501) staff       (20)     1512 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 johnyan    (501) staff       (20)     1520 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 johnyan    (501) staff       (20)     1384 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/ISSUE_TEMPLATE/installation_trouble.yaml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.795950 smart_chromadb-0.1.dev732/.github/workflows/
--rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/workflows/chroma-client-integration-test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1187 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/workflows/chroma-integration-test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1338 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/workflows/chroma-release-python-client.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     4169 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/workflows/chroma-release.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1205 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/workflows/chroma-test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1734 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/workflows/pr-review-checklist.yml
--rw-r--r--   0 johnyan    (501) staff       (20)      228 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.gitignore
--rw-r--r--   0 johnyan    (501) staff       (20)     1167 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.pre-commit-config.yaml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.797329 smart_chromadb-0.1.dev732/.vscode/
--rw-r--r--   0 johnyan    (501) staff       (20)     1020 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.vscode/settings.json
--rw-r--r--   0 johnyan    (501) staff       (20)     3323 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/DEVELOP.md
--rw-r--r--   0 johnyan    (501) staff       (20)      647 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/Dockerfile
--rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/LICENSE
--rw-r--r--   0 johnyan    (501) staff       (20)     6220 2023-07-05 00:31:23.006133 smart_chromadb-0.1.dev732/PKG-INFO
--rw-r--r--   0 johnyan    (501) staff       (20)     5679 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)      619 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/RELEASE_PROCESS.md
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.813519 smart_chromadb-0.1.dev732/bin/
--rw-r--r--   0 johnyan    (501) staff       (20)     1610 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/backup.sh
--rwxr-xr-x   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/build
--rwxr-xr-x   0 johnyan    (501) staff       (20)      234 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/docker_entrypoint.sh
--rw-r--r--   0 johnyan    (501) staff       (20)     6462 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/generate_cloudformation.py
--rwxr-xr-x   0 johnyan    (501) staff       (20)      463 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/integration-test
--rw-r--r--   0 johnyan    (501) staff       (20)     1688 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/restore.sh
--rw-r--r--   0 johnyan    (501) staff       (20)     1105 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/setup_linux.sh
--rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/setup_mac.sh
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.814539 smart_chromadb-0.1.dev732/bin/templates/
--rw-r--r--   0 johnyan    (501) staff       (20)      985 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/templates/docker-compose.yml
--rwxr-xr-x   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/test-package.sh
--rwxr-xr-x   0 johnyan    (501) staff       (20)      297 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/test-remote
--rw-r--r--   0 johnyan    (501) staff       (20)      205 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/test.py
--rwxr-xr-x   0 johnyan    (501) staff       (20)      151 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/version
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.821079 smart_chromadb-0.1.dev732/chromadb/
--rw-r--r--   0 johnyan    (501) staff       (20)      894 2023-07-04 08:34:52.000000 smart_chromadb-0.1.dev732/chromadb/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.827730 smart_chromadb-0.1.dev732/chromadb/api/
--rw-r--r--   0 johnyan    (501) staff       (20)    10898 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/api/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12480 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/api/fastapi.py
--rw-r--r--   0 johnyan    (501) staff       (20)    17852 2023-07-03 08:25:25.000000 smart_chromadb-0.1.dev732/chromadb/api/local.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.828565 smart_chromadb-0.1.dev732/chromadb/api/models/
--rw-r--r--   0 johnyan    (501) staff       (20)    15103 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/api/models/Collection.py
--rw-r--r--   0 johnyan    (501) staff       (20)      819 2023-07-03 07:56:58.000000 smart_chromadb-0.1.dev732/chromadb/api/smartapi.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11283 2023-07-03 09:25:09.000000 smart_chromadb-0.1.dev732/chromadb/api/types.py
--rw-r--r--   0 johnyan    (501) staff       (20)      168 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/app.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7231 2023-07-03 08:16:05.000000 smart_chromadb-0.1.dev732/chromadb/config.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.837348 smart_chromadb-0.1.dev732/chromadb/db/
--rw-r--r--   0 johnyan    (501) staff       (20)     3390 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6004 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/base.py
--rw-r--r--   0 johnyan    (501) staff       (20)    22307 2023-07-03 08:25:52.000000 smart_chromadb-0.1.dev732/chromadb/db/clickhouse.py
--rw-r--r--   0 johnyan    (501) staff       (20)    18795 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/duckdb.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.840369 smart_chromadb-0.1.dev732/chromadb/db/impl/
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/impl/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6221 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/impl/sqlite.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.842981 smart_chromadb-0.1.dev732/chromadb/db/index/
--rw-r--r--   0 johnyan    (501) staff       (20)      447 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/index/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11060 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/index/hnswlib.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8096 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/migrations.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.845517 smart_chromadb-0.1.dev732/chromadb/db/mixins/
--rw-r--r--   0 johnyan    (501) staff       (20)     9193 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/mixins/embeddings_queue.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15557 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/mixins/sysdb.py
--rw-r--r--   0 johnyan    (501) staff       (20)    16619 2023-07-04 09:55:11.000000 smart_chromadb-0.1.dev732/chromadb/db/smartdb.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2656 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/system.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1293 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/errors.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.846654 smart_chromadb-0.1.dev732/chromadb/ingest/
--rw-r--r--   0 johnyan    (501) staff       (20)     3643 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/ingest/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.849734 smart_chromadb-0.1.dev732/chromadb/segment/
--rw-r--r--   0 johnyan    (501) staff       (20)     3059 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/segment/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.753169 smart_chromadb-0.1.dev732/chromadb/segment/impl/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.851893 smart_chromadb-0.1.dev732/chromadb/segment/impl/manager/
--rw-r--r--   0 johnyan    (501) staff       (20)     4358 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/segment/impl/manager/local.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.853044 smart_chromadb-0.1.dev732/chromadb/segment/impl/metadata/
--rw-r--r--   0 johnyan    (501) staff       (20)    17879 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/segment/impl/metadata/sqlite.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.854194 smart_chromadb-0.1.dev732/chromadb/segment/impl/vector/
--rw-r--r--   0 johnyan    (501) staff       (20)    11965 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/segment/impl/vector/local_hnsw.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.855059 smart_chromadb-0.1.dev732/chromadb/server/
--rw-r--r--   0 johnyan    (501) staff       (20)      172 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/server/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.857413 smart_chromadb-0.1.dev732/chromadb/server/fastapi/
--rw-r--r--   0 johnyan    (501) staff       (20)     9064 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/server/fastapi/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2134 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/server/fastapi/types.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.862695 smart_chromadb-0.1.dev732/chromadb/telemetry/
--rw-r--r--   0 johnyan    (501) staff       (20)     3214 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/telemetry/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)      591 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/telemetry/events.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1161 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/telemetry/posthog.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.868115 smart_chromadb-0.1.dev732/chromadb/test/
--rw-r--r--   0 johnyan    (501) staff       (20)     3993 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/conftest.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.871547 smart_chromadb-0.1.dev732/chromadb/test/db/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.877841 smart_chromadb-0.1.dev732/chromadb/test/db/migrations/
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/migrations/00001-migration-1.psql.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/migrations/00002-migration-2.psql.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/migrations/00003-migration-3.psql.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)     1168 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/test_base.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5026 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/test_migrations.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9773 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/test_system.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.878866 smart_chromadb-0.1.dev732/chromadb/test/hnswlib/
--rw-r--r--   0 johnyan    (501) staff       (20)     2337 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/hnswlib/test_hnswlib.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.880568 smart_chromadb-0.1.dev732/chromadb/test/ingest/
--rw-r--r--   0 johnyan    (501) staff       (20)     8117 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/ingest/test_producer_consumer.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.890321 smart_chromadb-0.1.dev732/chromadb/test/property/
--rw-r--r--   0 johnyan    (501) staff       (20)    11294 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/property/invariants.py
--rw-r--r--   0 johnyan    (501) staff       (20)    18662 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/property/strategies.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2213 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/property/test_add.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6211 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/property/test_collections.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9123 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/property/test_cross_version_persist.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11073 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/property/test_embeddings.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9062 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/property/test_filtering.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5146 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/property/test_persist.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.893849 smart_chromadb-0.1.dev732/chromadb/test/segment/
--rw-r--r--   0 johnyan    (501) staff       (20)    15026 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/segment/test_metadata.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12132 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/segment/test_vector.py
--rw-r--r--   0 johnyan    (501) staff       (20)    40340 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/test_api.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2234 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/test_chroma.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4127 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/test_config.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.895346 smart_chromadb-0.1.dev732/chromadb/test/utils/
--rw-r--r--   0 johnyan    (501) staff       (20)     3544 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/utils/test_messagid.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3702 2023-06-30 03:21:44.000000 smart_chromadb-0.1.dev732/chromadb/types.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.897254 smart_chromadb-0.1.dev732/chromadb/utils/
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/utils/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    16311 2023-06-30 06:12:24.000000 smart_chromadb-0.1.dev732/chromadb/utils/embedding_functions.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2301 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/utils/messageid.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.763949 smart_chromadb-0.1.dev732/clients/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.917463 smart_chromadb-0.1.dev732/clients/js/
--rw-r--r--   0 johnyan    (501) staff       (20)       66 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/.gitignore
--rw-r--r--   0 johnyan    (501) staff       (20)       32 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/.prettierignore
--rw-r--r--   0 johnyan    (501) staff       (20)        3 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/.prettierrc.json
--rw-r--r--   0 johnyan    (501) staff       (20)     1256 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/DEVELOP.md
--rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/LICENSE
--rw-r--r--   0 johnyan    (501) staff       (20)     1266 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)      324 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/config.yml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.762288 smart_chromadb-0.1.dev732/clients/js/examples/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.925135 smart_chromadb-0.1.dev732/clients/js/examples/browser/
--rw-r--r--   0 johnyan    (501) staff       (20)      358 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/browser/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)     1787 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/browser/app.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      834 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/browser/index.html
--rw-r--r--   0 johnyan    (501) staff       (20)      409 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/browser/package.json
--rw-r--r--   0 johnyan    (501) staff       (20)    71072 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/browser/yarn.lock
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.932932 smart_chromadb-0.1.dev732/clients/js/examples/node/
--rw-r--r--   0 johnyan    (501) staff       (20)       57 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/node/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)     1191 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/node/app.js
--rw-r--r--   0 johnyan    (501) staff       (20)    46542 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/node/package-lock.json
--rw-r--r--   0 johnyan    (501) staff       (20)      503 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/node/package.json
--rw-r--r--   0 johnyan    (501) staff       (20)    17116 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/node/yarn.lock
--rwxr-xr-x   0 johnyan    (501) staff       (20)     1075 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/genapi.sh
--rw-r--r--   0 johnyan    (501) staff       (20)      469 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/jest.config.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      153 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/openapitools.json
--rw-r--r--   0 johnyan    (501) staff       (20)   450648 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/package-lock.json
--rw-r--r--   0 johnyan    (501) staff       (20)     1455 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/package.json
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.940660 smart_chromadb-0.1.dev732/clients/js/src/
--rw-r--r--   0 johnyan    (501) staff       (20)     8171 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/ChromaClient.ts
--rw-r--r--   0 johnyan    (501) staff       (20)    19403 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/Collection.ts
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.947473 smart_chromadb-0.1.dev732/clients/js/src/embeddings/
--rw-r--r--   0 johnyan    (501) staff       (20)      938 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/embeddings/CohereEmbeddingFunction.ts
--rw-r--r--   0 johnyan    (501) staff       (20)       92 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/embeddings/IEmbeddingFunction.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1563 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2493 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
--rwxr-xr-x   0 johnyan    (501) staff       (20)     3402 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.956820 smart_chromadb-0.1.dev732/clients/js/src/generated/
--rw-r--r--   0 johnyan    (501) staff       (20)      921 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/generated/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)    56700 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/generated/api.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1478 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/generated/configuration.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      429 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/generated/index.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     5862 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/generated/models.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1307 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/generated/runtime.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      490 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/index.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1715 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/types.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2002 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/utils.ts
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.973560 smart_chromadb-0.1.dev732/clients/js/test/
--rw-r--r--   0 johnyan    (501) staff       (20)     2625 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/add.collections.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     7586 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/client.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     3284 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/collection.client.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2551 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/data.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/delete.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2599 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/get.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      206 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/initClient.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      577 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/peek.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1990 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/query.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2160 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/update.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      802 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/upsert.collections.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      367 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/tsconfig.json
--rw-r--r--   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/tsconfig.module.json
--rw-r--r--   0 johnyan    (501) staff       (20)   157735 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/yarn.lock
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.980263 smart_chromadb-0.1.dev732/clients/python/
--rw-r--r--   0 johnyan    (501) staff       (20)     1627 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/python/README.md
--rwxr-xr-x   0 johnyan    (501) staff       (20)     1257 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/python/build_python_thin_client.sh
--rwxr-xr-x   0 johnyan    (501) staff       (20)      826 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/python/integration-test.sh
--rw-r--r--   0 johnyan    (501) staff       (20)       22 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/python/is_thin_client.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1166 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/python/pyproject.toml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.983249 smart_chromadb-0.1.dev732/config/
--rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/config/backup_disk.xml
--rw-r--r--   0 johnyan    (501) staff       (20)      233 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/config/chroma_users.xml
--rw-r--r--   0 johnyan    (501) staff       (20)     1080 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/docker-compose.server.example.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1221 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/docker-compose.test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1226 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/docker-compose.yml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.986097 smart_chromadb-0.1.dev732/examples/
--rw-r--r--   0 johnyan    (501) staff       (20)    10346 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/examples/alternative_embeddings.ipynb
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.765338 smart_chromadb-0.1.dev732/examples/deployments/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.993631 smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/
--rw-r--r--   0 johnyan    (501) staff       (20)      611 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)      752 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/chroma.tf
--rw-r--r--   0 johnyan    (501) staff       (20)      125 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/main.tf
--rw-r--r--   0 johnyan    (501) staff       (20)     2271 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/startup.sh
--rw-r--r--   0 johnyan    (501) staff       (20)      181 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/variables.tf
--rw-r--r--   0 johnyan    (501) staff       (20)     5830 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/examples/local_persistence.ipynb
--rw-r--r--   0 johnyan    (501) staff       (20)     5493 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/examples/where_filtering.ipynb
--rw-r--r--   0 johnyan    (501) staff       (20)      495 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/log_config.yml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.766614 smart_chromadb-0.1.dev732/migrations/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.994820 smart_chromadb-0.1.dev732/migrations/embeddings_queue/
--rw-r--r--   0 johnyan    (501) staff       (20)      261 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/migrations/embeddings_queue/00001-embeddings.sqlite.sql
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.996007 smart_chromadb-0.1.dev732/migrations/metadb/
--rw-r--r--   0 johnyan    (501) staff       (20)      620 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/migrations/metadb/00001-embedding-metadata.sqlite.sql
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.998389 smart_chromadb-0.1.dev732/migrations/sysdb/
--rw-r--r--   0 johnyan    (501) staff       (20)      336 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/migrations/sysdb/00001-collections.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/migrations/sysdb/00002-segments.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)      372 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/pull_request_template.md
--rw-r--r--   0 johnyan    (501) staff       (20)     1455 2023-06-26 07:09:55.000000 smart_chromadb-0.1.dev732/pyproject.toml
--rw-r--r--   0 johnyan    (501) staff       (20)      352 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/requirements.txt
--rw-r--r--   0 johnyan    (501) staff       (20)      161 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/requirements_dev.txt
--rw-r--r--   0 johnyan    (501) staff       (20)       38 2023-07-05 00:31:23.007148 smart_chromadb-0.1.dev732/setup.cfg
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:23.005192 smart_chromadb-0.1.dev732/smart_chromadb.egg-info/
--rw-r--r--   0 johnyan    (501) staff       (20)     6220 2023-07-05 00:31:22.000000 smart_chromadb-0.1.dev732/smart_chromadb.egg-info/PKG-INFO
--rw-r--r--   0 johnyan    (501) staff       (20)     5825 2023-07-05 00:31:22.000000 smart_chromadb-0.1.dev732/smart_chromadb.egg-info/SOURCES.txt
--rw-r--r--   0 johnyan    (501) staff       (20)        1 2023-07-05 00:31:22.000000 smart_chromadb-0.1.dev732/smart_chromadb.egg-info/dependency_links.txt
--rw-r--r--   0 johnyan    (501) staff       (20)      340 2023-07-05 00:31:22.000000 smart_chromadb-0.1.dev732/smart_chromadb.egg-info/requires.txt
--rw-r--r--   0 johnyan    (501) staff       (20)        9 2023-07-05 00:31:22.000000 smart_chromadb-0.1.dev732/smart_chromadb.egg-info/top_level.txt
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.065730 smart_chromadb-0.1.dev733/
+-rw-r--r--   0 johnyan    (501) staff       (20)       84 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.dockerignore
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.814016 smart_chromadb-0.1.dev733/.github/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.845879 smart_chromadb-0.1.dev733/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1512 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1520 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1384 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/ISSUE_TEMPLATE/installation_trouble.yaml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.850908 smart_chromadb-0.1.dev733/.github/workflows/
+-rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/workflows/chroma-client-integration-test.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1187 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/workflows/chroma-integration-test.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1338 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/workflows/chroma-release-python-client.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     4169 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/workflows/chroma-release.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1205 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/workflows/chroma-test.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1734 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.github/workflows/pr-review-checklist.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)      228 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.gitignore
+-rw-r--r--   0 johnyan    (501) staff       (20)     1167 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.pre-commit-config.yaml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.851862 smart_chromadb-0.1.dev733/.vscode/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1020 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/.vscode/settings.json
+-rw-r--r--   0 johnyan    (501) staff       (20)     3323 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/DEVELOP.md
+-rw-r--r--   0 johnyan    (501) staff       (20)      647 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/Dockerfile
+-rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/LICENSE
+-rw-r--r--   0 johnyan    (501) staff       (20)     6220 2023-07-05 01:00:13.065086 smart_chromadb-0.1.dev733/PKG-INFO
+-rw-r--r--   0 johnyan    (501) staff       (20)     5679 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)      619 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/RELEASE_PROCESS.md
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.869128 smart_chromadb-0.1.dev733/bin/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1610 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/backup.sh
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/build
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      234 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/docker_entrypoint.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)     6462 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/generate_cloudformation.py
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      463 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/integration-test
+-rw-r--r--   0 johnyan    (501) staff       (20)     1688 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/restore.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)     1105 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/setup_linux.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/setup_mac.sh
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.871204 smart_chromadb-0.1.dev733/bin/templates/
+-rw-r--r--   0 johnyan    (501) staff       (20)      985 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/templates/docker-compose.yml
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/test-package.sh
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      297 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/test-remote
+-rw-r--r--   0 johnyan    (501) staff       (20)      205 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/test.py
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      151 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/bin/version
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.875763 smart_chromadb-0.1.dev733/chromadb/
+-rw-r--r--   0 johnyan    (501) staff       (20)      894 2023-07-04 08:34:52.000000 smart_chromadb-0.1.dev733/chromadb/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.883748 smart_chromadb-0.1.dev733/chromadb/api/
+-rw-r--r--   0 johnyan    (501) staff       (20)    10898 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/api/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    12480 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/api/fastapi.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    17852 2023-07-03 08:25:25.000000 smart_chromadb-0.1.dev733/chromadb/api/local.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.884529 smart_chromadb-0.1.dev733/chromadb/api/models/
+-rw-r--r--   0 johnyan    (501) staff       (20)    15103 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/api/models/Collection.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      819 2023-07-03 07:56:58.000000 smart_chromadb-0.1.dev733/chromadb/api/smartapi.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11283 2023-07-03 09:25:09.000000 smart_chromadb-0.1.dev733/chromadb/api/types.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      168 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/app.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7231 2023-07-03 08:16:05.000000 smart_chromadb-0.1.dev733/chromadb/config.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.895630 smart_chromadb-0.1.dev733/chromadb/db/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3390 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6004 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/base.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    22307 2023-07-03 08:25:52.000000 smart_chromadb-0.1.dev733/chromadb/db/clickhouse.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    18795 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/duckdb.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.897485 smart_chromadb-0.1.dev733/chromadb/db/impl/
+-rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/impl/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6221 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/impl/sqlite.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.899510 smart_chromadb-0.1.dev733/chromadb/db/index/
+-rw-r--r--   0 johnyan    (501) staff       (20)      447 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/index/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11060 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/index/hnswlib.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8096 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/migrations.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.903241 smart_chromadb-0.1.dev733/chromadb/db/mixins/
+-rw-r--r--   0 johnyan    (501) staff       (20)     9193 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/mixins/embeddings_queue.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    15557 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/mixins/sysdb.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    16627 2023-07-05 00:49:42.000000 smart_chromadb-0.1.dev733/chromadb/db/smartdb.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2656 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/db/system.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1293 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/errors.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.905239 smart_chromadb-0.1.dev733/chromadb/ingest/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3643 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/ingest/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.907332 smart_chromadb-0.1.dev733/chromadb/segment/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3059 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/segment/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.816756 smart_chromadb-0.1.dev733/chromadb/segment/impl/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.909423 smart_chromadb-0.1.dev733/chromadb/segment/impl/manager/
+-rw-r--r--   0 johnyan    (501) staff       (20)     4358 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/segment/impl/manager/local.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.911260 smart_chromadb-0.1.dev733/chromadb/segment/impl/metadata/
+-rw-r--r--   0 johnyan    (501) staff       (20)    17879 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/segment/impl/metadata/sqlite.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.913905 smart_chromadb-0.1.dev733/chromadb/segment/impl/vector/
+-rw-r--r--   0 johnyan    (501) staff       (20)    11965 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/segment/impl/vector/local_hnsw.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.914955 smart_chromadb-0.1.dev733/chromadb/server/
+-rw-r--r--   0 johnyan    (501) staff       (20)      172 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/server/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.918217 smart_chromadb-0.1.dev733/chromadb/server/fastapi/
+-rw-r--r--   0 johnyan    (501) staff       (20)     9064 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/server/fastapi/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2134 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/server/fastapi/types.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.922855 smart_chromadb-0.1.dev733/chromadb/telemetry/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3214 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/telemetry/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      591 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/telemetry/events.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1161 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/telemetry/posthog.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.928389 smart_chromadb-0.1.dev733/chromadb/test/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3993 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/conftest.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.934819 smart_chromadb-0.1.dev733/chromadb/test/db/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.942083 smart_chromadb-0.1.dev733/chromadb/test/db/migrations/
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/migrations/00001-migration-1.psql.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/migrations/00002-migration-2.psql.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/migrations/00003-migration-3.psql.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)     1168 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/test_base.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5026 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/test_migrations.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9773 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/db/test_system.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.943456 smart_chromadb-0.1.dev733/chromadb/test/hnswlib/
+-rw-r--r--   0 johnyan    (501) staff       (20)     2337 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/hnswlib/test_hnswlib.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.945671 smart_chromadb-0.1.dev733/chromadb/test/ingest/
+-rw-r--r--   0 johnyan    (501) staff       (20)     8117 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/ingest/test_producer_consumer.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.956335 smart_chromadb-0.1.dev733/chromadb/test/property/
+-rw-r--r--   0 johnyan    (501) staff       (20)    11294 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/property/invariants.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    18662 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/property/strategies.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2213 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/property/test_add.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6211 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/property/test_collections.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9123 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/property/test_cross_version_persist.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11073 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/property/test_embeddings.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9062 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/property/test_filtering.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5146 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/property/test_persist.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.959593 smart_chromadb-0.1.dev733/chromadb/test/segment/
+-rw-r--r--   0 johnyan    (501) staff       (20)    15026 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/segment/test_metadata.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    12132 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/segment/test_vector.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    40340 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/test_api.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2234 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/test_chroma.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4127 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/test_config.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.960838 smart_chromadb-0.1.dev733/chromadb/test/utils/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3544 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/test/utils/test_messagid.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3702 2023-06-30 03:21:44.000000 smart_chromadb-0.1.dev733/chromadb/types.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.963212 smart_chromadb-0.1.dev733/chromadb/utils/
+-rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/utils/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    16311 2023-06-30 06:12:24.000000 smart_chromadb-0.1.dev733/chromadb/utils/embedding_functions.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2301 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/chromadb/utils/messageid.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.821744 smart_chromadb-0.1.dev733/clients/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.980560 smart_chromadb-0.1.dev733/clients/js/
+-rw-r--r--   0 johnyan    (501) staff       (20)       66 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/.gitignore
+-rw-r--r--   0 johnyan    (501) staff       (20)       32 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/.prettierignore
+-rw-r--r--   0 johnyan    (501) staff       (20)        3 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/.prettierrc.json
+-rw-r--r--   0 johnyan    (501) staff       (20)     1256 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/DEVELOP.md
+-rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/LICENSE
+-rw-r--r--   0 johnyan    (501) staff       (20)     1266 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)      324 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/config.yml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.820147 smart_chromadb-0.1.dev733/clients/js/examples/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.988642 smart_chromadb-0.1.dev733/clients/js/examples/browser/
+-rw-r--r--   0 johnyan    (501) staff       (20)      358 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/browser/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)     1787 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/browser/app.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      834 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/browser/index.html
+-rw-r--r--   0 johnyan    (501) staff       (20)      409 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/browser/package.json
+-rw-r--r--   0 johnyan    (501) staff       (20)    71072 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/browser/yarn.lock
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.995260 smart_chromadb-0.1.dev733/clients/js/examples/node/
+-rw-r--r--   0 johnyan    (501) staff       (20)       57 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/node/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)     1191 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/node/app.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    46542 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/node/package-lock.json
+-rw-r--r--   0 johnyan    (501) staff       (20)      503 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/node/package.json
+-rw-r--r--   0 johnyan    (501) staff       (20)    17116 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/examples/node/yarn.lock
+-rwxr-xr-x   0 johnyan    (501) staff       (20)     1075 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/genapi.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)      469 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/jest.config.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      153 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/openapitools.json
+-rw-r--r--   0 johnyan    (501) staff       (20)   450648 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/package-lock.json
+-rw-r--r--   0 johnyan    (501) staff       (20)     1455 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/package.json
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.002684 smart_chromadb-0.1.dev733/clients/js/src/
+-rw-r--r--   0 johnyan    (501) staff       (20)     8171 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/ChromaClient.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)    19403 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/Collection.ts
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.009777 smart_chromadb-0.1.dev733/clients/js/src/embeddings/
+-rw-r--r--   0 johnyan    (501) staff       (20)      938 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/embeddings/CohereEmbeddingFunction.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)       92 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/embeddings/IEmbeddingFunction.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1563 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2493 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
+-rwxr-xr-x   0 johnyan    (501) staff       (20)     3402 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.018984 smart_chromadb-0.1.dev733/clients/js/src/generated/
+-rw-r--r--   0 johnyan    (501) staff       (20)      921 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/generated/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)    56700 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/generated/api.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1478 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/generated/configuration.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      429 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/generated/index.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     5862 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/generated/models.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1307 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/generated/runtime.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      490 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/index.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1715 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/types.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2002 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/src/utils.ts
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.033037 smart_chromadb-0.1.dev733/clients/js/test/
+-rw-r--r--   0 johnyan    (501) staff       (20)     2625 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/add.collections.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     7586 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/client.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     3284 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/collection.client.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2551 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/data.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/delete.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2599 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/get.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      206 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/initClient.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      577 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/peek.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1990 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/query.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2160 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/update.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      802 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/test/upsert.collections.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      367 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/tsconfig.json
+-rw-r--r--   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/tsconfig.module.json
+-rw-r--r--   0 johnyan    (501) staff       (20)   157735 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/js/yarn.lock
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.040822 smart_chromadb-0.1.dev733/clients/python/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1627 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/python/README.md
+-rwxr-xr-x   0 johnyan    (501) staff       (20)     1257 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/python/build_python_thin_client.sh
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      826 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/python/integration-test.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)       22 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/python/is_thin_client.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1166 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/clients/python/pyproject.toml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.043344 smart_chromadb-0.1.dev733/config/
+-rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/config/backup_disk.xml
+-rw-r--r--   0 johnyan    (501) staff       (20)      233 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/config/chroma_users.xml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1080 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/docker-compose.server.example.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1221 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/docker-compose.test.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1226 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/docker-compose.yml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.046211 smart_chromadb-0.1.dev733/examples/
+-rw-r--r--   0 johnyan    (501) staff       (20)    10346 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/examples/alternative_embeddings.ipynb
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.822587 smart_chromadb-0.1.dev733/examples/deployments/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.052843 smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/
+-rw-r--r--   0 johnyan    (501) staff       (20)      611 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)      752 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/chroma.tf
+-rw-r--r--   0 johnyan    (501) staff       (20)      125 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/main.tf
+-rw-r--r--   0 johnyan    (501) staff       (20)     2271 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/startup.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)      181 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/variables.tf
+-rw-r--r--   0 johnyan    (501) staff       (20)     5830 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/examples/local_persistence.ipynb
+-rw-r--r--   0 johnyan    (501) staff       (20)     5493 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/examples/where_filtering.ipynb
+-rw-r--r--   0 johnyan    (501) staff       (20)      495 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/log_config.yml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:12.824657 smart_chromadb-0.1.dev733/migrations/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.054250 smart_chromadb-0.1.dev733/migrations/embeddings_queue/
+-rw-r--r--   0 johnyan    (501) staff       (20)      261 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/migrations/embeddings_queue/00001-embeddings.sqlite.sql
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.055369 smart_chromadb-0.1.dev733/migrations/metadb/
+-rw-r--r--   0 johnyan    (501) staff       (20)      620 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/migrations/metadb/00001-embedding-metadata.sqlite.sql
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.058329 smart_chromadb-0.1.dev733/migrations/sysdb/
+-rw-r--r--   0 johnyan    (501) staff       (20)      336 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/migrations/sysdb/00001-collections.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/migrations/sysdb/00002-segments.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)      372 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/pull_request_template.md
+-rw-r--r--   0 johnyan    (501) staff       (20)     1455 2023-06-26 07:09:55.000000 smart_chromadb-0.1.dev733/pyproject.toml
+-rw-r--r--   0 johnyan    (501) staff       (20)      352 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/requirements.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)      161 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev733/requirements_dev.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)       38 2023-07-05 01:00:13.066034 smart_chromadb-0.1.dev733/setup.cfg
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 01:00:13.063993 smart_chromadb-0.1.dev733/smart_chromadb.egg-info/
+-rw-r--r--   0 johnyan    (501) staff       (20)     6220 2023-07-05 01:00:12.000000 smart_chromadb-0.1.dev733/smart_chromadb.egg-info/PKG-INFO
+-rw-r--r--   0 johnyan    (501) staff       (20)     5825 2023-07-05 01:00:12.000000 smart_chromadb-0.1.dev733/smart_chromadb.egg-info/SOURCES.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)        1 2023-07-05 01:00:12.000000 smart_chromadb-0.1.dev733/smart_chromadb.egg-info/dependency_links.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)      340 2023-07-05 01:00:12.000000 smart_chromadb-0.1.dev733/smart_chromadb.egg-info/requires.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)        9 2023-07-05 01:00:12.000000 smart_chromadb-0.1.dev733/smart_chromadb.egg-info/top_level.txt
```

### Comparing `smart_chromadb-0.1.dev732/.github/ISSUE_TEMPLATE/bug_report.yaml` & `smart_chromadb-0.1.dev733/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/.github/ISSUE_TEMPLATE/feature_request.yaml` & `smart_chromadb-0.1.dev733/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/.github/ISSUE_TEMPLATE/installation_trouble.yaml` & `smart_chromadb-0.1.dev733/.github/ISSUE_TEMPLATE/installation_trouble.yaml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/.github/workflows/chroma-client-integration-test.yml` & `smart_chromadb-0.1.dev733/.github/workflows/chroma-client-integration-test.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/.github/workflows/chroma-integration-test.yml` & `smart_chromadb-0.1.dev733/.github/workflows/chroma-integration-test.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/.github/workflows/chroma-release-python-client.yml` & `smart_chromadb-0.1.dev733/.github/workflows/chroma-release-python-client.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/.github/workflows/chroma-release.yml` & `smart_chromadb-0.1.dev733/.github/workflows/chroma-release.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/.github/workflows/chroma-test.yml` & `smart_chromadb-0.1.dev733/.github/workflows/chroma-test.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/.github/workflows/pr-review-checklist.yml` & `smart_chromadb-0.1.dev733/.github/workflows/pr-review-checklist.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/.pre-commit-config.yaml` & `smart_chromadb-0.1.dev733/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/.vscode/settings.json` & `smart_chromadb-0.1.dev733/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/DEVELOP.md` & `smart_chromadb-0.1.dev733/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/Dockerfile` & `smart_chromadb-0.1.dev733/Dockerfile`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/LICENSE` & `smart_chromadb-0.1.dev733/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/PKG-INFO` & `smart_chromadb-0.1.dev733/smart_chromadb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: smart_chromadb
-Version: 0.1.dev732
+Name: smart-chromadb
+Version: 0.1.dev733
 Summary: Chroma.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smart_chromadb Version: 0.1.dev732 Summary: Chroma.
+Metadata-Version: 2.1 Name: smart-chromadb Version: 0.1.dev733 Summary: Chroma.
 Author-email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `smart_chromadb-0.1.dev732/README.md` & `smart_chromadb-0.1.dev733/README.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/RELEASE_PROCESS.md` & `smart_chromadb-0.1.dev733/RELEASE_PROCESS.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/bin/backup.sh` & `smart_chromadb-0.1.dev733/bin/backup.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/bin/generate_cloudformation.py` & `smart_chromadb-0.1.dev733/bin/generate_cloudformation.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/bin/restore.sh` & `smart_chromadb-0.1.dev733/bin/restore.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/bin/setup_linux.sh` & `smart_chromadb-0.1.dev733/bin/setup_linux.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/bin/templates/docker-compose.yml` & `smart_chromadb-0.1.dev733/bin/templates/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/__init__.py` & `smart_chromadb-0.1.dev733/chromadb/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/api/__init__.py` & `smart_chromadb-0.1.dev733/chromadb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/api/fastapi.py` & `smart_chromadb-0.1.dev733/chromadb/api/fastapi.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/api/local.py` & `smart_chromadb-0.1.dev733/chromadb/api/local.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/api/models/Collection.py` & `smart_chromadb-0.1.dev733/chromadb/api/models/Collection.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/api/smartapi.py` & `smart_chromadb-0.1.dev733/chromadb/api/smartapi.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/api/types.py` & `smart_chromadb-0.1.dev733/chromadb/api/types.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/config.py` & `smart_chromadb-0.1.dev733/chromadb/config.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/db/__init__.py` & `smart_chromadb-0.1.dev733/chromadb/db/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/db/base.py` & `smart_chromadb-0.1.dev733/chromadb/db/base.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/db/clickhouse.py` & `smart_chromadb-0.1.dev733/chromadb/db/clickhouse.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/db/duckdb.py` & `smart_chromadb-0.1.dev733/chromadb/db/duckdb.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/db/impl/sqlite.py` & `smart_chromadb-0.1.dev733/chromadb/db/impl/sqlite.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/db/index/hnswlib.py` & `smart_chromadb-0.1.dev733/chromadb/db/index/hnswlib.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/db/migrations.py` & `smart_chromadb-0.1.dev733/chromadb/db/migrations.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/db/mixins/embeddings_queue.py` & `smart_chromadb-0.1.dev733/chromadb/db/mixins/embeddings_queue.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/db/mixins/sysdb.py` & `smart_chromadb-0.1.dev733/chromadb/db/mixins/sysdb.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/db/smartdb.py` & `smart_chromadb-0.1.dev733/chromadb/db/smartdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,12 +414,12 @@
             where_document=where_document,
         )
         # 用自定义的方法, 需建表为字符串
         # sql = f"""SELECT document, CosineSimilarity(embedding, '{embeddings[0]}') as d FROM embeddings {where_str} order by d desc limit {n_results}"""
         # sql = f"""SELECT document, CosineSquaredL2(embedding, '{embeddings[0]}') as d FROM embeddings {where_str} order by d desc limit {n_results}"""
         import time
         start_time = time.time()
-        sql = f"""SELECT document, array_sum(array_map((x,y)->pow((x-y),2), embedding,{embeddings[0]})) as distance FROM embeddings {where_str} order by distance  limit {n_results}"""
+        sql = f"""SELECT document,metadata,array_sum(array_map((x,y)->pow((x-y),2), embedding,{embeddings[0]})) as distance FROM embeddings {where_str} order by distance  limit {n_results}"""
         val = self._execute_sql(sql)
         print('starrocks cost:', time.time() - start_time)
 
         return val
```

### Comparing `smart_chromadb-0.1.dev732/chromadb/db/system.py` & `smart_chromadb-0.1.dev733/chromadb/db/system.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/errors.py` & `smart_chromadb-0.1.dev733/chromadb/errors.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/ingest/__init__.py` & `smart_chromadb-0.1.dev733/chromadb/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/segment/__init__.py` & `smart_chromadb-0.1.dev733/chromadb/segment/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/segment/impl/manager/local.py` & `smart_chromadb-0.1.dev733/chromadb/segment/impl/manager/local.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/segment/impl/metadata/sqlite.py` & `smart_chromadb-0.1.dev733/chromadb/segment/impl/metadata/sqlite.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/segment/impl/vector/local_hnsw.py` & `smart_chromadb-0.1.dev733/chromadb/segment/impl/vector/local_hnsw.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/server/fastapi/__init__.py` & `smart_chromadb-0.1.dev733/chromadb/server/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/server/fastapi/types.py` & `smart_chromadb-0.1.dev733/chromadb/server/fastapi/types.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/telemetry/__init__.py` & `smart_chromadb-0.1.dev733/chromadb/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/telemetry/events.py` & `smart_chromadb-0.1.dev733/chromadb/telemetry/events.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/telemetry/posthog.py` & `smart_chromadb-0.1.dev733/chromadb/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/conftest.py` & `smart_chromadb-0.1.dev733/chromadb/test/conftest.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/db/test_base.py` & `smart_chromadb-0.1.dev733/chromadb/test/db/test_base.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/db/test_migrations.py` & `smart_chromadb-0.1.dev733/chromadb/test/db/test_migrations.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/db/test_system.py` & `smart_chromadb-0.1.dev733/chromadb/test/db/test_system.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/hnswlib/test_hnswlib.py` & `smart_chromadb-0.1.dev733/chromadb/test/hnswlib/test_hnswlib.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/ingest/test_producer_consumer.py` & `smart_chromadb-0.1.dev733/chromadb/test/ingest/test_producer_consumer.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/property/invariants.py` & `smart_chromadb-0.1.dev733/chromadb/test/property/invariants.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/property/strategies.py` & `smart_chromadb-0.1.dev733/chromadb/test/property/strategies.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/property/test_add.py` & `smart_chromadb-0.1.dev733/chromadb/test/property/test_add.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/property/test_collections.py` & `smart_chromadb-0.1.dev733/chromadb/test/property/test_collections.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/property/test_cross_version_persist.py` & `smart_chromadb-0.1.dev733/chromadb/test/property/test_cross_version_persist.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/property/test_embeddings.py` & `smart_chromadb-0.1.dev733/chromadb/test/property/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/property/test_filtering.py` & `smart_chromadb-0.1.dev733/chromadb/test/property/test_filtering.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/property/test_persist.py` & `smart_chromadb-0.1.dev733/chromadb/test/property/test_persist.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/segment/test_metadata.py` & `smart_chromadb-0.1.dev733/chromadb/test/segment/test_metadata.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/segment/test_vector.py` & `smart_chromadb-0.1.dev733/chromadb/test/segment/test_vector.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/test_api.py` & `smart_chromadb-0.1.dev733/chromadb/test/test_api.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/test_chroma.py` & `smart_chromadb-0.1.dev733/chromadb/test/test_chroma.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/test_config.py` & `smart_chromadb-0.1.dev733/chromadb/test/test_config.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/test/utils/test_messagid.py` & `smart_chromadb-0.1.dev733/chromadb/test/utils/test_messagid.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/types.py` & `smart_chromadb-0.1.dev733/chromadb/types.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/utils/embedding_functions.py` & `smart_chromadb-0.1.dev733/chromadb/utils/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/chromadb/utils/messageid.py` & `smart_chromadb-0.1.dev733/chromadb/utils/messageid.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/DEVELOP.md` & `smart_chromadb-0.1.dev733/clients/js/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/LICENSE` & `smart_chromadb-0.1.dev733/clients/js/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/README.md` & `smart_chromadb-0.1.dev733/clients/js/README.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/examples/browser/app.ts` & `smart_chromadb-0.1.dev733/clients/js/examples/browser/app.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/examples/browser/index.html` & `smart_chromadb-0.1.dev733/clients/js/examples/browser/index.html`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/examples/browser/yarn.lock` & `smart_chromadb-0.1.dev733/clients/js/examples/browser/yarn.lock`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/examples/node/app.js` & `smart_chromadb-0.1.dev733/clients/js/examples/node/app.js`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/examples/node/package-lock.json` & `smart_chromadb-0.1.dev733/clients/js/examples/node/package-lock.json`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/examples/node/yarn.lock` & `smart_chromadb-0.1.dev733/clients/js/examples/node/yarn.lock`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/genapi.sh` & `smart_chromadb-0.1.dev733/clients/js/genapi.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/package-lock.json` & `smart_chromadb-0.1.dev733/clients/js/package-lock.json`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/package.json` & `smart_chromadb-0.1.dev733/clients/js/package.json`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/src/ChromaClient.ts` & `smart_chromadb-0.1.dev733/clients/js/src/ChromaClient.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/src/Collection.ts` & `smart_chromadb-0.1.dev733/clients/js/src/Collection.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/src/embeddings/CohereEmbeddingFunction.ts` & `smart_chromadb-0.1.dev733/clients/js/src/embeddings/CohereEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts` & `smart_chromadb-0.1.dev733/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/src/embeddings/TransformersEmbeddingFunction.ts` & `smart_chromadb-0.1.dev733/clients/js/src/embeddings/TransformersEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/src/embeddings/WebAIEmbeddingFunction.ts` & `smart_chromadb-0.1.dev733/clients/js/src/embeddings/WebAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/src/generated/README.md` & `smart_chromadb-0.1.dev733/clients/js/src/generated/README.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/src/generated/api.ts` & `smart_chromadb-0.1.dev733/clients/js/src/generated/api.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/src/generated/configuration.ts` & `smart_chromadb-0.1.dev733/clients/js/src/generated/configuration.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/src/generated/models.ts` & `smart_chromadb-0.1.dev733/clients/js/src/generated/models.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/src/generated/runtime.ts` & `smart_chromadb-0.1.dev733/clients/js/src/generated/runtime.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/src/types.ts` & `smart_chromadb-0.1.dev733/clients/js/src/types.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/src/utils.ts` & `smart_chromadb-0.1.dev733/clients/js/src/utils.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/test/add.collections.test.ts` & `smart_chromadb-0.1.dev733/clients/js/test/add.collections.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/test/client.test.ts` & `smart_chromadb-0.1.dev733/clients/js/test/client.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/test/collection.client.test.ts` & `smart_chromadb-0.1.dev733/clients/js/test/collection.client.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/test/collection.test.ts` & `smart_chromadb-0.1.dev733/clients/js/test/collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/test/delete.collection.test.ts` & `smart_chromadb-0.1.dev733/clients/js/test/delete.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/test/get.collection.test.ts` & `smart_chromadb-0.1.dev733/clients/js/test/get.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/test/peek.collection.test.ts` & `smart_chromadb-0.1.dev733/clients/js/test/peek.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/test/query.collection.test.ts` & `smart_chromadb-0.1.dev733/clients/js/test/query.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/test/update.collection.test.ts` & `smart_chromadb-0.1.dev733/clients/js/test/update.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/test/upsert.collections.test.ts` & `smart_chromadb-0.1.dev733/clients/js/test/upsert.collections.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/js/yarn.lock` & `smart_chromadb-0.1.dev733/clients/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/python/README.md` & `smart_chromadb-0.1.dev733/clients/python/README.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/python/build_python_thin_client.sh` & `smart_chromadb-0.1.dev733/clients/python/build_python_thin_client.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/python/integration-test.sh` & `smart_chromadb-0.1.dev733/clients/python/integration-test.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/clients/python/pyproject.toml` & `smart_chromadb-0.1.dev733/clients/python/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/docker-compose.server.example.yml` & `smart_chromadb-0.1.dev733/docker-compose.server.example.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/docker-compose.test.yml` & `smart_chromadb-0.1.dev733/docker-compose.test.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/docker-compose.yml` & `smart_chromadb-0.1.dev733/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/examples/alternative_embeddings.ipynb` & `smart_chromadb-0.1.dev733/examples/alternative_embeddings.ipynb`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/README.md` & `smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/README.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/chroma.tf` & `smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/chroma.tf`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/startup.sh` & `smart_chromadb-0.1.dev733/examples/deployments/google-cloud-compute/startup.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/examples/local_persistence.ipynb` & `smart_chromadb-0.1.dev733/examples/local_persistence.ipynb`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/examples/where_filtering.ipynb` & `smart_chromadb-0.1.dev733/examples/where_filtering.ipynb`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/migrations/metadb/00001-embedding-metadata.sqlite.sql` & `smart_chromadb-0.1.dev733/migrations/metadb/00001-embedding-metadata.sqlite.sql`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/pyproject.toml` & `smart_chromadb-0.1.dev733/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev732/smart_chromadb.egg-info/PKG-INFO` & `smart_chromadb-0.1.dev733/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: smart-chromadb
-Version: 0.1.dev732
+Name: smart_chromadb
+Version: 0.1.dev733
 Summary: Chroma.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smart-chromadb Version: 0.1.dev732 Summary: Chroma.
+Metadata-Version: 2.1 Name: smart_chromadb Version: 0.1.dev733 Summary: Chroma.
 Author-email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `smart_chromadb-0.1.dev732/smart_chromadb.egg-info/SOURCES.txt` & `smart_chromadb-0.1.dev733/smart_chromadb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

