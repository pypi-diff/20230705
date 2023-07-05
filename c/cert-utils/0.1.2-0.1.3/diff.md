# Comparing `tmp/cert_utils-0.1.2.tar.gz` & `tmp/cert_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cert_utils-0.1.2.tar", last modified: Fri Jun 23 18:06:35 2023, max compression
+gzip compressed data, was "cert_utils-0.1.3.tar", last modified: Wed Jul  5 18:34:11 2023, max compression
```

## Comparing `cert_utils-0.1.2.tar` & `cert_utils-0.1.3.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.837060 cert_utils-0.1.2/
--rw-r--r--   0 jvanasco   (501) admin       (80)      515 2023-06-23 18:06:28.000000 cert_utils-0.1.2/CHANGES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)    12231 2023-06-23 17:24:49.000000 cert_utils-0.1.2/LICENSE.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      191 2023-06-23 17:24:49.000000 cert_utils-0.1.2/MANIFEST.in
--rw-r--r--   0 jvanasco   (501) admin       (80)     4951 2023-06-23 18:06:35.837431 cert_utils-0.1.2/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)     4121 2023-06-23 17:24:49.000000 cert_utils-0.1.2/README.md
--rw-r--r--   0 jvanasco   (501) admin       (80)       39 2023-06-23 17:24:49.000000 cert_utils-0.1.2/pyproject.toml
--rw-r--r--   0 jvanasco   (501) admin       (80)      403 2023-06-23 18:06:35.840674 cert_utils-0.1.2/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)     2801 2023-06-23 17:24:49.000000 cert_utils-0.1.2/setup.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.318617 cert_utils-0.1.2/src/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.373574 cert_utils-0.1.2/src/cert_utils/
--rw-r--r--   0 jvanasco   (501) admin       (80)      145 2023-06-23 18:06:28.000000 cert_utils-0.1.2/src/cert_utils/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)   131576 2023-06-23 18:06:28.000000 cert_utils-0.1.2/src/cert_utils/core.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      441 2023-06-23 18:06:28.000000 cert_utils-0.1.2/src/cert_utils/errors.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.522841 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1680 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/fakeleintermediatex1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1797 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/fakelerootx1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1696 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/isrg-root-ocsp-x1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1955 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/isrg-root-x1-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1578 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/isrg-root-x2-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      790 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/isrg-root-x2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1939 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/isrgrootx1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1391 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/isrgrootx1.pkix
--rw-r--r--   0 jvanasco   (501) admin       (80)     1021 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-e1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1021 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-e2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1586 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-r3-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1826 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-r3.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1586 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-r4-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1826 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-r4.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-x1-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-x2-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1647 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-x3-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1647 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-x4-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2013 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/letsencryptauthorityx1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2013 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/letsencryptauthorityx2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1984 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/letsencryptauthorityx3.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1984 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/letsencryptauthorityx4.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      893 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/trustid-x3-root.p7c
--rw-r--r--   0 jvanasco   (501) admin       (80)     1199 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/trustid-x3-root.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)    16333 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/letsencrypt_info.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1597 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/model.py
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/py.typed
--rw-r--r--   0 jvanasco   (501) admin       (80)     3441 2023-06-23 17:24:49.000000 cert_utils-0.1.2/src/cert_utils/utils.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.393001 cert_utils-0.1.2/src/cert_utils.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)     4951 2023-06-23 18:06:35.000000 cert_utils-0.1.2/src/cert_utils.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)     7615 2023-06-23 18:06:35.000000 cert_utils-0.1.2/src/cert_utils.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-23 18:06:35.000000 cert_utils-0.1.2/src/cert_utils.egg-info/dependency_links.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-23 18:06:35.000000 cert_utils-0.1.2/src/cert_utils.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)      200 2023-06-23 18:06:35.000000 cert_utils-0.1.2/src/cert_utils.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       11 2023-06-23 18:06:35.000000 cert_utils-0.1.2/src/cert_utils.egg-info/top_level.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.535864 cert_utils-0.1.2/tests/
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     7702 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/_utils.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.540612 cert_utils-0.1.2/tests/test_data/
--rw-r--r--   0 jvanasco   (501) admin       (80)     3303 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/__README__.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.321847 cert_utils-0.1.2/tests/test_data/alternate_chains/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.549133 cert_utils-0.1.2/tests/test_data/alternate_chains/1/
--rw-r--r--   0 jvanasco   (501) admin       (80)       48 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/alternate_chains/1/__README__.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.323837 cert_utils-0.1.2/tests/test_data/alternate_chains/1/alternate_chains/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.552786 cert_utils-0.1.2/tests/test_data/alternate_chains/1/alternate_chains/1/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/alternate_chains/1/alternate_chains/1/chain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/alternate_chains/1/alternate_chains/1/fullchain.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.558379 cert_utils-0.1.2/tests/test_data/alternate_chains/1/alternate_chains/2/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/alternate_chains/1/alternate_chains/2/chain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/alternate_chains/1/alternate_chains/2/fullchain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1570 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/alternate_chains/1/cert.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/alternate_chains/1/chain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/alternate_chains/1/fullchain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     3272 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/alternate_chains/1/privkey.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.563493 cert_utils-0.1.2/tests/test_data/key_technology-ec/
--rw-r--r--   0 jvanasco   (501) admin       (80)      288 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-ec/ec384-1-key.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      452 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-ec/ec384-1.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)      288 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-ec/ec384-2-key.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.668269 cert_utils-0.1.2/tests/test_data/key_technology-rsa/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-3.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-4.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-5.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_daily.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_weekly.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_daily.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1671 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_weekly.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-single_certificate.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/acme_account_1.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/acme_account_2.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/acme_account_3.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/acme_account_4.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/acme_account_5.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/private_1.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/private_2.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/private_3.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/private_4.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3247 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/private_5.key
--rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_1-server.crt
--rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_1-server.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)      891 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_1-server.key
--rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_2-server.crt
--rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_2-server.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_2-server.key
--rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_3-server.crt
--rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_3-server.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_3-server.key
--rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_4-server.crt
--rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_4-server.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_4-server.key
--rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_5-server.crt
--rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_5-server.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_5-server.key
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.670660 cert_utils-0.1.2/tests/test_data/long_chains/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.691007 cert_utils-0.1.2/tests/test_data/long_chains/TestA/
--rw-r--r--   0 jvanasco   (501) admin       (80)      573 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/long_chains/TestA/__README__.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       76 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/long_chains/TestA/_data.json
--rw-r--r--   0 jvanasco   (501) admin       (80)     2683 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/long_chains/TestA/_demo.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/long_chains/TestA/cert.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/long_chains/TestA/chain_0.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     3664 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/long_chains/TestA/chain_0_bad.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/long_chains/TestA/chain_1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/long_chains/TestA/chain_2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/long_chains/TestA/root_0.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/long_chains/TestA/root_1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/long_chains/TestA/root_2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)       46 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/long_chains/__README__.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.764612 cert_utils-0.1.2/tests/test_data/pebble-certs/
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/cert1.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/cert2.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/cert3.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/cert4.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/cert5.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/cert6.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/chain1.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/chain2.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/chain3.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/chain4.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/chain5.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/chain6.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/fullchain1.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/fullchain2.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/fullchain3.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/fullchain4.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/fullchain5.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/fullchain6.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/privkey1.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/privkey2.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/privkey3.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/privkey4.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/privkey5.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3247 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/pebble-certs/privkey6.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.335425 cert_utils-0.1.2/tests/test_data/unit_tests/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.771775 cert_utils-0.1.2/tests/test_data/unit_tests/_support/
--rw-r--r--   0 jvanasco   (501) admin       (80)     3247 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/_support/account.key
--rw-r--r--   0 jvanasco   (501) admin       (80)      913 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/_support/info.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.786567 cert_utils-0.1.2/tests/test_data/unit_tests/account_001/
--rw-r--r--   0 jvanasco   (501) admin       (80)      212 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/account_001/info.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       70 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/account_001/meta.json
--rw-r--r--   0 jvanasco   (501) admin       (80)     1632 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/account_001/private_key.json
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/account_001/private_key.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)       86 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/account_001/regr.json
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.799263 cert_utils-0.1.2/tests/test_data/unit_tests/cert_001/
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1635 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_001/cert.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_001/chain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1674 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_001/csr.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2844 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_001/fullchain.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)      387 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_001/info.txt
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_001/privkey.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1516 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_001/test.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.805300 cert_utils-0.1.2/tests/test_data/unit_tests/cert_002/
--rw-r--r--   0 jvanasco   (501) admin       (80)      538 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_002/csr.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)      889 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_002/info.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_002/privkey.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.820056 cert_utils-0.1.2/tests/test_data/unit_tests/cert_003/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1042 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_003/cert.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      566 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_003/csr.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2250 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_003/fullchain.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)      569 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_003/info.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      891 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_003/privkey.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.830054 cert_utils-0.1.2/tests/test_data/unit_tests/cert_004/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1111 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_004/cert.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      631 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_004/csr.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2319 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_004/fullchain.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)      751 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_004/info.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_004/privkey.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 18:06:35.835151 cert_utils-0.1.2/tests/test_data/unit_tests/cert_005/
--rw-r--r--   0 jvanasco   (501) admin       (80)      643 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_005/csr.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1146 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_005/info.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_data/unit_tests/cert_005/privkey.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)    73620 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tests/test_unit.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-06-23 17:24:49.000000 cert_utils-0.1.2/tox.ini
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.244939 cert_utils-0.1.3/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      559 2023-07-05 18:33:55.000000 cert_utils-0.1.3/CHANGES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)    12231 2023-06-23 17:24:49.000000 cert_utils-0.1.3/LICENSE.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      191 2023-06-23 17:24:49.000000 cert_utils-0.1.3/MANIFEST.in
+-rw-r--r--   0 jvanasco   (501) admin       (80)     4951 2023-07-05 18:34:11.245333 cert_utils-0.1.3/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     4121 2023-06-23 17:24:49.000000 cert_utils-0.1.3/README.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)       39 2023-06-23 17:24:49.000000 cert_utils-0.1.3/pyproject.toml
+-rw-r--r--   0 jvanasco   (501) admin       (80)      403 2023-07-05 18:34:11.248645 cert_utils-0.1.3/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2801 2023-06-23 17:24:49.000000 cert_utils-0.1.3/setup.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.758927 cert_utils-0.1.3/src/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.805271 cert_utils-0.1.3/src/cert_utils/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      145 2023-07-05 18:33:55.000000 cert_utils-0.1.3/src/cert_utils/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)   131802 2023-07-05 18:33:55.000000 cert_utils-0.1.3/src/cert_utils/core.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      441 2023-06-23 18:06:28.000000 cert_utils-0.1.3/src/cert_utils/errors.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.869991 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1680 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/fakeleintermediatex1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1797 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/fakelerootx1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1696 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrg-root-ocsp-x1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1955 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrg-root-x1-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1578 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrg-root-x2-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)      790 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrg-root-x2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1939 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrgrootx1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1391 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrgrootx1.pkix
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1021 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-e1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1021 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-e2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1586 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-r3-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1826 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-r3.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1586 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-r4-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1826 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-r4.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-x1-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-x2-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1647 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-x3-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1647 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-x4-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2013 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/letsencryptauthorityx1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2013 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/letsencryptauthorityx2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1984 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/letsencryptauthorityx3.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1984 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/letsencryptauthorityx4.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)      893 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/trustid-x3-root.p7c
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1199 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/trustid-x3-root.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)    16333 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt_info.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1597 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/model.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/py.typed
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3441 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/utils.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.814577 cert_utils-0.1.3/src/cert_utils.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     4951 2023-07-05 18:34:10.000000 cert_utils-0.1.3/src/cert_utils.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     7615 2023-07-05 18:34:10.000000 cert_utils-0.1.3/src/cert_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-07-05 18:34:10.000000 cert_utils-0.1.3/src/cert_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-23 18:06:35.000000 cert_utils-0.1.3/src/cert_utils.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)      200 2023-07-05 18:34:10.000000 cert_utils-0.1.3/src/cert_utils.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       11 2023-07-05 18:34:10.000000 cert_utils-0.1.3/src/cert_utils.egg-info/top_level.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.880580 cert_utils-0.1.3/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     7702 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/_utils.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.884175 cert_utils-0.1.3/tests/test_data/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3303 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/__README__.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.761690 cert_utils-0.1.3/tests/test_data/alternate_chains/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.894009 cert_utils-0.1.3/tests/test_data/alternate_chains/1/
+-rw-r--r--   0 jvanasco   (501) admin       (80)       48 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/__README__.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.763553 cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.905522 cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/1/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/1/chain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/1/fullchain.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.909542 cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/2/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/2/chain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/2/fullchain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1570 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/cert.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/chain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/fullchain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3272 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/privkey.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.947474 cert_utils-0.1.3/tests/test_data/key_technology-ec/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      288 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-ec/ec384-1-key.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)      452 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-ec/ec384-1.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      288 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-ec/ec384-2-key.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.044438 cert_utils-0.1.3/tests/test_data/key_technology-rsa/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-3.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-4.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-5.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_daily.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_weekly.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_daily.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1671 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_weekly.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-single_certificate.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_1.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_2.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_3.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_4.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_5.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_1.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_2.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_3.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_4.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3247 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_5.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_1-server.crt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_1-server.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      891 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_1-server.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_2-server.crt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_2-server.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_2-server.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_3-server.crt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_3-server.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_3-server.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_4-server.crt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_4-server.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_4-server.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_5-server.crt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_5-server.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_5-server.key
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.045961 cert_utils-0.1.3/tests/test_data/long_chains/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.078399 cert_utils-0.1.3/tests/test_data/long_chains/TestA/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      573 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/__README__.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       76 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/_data.json
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2683 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/_demo.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/cert.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/chain_0.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3664 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/chain_0_bad.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/chain_1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/chain_2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/root_0.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/root_1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/root_2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)       46 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/__README__.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.131146 cert_utils-0.1.3/tests/test_data/pebble-certs/
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/cert1.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/cert2.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/cert3.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/cert4.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/cert5.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/cert6.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/chain1.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/chain2.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/chain3.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/chain4.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/chain5.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/chain6.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain1.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain2.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain3.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain4.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain5.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain6.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/privkey1.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/privkey2.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/privkey3.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/privkey4.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/privkey5.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3247 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/privkey6.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.774002 cert_utils-0.1.3/tests/test_data/unit_tests/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.135444 cert_utils-0.1.3/tests/test_data/unit_tests/_support/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3247 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/_support/account.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      913 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/_support/info.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.143628 cert_utils-0.1.3/tests/test_data/unit_tests/account_001/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      212 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/account_001/info.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       70 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/account_001/meta.json
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1632 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/account_001/private_key.json
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/account_001/private_key.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)       86 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/account_001/regr.json
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.163585 cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1635 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/cert.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/chain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1674 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/csr.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2844 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/fullchain.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)      387 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/info.txt
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/privkey.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1516 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/test.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.172372 cert_utils-0.1.3/tests/test_data/unit_tests/cert_002/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      538 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_002/csr.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)      889 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_002/info.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_002/privkey.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.179525 cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1042 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/cert.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)      566 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/csr.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2250 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/fullchain.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)      569 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/info.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      891 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/privkey.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.197273 cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1111 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/cert.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)      631 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/csr.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2319 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/fullchain.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)      751 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/info.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/privkey.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.243036 cert_utils-0.1.3/tests/test_data/unit_tests/cert_005/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      643 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_005/csr.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1146 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_005/info.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_005/privkey.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)    73620 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_unit.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tox.ini
```

### Comparing `cert_utils-0.1.2/CHANGES.txt` & `cert_utils-0.1.3/CHANGES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+0.1.3
+    new mypy version caught an issue
+
 0.1.2
     docs improvements
     raise a new `FallbackError_FilepathRequired` exception when missing a
         required fallback filepath
 
 0.1.1
     minor formatting
