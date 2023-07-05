# Comparing `tmp/smart_chromadb-0.1.dev731.tar.gz` & `tmp/smart_chromadb-0.1.dev732.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/johnyan/Documents/project/chroma/dist/.tmp-5twmxy3t/smart_chromadb-0.1.dev731.tar", last modified: Wed Jun 28 02:16:30 2023, max compression
+gzip compressed data, was "/Users/johnyan/Documents/project/chroma/dist/.tmp-g3z0s293/smart_chromadb-0.1.dev732.tar", last modified: Wed Jul  5 00:31:23 2023, max compression
```

## Comparing `smart_chromadb-0.1.dev731.tar` & `smart_chromadb-0.1.dev732.tar`

### file list

```diff
@@ -1,232 +1,233 @@
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.796071 smart_chromadb-0.1.dev731/
--rw-r--r--   0 johnyan    (501) staff       (20)       84 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/.dockerignore
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.470589 smart_chromadb-0.1.dev731/.github/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.523072 smart_chromadb-0.1.dev731/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 johnyan    (501) staff       (20)     1512 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 johnyan    (501) staff       (20)     1520 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 johnyan    (501) staff       (20)     1384 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/.github/ISSUE_TEMPLATE/installation_trouble.yaml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.529232 smart_chromadb-0.1.dev731/.github/workflows/
--rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/.github/workflows/chroma-client-integration-test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1187 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/.github/workflows/chroma-integration-test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1338 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/.github/workflows/chroma-release-python-client.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     4169 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/.github/workflows/chroma-release.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1205 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/.github/workflows/chroma-test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1734 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/.github/workflows/pr-review-checklist.yml
--rw-r--r--   0 johnyan    (501) staff       (20)      228 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/.gitignore
--rw-r--r--   0 johnyan    (501) staff       (20)     1167 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/.pre-commit-config.yaml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.538612 smart_chromadb-0.1.dev731/.vscode/
--rw-r--r--   0 johnyan    (501) staff       (20)     1020 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/.vscode/settings.json
--rw-r--r--   0 johnyan    (501) staff       (20)     3323 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/DEVELOP.md
--rw-r--r--   0 johnyan    (501) staff       (20)      647 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/Dockerfile
--rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/LICENSE
--rw-r--r--   0 johnyan    (501) staff       (20)     6220 2023-06-28 02:16:30.794772 smart_chromadb-0.1.dev731/PKG-INFO
--rw-r--r--   0 johnyan    (501) staff       (20)     5679 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)      619 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/RELEASE_PROCESS.md
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.569257 smart_chromadb-0.1.dev731/bin/
--rw-r--r--   0 johnyan    (501) staff       (20)     1610 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/bin/backup.sh
--rwxr-xr-x   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/bin/build
--rwxr-xr-x   0 johnyan    (501) staff       (20)      234 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/bin/docker_entrypoint.sh
--rw-r--r--   0 johnyan    (501) staff       (20)     6462 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/bin/generate_cloudformation.py
--rwxr-xr-x   0 johnyan    (501) staff       (20)      463 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/bin/integration-test
--rw-r--r--   0 johnyan    (501) staff       (20)     1688 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/bin/restore.sh
--rw-r--r--   0 johnyan    (501) staff       (20)     1105 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/bin/setup_linux.sh
--rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/bin/setup_mac.sh
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.570366 smart_chromadb-0.1.dev731/bin/templates/
--rw-r--r--   0 johnyan    (501) staff       (20)      985 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/bin/templates/docker-compose.yml
--rwxr-xr-x   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/bin/test-package.sh
--rwxr-xr-x   0 johnyan    (501) staff       (20)      297 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/bin/test-remote
--rw-r--r--   0 johnyan    (501) staff       (20)      205 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/bin/test.py
--rwxr-xr-x   0 johnyan    (501) staff       (20)      151 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/bin/version
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.576052 smart_chromadb-0.1.dev731/chromadb/
--rw-r--r--   0 johnyan    (501) staff       (20)      894 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.581357 smart_chromadb-0.1.dev731/chromadb/api/
--rw-r--r--   0 johnyan    (501) staff       (20)    10898 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/api/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12480 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/api/fastapi.py
--rw-r--r--   0 johnyan    (501) staff       (20)    17852 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/api/local.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.582194 smart_chromadb-0.1.dev731/chromadb/api/models/
--rw-r--r--   0 johnyan    (501) staff       (20)    15103 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/api/models/Collection.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11270 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/api/types.py
--rw-r--r--   0 johnyan    (501) staff       (20)      168 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/app.py
--rw-r--r--   0 johnyan    (501) staff       (20)     7132 2023-06-28 01:41:06.000000 smart_chromadb-0.1.dev731/chromadb/config.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.591613 smart_chromadb-0.1.dev731/chromadb/db/
--rw-r--r--   0 johnyan    (501) staff       (20)     3390 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/db/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6004 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/db/base.py
--rw-r--r--   0 johnyan    (501) staff       (20)    22207 2023-06-28 02:00:02.000000 smart_chromadb-0.1.dev731/chromadb/db/clickhouse.py
--rw-r--r--   0 johnyan    (501) staff       (20)    18795 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/db/duckdb.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.594527 smart_chromadb-0.1.dev731/chromadb/db/impl/
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/db/impl/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6221 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/db/impl/sqlite.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.597174 smart_chromadb-0.1.dev731/chromadb/db/index/
--rw-r--r--   0 johnyan    (501) staff       (20)      447 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/db/index/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11060 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/db/index/hnswlib.py
--rw-r--r--   0 johnyan    (501) staff       (20)     8096 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/db/migrations.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.599335 smart_chromadb-0.1.dev731/chromadb/db/mixins/
--rw-r--r--   0 johnyan    (501) staff       (20)     9193 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/db/mixins/embeddings_queue.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15557 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/db/mixins/sysdb.py
--rw-r--r--   0 johnyan    (501) staff       (20)    15068 2023-06-28 02:02:16.000000 smart_chromadb-0.1.dev731/chromadb/db/smartdb.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2656 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/db/system.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1293 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/errors.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.600100 smart_chromadb-0.1.dev731/chromadb/ingest/
--rw-r--r--   0 johnyan    (501) staff       (20)     3643 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/ingest/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.601127 smart_chromadb-0.1.dev731/chromadb/segment/
--rw-r--r--   0 johnyan    (501) staff       (20)     3059 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/segment/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.473779 smart_chromadb-0.1.dev731/chromadb/segment/impl/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.601879 smart_chromadb-0.1.dev731/chromadb/segment/impl/manager/
--rw-r--r--   0 johnyan    (501) staff       (20)     4358 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/segment/impl/manager/local.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.602811 smart_chromadb-0.1.dev731/chromadb/segment/impl/metadata/
--rw-r--r--   0 johnyan    (501) staff       (20)    17879 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/segment/impl/metadata/sqlite.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.604308 smart_chromadb-0.1.dev731/chromadb/segment/impl/vector/
--rw-r--r--   0 johnyan    (501) staff       (20)    11965 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/segment/impl/vector/local_hnsw.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.605319 smart_chromadb-0.1.dev731/chromadb/server/
--rw-r--r--   0 johnyan    (501) staff       (20)      172 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/server/__init__.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.607364 smart_chromadb-0.1.dev731/chromadb/server/fastapi/
--rw-r--r--   0 johnyan    (501) staff       (20)     9064 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/server/fastapi/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2134 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/server/fastapi/types.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.611728 smart_chromadb-0.1.dev731/chromadb/telemetry/
--rw-r--r--   0 johnyan    (501) staff       (20)     3214 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/telemetry/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)      591 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/telemetry/events.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1161 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/telemetry/posthog.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.618221 smart_chromadb-0.1.dev731/chromadb/test/
--rw-r--r--   0 johnyan    (501) staff       (20)     3993 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/conftest.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.621227 smart_chromadb-0.1.dev731/chromadb/test/db/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.627370 smart_chromadb-0.1.dev731/chromadb/test/db/migrations/
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/db/migrations/00001-migration-1.psql.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/db/migrations/00002-migration-2.psql.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/db/migrations/00003-migration-3.psql.sql
--rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)     1168 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/db/test_base.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5026 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/db/test_migrations.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9773 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/db/test_system.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.628666 smart_chromadb-0.1.dev731/chromadb/test/hnswlib/
--rw-r--r--   0 johnyan    (501) staff       (20)     2337 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/hnswlib/test_hnswlib.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.630064 smart_chromadb-0.1.dev731/chromadb/test/ingest/
--rw-r--r--   0 johnyan    (501) staff       (20)     8117 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/ingest/test_producer_consumer.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.639135 smart_chromadb-0.1.dev731/chromadb/test/property/
--rw-r--r--   0 johnyan    (501) staff       (20)    11294 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/property/invariants.py
--rw-r--r--   0 johnyan    (501) staff       (20)    18662 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/property/strategies.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2213 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/property/test_add.py
--rw-r--r--   0 johnyan    (501) staff       (20)     6211 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/property/test_collections.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9123 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/property/test_cross_version_persist.py
--rw-r--r--   0 johnyan    (501) staff       (20)    11073 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/property/test_embeddings.py
--rw-r--r--   0 johnyan    (501) staff       (20)     9062 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/property/test_filtering.py
--rw-r--r--   0 johnyan    (501) staff       (20)     5146 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/property/test_persist.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.640957 smart_chromadb-0.1.dev731/chromadb/test/segment/
--rw-r--r--   0 johnyan    (501) staff       (20)    15026 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/segment/test_metadata.py
--rw-r--r--   0 johnyan    (501) staff       (20)    12132 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/segment/test_vector.py
--rw-r--r--   0 johnyan    (501) staff       (20)    40340 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/test_api.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2234 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/test_chroma.py
--rw-r--r--   0 johnyan    (501) staff       (20)     4127 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/test_config.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.641518 smart_chromadb-0.1.dev731/chromadb/test/utils/
--rw-r--r--   0 johnyan    (501) staff       (20)     3544 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/test/utils/test_messagid.py
--rw-r--r--   0 johnyan    (501) staff       (20)     3695 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/types.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.642592 smart_chromadb-0.1.dev731/chromadb/utils/
--rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/utils/__init__.py
--rw-r--r--   0 johnyan    (501) staff       (20)    16226 2023-06-28 02:15:34.000000 smart_chromadb-0.1.dev731/chromadb/utils/embedding_functions.py
--rw-r--r--   0 johnyan    (501) staff       (20)     2301 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/chromadb/utils/messageid.py
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.479513 smart_chromadb-0.1.dev731/clients/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.659745 smart_chromadb-0.1.dev731/clients/js/
--rw-r--r--   0 johnyan    (501) staff       (20)       66 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/.gitignore
--rw-r--r--   0 johnyan    (501) staff       (20)       32 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/.prettierignore
--rw-r--r--   0 johnyan    (501) staff       (20)        3 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/.prettierrc.json
--rw-r--r--   0 johnyan    (501) staff       (20)     1256 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/DEVELOP.md
--rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/LICENSE
--rw-r--r--   0 johnyan    (501) staff       (20)     1266 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)      324 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/config.yml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.478499 smart_chromadb-0.1.dev731/clients/js/examples/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.665893 smart_chromadb-0.1.dev731/clients/js/examples/browser/
--rw-r--r--   0 johnyan    (501) staff       (20)      358 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/examples/browser/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)     1787 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/examples/browser/app.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      834 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/examples/browser/index.html
--rw-r--r--   0 johnyan    (501) staff       (20)      409 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/examples/browser/package.json
--rw-r--r--   0 johnyan    (501) staff       (20)    71072 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/examples/browser/yarn.lock
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.670784 smart_chromadb-0.1.dev731/clients/js/examples/node/
--rw-r--r--   0 johnyan    (501) staff       (20)       57 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/examples/node/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)     1191 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/examples/node/app.js
--rw-r--r--   0 johnyan    (501) staff       (20)    46542 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/examples/node/package-lock.json
--rw-r--r--   0 johnyan    (501) staff       (20)      503 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/examples/node/package.json
--rw-r--r--   0 johnyan    (501) staff       (20)    17116 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/examples/node/yarn.lock
--rwxr-xr-x   0 johnyan    (501) staff       (20)     1075 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/genapi.sh
--rw-r--r--   0 johnyan    (501) staff       (20)      469 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/jest.config.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      153 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/openapitools.json
--rw-r--r--   0 johnyan    (501) staff       (20)   450648 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/package-lock.json
--rw-r--r--   0 johnyan    (501) staff       (20)     1455 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/package.json
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.676257 smart_chromadb-0.1.dev731/clients/js/src/
--rw-r--r--   0 johnyan    (501) staff       (20)     8171 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/src/ChromaClient.ts
--rw-r--r--   0 johnyan    (501) staff       (20)    19403 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/src/Collection.ts
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.682933 smart_chromadb-0.1.dev731/clients/js/src/embeddings/
--rw-r--r--   0 johnyan    (501) staff       (20)      938 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/src/embeddings/CohereEmbeddingFunction.ts
--rw-r--r--   0 johnyan    (501) staff       (20)       92 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/src/embeddings/IEmbeddingFunction.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1563 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2493 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
--rwxr-xr-x   0 johnyan    (501) staff       (20)     3402 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.688490 smart_chromadb-0.1.dev731/clients/js/src/generated/
--rw-r--r--   0 johnyan    (501) staff       (20)      921 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/src/generated/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)    56700 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/src/generated/api.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1478 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/src/generated/configuration.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      429 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/src/generated/index.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     5862 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/src/generated/models.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1307 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/src/generated/runtime.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      490 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/src/index.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1715 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/src/types.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2002 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/src/utils.ts
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.702600 smart_chromadb-0.1.dev731/clients/js/test/
--rw-r--r--   0 johnyan    (501) staff       (20)     2625 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/test/add.collections.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     7586 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/test/client.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     3284 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/test/collection.client.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2551 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/test/collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/test/data.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/test/delete.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2599 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/test/get.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      206 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/test/initClient.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      577 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/test/peek.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     1990 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/test/query.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)     2160 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/test/update.collection.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      802 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/test/upsert.collections.test.ts
--rw-r--r--   0 johnyan    (501) staff       (20)      367 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/tsconfig.json
--rw-r--r--   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/tsconfig.module.json
--rw-r--r--   0 johnyan    (501) staff       (20)   157735 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/js/yarn.lock
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.708974 smart_chromadb-0.1.dev731/clients/python/
--rw-r--r--   0 johnyan    (501) staff       (20)     1627 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/python/README.md
--rwxr-xr-x   0 johnyan    (501) staff       (20)     1257 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/python/build_python_thin_client.sh
--rwxr-xr-x   0 johnyan    (501) staff       (20)      826 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/python/integration-test.sh
--rw-r--r--   0 johnyan    (501) staff       (20)       22 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/python/is_thin_client.py
--rw-r--r--   0 johnyan    (501) staff       (20)     1166 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/clients/python/pyproject.toml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.711104 smart_chromadb-0.1.dev731/config/
--rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/config/backup_disk.xml
--rw-r--r--   0 johnyan    (501) staff       (20)      233 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/config/chroma_users.xml
--rw-r--r--   0 johnyan    (501) staff       (20)     1080 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/docker-compose.server.example.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1221 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/docker-compose.test.yml
--rw-r--r--   0 johnyan    (501) staff       (20)     1226 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/docker-compose.yml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.714801 smart_chromadb-0.1.dev731/examples/
--rw-r--r--   0 johnyan    (501) staff       (20)    10346 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/examples/alternative_embeddings.ipynb
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.480192 smart_chromadb-0.1.dev731/examples/deployments/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.749932 smart_chromadb-0.1.dev731/examples/deployments/google-cloud-compute/
--rw-r--r--   0 johnyan    (501) staff       (20)      611 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/examples/deployments/google-cloud-compute/README.md
--rw-r--r--   0 johnyan    (501) staff       (20)      752 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/examples/deployments/google-cloud-compute/chroma.tf
--rw-r--r--   0 johnyan    (501) staff       (20)      125 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/examples/deployments/google-cloud-compute/main.tf
--rw-r--r--   0 johnyan    (501) staff       (20)     2271 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/examples/deployments/google-cloud-compute/startup.sh
--rw-r--r--   0 johnyan    (501) staff       (20)      181 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/examples/deployments/google-cloud-compute/variables.tf
--rw-r--r--   0 johnyan    (501) staff       (20)     5830 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/examples/local_persistence.ipynb
--rw-r--r--   0 johnyan    (501) staff       (20)     5493 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/examples/where_filtering.ipynb
--rw-r--r--   0 johnyan    (501) staff       (20)      495 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/log_config.yml
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.481329 smart_chromadb-0.1.dev731/migrations/
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.771082 smart_chromadb-0.1.dev731/migrations/embeddings_queue/
--rw-r--r--   0 johnyan    (501) staff       (20)      261 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/migrations/embeddings_queue/00001-embeddings.sqlite.sql
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.781124 smart_chromadb-0.1.dev731/migrations/metadb/
--rw-r--r--   0 johnyan    (501) staff       (20)      620 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/migrations/metadb/00001-embedding-metadata.sqlite.sql
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.785112 smart_chromadb-0.1.dev731/migrations/sysdb/
--rw-r--r--   0 johnyan    (501) staff       (20)      336 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/migrations/sysdb/00001-collections.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/migrations/sysdb/00002-segments.sqlite.sql
--rw-r--r--   0 johnyan    (501) staff       (20)      372 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/pull_request_template.md
--rw-r--r--   0 johnyan    (501) staff       (20)     1455 2023-06-26 07:09:55.000000 smart_chromadb-0.1.dev731/pyproject.toml
--rw-r--r--   0 johnyan    (501) staff       (20)      352 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/requirements.txt
--rw-r--r--   0 johnyan    (501) staff       (20)      161 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev731/requirements_dev.txt
--rw-r--r--   0 johnyan    (501) staff       (20)       38 2023-06-28 02:16:30.796512 smart_chromadb-0.1.dev731/setup.cfg
-drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-06-28 02:16:30.793679 smart_chromadb-0.1.dev731/smart_chromadb.egg-info/
--rw-r--r--   0 johnyan    (501) staff       (20)     6220 2023-06-28 02:16:30.000000 smart_chromadb-0.1.dev731/smart_chromadb.egg-info/PKG-INFO
--rw-r--r--   0 johnyan    (501) staff       (20)     5800 2023-06-28 02:16:30.000000 smart_chromadb-0.1.dev731/smart_chromadb.egg-info/SOURCES.txt
--rw-r--r--   0 johnyan    (501) staff       (20)        1 2023-06-28 02:16:30.000000 smart_chromadb-0.1.dev731/smart_chromadb.egg-info/dependency_links.txt
--rw-r--r--   0 johnyan    (501) staff       (20)      340 2023-06-28 02:16:30.000000 smart_chromadb-0.1.dev731/smart_chromadb.egg-info/requires.txt
--rw-r--r--   0 johnyan    (501) staff       (20)        9 2023-06-28 02:16:30.000000 smart_chromadb-0.1.dev731/smart_chromadb.egg-info/top_level.txt
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:23.006915 smart_chromadb-0.1.dev732/
+-rw-r--r--   0 johnyan    (501) staff       (20)       84 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.dockerignore
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.747999 smart_chromadb-0.1.dev732/.github/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.788118 smart_chromadb-0.1.dev732/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1512 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1520 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1384 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/ISSUE_TEMPLATE/installation_trouble.yaml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.795950 smart_chromadb-0.1.dev732/.github/workflows/
+-rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/workflows/chroma-client-integration-test.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1187 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/workflows/chroma-integration-test.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1338 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/workflows/chroma-release-python-client.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     4169 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/workflows/chroma-release.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1205 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/workflows/chroma-test.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1734 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.github/workflows/pr-review-checklist.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)      228 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.gitignore
+-rw-r--r--   0 johnyan    (501) staff       (20)     1167 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.pre-commit-config.yaml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.797329 smart_chromadb-0.1.dev732/.vscode/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1020 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/.vscode/settings.json
+-rw-r--r--   0 johnyan    (501) staff       (20)     3323 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/DEVELOP.md
+-rw-r--r--   0 johnyan    (501) staff       (20)      647 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/Dockerfile
+-rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/LICENSE
+-rw-r--r--   0 johnyan    (501) staff       (20)     6220 2023-07-05 00:31:23.006133 smart_chromadb-0.1.dev732/PKG-INFO
+-rw-r--r--   0 johnyan    (501) staff       (20)     5679 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)      619 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/RELEASE_PROCESS.md
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.813519 smart_chromadb-0.1.dev732/bin/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1610 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/backup.sh
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/build
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      234 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/docker_entrypoint.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)     6462 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/generate_cloudformation.py
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      463 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/integration-test
+-rw-r--r--   0 johnyan    (501) staff       (20)     1688 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/restore.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)     1105 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/setup_linux.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/setup_mac.sh
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.814539 smart_chromadb-0.1.dev732/bin/templates/
+-rw-r--r--   0 johnyan    (501) staff       (20)      985 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/templates/docker-compose.yml
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/test-package.sh
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      297 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/test-remote
+-rw-r--r--   0 johnyan    (501) staff       (20)      205 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/test.py
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      151 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/bin/version
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.821079 smart_chromadb-0.1.dev732/chromadb/
+-rw-r--r--   0 johnyan    (501) staff       (20)      894 2023-07-04 08:34:52.000000 smart_chromadb-0.1.dev732/chromadb/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.827730 smart_chromadb-0.1.dev732/chromadb/api/
+-rw-r--r--   0 johnyan    (501) staff       (20)    10898 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/api/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    12480 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/api/fastapi.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    17852 2023-07-03 08:25:25.000000 smart_chromadb-0.1.dev732/chromadb/api/local.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.828565 smart_chromadb-0.1.dev732/chromadb/api/models/
+-rw-r--r--   0 johnyan    (501) staff       (20)    15103 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/api/models/Collection.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      819 2023-07-03 07:56:58.000000 smart_chromadb-0.1.dev732/chromadb/api/smartapi.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11283 2023-07-03 09:25:09.000000 smart_chromadb-0.1.dev732/chromadb/api/types.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      168 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/app.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     7231 2023-07-03 08:16:05.000000 smart_chromadb-0.1.dev732/chromadb/config.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.837348 smart_chromadb-0.1.dev732/chromadb/db/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3390 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6004 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/base.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    22307 2023-07-03 08:25:52.000000 smart_chromadb-0.1.dev732/chromadb/db/clickhouse.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    18795 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/duckdb.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.840369 smart_chromadb-0.1.dev732/chromadb/db/impl/
+-rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/impl/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6221 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/impl/sqlite.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.842981 smart_chromadb-0.1.dev732/chromadb/db/index/
+-rw-r--r--   0 johnyan    (501) staff       (20)      447 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/index/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11060 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/index/hnswlib.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     8096 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/migrations.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.845517 smart_chromadb-0.1.dev732/chromadb/db/mixins/
+-rw-r--r--   0 johnyan    (501) staff       (20)     9193 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/mixins/embeddings_queue.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    15557 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/mixins/sysdb.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    16619 2023-07-04 09:55:11.000000 smart_chromadb-0.1.dev732/chromadb/db/smartdb.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2656 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/db/system.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1293 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/errors.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.846654 smart_chromadb-0.1.dev732/chromadb/ingest/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3643 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/ingest/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.849734 smart_chromadb-0.1.dev732/chromadb/segment/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3059 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/segment/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.753169 smart_chromadb-0.1.dev732/chromadb/segment/impl/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.851893 smart_chromadb-0.1.dev732/chromadb/segment/impl/manager/
+-rw-r--r--   0 johnyan    (501) staff       (20)     4358 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/segment/impl/manager/local.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.853044 smart_chromadb-0.1.dev732/chromadb/segment/impl/metadata/
+-rw-r--r--   0 johnyan    (501) staff       (20)    17879 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/segment/impl/metadata/sqlite.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.854194 smart_chromadb-0.1.dev732/chromadb/segment/impl/vector/
+-rw-r--r--   0 johnyan    (501) staff       (20)    11965 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/segment/impl/vector/local_hnsw.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.855059 smart_chromadb-0.1.dev732/chromadb/server/
+-rw-r--r--   0 johnyan    (501) staff       (20)      172 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/server/__init__.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.857413 smart_chromadb-0.1.dev732/chromadb/server/fastapi/
+-rw-r--r--   0 johnyan    (501) staff       (20)     9064 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/server/fastapi/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2134 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/server/fastapi/types.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.862695 smart_chromadb-0.1.dev732/chromadb/telemetry/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3214 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/telemetry/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)      591 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/telemetry/events.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1161 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/telemetry/posthog.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.868115 smart_chromadb-0.1.dev732/chromadb/test/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3993 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/conftest.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.871547 smart_chromadb-0.1.dev732/chromadb/test/db/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.877841 smart_chromadb-0.1.dev732/chromadb/test/db/migrations/
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/migrations/00001-migration-1.psql.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/migrations/00002-migration-2.psql.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/migrations/00003-migration-3.psql.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)       51 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)     1168 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/test_base.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5026 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/test_migrations.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9773 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/db/test_system.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.878866 smart_chromadb-0.1.dev732/chromadb/test/hnswlib/
+-rw-r--r--   0 johnyan    (501) staff       (20)     2337 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/hnswlib/test_hnswlib.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.880568 smart_chromadb-0.1.dev732/chromadb/test/ingest/
+-rw-r--r--   0 johnyan    (501) staff       (20)     8117 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/ingest/test_producer_consumer.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.890321 smart_chromadb-0.1.dev732/chromadb/test/property/
+-rw-r--r--   0 johnyan    (501) staff       (20)    11294 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/property/invariants.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    18662 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/property/strategies.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2213 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/property/test_add.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     6211 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/property/test_collections.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9123 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/property/test_cross_version_persist.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    11073 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/property/test_embeddings.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     9062 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/property/test_filtering.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     5146 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/property/test_persist.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.893849 smart_chromadb-0.1.dev732/chromadb/test/segment/
+-rw-r--r--   0 johnyan    (501) staff       (20)    15026 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/segment/test_metadata.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    12132 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/segment/test_vector.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    40340 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/test_api.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2234 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/test_chroma.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     4127 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/test_config.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.895346 smart_chromadb-0.1.dev732/chromadb/test/utils/
+-rw-r--r--   0 johnyan    (501) staff       (20)     3544 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/test/utils/test_messagid.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     3702 2023-06-30 03:21:44.000000 smart_chromadb-0.1.dev732/chromadb/types.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.897254 smart_chromadb-0.1.dev732/chromadb/utils/
+-rw-r--r--   0 johnyan    (501) staff       (20)        0 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/utils/__init__.py
+-rw-r--r--   0 johnyan    (501) staff       (20)    16311 2023-06-30 06:12:24.000000 smart_chromadb-0.1.dev732/chromadb/utils/embedding_functions.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     2301 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/chromadb/utils/messageid.py
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.763949 smart_chromadb-0.1.dev732/clients/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.917463 smart_chromadb-0.1.dev732/clients/js/
+-rw-r--r--   0 johnyan    (501) staff       (20)       66 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/.gitignore
+-rw-r--r--   0 johnyan    (501) staff       (20)       32 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/.prettierignore
+-rw-r--r--   0 johnyan    (501) staff       (20)        3 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/.prettierrc.json
+-rw-r--r--   0 johnyan    (501) staff       (20)     1256 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/DEVELOP.md
+-rw-r--r--   0 johnyan    (501) staff       (20)    11357 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/LICENSE
+-rw-r--r--   0 johnyan    (501) staff       (20)     1266 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)      324 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/config.yml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.762288 smart_chromadb-0.1.dev732/clients/js/examples/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.925135 smart_chromadb-0.1.dev732/clients/js/examples/browser/
+-rw-r--r--   0 johnyan    (501) staff       (20)      358 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/browser/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)     1787 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/browser/app.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      834 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/browser/index.html
+-rw-r--r--   0 johnyan    (501) staff       (20)      409 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/browser/package.json
+-rw-r--r--   0 johnyan    (501) staff       (20)    71072 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/browser/yarn.lock
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.932932 smart_chromadb-0.1.dev732/clients/js/examples/node/
+-rw-r--r--   0 johnyan    (501) staff       (20)       57 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/node/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)     1191 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/node/app.js
+-rw-r--r--   0 johnyan    (501) staff       (20)    46542 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/node/package-lock.json
+-rw-r--r--   0 johnyan    (501) staff       (20)      503 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/node/package.json
+-rw-r--r--   0 johnyan    (501) staff       (20)    17116 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/examples/node/yarn.lock
+-rwxr-xr-x   0 johnyan    (501) staff       (20)     1075 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/genapi.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)      469 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/jest.config.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      153 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/openapitools.json
+-rw-r--r--   0 johnyan    (501) staff       (20)   450648 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/package-lock.json
+-rw-r--r--   0 johnyan    (501) staff       (20)     1455 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/package.json
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.940660 smart_chromadb-0.1.dev732/clients/js/src/
+-rw-r--r--   0 johnyan    (501) staff       (20)     8171 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/ChromaClient.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)    19403 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/Collection.ts
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.947473 smart_chromadb-0.1.dev732/clients/js/src/embeddings/
+-rw-r--r--   0 johnyan    (501) staff       (20)      938 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/embeddings/CohereEmbeddingFunction.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)       92 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/embeddings/IEmbeddingFunction.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1563 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2493 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
+-rwxr-xr-x   0 johnyan    (501) staff       (20)     3402 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.956820 smart_chromadb-0.1.dev732/clients/js/src/generated/
+-rw-r--r--   0 johnyan    (501) staff       (20)      921 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/generated/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)    56700 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/generated/api.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1478 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/generated/configuration.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      429 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/generated/index.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     5862 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/generated/models.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1307 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/generated/runtime.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      490 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/index.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1715 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/types.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2002 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/src/utils.ts
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.973560 smart_chromadb-0.1.dev732/clients/js/test/
+-rw-r--r--   0 johnyan    (501) staff       (20)     2625 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/add.collections.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     7586 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/client.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     3284 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/collection.client.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2551 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      451 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/data.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      711 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/delete.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2599 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/get.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      206 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/initClient.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      577 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/peek.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     1990 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/query.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)     2160 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/update.collection.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      802 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/test/upsert.collections.test.ts
+-rw-r--r--   0 johnyan    (501) staff       (20)      367 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/tsconfig.json
+-rw-r--r--   0 johnyan    (501) staff       (20)      110 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/tsconfig.module.json
+-rw-r--r--   0 johnyan    (501) staff       (20)   157735 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/js/yarn.lock
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.980263 smart_chromadb-0.1.dev732/clients/python/
+-rw-r--r--   0 johnyan    (501) staff       (20)     1627 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/python/README.md
+-rwxr-xr-x   0 johnyan    (501) staff       (20)     1257 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/python/build_python_thin_client.sh
+-rwxr-xr-x   0 johnyan    (501) staff       (20)      826 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/python/integration-test.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)       22 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/python/is_thin_client.py
+-rw-r--r--   0 johnyan    (501) staff       (20)     1166 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/clients/python/pyproject.toml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.983249 smart_chromadb-0.1.dev732/config/
+-rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/config/backup_disk.xml
+-rw-r--r--   0 johnyan    (501) staff       (20)      233 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/config/chroma_users.xml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1080 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/docker-compose.server.example.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1221 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/docker-compose.test.yml
+-rw-r--r--   0 johnyan    (501) staff       (20)     1226 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/docker-compose.yml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.986097 smart_chromadb-0.1.dev732/examples/
+-rw-r--r--   0 johnyan    (501) staff       (20)    10346 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/examples/alternative_embeddings.ipynb
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.765338 smart_chromadb-0.1.dev732/examples/deployments/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.993631 smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/
+-rw-r--r--   0 johnyan    (501) staff       (20)      611 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/README.md
+-rw-r--r--   0 johnyan    (501) staff       (20)      752 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/chroma.tf
+-rw-r--r--   0 johnyan    (501) staff       (20)      125 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/main.tf
+-rw-r--r--   0 johnyan    (501) staff       (20)     2271 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/startup.sh
+-rw-r--r--   0 johnyan    (501) staff       (20)      181 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/variables.tf
+-rw-r--r--   0 johnyan    (501) staff       (20)     5830 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/examples/local_persistence.ipynb
+-rw-r--r--   0 johnyan    (501) staff       (20)     5493 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/examples/where_filtering.ipynb
+-rw-r--r--   0 johnyan    (501) staff       (20)      495 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/log_config.yml
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.766614 smart_chromadb-0.1.dev732/migrations/
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.994820 smart_chromadb-0.1.dev732/migrations/embeddings_queue/
+-rw-r--r--   0 johnyan    (501) staff       (20)      261 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/migrations/embeddings_queue/00001-embeddings.sqlite.sql
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.996007 smart_chromadb-0.1.dev732/migrations/metadb/
+-rw-r--r--   0 johnyan    (501) staff       (20)      620 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/migrations/metadb/00001-embedding-metadata.sqlite.sql
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:22.998389 smart_chromadb-0.1.dev732/migrations/sysdb/
+-rw-r--r--   0 johnyan    (501) staff       (20)      336 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/migrations/sysdb/00001-collections.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)      385 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/migrations/sysdb/00002-segments.sqlite.sql
+-rw-r--r--   0 johnyan    (501) staff       (20)      372 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/pull_request_template.md
+-rw-r--r--   0 johnyan    (501) staff       (20)     1455 2023-06-26 07:09:55.000000 smart_chromadb-0.1.dev732/pyproject.toml
+-rw-r--r--   0 johnyan    (501) staff       (20)      352 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/requirements.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)      161 2023-06-25 09:21:06.000000 smart_chromadb-0.1.dev732/requirements_dev.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)       38 2023-07-05 00:31:23.007148 smart_chromadb-0.1.dev732/setup.cfg
+drwxr-xr-x   0 johnyan    (501) staff       (20)        0 2023-07-05 00:31:23.005192 smart_chromadb-0.1.dev732/smart_chromadb.egg-info/
+-rw-r--r--   0 johnyan    (501) staff       (20)     6220 2023-07-05 00:31:22.000000 smart_chromadb-0.1.dev732/smart_chromadb.egg-info/PKG-INFO
+-rw-r--r--   0 johnyan    (501) staff       (20)     5825 2023-07-05 00:31:22.000000 smart_chromadb-0.1.dev732/smart_chromadb.egg-info/SOURCES.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)        1 2023-07-05 00:31:22.000000 smart_chromadb-0.1.dev732/smart_chromadb.egg-info/dependency_links.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)      340 2023-07-05 00:31:22.000000 smart_chromadb-0.1.dev732/smart_chromadb.egg-info/requires.txt
+-rw-r--r--   0 johnyan    (501) staff       (20)        9 2023-07-05 00:31:22.000000 smart_chromadb-0.1.dev732/smart_chromadb.egg-info/top_level.txt
```

### Comparing `smart_chromadb-0.1.dev731/.github/ISSUE_TEMPLATE/bug_report.yaml` & `smart_chromadb-0.1.dev732/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/.github/ISSUE_TEMPLATE/feature_request.yaml` & `smart_chromadb-0.1.dev732/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/.github/ISSUE_TEMPLATE/installation_trouble.yaml` & `smart_chromadb-0.1.dev732/.github/ISSUE_TEMPLATE/installation_trouble.yaml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/.github/workflows/chroma-client-integration-test.yml` & `smart_chromadb-0.1.dev732/.github/workflows/chroma-client-integration-test.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/.github/workflows/chroma-integration-test.yml` & `smart_chromadb-0.1.dev732/.github/workflows/chroma-integration-test.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/.github/workflows/chroma-release-python-client.yml` & `smart_chromadb-0.1.dev732/.github/workflows/chroma-release-python-client.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/.github/workflows/chroma-release.yml` & `smart_chromadb-0.1.dev732/.github/workflows/chroma-release.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/.github/workflows/chroma-test.yml` & `smart_chromadb-0.1.dev732/.github/workflows/chroma-test.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/.github/workflows/pr-review-checklist.yml` & `smart_chromadb-0.1.dev732/.github/workflows/pr-review-checklist.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/.pre-commit-config.yaml` & `smart_chromadb-0.1.dev732/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/.vscode/settings.json` & `smart_chromadb-0.1.dev732/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/DEVELOP.md` & `smart_chromadb-0.1.dev732/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/Dockerfile` & `smart_chromadb-0.1.dev732/Dockerfile`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/LICENSE` & `smart_chromadb-0.1.dev732/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/PKG-INFO` & `smart_chromadb-0.1.dev732/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart_chromadb
-Version: 0.1.dev731
+Version: 0.1.dev732
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
-Metadata-Version: 2.1 Name: smart_chromadb Version: 0.1.dev731 Summary: Chroma.
+Metadata-Version: 2.1 Name: smart_chromadb Version: 0.1.dev732 Summary: Chroma.
 Author-email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `smart_chromadb-0.1.dev731/README.md` & `smart_chromadb-0.1.dev732/README.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/RELEASE_PROCESS.md` & `smart_chromadb-0.1.dev732/RELEASE_PROCESS.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/bin/backup.sh` & `smart_chromadb-0.1.dev732/bin/backup.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/bin/generate_cloudformation.py` & `smart_chromadb-0.1.dev732/bin/generate_cloudformation.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/bin/restore.sh` & `smart_chromadb-0.1.dev732/bin/restore.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/bin/setup_linux.sh` & `smart_chromadb-0.1.dev732/bin/setup_linux.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/bin/templates/docker-compose.yml` & `smart_chromadb-0.1.dev732/bin/templates/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/__init__.py` & `smart_chromadb-0.1.dev732/chromadb/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/api/__init__.py` & `smart_chromadb-0.1.dev732/chromadb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/api/fastapi.py` & `smart_chromadb-0.1.dev732/chromadb/api/fastapi.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/api/local.py` & `smart_chromadb-0.1.dev732/chromadb/api/local.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/api/models/Collection.py` & `smart_chromadb-0.1.dev732/chromadb/api/models/Collection.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/api/types.py` & `smart_chromadb-0.1.dev732/chromadb/api/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         raise ValueError(f"Expected where to have exactly one operator, got {where}")
     for key, value in where.items():
         if not isinstance(key, str):
             raise ValueError(f"Expected where key to be a str, got {key}")
         if (
             key != "$and"
             and key != "$or"
-            and not isinstance(value, (str, int, float, dict))
+            and not isinstance(value, (str, int, float, dict, tuple, list))
         ):
             raise ValueError(
                 f"Expected where value to be a str, int, float, or operator expression, got {value}"
             )
         if key == "$and" or key == "$or":
             if not isinstance(value, list):
                 raise ValueError(
```

### Comparing `smart_chromadb-0.1.dev731/chromadb/config.py` & `smart_chromadb-0.1.dev732/chromadb/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 _legacy_config_values = {
     "duckdb": "chromadb.db.duckdb.DuckDB",
     "duckdb+parquet": "chromadb.db.duckdb.PersistentDuckDB",
     "clickhouse": "chromadb.db.clickhouse.Clickhouse",
     "rest": "chromadb.api.fastapi.FastAPI",
     "local": "chromadb.api.local.LocalAPI",
+    "smart": "chromadb.api.smartapi.SmartAPI",
     "starrocksdb": "chromadb.db.smartdb.StarRocksDB",
 }
 
 # TODO: Don't use concrete types here to avoid circular deps. Strings are fine for right here!
 _abstract_type_keys: Dict[str, str] = {
     "chromadb.db.DB": "chroma_db_impl",
     "chromadb.api.API": "chroma_api_impl",
@@ -50,14 +51,15 @@
     chroma_consumer_impl: str = "chromadb.db.impl.sqlite.SqliteDB"
 
     clickhouse_host: Optional[str] = None
     clickhouse_port: Optional[str] = None
 
     persist_directory: str = ".chroma"
 
+    # smartdb host, port, user, password, load_host
     db_config: dict = None
 
     chroma_server_host: Optional[str] = None
     chroma_server_http_port: Optional[str] = None
     chroma_server_ssl_enabled: Optional[bool] = False
     chroma_server_grpc_port: Optional[str] = None
     chroma_server_cors_allow_origins: List[str] = []  # eg ["http://localhost:3000"]
```

### Comparing `smart_chromadb-0.1.dev731/chromadb/db/__init__.py` & `smart_chromadb-0.1.dev732/chromadb/db/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/db/base.py` & `smart_chromadb-0.1.dev732/chromadb/db/base.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/db/clickhouse.py` & `smart_chromadb-0.1.dev732/chromadb/db/clickhouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,17 +122,15 @@
         raise NotImplementedError(
             "Clickhouse is a persistent database, this method is not needed"
         )
 
     @override
     def get_collection_uuid_from_name(self, collection_name: str) -> UUID:
         res = self._get_conn().query(
-            f"""
-            SELECT uuid FROM collections WHERE name = '{collection_name}'
-        """
+            f"""SELECT uuid FROM collections WHERE name = '{collection_name}'"""
         )
         return res.result_rows[0][0]
 
     def _create_where_clause(
         self,
         collection_uuid: str,
         ids: Optional[List[str]] = None,
@@ -444,14 +442,16 @@
                     all_subresults.append(subresults[0])
                 if key == "$or":
                     result.append(f"({' OR '.join(all_subresults)})")
                 elif key == "$and":
                     result.append(f"({' AND '.join(all_subresults)})")
                 else:
                     raise ValueError(f"Expected one of $or, $and, got {key}")
+            elif type(value) == tuple:
+                result.append(f" JSONExtractString(metadata,'{key}') in {value} ")
 
     def _format_where_document(self, where_document, results):
         operator = list(where_document.keys())[0]
         if operator == "$contains":
             results.append(f"position(document, '{where_document[operator]}') > 0")
         elif operator == "$and" or operator == "$or":
             all_subresults = []
```

### Comparing `smart_chromadb-0.1.dev731/chromadb/db/duckdb.py` & `smart_chromadb-0.1.dev732/chromadb/db/duckdb.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/db/impl/sqlite.py` & `smart_chromadb-0.1.dev732/chromadb/db/impl/sqlite.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/db/index/hnswlib.py` & `smart_chromadb-0.1.dev732/chromadb/db/index/hnswlib.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/db/migrations.py` & `smart_chromadb-0.1.dev732/chromadb/db/migrations.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/db/mixins/embeddings_queue.py` & `smart_chromadb-0.1.dev732/chromadb/db/mixins/embeddings_queue.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/db/mixins/sysdb.py` & `smart_chromadb-0.1.dev732/chromadb/db/mixins/sysdb.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/db/smartdb.py` & `smart_chromadb-0.1.dev732/chromadb/db/smartdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # type: ignore
 from chromadb.config import System
 from chromadb.api.types import Documents, Embeddings, IDs, Metadatas
 from chromadb.db.clickhouse import (
     Clickhouse,
-    db_schema_to_keys,
+    db_schema_to_keys, Where, WhereDocument, cast
 )
 from typing import List, Optional, Sequence
 import pandas as pd
 import json
 import uuid
 import logging
 from uuid import UUID
@@ -24,23 +24,24 @@
     def __init__(self, system: System):
         self._conn = DB_conn()
         self._settings = system.settings
         self._settings.require("db_config")
         connect_dict = self._settings.db_config
         connect_dict['dbtype'] = 'starrocks'
         self._connect_dict = connect_dict
-        self._create_table_collections(None)
-        self._create_table_embeddings(None)
+        # self._create_table_collections(None)
+        # self._create_table_embeddings(None)
         self._settings = system.settings
         self._load_dict = None
         load_host = self._connect_dict.get('load_host')
         if load_host:
             self._load_dict = {**connect_dict, 'host': load_host}
         self._dependencies = set()
 
+
     def _execute_sql(self, sql):
         return self._conn.execute_sql_list([sql], self._connect_dict)
 
     def _execute_load(self, contents, table):
         if self._load_dict:
             table = f"{self._connect_dict['db']}.{table}"
             contents[0][0] = '__' + contents[0][0]
@@ -50,22 +51,21 @@
             contents = contents[1:]
             self._conn.insert_contents_mysql(contents, table, 100, self._connect_dict)
 
     @override
     def _create_table_collections(self, conn):
         sql = """CREATE TABLE IF NOT EXISTS collections (
             uuid String, name String, metadata String
-        )PRIMARY KEY (uuid) comment 'collections' DISTRIBUTED BY HASH(uuid) BUCKETS 12 """
+        )PRIMARY KEY (uuid) comment 'collections' DISTRIBUTED BY HASH(uuid) """
         self._execute_sql(sql)
 
-    # duckdb has different types, so we want to convert the clickhouse schema to duckdb schema
     @override
     def _create_table_embeddings(self, conn):
-        sql = """CREATE TABLE IF NOT EXISTS embeddings(uuid String, collection_uuid String, embedding Array<FLOAT>, document String, id String, metadata String)
-        PRIMARY KEY (uuid) comment 'embeddings' DISTRIBUTED BY HASH(uuid) BUCKETS 12"""
+        sql = """CREATE TABLE IF NOT EXISTS embeddings(collection_uuid String,uuid String, embedding Array<Float>, document String, id String, metadata String)
+        DUPLICATE KEY (collection_uuid,uuid) comment 'embeddings' DISTRIBUTED BY HASH(collection_uuid)"""
         self._execute_sql(sql)
 
     #  UTILITY METHODS
     #
     @override
     def get_collection_uuid_from_name(self, collection_name: str) -> UUID:
         sql = f"SELECT uuid FROM collections WHERE name = {collection_name}"
@@ -182,77 +182,82 @@
     def _format_where(self, where, result):
         for key, value in where.items():
             # Shortcut for $eq
             if type(value) == str:
                 result.append(f" get_json_string(metadata,'$.{key}') = '{value}'")
             if type(value) == int:
                 result.append(
-                    f" CAST(get_json_string(metadata,'$.{key}') AS INT) = {value}"
+                    f" get_json_int(metadata,'$.{key}') = {value}"
                 )
             if type(value) == float:
                 result.append(
-                    f" CAST(get_json_string(metadata,'$.{key}') AS DOUBLE) = {value}"
+                    f" get_json_double(metadata,'$.{key}') = {value}"
                 )
             # Operator expression
             elif type(value) == dict:
                 operator, operand = list(value.items())[0]
                 if operator == "$gt":
                     result.append(
-                        f" CAST(get_json_string(metadata,'$.{key}') AS DOUBLE) > {operand}"
+                        f" get_json_double(metadata,'$.{key}') > {operand}"
                     )
                 elif operator == "$lt":
                     result.append(
-                        f" CAST(get_json_string(metadata,'$.{key}') AS DOUBLE) < {operand}"
+                        f" get_json_double(metadata,'$.{key}') < {operand}"
                     )
                 elif operator == "$gte":
                     result.append(
-                        f" CAST(get_json_string(metadata,'$.{key}') AS DOUBLE) >= {operand}"
+                        f" get_json_double(metadata,'$.{key}') >= {operand}"
                     )
                 elif operator == "$lte":
                     result.append(
-                        f" CAST(get_json_string(metadata,'$.{key}') AS DOUBLE) <= {operand}"
+                        f" get_json_string(metadata,'$.{key}') <= {operand}"
                     )
                 elif operator == "$ne":
                     if type(operand) == str:
                         return result.append(
                             f" get_json_string(metadata,'$.{key}') != '{operand}'"
                         )
                     return result.append(
-                        f" CAST(get_json_string(metadata,'$.{key}') AS DOUBLE) != {operand}"
+                        f" get_json_double(metadata,'$.{key}') != {operand}"
                     )
                 elif operator == "$eq":
                     if type(operand) == str:
                         return result.append(
                             f" get_json_string(metadata,'$.{key}') = '{operand}'"
                         )
                     return result.append(
-                        f" CAST(get_json_string(metadata,'$.{key}') AS DOUBLE) = {operand}"
+                        f" get_json_double(metadata,'$.{key}') = {operand}"
                     )
                 else:
                     raise ValueError(f"Operator {operator} not supported")
             elif type(value) == list:
+                if len(value) > 0 and type(value[0]) == str:
+                    result.append(f" get_json_string(metadata,'{key}') in {tuple(value)} ")
+                    continue
                 all_subresults = []
                 for subwhere in value:
                     subresults = []
                     self._format_where(subwhere, subresults)
                     all_subresults.append(subresults[0])
                 if key == "$or":
                     result.append(f"({' OR '.join(all_subresults)})")
                 elif key == "$and":
                     result.append(f"({' AND '.join(all_subresults)})")
                 else:
                     raise ValueError(
                         f"Operator {key} not supported with a list of where clauses"
                     )
+            elif type(value) == tuple:
+                result.append(f" get_json_string(metadata,'{key}') in {value} ")
 
     @override
     def _format_where_document(self, where_document, results):
         operator = list(where_document.keys())[0]
         if operator == "$contains":
-            results.append(f"position('{where_document[operator]}' in document) > 0")
+            results.append(f"document like '%{where_document[operator]}%' ")
         elif operator == "$and" or operator == "$or":
             all_subresults = []
             for subwhere in where_document[operator]:
                 subresults = []
                 self._format_where_document(subwhere, subresults)
                 all_subresults.append(subresults[0])
             if operator == "$or":
@@ -384,8 +389,37 @@
         logger.info("Exiting: Cleaning up .chroma directory")
         self.reset_indexes()
 
     @override
     def persist(self) -> None:
         raise NotImplementedError(
             "Set chroma_db_impl='starrocks' to get persistence functionality"
-        )
+        )
+
+    def get_nearest_neighbors_smart(
+            self,
+            collection_uuid: UUID,
+            where: Where = {},
+            embeddings: Optional[Embeddings] = None,
+            n_results: int = 10,
+            where_document: WhereDocument = {},
+    ):
+        # Either the collection name or the collection uuid must be provided
+        if collection_uuid is None:
+            raise TypeError("Argument collection_uuid cannot be None")
+            # 取消采用ids
+        where_str = self._create_where_clause(
+            # collection_uuid must be defined at this point, cast it for typechecker
+            cast(str, collection_uuid),
+            where=where,
+            where_document=where_document,
+        )
+        # 用自定义的方法, 需建表为字符串
+        # sql = f"""SELECT document, CosineSimilarity(embedding, '{embeddings[0]}') as d FROM embeddings {where_str} order by d desc limit {n_results}"""
+        # sql = f"""SELECT document, CosineSquaredL2(embedding, '{embeddings[0]}') as d FROM embeddings {where_str} order by d desc limit {n_results}"""
+        import time
+        start_time = time.time()
+        sql = f"""SELECT document, array_sum(array_map((x,y)->pow((x-y),2), embedding,{embeddings[0]})) as distance FROM embeddings {where_str} order by distance  limit {n_results}"""
+        val = self._execute_sql(sql)
+        print('starrocks cost:', time.time() - start_time)
+
+        return val
```

### Comparing `smart_chromadb-0.1.dev731/chromadb/db/system.py` & `smart_chromadb-0.1.dev732/chromadb/db/system.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/errors.py` & `smart_chromadb-0.1.dev732/chromadb/errors.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/ingest/__init__.py` & `smart_chromadb-0.1.dev732/chromadb/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/segment/__init__.py` & `smart_chromadb-0.1.dev732/chromadb/segment/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/segment/impl/manager/local.py` & `smart_chromadb-0.1.dev732/chromadb/segment/impl/manager/local.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/segment/impl/metadata/sqlite.py` & `smart_chromadb-0.1.dev732/chromadb/segment/impl/metadata/sqlite.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/segment/impl/vector/local_hnsw.py` & `smart_chromadb-0.1.dev732/chromadb/segment/impl/vector/local_hnsw.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/server/fastapi/__init__.py` & `smart_chromadb-0.1.dev732/chromadb/server/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/server/fastapi/types.py` & `smart_chromadb-0.1.dev732/chromadb/server/fastapi/types.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/telemetry/__init__.py` & `smart_chromadb-0.1.dev732/chromadb/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/telemetry/events.py` & `smart_chromadb-0.1.dev732/chromadb/telemetry/events.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/telemetry/posthog.py` & `smart_chromadb-0.1.dev732/chromadb/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/conftest.py` & `smart_chromadb-0.1.dev732/chromadb/test/conftest.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/db/test_base.py` & `smart_chromadb-0.1.dev732/chromadb/test/db/test_base.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/db/test_migrations.py` & `smart_chromadb-0.1.dev732/chromadb/test/db/test_migrations.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/db/test_system.py` & `smart_chromadb-0.1.dev732/chromadb/test/db/test_system.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/hnswlib/test_hnswlib.py` & `smart_chromadb-0.1.dev732/chromadb/test/hnswlib/test_hnswlib.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/ingest/test_producer_consumer.py` & `smart_chromadb-0.1.dev732/chromadb/test/ingest/test_producer_consumer.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/property/invariants.py` & `smart_chromadb-0.1.dev732/chromadb/test/property/invariants.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/property/strategies.py` & `smart_chromadb-0.1.dev732/chromadb/test/property/strategies.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/property/test_add.py` & `smart_chromadb-0.1.dev732/chromadb/test/property/test_add.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/property/test_collections.py` & `smart_chromadb-0.1.dev732/chromadb/test/property/test_collections.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/property/test_cross_version_persist.py` & `smart_chromadb-0.1.dev732/chromadb/test/property/test_cross_version_persist.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/property/test_embeddings.py` & `smart_chromadb-0.1.dev732/chromadb/test/property/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/property/test_filtering.py` & `smart_chromadb-0.1.dev732/chromadb/test/property/test_filtering.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/property/test_persist.py` & `smart_chromadb-0.1.dev732/chromadb/test/property/test_persist.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/segment/test_metadata.py` & `smart_chromadb-0.1.dev732/chromadb/test/segment/test_metadata.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/segment/test_vector.py` & `smart_chromadb-0.1.dev732/chromadb/test/segment/test_vector.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/test_api.py` & `smart_chromadb-0.1.dev732/chromadb/test/test_api.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/test_chroma.py` & `smart_chromadb-0.1.dev732/chromadb/test/test_chroma.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/test_config.py` & `smart_chromadb-0.1.dev732/chromadb/test/test_config.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/test/utils/test_messagid.py` & `smart_chromadb-0.1.dev732/chromadb/test/utils/test_messagid.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/chromadb/types.py` & `smart_chromadb-0.1.dev732/chromadb/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     Literal["$lte"],
     Literal["$ne"],
     Literal["$eq"],
 ]
 OperatorExpression = Dict[Union[WhereOperator, LogicalOperator], LiteralValue]
 
 Where = Dict[
-    Union[str, LogicalOperator], Union[LiteralValue, OperatorExpression, List["Where"]]
+    Union[str, LogicalOperator], Union[LiteralValue, OperatorExpression, List["Where"], tuple]
 ]
 
 WhereDocumentOperator = Union[Literal["$contains"], LogicalOperator]
 WhereDocument = Dict[WhereDocumentOperator, Union[str, List["WhereDocument"]]]
 
 
 class Unspecified:
```

### Comparing `smart_chromadb-0.1.dev731/chromadb/utils/embedding_functions.py` & `smart_chromadb-0.1.dev732/chromadb/utils/embedding_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,20 +51,20 @@
 
     def __call__(self, texts: Documents) -> Embeddings:
         return self._model.encode(list(texts), convert_to_numpy=True).tolist()  # type: ignore # noqa E501
 
 
 class OpenAIEmbeddingFunction(EmbeddingFunction):
     def __init__(
-        self,
-        api_key: Optional[str] = None,
-        model_name: str = "text-embedding-ada-002",
-        organization_id: Optional[str] = None,
-        api_base: Optional[str] = None,
-        api_type: Optional[str] = None,
+            self,
+            api_key: Optional[str] = None,
+            model_name: str = "text-embedding-ada-002",
+            organization_id: Optional[str] = None,
+            api_base: Optional[str] = None,
+            api_type: Optional[str] = None,
     ):
         """
         Initialize the OpenAIEmbeddingFunction.
 
         Args:
             api_key (str, optional): Your API key for the OpenAI API. If not
                 provided, it will raise an error to provide an OpenAI API key.
@@ -138,15 +138,15 @@
             embeddings
             for embeddings in self._client.embed(texts=texts, model=self._model_name)
         ]
 
 
 class HuggingFaceEmbeddingFunction(EmbeddingFunction):
     def __init__(
-        self, api_key: str, model_name: str = "sentence-transformers/all-MiniLM-L6-v2"
+            self, api_key: str, model_name: str = "sentence-transformers/all-MiniLM-L6-v2"
     ):
         try:
             import requests
         except ImportError:
             raise ValueError(
                 "The requests python package is not installed. Please install it with `pip install requests`"
             )
@@ -161,18 +161,18 @@
         ).json()
 
 
 class InstructorEmbeddingFunction(EmbeddingFunction):
     # If you have a GPU with at least 6GB try model_name = "hkunlp/instructor-xl" and device = "cuda"
     # for a full list of options: https://github.com/HKUNLP/instructor-embedding#model-list
     def __init__(
-        self,
-        model_name: str = "hkunlp/instructor-base",
-        device: str = "cpu",
-        instruction: Optional[str] = None,
+            self,
+            model_name: str = "hkunlp/instructor-base",
+            device: str = "cpu",
+            instruction: Optional[str] = None,
     ):
         try:
             from InstructorEmbedding import INSTRUCTOR
         except ImportError:
             raise ValueError(
                 "The InstructorEmbedding python package is not installed. Please install it with `pip install InstructorEmbedding`"
             )
