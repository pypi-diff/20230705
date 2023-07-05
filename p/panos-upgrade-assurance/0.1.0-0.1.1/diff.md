# Comparing `tmp/panos_upgrade_assurance-0.1.0.tar.gz` & `tmp/panos_upgrade_assurance-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panos_upgrade_assurance-0.1.0.tar", max compression
+gzip compressed data, was "panos_upgrade_assurance-0.1.1.tar", max compression
```

## Comparing `panos_upgrade_assurance-0.1.0.tar` & `panos_upgrade_assurance-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-06-21 08:45:29.863809 panos_upgrade_assurance-0.1.0/LICENSE
--rw-r--r--   0        0        0      930 2023-06-21 08:45:29.863809 panos_upgrade_assurance-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-21 08:45:29.863809 panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/__init__.py
--rw-r--r--   0        0        0    37984 2023-06-21 08:45:29.867810 panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/check_firewall.py
--rw-r--r--   0        0        0     2325 2023-06-21 08:45:29.867810 panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/exceptions.py
--rw-r--r--   0        0        0    36113 2023-06-21 08:45:29.867810 panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/firewall_proxy.py
--rw-r--r--   0        0        0    31244 2023-06-21 08:45:29.867810 panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/snapshot_compare.py
--rw-r--r--   0        0        0    11662 2023-06-21 08:45:29.867810 panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/utils.py
--rw-r--r--   0        0        0     1120 2023-06-21 08:45:52.296277 panos_upgrade_assurance-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 panos_upgrade_assurance-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-05 01:34:01.761817 panos_upgrade_assurance-0.1.1/LICENSE
+-rw-r--r--   0        0        0      930 2023-07-05 01:34:01.761817 panos_upgrade_assurance-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 01:34:01.765817 panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/__init__.py
+-rw-r--r--   0        0        0    44057 2023-07-05 01:34:01.765817 panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/check_firewall.py
+-rw-r--r--   0        0        0     2472 2023-07-05 01:34:01.765817 panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/exceptions.py
+-rw-r--r--   0        0        0    39216 2023-07-05 01:34:01.765817 panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/firewall_proxy.py
+-rw-r--r--   0        0        0    31244 2023-07-05 01:34:01.765817 panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/snapshot_compare.py
+-rw-r--r--   0        0        0    12349 2023-07-05 01:34:01.765817 panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/utils.py
+-rw-r--r--   0        0        0     1140 2023-07-05 01:34:23.706229 panos_upgrade_assurance-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1617 1970-01-01 00:00:00.000000 panos_upgrade_assurance-0.1.1/PKG-INFO
```

### Comparing `panos_upgrade_assurance-0.1.0/LICENSE` & `panos_upgrade_assurance-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.1.0/README.md` & `panos_upgrade_assurance-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/check_firewall.py` & `panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/check_firewall.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 from panos_upgrade_assurance.utils import (
     CheckResult,
     ConfigParser,
     interpret_yes_no,
     CheckType,
     SnapType,
     CheckStatus,
+    SupportedHashes,
 )
 from panos_upgrade_assurance.firewall_proxy import FirewallProxy
 from panos_upgrade_assurance import exceptions
 from panos import PanOSVersion
+from OpenSSL import crypto as oSSL
 
 
 class CheckFirewall:
     """Class responsible for running readiness checks and creating Firewall state snapshots.
 
     This class is designed to:
 
@@ -85,14 +87,15 @@
             CheckType.ACTIVE_SUPPORT: self.check_active_support_license,
             CheckType.CONTENT_VERSION: self.check_content_version,
             CheckType.SESSION_EXIST: self.check_critical_session,
             CheckType.ARP_ENTRY_EXIST: self.check_arp_entry,
             CheckType.IPSEC_TUNNEL_STATUS: self.check_ipsec_tunnel_status,
             CheckType.FREE_DISK_SPACE: self.check_free_disk_space,
             CheckType.MP_DP_CLOCK_SYNC: self.check_mp_dp_sync,
+            CheckType.CERTS: self.check_ssl_cert_requirements,
         }
         locale.setlocale(
             locale.LC_ALL, "en_US.UTF-8"
         )  # force locale for datetime string parsing when non-English locale is set on host
 
     def check_pending_changes(self) -> CheckResult:
         """Check if there are pending changes on device.