```

### Comparing `cert_utils-0.1.2/LICENSE.txt` & `cert_utils-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/PKG-INFO` & `cert_utils-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cert_utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: TLS/SSL Certiicate Utilities
 Home-page: https://github.com/aptise/cert_utils
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: MIT
 Keywords: web
 Classifier: Intended Audience :: Developers
```

### Comparing `cert_utils-0.1.2/README.md` & `cert_utils-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/setup.py` & `cert_utils-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/core.py` & `cert_utils-0.1.3/src/cert_utils/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2320,14 +2320,16 @@
         raise FallbackError_FilepathRequired("Must submit `cert_pem_filepath`.")
     tmpfile_pem = None
     try:
         if key_technology is None:
             key_technology = parse_cert__key_technology(
                 cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
             )
+            if not key_technology:
+                raise ValueError("Could not parse key_technology for backup")
         spki_sha256 = _openssl_spki_hash_cert(
             key_technology=key_technology,
             cert_pem_filepath=cert_pem_filepath,
             as_b64=as_b64,
         )
         return spki_sha256
     except Exception as exc:  # noqa: F841
@@ -2651,14 +2653,16 @@
         raise FallbackError_FilepathRequired("Must submit `csr_pem_filepath`.")
     tmpfile_pem = None
     try:
         if key_technology is None:
             key_technology = parse_csr__key_technology(
                 csr_pem=csr_pem, csr_pem_filepath=csr_pem_filepath
             )