@@ -232,19 +232,19 @@
 
     # Borrowed from https://gist.github.com/yanqd0/c13ed29e29432e3cf3e7c38467f42f51
     # Download with tqdm to preserve the sentence-transformers experience
     def _download(self, url: str, fname: Path, chunk_size: int = 1024) -> None:
         resp = requests.get(url, stream=True)
         total = int(resp.headers.get("content-length", 0))
         with open(fname, "wb") as file, self.tqdm(
-            desc=str(fname),
-            total=total,
-            unit="iB",
-            unit_scale=True,
-            unit_divisor=1024,
+                desc=str(fname),
+                total=total,
+                unit="iB",
+                unit_scale=True,
+                unit_divisor=1024,
         ) as bar:
             for data in resp.iter_content(chunk_size=chunk_size):
                 size = file.write(data)
                 bar.update(size)
 
     # Use pytorches default epsilon for division by zero
     # https://pytorch.org/docs/stable/generated/torch.nn.functional.normalize.html
@@ -255,15 +255,15 @@
 
     def _forward(self, documents: List[str], batch_size: int = 32) -> npt.NDArray:
         # We need to cast to the correct type because the type checker doesn't know that init_model_and_tokenizer will set the values
         self.tokenizer = cast(self.Tokenizer, self.tokenizer)  # type: ignore
         self.model = cast(self.ort.InferenceSession, self.model)  # type: ignore
         all_embeddings = []
         for i in range(0, len(documents), batch_size):