@@ -739,14 +742,133 @@
         if time_fluctuation > diff_threshold:
             result.reason = f"The data plane clock and management clock are different by {time_fluctuation} seconds."
         else:
             result.status = CheckStatus.SUCCESS
 
         return result
 
+    def check_ssl_cert_requirements(self, rsa: dict = {}, ecdsa: dict = {}) -> CheckResult:
+        """Check if the certificates' keys meet minimum size requirements.
+
+        This method loops over all certificates installed on a device and compares certificate's properties with the ones
+        provided in input parameters. There are two parameters available, one describing `RSA` certificate requirements, the
+        other for `ECDSA` certificates. Both parameters are dictionaries accepting the following keys:
+
+        - `hash_method` - a minimum (from security perspective) required hashing method,
+        - `key_size` - a minimum size of a key.
+
+        # Parameters
+
+        rsa (dict, optional): A dictionary describing minimum security requirements of a `RSA` certificate. Default values \
+            for the certificate requirements are as follows:
+
+            - `hash_method` - `SHA256`,
+            - `key_size` - `2048`.
+
+        ecdsa (dict, optional): A dictionary describing minimum security requirements of a `ECDSA` certificate. Default values \
+        for the certificate requirements are as follows:
+
+            - `hash_method` - `SHA256`,
+            - `key_size` - `256`.
+
+        # Returns
+
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking \
+            value of:
+
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when all certs meet the size
+            requirements.
+        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) if a least one cert
+            does not meet the requirements - certificate names with their current sizes are provided in `CheckResult.reason`
+            property.
+        * [`CheckStatus.SKIPPED`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when device does not have
+            certificates installed.
+        * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when the certificate's
+            properties (installed or required) are not supported.
+
+        """
+        result = CheckResult()
+
+        allowed_keys = ["hash_method", "key_size"]
+
+        if not all(key in allowed_keys for key in rsa.keys()):
+            raise exceptions.UnknownParameterException(
+                f"Unknown configuration parameter(s) found in the `rsa` dictionary: {', '.join(rsa.keys())}."
+            )
+        if not all(key in allowed_keys for key in ecdsa.keys()):
+            raise exceptions.UnknownParameterException(
+                f"Unknown configuration parameter(s) found in the `ecdsa` dictionary: {', '.join(ecdsa.keys())}."
+            )
+
+        certificates = self._node.get_certificates()
+        if not certificates:
+            result.status = CheckStatus.SKIPPED
+            result.reason = "No certificates installed on device."
+            return result
+
+        rsa_min_hash_method = rsa.get("hash_method", "sha256").upper()
+        if rsa_min_hash_method in [member.name for member in SupportedHashes]:
+            rsa_min_hash = SupportedHashes[rsa_min_hash_method]
+        else:
+            result.status = CheckStatus.ERROR
+            result.reason = f"The provided minimum RSA hashing method ({rsa_min_hash_method}) is not supported."
+            return result
+
+        ecdsa_min_hash_method = ecdsa.get("hash_method", "sha256").upper()
+        if ecdsa_min_hash_method in [member.name for member in SupportedHashes]:
+            ecdsa_min_hash = SupportedHashes[ecdsa_min_hash_method]
+        else:
+            result.status = CheckStatus.ERROR
+            result.reason = f"The provided minimum ECDSA hashing method ({ecdsa_min_hash_method}) is not supported."
+            return result
+
+        rsa_min_key_size = rsa.get("key_size", 2048)
+        if not (isinstance(rsa_min_key_size, int) and rsa_min_key_size > 0):
+            result.status = CheckStatus.ERROR
+            result.reason = "The provided minimum RSA key size should be an integer grater than 0."
+            return result
+
+        ecdsa_min_key_size = ecdsa.get("key_size", 256)
+        if not (isinstance(ecdsa_min_key_size, int) and ecdsa_min_key_size > 0):
+            result.status = CheckStatus.ERROR
+            result.reason = "The provided minimum ECDSA key size should be an integer grater than 0."
+            return result
+
+        failed_certs = []
+        for cert_name, certificate in certificates.items():
+            cert = oSSL.load_certificate(oSSL.FILETYPE_PEM, certificate["public-key"])
+
+            cert_key_size = cert.get_pubkey().bits()
+
+            cert_algorithm = certificate["algorithm"]
+            if cert_algorithm not in ["RSA", "EC"]:
+                result.status = CheckStatus.ERROR
+                result.reason = f"Failed for certificate: {cert_name}: unknown algorithm {cert_algorithm}."
+                return result
+
+            cert_hash_method = cert.to_cryptography().signature_hash_algorithm.name.upper()
+            if cert_hash_method in [member.name for member in SupportedHashes]:
+                cert_hash = SupportedHashes[cert_hash_method]
+            else:
+                result.status = CheckStatus.ERROR
+                result.reason = f"The certificate's hashing method ({cert_hash}) is not supported? Please check the device."
+                return result
+
+            if (cert_key_size < (rsa_min_key_size if cert_algorithm == "RSA" else ecdsa_min_key_size)) or (
+                cert_hash.value < (rsa_min_hash.value if cert_algorithm == "RSA" else ecdsa_min_hash.value)
+            ):
+                failed_certs.append(f"{cert_name} (size: {cert_key_size}, hash: {cert_hash_method})")
+
+        if failed_certs:
+            result.reason = f"Following certificates do not meet required criteria: {', '.join(failed_certs)}."
+            return result
+
+        result.status = CheckStatus.SUCCESS
+        return result
+
     def get_content_db_version(self) -> Dict[str, str]:
         """Get Content DB version.
 
         # Returns
 
         dict(str): To keep the standard of all `get` methods returning a dictionary this value is also returned as a dictionary \
             in the following format:
```

### Comparing `panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/exceptions.py` & `panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 class WrongDataTypeException(Exception):
     """Used when passed configuration does not meet the data type requirements. Used in all modules."""
 
     pass
 
 
 class FirewallProxyException(Exception):
-    """Parent class for all exceptions comming from [FirewallProxy](/panos/docs/panos-upgrade-assurance/api/firewall_proxy)
+    """Parent class for all exceptions coming from [FirewallProxy](/panos/docs/panos-upgrade-assurance/api/firewall_proxy)
+    module."""
+
+    pass
+
+
+class CheckFirewallException(Exception):
+    """Parent class for all exceptions coming from [CheckFirewall](/panos/docs/panos-upgrade-assurance/api/check_firewall)
     module."""
 
     pass
 
 
 class SnapshotCompareException(Exception):