+            if not key_technology:
+                raise ValueError("Could not parse key_technology for backup")
         spki_sha256 = _openssl_spki_hash_csr(
             key_technology=key_technology,
             csr_pem_filepath=csr_pem_filepath,
             as_b64=as_b64,
         )
         return spki_sha256
     except Exception as exc:  # noqa: F841
```

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/fakeleintermediatex1.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/fakeleintermediatex1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/fakelerootx1.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/fakelerootx1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/isrg-root-ocsp-x1.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrg-root-ocsp-x1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/isrg-root-x1-cross-signed.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrg-root-x1-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/isrg-root-x2-cross-signed.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrg-root-x2-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/isrg-root-x2.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrg-root-x2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/isrgrootx1.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrgrootx1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/isrgrootx1.pkix` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrgrootx1.pkix`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-e1.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-e1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-e2.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-e2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-r3-cross-signed.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-r3-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-r3.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-r3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-r4-cross-signed.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-r4-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-r4.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-r4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-x1-cross-signed.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-x1-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-x2-cross-signed.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-x2-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-x3-cross-signed.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-x3-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/lets-encrypt-x4-cross-signed.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-x4-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/letsencryptauthorityx1.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/letsencryptauthorityx1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/letsencryptauthorityx2.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/letsencryptauthorityx2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/letsencryptauthorityx3.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/letsencryptauthorityx3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/letsencryptauthorityx4.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/letsencryptauthorityx4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/trustid-x3-root.p7c` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/trustid-x3-root.p7c`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt-certs/trustid-x3-root.pem` & `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/trustid-x3-root.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/letsencrypt_info.py` & `cert_utils-0.1.3/src/cert_utils/letsencrypt_info.py`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/model.py` & `cert_utils-0.1.3/src/cert_utils/model.py`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils/utils.py` & `cert_utils-0.1.3/src/cert_utils/utils.py`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/src/cert_utils.egg-info/PKG-INFO` & `cert_utils-0.1.3/src/cert_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cert-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: TLS/SSL Certiicate Utilities
 Home-page: https://github.com/aptise/cert_utils
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: MIT
 Keywords: web
 Classifier: Intended Audience :: Developers