-            batch = documents[i : i + batch_size]
+            batch = documents[i: i + batch_size]
             encoded = [self.tokenizer.encode(d) for d in batch]
             input_ids = np.array([e.ids for e in encoded])
             attention_mask = np.array([e.attention_mask for e in encoded])
             onnx_input = {
                 "input_ids": np.array(input_ids, dtype=np.int64),
                 "attention_mask": np.array(attention_mask, dtype=np.int64),
                 "token_type_ids": np.array(
@@ -308,26 +308,28 @@
         # Model is not downloaded yet
         if not os.path.exists(self.DOWNLOAD_PATH / self.ARCHIVE_FILENAME):
             os.makedirs(self.DOWNLOAD_PATH, exist_ok=True)
             self._download(
                 self.MODEL_DOWNLOAD_URL, self.DOWNLOAD_PATH / self.ARCHIVE_FILENAME
             )
             with tarfile.open(
-                self.DOWNLOAD_PATH / self.ARCHIVE_FILENAME, "r:gz"
+                    self.DOWNLOAD_PATH / self.ARCHIVE_FILENAME, "r:gz"
             ) as tar:
                 tar.extractall(self.DOWNLOAD_PATH)
 
 
-DefaultEmbedding = Text2VecEmbeddingFunction()
+if is_thin_client:
+    DefaultEmbedding = None
+else:
+    DefaultEmbedding = Text2VecEmbeddingFunction()
+
+
 def DefaultEmbeddingFunction() -> Optional[EmbeddingFunction]:
-    if is_thin_client:
-        return None
-    else:
-        return DefaultEmbedding
-        # return ONNXMiniLM_L6_V2()
+    return DefaultEmbedding
+    # return ONNXMiniLM_L6_V2()
 
 
 class GooglePalmEmbeddingFunction(EmbeddingFunction):
     """To use this EmbeddingFunction, you must have the google.generativeai Python package installed and have a PaLM API key."""
 
     def __init__(self, api_key: str, model_name: str = "models/embedding-gecko-001"):
         if not api_key:
@@ -358,19 +360,19 @@
 
 class GoogleVertexEmbeddingFunction(EmbeddingFunction):
     # Follow API Quickstart for Google Vertex AI
     # https://cloud.google.com/vertex-ai/docs/generative-ai/start/quickstarts/api-quickstart
     # Information about the text embedding modules in Google Vertex AI
     # https://cloud.google.com/vertex-ai/docs/generative-ai/embeddings/get-text-embeddings
     def __init__(
-        self,
-        api_key: str,
-        model_name: str = "textembedding-gecko-001",
-        project_id: str = "cloud-large-language-models",
-        region: str = "us-central1",
+            self,
+            api_key: str,
+            model_name: str = "textembedding-gecko-001",
+            project_id: str = "cloud-large-language-models",
+            region: str = "us-central1",
     ):
         self._api_url = f"https://{region}-aiplatform.googleapis.com/v1/projects/{project_id}/locations/{region}/endpoints/{model_name}:predict"
         self._session = requests.Session()
         self._session.headers.update({"Authorization": f"Bearer {api_key}"})
 
     def __call__(self, texts: Documents) -> Embeddings:
         response = self._session.post(
```

### Comparing `smart_chromadb-0.1.dev731/chromadb/utils/messageid.py` & `smart_chromadb-0.1.dev732/chromadb/utils/messageid.py`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/DEVELOP.md` & `smart_chromadb-0.1.dev732/clients/js/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/LICENSE` & `smart_chromadb-0.1.dev732/clients/js/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/README.md` & `smart_chromadb-0.1.dev732/clients/js/README.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/examples/browser/app.ts` & `smart_chromadb-0.1.dev732/clients/js/examples/browser/app.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/examples/browser/index.html` & `smart_chromadb-0.1.dev732/clients/js/examples/browser/index.html`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/examples/browser/yarn.lock` & `smart_chromadb-0.1.dev732/clients/js/examples/browser/yarn.lock`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/examples/node/app.js` & `smart_chromadb-0.1.dev732/clients/js/examples/node/app.js`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/examples/node/package-lock.json` & `smart_chromadb-0.1.dev732/clients/js/examples/node/package-lock.json`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/examples/node/yarn.lock` & `smart_chromadb-0.1.dev732/clients/js/examples/node/yarn.lock`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/genapi.sh` & `smart_chromadb-0.1.dev732/clients/js/genapi.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/package-lock.json` & `smart_chromadb-0.1.dev732/clients/js/package-lock.json`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/package.json` & `smart_chromadb-0.1.dev732/clients/js/package.json`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/src/ChromaClient.ts` & `smart_chromadb-0.1.dev732/clients/js/src/ChromaClient.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/src/Collection.ts` & `smart_chromadb-0.1.dev732/clients/js/src/Collection.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/src/embeddings/CohereEmbeddingFunction.ts` & `smart_chromadb-0.1.dev732/clients/js/src/embeddings/CohereEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts` & `smart_chromadb-0.1.dev732/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/src/embeddings/TransformersEmbeddingFunction.ts` & `smart_chromadb-0.1.dev732/clients/js/src/embeddings/TransformersEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/src/embeddings/WebAIEmbeddingFunction.ts` & `smart_chromadb-0.1.dev732/clients/js/src/embeddings/WebAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/src/generated/README.md` & `smart_chromadb-0.1.dev732/clients/js/src/generated/README.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/src/generated/api.ts` & `smart_chromadb-0.1.dev732/clients/js/src/generated/api.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/src/generated/configuration.ts` & `smart_chromadb-0.1.dev732/clients/js/src/generated/configuration.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/src/generated/models.ts` & `smart_chromadb-0.1.dev732/clients/js/src/generated/models.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/src/generated/runtime.ts` & `smart_chromadb-0.1.dev732/clients/js/src/generated/runtime.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/src/types.ts` & `smart_chromadb-0.1.dev732/clients/js/src/types.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/src/utils.ts` & `smart_chromadb-0.1.dev732/clients/js/src/utils.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/test/add.collections.test.ts` & `smart_chromadb-0.1.dev732/clients/js/test/add.collections.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/test/client.test.ts` & `smart_chromadb-0.1.dev732/clients/js/test/client.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/test/collection.client.test.ts` & `smart_chromadb-0.1.dev732/clients/js/test/collection.client.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/test/collection.test.ts` & `smart_chromadb-0.1.dev732/clients/js/test/collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/test/delete.collection.test.ts` & `smart_chromadb-0.1.dev732/clients/js/test/delete.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/test/get.collection.test.ts` & `smart_chromadb-0.1.dev732/clients/js/test/get.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/test/peek.collection.test.ts` & `smart_chromadb-0.1.dev732/clients/js/test/peek.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/test/query.collection.test.ts` & `smart_chromadb-0.1.dev732/clients/js/test/query.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/test/update.collection.test.ts` & `smart_chromadb-0.1.dev732/clients/js/test/update.collection.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/test/upsert.collections.test.ts` & `smart_chromadb-0.1.dev732/clients/js/test/upsert.collections.test.ts`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/js/yarn.lock` & `smart_chromadb-0.1.dev732/clients/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/python/README.md` & `smart_chromadb-0.1.dev732/clients/python/README.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/python/build_python_thin_client.sh` & `smart_chromadb-0.1.dev732/clients/python/build_python_thin_client.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/python/integration-test.sh` & `smart_chromadb-0.1.dev732/clients/python/integration-test.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/clients/python/pyproject.toml` & `smart_chromadb-0.1.dev732/clients/python/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/docker-compose.server.example.yml` & `smart_chromadb-0.1.dev732/docker-compose.server.example.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/docker-compose.test.yml` & `smart_chromadb-0.1.dev732/docker-compose.test.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/docker-compose.yml` & `smart_chromadb-0.1.dev732/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/examples/alternative_embeddings.ipynb` & `smart_chromadb-0.1.dev732/examples/alternative_embeddings.ipynb`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/examples/deployments/google-cloud-compute/README.md` & `smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/README.md`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/examples/deployments/google-cloud-compute/chroma.tf` & `smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/chroma.tf`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/examples/deployments/google-cloud-compute/startup.sh` & `smart_chromadb-0.1.dev732/examples/deployments/google-cloud-compute/startup.sh`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/examples/local_persistence.ipynb` & `smart_chromadb-0.1.dev732/examples/local_persistence.ipynb`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/examples/where_filtering.ipynb` & `smart_chromadb-0.1.dev732/examples/where_filtering.ipynb`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/migrations/metadb/00001-embedding-metadata.sqlite.sql` & `smart_chromadb-0.1.dev732/migrations/metadb/00001-embedding-metadata.sqlite.sql`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/pyproject.toml` & `smart_chromadb-0.1.dev732/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smart_chromadb-0.1.dev731/smart_chromadb.egg-info/PKG-INFO` & `smart_chromadb-0.1.dev732/smart_chromadb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-chromadb
-Version: 0.1.dev731
+Version: 0.1.dev732
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
-Metadata-Version: 2.1 Name: smart-chromadb Version: 0.1.dev731 Summary: Chroma.
+Metadata-Version: 2.1 Name: smart-chromadb Version: 0.1.dev732 Summary: Chroma.
 Author-email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `smart_chromadb-0.1.dev731/smart_chromadb.egg-info/SOURCES.txt` & `smart_chromadb-0.1.dev732/smart_chromadb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 chromadb/app.py
 chromadb/config.py
 chromadb/errors.py
 chromadb/types.py
 chromadb/api/__init__.py
 chromadb/api/fastapi.py
 chromadb/api/local.py
+chromadb/api/smartapi.py
 chromadb/api/types.py
 chromadb/api/models/Collection.py
 chromadb/db/__init__.py
 chromadb/db/base.py
 chromadb/db/clickhouse.py
 chromadb/db/duckdb.py
 chromadb/db/migrations.py
```