-    """Parent class for all exceptions comming from [SnapshotCompare](/panos/docs/panos-upgrade-assurance/api/snapshot_compare)
+    """Parent class for all exceptions coming from [SnapshotCompare](/panos/docs/panos-upgrade-assurance/api/snapshot_compare)
     module."""
 
     pass
 
 
 class UtilsException(Exception):
-    """Parent class for all exceptions comming from [Utils](/panos/docs/panos-upgrade-assurance/api/utils) module."""
+    """Parent class for all exceptions coming from [Utils](/panos/docs/panos-upgrade-assurance/api/utils) module."""
 
     pass
 
 
 class CommandRunFailedException(FirewallProxyException):
     """Used when a command run on a device does not return the `success` status."""
 
@@ -74,12 +81,11 @@
 
 class SnapshotSchemeMismatchException(SnapshotCompareException):
     """Used when a snapshot element contains different properties in both snapshots."""
 
     pass
 
 
-class UnknownParameterException(UtilsException):
-    """Used when one of the requested configuration parameters processed by [`ConfigParser`](#class-configparser) is not a valid
-    parameter."""
+class UnknownParameterException(CheckFirewallException, UtilsException):
+    """Used when one of the requested configuration parameters is not a valid."""
 
     pass
```

### Comparing `panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/firewall_proxy.py` & `panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/firewall_proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1019,7 +1019,69 @@
             "day": time_dict[4],
             "month": time_dict[3],
             "year": time_dict[7],
             "day_of_week": time_dict[2],
         }
 
         return result
+
+    def get_certificates(self) -> dict:
+        """Get information about certificates installed on a device.
+
+        This method retrieves every information that is available about a certificate except for the `private-key`.
+        This limitation is here due to security measures.
+
+        The actual API command is `show config running`.
+
+        # Returns
+
+        dict: Information about installed certificates, where key is the certificate name and value contains a dictionary of
+            certificate properties.
+
+        ```python showLineNumbers title="Sample output"
+        {
+            'acertificate': {
+                'algorithm': 'RSA',
+                'ca': 'no',
+                'common-name': 'cert',
+                'expiry-epoch': '1718699772',
+                'issuer': 'root',
+                'issuer-hash': '5198cade',
+                'not-valid-after': 'Jun 18 08:36:12 2024 GMT',
+                'not-valid-before': 'Jun 19 08:36:12 2023 GMT',
+                'public-key': '''-----BEGIN CERTIFICATE-----
+                                MIICiDCCAfGgAwIBAgIEWo92UzANBgkqhkiG9w0BAQsFADAPMQ0wCwYDVQQDDARy
+                                b290MB4XDTIzMDYxOTA4MzYxMloXDTI0MDYxODA4MzYxMlowDzENMAsGA1UEAwwE
+                                Y2VydDCCASIwDQYJKoZIhvcNAQEBBQADggEPADCCAQoCggEBAO7CKS7qrdSblk8E
+                                56Abkd9ikJVFDiDM7kC6l9ezKF4TK5q3tYbKywBiiNHw3DrRvuzwg3GsXDMSaUZZ
+                                ItsyOOxE4G6Ai48X0gSzAY5aQU2WY+1MErEWR0sMSxSVzNGkPVEDAQmI2KFPrzvX
+                                U4JGoOXwEsq4tH39nkj7Mo7VfKM/bsZ0obA8llt9VyjBCF1uN9+J1G+nY9mUzyEC
+                                yFemEexgMqWqmSY9DiL1xwFLfTog73zCvu9SfzvFzUEg+q/16RJF766AVb8TT27d
+                                KBowEpPdOqmWOXLbiZh9CzP4/GZZQuIWjS+DmSzI3nyDGF591iridlmmuTjPOyEy
+                                FnEfwsUCAwEAAaNtMGswCQYDVR0TBAIwADALBgNVHQ8EBAMCA7gwJwYDVR0lBCAw
+                                HgYIKwYBBQUHAwEGCCsGAQUFBwMCBggrBgEFBQcDBTAJBgNVHSMEAjAAMB0GA1Ud
+                                DgQWBBRmVL1rXamoHiqE1+MWuKhFx4y3lzANBgkqhkiG9w0BAQsFAAOBgQA2d4v4
+                                ABP1sOk603DTgwF3BmKGJLmdsbzD/GGYH1vs9INOxs/ftcbyld5uNJ8XCVZIX16l
+                                DbCDmPxxUkiQsjjGxKNKUh33xiqPWM8oqzGxbaLy9SK3YBl5leBPbI4rNozderlm
+                                BHR62OTIlfRtS0hwLUYkwdis/Tt0v0sc2hJxVw==
+                                -----END CERTIFICATE-----''',
+                'subject': 'cert',
+                'subject-hash': '5ec67661'
+            },
+            ...
+        }
+        ```
+
+        """
+        configuration = self.op_parser(cmd="show config running")
+        shared_config = configuration["config"]["shared"]
+
+        result = dict()
+
+        if "certificate" in shared_config:
+            certificates = shared_config["certificate"]["entry"]
+            for certificate in certificates if isinstance(certificates, list) else [certificates]:
+                certificate.pop("private-key")
+                cert_name = certificate.pop("@name")
+                result[cert_name] = certificate
+
+        return result
```

### Comparing `panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/snapshot_compare.py` & `panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/snapshot_compare.py`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/utils.py` & `panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     ACTIVE_SUPPORT = "active_support"
     CONTENT_VERSION = "content_version"
     SESSION_EXIST = "session_exist"
     ARP_ENTRY_EXIST = "arp_entry_exist"
     IPSEC_TUNNEL_STATUS = "ip_sec_tunnel_status"
     FREE_DISK_SPACE = "free_disk_space"
     MP_DP_CLOCK_SYNC = "planes_clock_sync"
+    CERTS = "certificates_requirements"
 
 
 class SnapType:
     """Class mapping the snapshot configuration strings to the commonly used variables.
 
     Snapshot configuration passed to the
     [`CheckFirewall`](/panos/docs/panos-upgrade-assurance/api/check_firewall#class-checkfirewall) class is in a form of a list of
@@ -63,14 +64,37 @@
 
     SUCCESS = 0
     FAIL = 1
     ERROR = 2
     SKIPPED = 3
 
 
+class SupportedHashes(Enum):
+    """Class listing supported hashing methods.
+
+    Algorithms listed here are order from less to most secure (this order follows many criteria, some of them are mentioned
+    [here](https://en.wikipedia.org/wiki/Hash_function_security_summary)).
+
+    By extending the `Enum` class we can easily use this class to compare two hashing methods in terms of their security,
+    for example:
+
+    ```python showLineNumbers title="Example"
+    bool(SupportedHashes.MD5.value < SupportedHashes.SHA256.value)
+    ```
+
+    would produce `True`.
+    """
+
+    MD5 = 1
+    SHA1 = 2
+    SHA256 = 3
+    SHA384 = 4
+    SHA512 = 5
+
+
 @dataclass
 class CheckResult:
     """Class representing the readiness check results.
 
     It provides two types of information:
 
     * `status` which represents information about the check outcome,
```

### Comparing `panos_upgrade_assurance-0.1.0/pyproject.toml` & `panos_upgrade_assurance-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "panos-upgrade-assurance"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Palo Alto Networks"]
 readme = "README.md"
 packages = [
     { include = "panos_upgrade_assurance" }
 ]
 classifiers = [
@@ -18,21 +18,22 @@
 "Bug Tracker" = "https://github.com/PaloAltoNetworks/pan-os-upgrade-assurance/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 pan-os-python = "^1.8"
 pan-python = "^0.17"
 xmltodict = "^0.13"
+pyopenssl = "^23.2"
 
 [tool.poetry.group.dev.dependencies]
 pydoc-markdown = "^4.6"
 flake8 = "^6.0"
 black = "^23.3"
 bandit = "^1.7"
-Flake8-pyproject = "^1.2"
+flake8-pyproject = "^1.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
 exclude_dirs = ["docs", ".venv", ".github", "docker_image", "dist"]
```

### Comparing `panos_upgrade_assurance-0.1.0/PKG-INFO` & `panos_upgrade_assurance-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: panos-upgrade-assurance
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Palo Alto Networks
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: pan-os-python (>=1.8,<2.0)
 Requires-Dist: pan-python (>=0.17,<0.18)
+Requires-Dist: pyopenssl (>=23.2,<24.0)
 Requires-Dist: xmltodict (>=0.13,<0.14)
 Description-Content-Type: text/markdown
 
 # PAN-OS Upgrade Assurance
 
 ## Overview
```