```

### Comparing `cert_utils-0.1.2/src/cert_utils.egg-info/SOURCES.txt` & `cert_utils-0.1.3/src/cert_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/_utils.py` & `cert_utils-0.1.3/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/__README__.txt` & `cert_utils-0.1.3/tests/test_data/__README__.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/alternate_chains/1/alternate_chains/1/chain.pem` & `cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/1/chain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/alternate_chains/1/alternate_chains/1/fullchain.pem` & `cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/1/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/alternate_chains/1/alternate_chains/2/chain.pem` & `cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/2/chain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/alternate_chains/1/alternate_chains/2/fullchain.pem` & `cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/2/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/alternate_chains/1/cert.pem` & `cert_utils-0.1.3/tests/test_data/alternate_chains/1/cert.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/alternate_chains/1/chain.pem` & `cert_utils-0.1.3/tests/test_data/alternate_chains/1/chain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/alternate_chains/1/fullchain.pem` & `cert_utils-0.1.3/tests/test_data/alternate_chains/1/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/alternate_chains/1/privkey.pem` & `cert_utils-0.1.3/tests/test_data/alternate_chains/1/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-1.pem` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-2.pem` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-3.pem` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-4.pem` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-5.pem` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-5.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_daily.pem` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_daily.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_weekly.pem` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_weekly.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_daily.pem` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_daily.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_weekly.pem` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_weekly.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-single_certificate.pem` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-single_certificate.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/acme_account_1.key` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_1.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/acme_account_2.key` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_2.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/acme_account_3.key` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_3.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/acme_account_4.key` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_4.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/acme_account_5.key` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_5.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/private_1.key` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_1.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/private_2.key` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_2.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/private_3.key` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_3.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/private_4.key` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_4.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/private_5.key` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_5.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_1-server.crt` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_1-server.crt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_1-server.csr` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_1-server.csr`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_1-server.key` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_1-server.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_2-server.crt` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_2-server.crt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_2-server.csr` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_2-server.csr`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_2-server.key` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_2-server.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_3-server.crt` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_3-server.crt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_3-server.csr` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_3-server.csr`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_3-server.key` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_3-server.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_4-server.crt` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_4-server.crt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_4-server.csr` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_4-server.csr`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_4-server.key` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_4-server.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_5-server.crt` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_5-server.crt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_5-server.csr` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_5-server.csr`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/key_technology-rsa/selfsigned_5-server.key` & `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_5-server.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/long_chains/TestA/__README__.txt` & `cert_utils-0.1.3/tests/test_data/long_chains/TestA/__README__.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/long_chains/TestA/_demo.py` & `cert_utils-0.1.3/tests/test_data/long_chains/TestA/_demo.py`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/long_chains/TestA/cert.pem` & `cert_utils-0.1.3/tests/test_data/long_chains/TestA/cert.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/long_chains/TestA/chain_0.pem` & `cert_utils-0.1.3/tests/test_data/long_chains/TestA/chain_0.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/long_chains/TestA/chain_0_bad.pem` & `cert_utils-0.1.3/tests/test_data/long_chains/TestA/chain_0_bad.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/long_chains/TestA/chain_1.pem` & `cert_utils-0.1.3/tests/test_data/long_chains/TestA/chain_1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/long_chains/TestA/chain_2.pem` & `cert_utils-0.1.3/tests/test_data/long_chains/TestA/chain_2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/long_chains/TestA/root_0.pem` & `cert_utils-0.1.3/tests/test_data/long_chains/TestA/root_0.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/long_chains/TestA/root_1.pem` & `cert_utils-0.1.3/tests/test_data/long_chains/TestA/root_1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/long_chains/TestA/root_2.pem` & `cert_utils-0.1.3/tests/test_data/long_chains/TestA/root_2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/cert1.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/cert1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/cert2.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/cert2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/cert3.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/cert3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/cert4.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/cert4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/cert5.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/cert5.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/cert6.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/cert6.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/chain1.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/chain1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/chain2.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/chain2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/chain3.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/chain3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/chain4.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/chain4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/chain5.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/chain5.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/chain6.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/chain6.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/fullchain1.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/fullchain2.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/fullchain3.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/fullchain4.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/fullchain5.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain5.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/fullchain6.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain6.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/privkey1.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/privkey1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/privkey2.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/privkey2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/privkey3.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/privkey3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/privkey4.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/privkey4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/privkey5.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/privkey5.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/pebble-certs/privkey6.pem` & `cert_utils-0.1.3/tests/test_data/pebble-certs/privkey6.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/_support/account.key` & `cert_utils-0.1.3/tests/test_data/unit_tests/_support/account.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/_support/info.txt` & `cert_utils-0.1.3/tests/test_data/unit_tests/_support/info.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/account_001/private_key.json` & `cert_utils-0.1.3/tests/test_data/unit_tests/account_001/private_key.json`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/account_001/private_key.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/account_001/private_key.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_001/cert.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/cert.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_001/chain.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/chain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_001/csr.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/csr.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_001/fullchain.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_001/privkey.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_001/test.py` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/test.py`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_002/csr.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_002/csr.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_002/info.txt` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_002/info.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_002/privkey.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_002/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_003/cert.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/cert.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_003/csr.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/csr.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_003/fullchain.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_003/info.txt` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/info.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_003/privkey.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_004/cert.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/cert.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_004/csr.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/csr.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_004/fullchain.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_004/info.txt` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/info.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_004/privkey.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_005/csr.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_005/csr.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_005/info.txt` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_005/info.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_data/unit_tests/cert_005/privkey.pem` & `cert_utils-0.1.3/tests/test_data/unit_tests/cert_005/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.2/tests/test_unit.py` & `cert_utils-0.1.3/tests/test_unit.py`

 * *Files identical despite different names*

