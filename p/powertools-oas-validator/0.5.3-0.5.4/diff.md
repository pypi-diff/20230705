# Comparing `tmp/powertools_oas_validator-0.5.3.tar.gz` & `tmp/powertools_oas_validator-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powertools_oas_validator-0.5.3.tar", max compression
+gzip compressed data, was "powertools_oas_validator-0.5.4.tar", max compression
```

## Comparing `powertools_oas_validator-0.5.3.tar` & `powertools_oas_validator-0.5.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1077 2023-07-04 15:51:03.772420 powertools_oas_validator-0.5.3/LICENSE
--rw-r--r--   0        0        0     2327 2023-07-04 15:51:03.772420 powertools_oas_validator-0.5.3/README.md
--rw-r--r--   0        0        0       13 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/__init__.py
--rw-r--r--   0        0        0      252 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/exceptions.py
--rw-r--r--   0        0        0      928 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/middleware.py
--rw-r--r--   0        0        0      135 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/overrides/__init__.py
--rw-r--r--   0        0        0     1144 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/overrides/unmarshallers.py
--rw-r--r--   0        0        0     1031 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/overrides/validators.py
--rw-r--r--   0        0        0       13 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/services/__init__.py
--rw-r--r--   0        0        0     4720 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/services/error_handler.py
--rw-r--r--   0        0        0     3196 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/services/event_parser.py
--rw-r--r--   0        0        0     1120 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/services/spec_loader.py
--rw-r--r--   0        0        0      427 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/services/spec_parser.py
--rw-r--r--   0        0        0     2166 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/services/spec_validator.py
--rw-r--r--   0        0        0     1805 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/types.py
--rw-r--r--   0        0        0      975 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     3252 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.3/setup.py
--rw-r--r--   0        0        0     3177 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-04 16:21:27.114305 powertools_oas_validator-0.5.4/LICENSE
+-rw-r--r--   0        0        0     2375 2023-07-04 16:21:27.114305 powertools_oas_validator-0.5.4/README.md
+-rw-r--r--   0        0        0       13 2023-07-04 16:21:27.114305 powertools_oas_validator-0.5.4/powertools_oas_validator/__init__.py
+-rw-r--r--   0        0        0      252 2023-07-04 16:21:27.114305 powertools_oas_validator-0.5.4/powertools_oas_validator/exceptions.py
+-rw-r--r--   0        0        0      928 2023-07-04 16:21:27.114305 powertools_oas_validator-0.5.4/powertools_oas_validator/middleware.py
+-rw-r--r--   0        0        0      135 2023-07-04 16:21:27.114305 powertools_oas_validator-0.5.4/powertools_oas_validator/overrides/__init__.py
+-rw-r--r--   0        0        0     1144 2023-07-04 16:21:27.114305 powertools_oas_validator-0.5.4/powertools_oas_validator/overrides/unmarshallers.py
+-rw-r--r--   0        0        0     1031 2023-07-04 16:21:27.114305 powertools_oas_validator-0.5.4/powertools_oas_validator/overrides/validators.py
+-rw-r--r--   0        0        0       13 2023-07-04 16:21:27.114305 powertools_oas_validator-0.5.4/powertools_oas_validator/services/__init__.py
+-rw-r--r--   0        0        0     4720 2023-07-04 16:21:27.114305 powertools_oas_validator-0.5.4/powertools_oas_validator/services/error_handler.py
+-rw-r--r--   0        0        0     3196 2023-07-04 16:21:27.114305 powertools_oas_validator-0.5.4/powertools_oas_validator/services/event_parser.py
+-rw-r--r--   0        0        0     1120 2023-07-04 16:21:27.114305 powertools_oas_validator-0.5.4/powertools_oas_validator/services/spec_loader.py
+-rw-r--r--   0        0        0      427 2023-07-04 16:21:27.114305 powertools_oas_validator-0.5.4/powertools_oas_validator/services/spec_parser.py
+-rw-r--r--   0        0        0     2166 2023-07-04 16:21:27.114305 powertools_oas_validator-0.5.4/powertools_oas_validator/services/spec_validator.py
+-rw-r--r--   0        0        0     1805 2023-07-04 16:21:27.114305 powertools_oas_validator-0.5.4/powertools_oas_validator/types.py
+-rw-r--r--   0        0        0      975 2023-07-04 16:21:27.114305 powertools_oas_validator-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3300 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.4/setup.py
+-rw-r--r--   0        0        0     3225 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.4/PKG-INFO
```

### Comparing `powertools_oas_validator-0.5.3/LICENSE` & `powertools_oas_validator-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.3/README.md` & `powertools_oas_validator-0.5.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,146 +1,149 @@
 00000000: 2320 706f 7765 7274 6f6f 6c73 2d6f 6173  # powertools-oas
-00000010: 2d76 616c 6964 6174 6f72 0a3c 6272 3e5b  -validator.<br>[
-00000020: 215b 5079 5049 2076 6572 7369 6f6e 5d28  ![PyPI version](
-00000030: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
-00000040: 7279 2e69 6f2f 7079 2f70 6f77 6572 746f  ry.io/py/powerto
-00000050: 6f6c 732d 6f61 732d 7661 6c69 6461 746f  ols-oas-validato
-00000060: 722e 7376 6729 5d28 6874 7470 733a 2f2f  r.svg)](https://
-00000070: 6261 6467 652e 6675 7279 2e69 6f2f 7079  badge.fury.io/py
-00000080: 2f70 6f77 6572 746f 6f6c 732d 6f61 732d  /powertools-oas-
-00000090: 7661 6c69 6461 746f 7229 2021 5b52 656c  validator) ![Rel
-000000a0: 6561 7365 5d28 6874 7470 733a 2f2f 6769  ease](https://gi
-000000b0: 7468 7562 2e63 6f6d 2f52 6173 6d75 7346  thub.com/RasmusF
-000000c0: 616e 6765 6c2f 706f 7765 7274 6f6f 6c73  angel/powertools
-000000d0: 2d6f 6173 2d76 616c 6964 6174 6f72 2f77  -oas-validator/w
-000000e0: 6f72 6b66 6c6f 7773 2f52 656c 6561 7365  orkflows/Release
-000000f0: 2f62 6164 6765 2e73 7667 2920 215b 4349  /badge.svg) ![CI
-00000100: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000110: 2e63 6f6d 2f52 6173 6d75 7346 616e 6765  .com/RasmusFange
-00000120: 6c2f 706f 7765 7274 6f6f 6c73 2d6f 6173  l/powertools-oas
-00000130: 2d76 616c 6964 6174 6f72 2f77 6f72 6b66  -validator/workf
-00000140: 6c6f 7773 2f43 492f 6261 6467 652e 7376  lows/CI/badge.sv
-00000150: 6729 0a0a 2323 2049 6e74 726f 6475 6374  g)..## Introduct
-00000160: 696f 6e0a 0a5b 506f 7765 7274 6f6f 6c73  ion..[Powertools
-00000170: 2066 6f72 2041 5753 204c 616d 6264 6120   for AWS Lambda 
-00000180: 2850 7974 686f 6e29 5d28 6874 7470 733a  (Python)](https:
-00000190: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7773  //github.com/aws
-000001a0: 2d70 6f77 6572 746f 6f6c 732f 706f 7765  -powertools/powe
-000001b0: 7274 6f6f 6c73 2d6c 616d 6264 612d 7079  rtools-lambda-py
-000001c0: 7468 6f6e 2920 6973 2061 6e20 6177 6573  thon) is an awes
-000001d0: 6f6d 6520 7365 7420 6f66 2074 6f6f 6c73  ome set of tools
-000001e0: 2066 6f72 2073 7570 6572 6368 6172 6769   for superchargi
-000001f0: 6e67 2079 6f75 7220 6c61 6d62 6461 732e  ng your lambdas.
-00000200: 2050 6f77 6572 746f 6f6c 7320 7375 7070   Powertools supp
-00000210: 6f72 7473 2076 616c 6964 6174 696e 6720  orts validating 
-00000220: 696e 636f 6d69 6e67 2072 6571 7565 7374  incoming request
-00000230: 7320 286f 7220 6576 656e 7420 696e 2050  s (or event in P
-00000240: 5420 6c69 6e67 6f29 2061 6761 696e 7374  T lingo) against
-00000250: 205b 4a53 4f4e 5363 6865 6d61 5d28 6874   [JSONSchema](ht
-00000260: 7470 733a 2f2f 6a73 6f6e 2d73 6368 656d  tps://json-schem
-00000270: 612e 6f72 672f 2920 7768 6963 6820 6973  a.org/) which is
-00000280: 206e 6f74 2069 6465 616c 2069 6620 796f   not ideal if yo
-00000290: 7520 6172 6520 7573 696e 6720 4f70 656e  u are using Open
-000002a0: 4150 4920 7363 6865 6d61 7320 746f 2064  API schemas to d
-000002b0: 6566 696e 6520 796f 7572 2041 5049 2063  efine your API c
-000002c0: 6f6e 7472 6163 7473 2e0a 0a54 6865 202a  ontracts...The *
-000002d0: 506f 7765 7274 6f6f 6c73 204f 4153 2056  Powertools OAS V
-000002e0: 616c 6964 6174 6f72 2a20 6164 6473 2061  alidator* adds a
-000002f0: 2064 6563 6f72 6174 6f72 2074 6861 7420   decorator that 
-00000300: 796f 7520 6361 6e20 7573 6520 7769 7468  you can use with
-00000310: 2079 6f75 7220 6c61 6d62 6461 2068 616e   your lambda han
-00000320: 646c 6572 7320 616e 6420 6861 7665 2074  dlers and have t
-00000330: 6865 2065 7665 6e74 7320 7661 6c69 6461  he events valida
-00000340: 7465 6420 6167 6169 6e73 7420 616e 204f  ted against an O
-00000350: 7065 6e41 5049 2073 6368 656d 6120 696e  penAPI schema in
-00000360: 7374 6561 642e 0a0a 0a23 2320 496e 7374  stead....## Inst
-00000370: 616c 6c61 7469 6f6e 0a50 6f65 7472 793a  allation.Poetry:
-00000380: 0a60 706f 6574 7279 2061 6464 2070 6f77  .`poetry add pow
-00000390: 6572 746f 6f6c 732d 6f61 732d 7661 6c69  ertools-oas-vali
-000003a0: 6461 746f 7260 0a0a 5069 703a 0a60 7069  dator`..Pip:.`pi
-000003b0: 7020 696e 7374 616c 6c20 706f 7765 7274  p install powert
-000003c0: 6f6f 6c73 2d6f 6173 2d76 616c 6964 6174  ools-oas-validat
-000003d0: 6f72 600a 0a0a 2323 2055 7361 6765 0a44  or`...## Usage.D
-000003e0: 6563 6f72 6174 6520 796f 7572 2066 756e  ecorate your fun
-000003f0: 6374 696f 6e73 2077 6974 6820 6040 7661  ctions with `@va
-00000400: 6c69 6461 7465 5f72 6571 7565 7374 286f  lidate_request(o
-00000410: 6173 5f70 6174 683d 226f 7065 6e61 7069  as_path="openapi
-00000420: 2e79 616d 6c22 2960 2061 6e64 2079 6f75  .yaml")` and you
-00000430: 7220 7265 7175 6573 742f 6576 656e 7420  r request/event 
-00000440: 2861 6e64 2073 6368 656d 6129 2077 696c  (and schema) wil
-00000450: 6c20 6265 2076 616c 6964 6174 6564 206f  l be validated o
-00000460: 6e20 6120 7265 7175 6573 742e 0a0a 0a23  n a request....#
-00000470: 2323 204d 696e 696d 616c 2045 7861 6d70  ## Minimal Examp
-00000480: 6c65 0a0a 6060 6070 7974 686f 6e0a 6672  le..```python.fr
-00000490: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-000004a0: 2044 6963 740a 6672 6f6d 2061 7773 5f6c   Dict.from aws_l
-000004b0: 616d 6264 615f 706f 7765 7274 6f6f 6c73  ambda_powertools
-000004c0: 2e65 7665 6e74 5f68 616e 646c 6572 2069  .event_handler i
-000004d0: 6d70 6f72 7420 4150 4947 6174 6577 6179  mport APIGateway
-000004e0: 5265 7374 5265 736f 6c76 6572 2c20 5265  RestResolver, Re
-000004f0: 7370 6f6e 7365 0a66 726f 6d20 6177 735f  sponse.from aws_
-00000500: 6c61 6d62 6461 5f70 6f77 6572 746f 6f6c  lambda_powertool
-00000510: 732e 7574 696c 6974 6965 732e 7479 7069  s.utilities.typi
-00000520: 6e67 2069 6d70 6f72 7420 4c61 6d62 6461  ng import Lambda
-00000530: 436f 6e74 6578 740a 6672 6f6d 2070 6f77  Context.from pow
-00000540: 6572 746f 6f6c 735f 6f61 735f 7661 6c69  ertools_oas_vali
-00000550: 6461 746f 722e 6d69 6464 6c65 7761 7265  dator.middleware
-00000560: 2069 6d70 6f72 7420 7661 6c69 6461 7465   import validate
-00000570: 5f72 6571 7565 7374 0a0a 0a61 7070 203d  _request...app =
-00000580: 2041 5049 4761 7465 7761 7952 6573 7452   APIGatewayRestR
-00000590: 6573 6f6c 7665 7228 290a 0a40 6170 702e  esolver()..@app.
-000005a0: 706f 7374 2822 2f65 7861 6d70 6c65 2229  post("/example")
-000005b0: 0a64 6566 2065 7861 6d70 6c65 2829 202d  .def example() -
-000005c0: 3e20 5265 7370 6f6e 7365 3a0a 2020 2e2e  > Response:.  ..
-000005d0: 2e0a 0a40 7661 6c69 6461 7465 5f72 6571  ...@validate_req
-000005e0: 7565 7374 286f 6173 5f70 6174 683d 226f  uest(oas_path="o
-000005f0: 7065 6e61 7069 2e79 616d 6c22 290a 6465  penapi.yaml").de
-00000600: 6620 6c61 6d62 6461 5f68 616e 646c 6572  f lambda_handler
-00000610: 2865 7665 6e74 3a20 4469 6374 2c20 636f  (event: Dict, co
-00000620: 6e74 6578 743a 204c 616d 6264 6143 6f6e  ntext: LambdaCon
-00000630: 7465 7874 2920 2d3e 2044 6963 743a 0a20  text) -> Dict:. 
-00000640: 2020 2072 6573 706f 6e73 6520 3d20 6170     response = ap
-00000650: 702e 7265 736f 6c76 6528 6576 656e 742c  p.resolve(event,
-00000660: 2063 6f6e 7465 7874 290a 0a20 2020 2072   context)..    r
-00000670: 6574 7572 6e20 7265 7370 6f6e 7365 0a60  eturn response.`
-00000680: 6060 0a0a 2323 2045 7272 6f72 2048 616e  ``..## Error Han
-00000690: 646c 696e 670a 4966 2074 6865 2076 616c  dling.If the val
-000006a0: 6964 6174 696f 6e20 6661 696c 732c 2074  idation fails, t
-000006b0: 6865 2064 6563 6f72 6174 6f72 2074 6872  he decorator thr
-000006c0: 6f77 7320 6120 6053 6368 656d 6156 616c  ows a `SchemaVal
-000006d0: 6964 6174 6f6e 4572 726f 7260 2077 6974  idatonError` wit
-000006e0: 6820 7265 6c65 7661 6e74 2069 6e66 6f72  h relevant infor
-000006f0: 6d61 7469 6f6e 2061 626f 7574 2074 6865  mation about the
-00000700: 2066 6169 6c65 6420 7661 6c69 6461 7469   failed validati
-00000710: 6f6e 2e0a 0a0a 2323 204b 6e6f 7720 4973  on....## Know Is
-00000720: 7375 6573 0a57 6869 6c65 2061 6c6c 2076  sues.While all v
-00000730: 616c 6964 6174 696f 6e20 6572 726f 7273  alidation errors
-00000740: 2061 7265 2063 6175 6768 742c 2074 6865   are caught, the
-00000750: 7265 2069 7320 6f6e 6c79 206c 696d 6974  re is only limit
-00000760: 6564 2069 6e66 6f72 6d61 7469 6f6e 2061  ed information a
-00000770: 626f 7574 2074 6865 2076 6172 696f 7573  bout the various
-00000780: 2065 7272 6f72 732e 2054 6865 2064 6563   errors. The dec
-00000790: 6f72 6174 6f72 2077 696c 6c20 7472 7920  orator will try 
-000007a0: 6974 7320 6265 7374 2074 6f20 7468 726f  its best to thro
-000007b0: 7720 6120 6053 6368 656d 6156 616c 6964  w a `SchemaValid
-000007c0: 6174 6f6e 4572 726f 7260 0a28 7361 6d65  atonError`.(same
-000007d0: 2061 7320 7468 6520 506f 7765 7274 6f6f   as the Powertoo
-000007e0: 6c73 2076 616c 6964 6174 6f72 2077 6f75  ls validator wou
-000007f0: 6c64 292c 2077 6974 6820 6173 206d 7563  ld), with as muc
-00000800: 6820 6f66 2074 6865 206f 7074 696f 6e61  h of the optiona
-00000810: 6c20 6174 7472 6962 7574 6573 2061 7320  l attributes as 
-00000820: 706f 7373 6962 6c65 2e0a 0a49 6e20 7375  possible...In su
-00000830: 6d6d 6172 792c 2069 7420 6973 2070 6f73  mmary, it is pos
-00000840: 7369 626c 6520 7468 6174 206e 6f74 2061  sible that not a
-00000850: 6c6c 2060 5363 6865 6d61 5661 6c69 6461  ll `SchemaValida
-00000860: 7469 6f6e 4572 726f 7273 6027 7320 7769  tionErrors`'s wi
-00000870: 6c6c 2068 6176 6520 6120 6e69 6365 2076  ll have a nice v
-00000880: 616c 6964 6174 696f 6e20 6d65 7373 6167  alidation messag
-00000890: 652c 2069 6e20 6361 7365 2079 6f75 2072  e, in case you r
-000008a0: 656c 7920 6f6e 2070 6970 696e 6720 6974  ely on piping it
-000008b0: 2073 7472 6169 6768 7420 6261 636b 2074   straight back t
-000008c0: 6f20 7468 6520 636c 6965 6e74 2e0a 0a0a  o the client....
-000008d0: 2323 2043 6f6e 7472 6962 7574 696f 6e73  ## Contributions
-000008e0: 0a50 6c65 6173 6520 6d61 6b65 2061 2070  .Please make a p
-000008f0: 756c 6c20 7265 7175 6573 7420 616e 6420  ull request and 
-00000900: 4920 7769 6c6c 2072 6576 6965 7720 6974  I will review it
-00000910: 2041 5341 502e 0a                         ASAP..
+00000010: 2d76 616c 6964 6174 6f72 0a3c 6272 3e3c  -validator.<br><
+00000020: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000030: 6261 6467 652e 6675 7279 2e69 6f2f 7079  badge.fury.io/py
+00000040: 2f70 6f77 6572 746f 6f6c 732d 6f61 732d  /powertools-oas-
+00000050: 7661 6c69 6461 746f 7222 3e3c 696d 6720  validator"><img 
+00000060: 7372 633d 2268 7474 7073 3a2f 2f62 6164  src="https://bad
+00000070: 6765 2e66 7572 792e 696f 2f70 792f 706f  ge.fury.io/py/po
+00000080: 7765 7274 6f6f 6c73 2d6f 6173 2d76 616c  wertools-oas-val
+00000090: 6964 6174 6f72 2e73 7667 2220 616c 743d  idator.svg" alt=
+000000a0: 2250 7950 4920 7665 7273 696f 6e22 3e3c  "PyPI version"><
+000000b0: 2f61 3e20 2021 5b43 495d 2868 7474 7073  /a>  ![CI](https
+000000c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5261  ://github.com/Ra
+000000d0: 736d 7573 4661 6e67 656c 2f70 6f77 6572  smusFangel/power
+000000e0: 746f 6f6c 732d 6f61 732d 7661 6c69 6461  tools-oas-valida
+000000f0: 746f 722f 776f 726b 666c 6f77 732f 4349  tor/workflows/CI
+00000100: 2f62 6164 6765 2e73 7667 2920 3c69 6d67  /badge.svg) <img
+00000110: 2073 7263 3d22 6874 7470 733a 2f2f 636f   src="https://co
+00000120: 7665 7261 6c6c 732e 696f 2f72 6570 6f73  veralls.io/repos
+00000130: 2f52 6173 6d75 7346 616e 6765 6c2f 706f  /RasmusFangel/po
+00000140: 7765 7274 6f6f 6c73 2d6f 6173 2d76 616c  wertools-oas-val
+00000150: 6964 6174 6f72 2f62 6164 6765 2e73 7667  idator/badge.svg
+00000160: 3f62 7261 6e63 683d 6d61 696e 2220 616c  ?branch=main" al
+00000170: 743d 2243 6f76 6572 616c 6c73 223e 3c2f  t="Coveralls"></
+00000180: 613e 0a0a 2323 2049 6e74 726f 6475 6374  a>..## Introduct
+00000190: 696f 6e0a 0a5b 506f 7765 7274 6f6f 6c73  ion..[Powertools
+000001a0: 2066 6f72 2041 5753 204c 616d 6264 6120   for AWS Lambda 
+000001b0: 2850 7974 686f 6e29 5d28 6874 7470 733a  (Python)](https:
+000001c0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7773  //github.com/aws
+000001d0: 2d70 6f77 6572 746f 6f6c 732f 706f 7765  -powertools/powe
+000001e0: 7274 6f6f 6c73 2d6c 616d 6264 612d 7079  rtools-lambda-py
+000001f0: 7468 6f6e 2920 6973 2061 6e20 6177 6573  thon) is an awes
+00000200: 6f6d 6520 7365 7420 6f66 2074 6f6f 6c73  ome set of tools
+00000210: 2066 6f72 2073 7570 6572 6368 6172 6769   for superchargi
+00000220: 6e67 2079 6f75 7220 6c61 6d62 6461 732e  ng your lambdas.
+00000230: 2050 6f77 6572 746f 6f6c 7320 7375 7070   Powertools supp
+00000240: 6f72 7473 2076 616c 6964 6174 696e 6720  orts validating 
+00000250: 696e 636f 6d69 6e67 2072 6571 7565 7374  incoming request
+00000260: 7320 286f 7220 6576 656e 7420 696e 2050  s (or event in P
+00000270: 5420 6c69 6e67 6f29 2061 6761 696e 7374  T lingo) against
+00000280: 205b 4a53 4f4e 5363 6865 6d61 5d28 6874   [JSONSchema](ht
+00000290: 7470 733a 2f2f 6a73 6f6e 2d73 6368 656d  tps://json-schem
+000002a0: 612e 6f72 672f 2920 7768 6963 6820 6973  a.org/) which is
+000002b0: 206e 6f74 2069 6465 616c 2069 6620 796f   not ideal if yo
+000002c0: 7520 6172 6520 7573 696e 6720 4f70 656e  u are using Open
+000002d0: 4150 4920 7363 6865 6d61 7320 746f 2064  API schemas to d
+000002e0: 6566 696e 6520 796f 7572 2041 5049 2063  efine your API c
+000002f0: 6f6e 7472 6163 7473 2e0a 0a54 6865 202a  ontracts...The *
+00000300: 506f 7765 7274 6f6f 6c73 204f 4153 2056  Powertools OAS V
+00000310: 616c 6964 6174 6f72 2a20 6164 6473 2061  alidator* adds a
+00000320: 2064 6563 6f72 6174 6f72 2074 6861 7420   decorator that 
+00000330: 796f 7520 6361 6e20 7573 6520 7769 7468  you can use with
+00000340: 2079 6f75 7220 6c61 6d62 6461 2068 616e   your lambda han
+00000350: 646c 6572 7320 616e 6420 6861 7665 2074  dlers and have t
+00000360: 6865 2065 7665 6e74 7320 7661 6c69 6461  he events valida
+00000370: 7465 6420 6167 6169 6e73 7420 616e 204f  ted against an O
+00000380: 7065 6e41 5049 2073 6368 656d 6120 696e  penAPI schema in
+00000390: 7374 6561 642e 0a0a 0a23 2320 496e 7374  stead....## Inst
+000003a0: 616c 6c61 7469 6f6e 0a50 6f65 7472 793a  allation.Poetry:
+000003b0: 0a60 706f 6574 7279 2061 6464 2070 6f77  .`poetry add pow
+000003c0: 6572 746f 6f6c 732d 6f61 732d 7661 6c69  ertools-oas-vali
+000003d0: 6461 746f 7260 0a0a 5069 703a 0a60 7069  dator`..Pip:.`pi
+000003e0: 7020 696e 7374 616c 6c20 706f 7765 7274  p install powert
+000003f0: 6f6f 6c73 2d6f 6173 2d76 616c 6964 6174  ools-oas-validat
+00000400: 6f72 600a 0a0a 2323 2055 7361 6765 0a44  or`...## Usage.D
+00000410: 6563 6f72 6174 6520 796f 7572 2066 756e  ecorate your fun
+00000420: 6374 696f 6e73 2077 6974 6820 6040 7661  ctions with `@va
+00000430: 6c69 6461 7465 5f72 6571 7565 7374 286f  lidate_request(o
+00000440: 6173 5f70 6174 683d 226f 7065 6e61 7069  as_path="openapi
+00000450: 2e79 616d 6c22 2960 2061 6e64 2079 6f75  .yaml")` and you
+00000460: 7220 7265 7175 6573 742f 6576 656e 7420  r request/event 
+00000470: 2861 6e64 2073 6368 656d 6129 2077 696c  (and schema) wil
+00000480: 6c20 6265 2076 616c 6964 6174 6564 206f  l be validated o
+00000490: 6e20 6120 7265 7175 6573 742e 0a0a 0a23  n a request....#
+000004a0: 2323 204d 696e 696d 616c 2045 7861 6d70  ## Minimal Examp
+000004b0: 6c65 0a0a 6060 6070 7974 686f 6e0a 6672  le..```python.fr
+000004c0: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+000004d0: 2044 6963 740a 6672 6f6d 2061 7773 5f6c   Dict.from aws_l
+000004e0: 616d 6264 615f 706f 7765 7274 6f6f 6c73  ambda_powertools
+000004f0: 2e65 7665 6e74 5f68 616e 646c 6572 2069  .event_handler i
+00000500: 6d70 6f72 7420 4150 4947 6174 6577 6179  mport APIGateway
+00000510: 5265 7374 5265 736f 6c76 6572 2c20 5265  RestResolver, Re
+00000520: 7370 6f6e 7365 0a66 726f 6d20 6177 735f  sponse.from aws_
+00000530: 6c61 6d62 6461 5f70 6f77 6572 746f 6f6c  lambda_powertool
+00000540: 732e 7574 696c 6974 6965 732e 7479 7069  s.utilities.typi
+00000550: 6e67 2069 6d70 6f72 7420 4c61 6d62 6461  ng import Lambda
+00000560: 436f 6e74 6578 740a 6672 6f6d 2070 6f77  Context.from pow
+00000570: 6572 746f 6f6c 735f 6f61 735f 7661 6c69  ertools_oas_vali
+00000580: 6461 746f 722e 6d69 6464 6c65 7761 7265  dator.middleware
+00000590: 2069 6d70 6f72 7420 7661 6c69 6461 7465   import validate
+000005a0: 5f72 6571 7565 7374 0a0a 0a61 7070 203d  _request...app =
+000005b0: 2041 5049 4761 7465 7761 7952 6573 7452   APIGatewayRestR
+000005c0: 6573 6f6c 7665 7228 290a 0a40 6170 702e  esolver()..@app.
+000005d0: 706f 7374 2822 2f65 7861 6d70 6c65 2229  post("/example")
+000005e0: 0a64 6566 2065 7861 6d70 6c65 2829 202d  .def example() -
+000005f0: 3e20 5265 7370 6f6e 7365 3a0a 2020 2e2e  > Response:.  ..
+00000600: 2e0a 0a40 7661 6c69 6461 7465 5f72 6571  ...@validate_req
+00000610: 7565 7374 286f 6173 5f70 6174 683d 226f  uest(oas_path="o
+00000620: 7065 6e61 7069 2e79 616d 6c22 290a 6465  penapi.yaml").de
+00000630: 6620 6c61 6d62 6461 5f68 616e 646c 6572  f lambda_handler
+00000640: 2865 7665 6e74 3a20 4469 6374 2c20 636f  (event: Dict, co
+00000650: 6e74 6578 743a 204c 616d 6264 6143 6f6e  ntext: LambdaCon
+00000660: 7465 7874 2920 2d3e 2044 6963 743a 0a20  text) -> Dict:. 
+00000670: 2020 2072 6573 706f 6e73 6520 3d20 6170     response = ap
+00000680: 702e 7265 736f 6c76 6528 6576 656e 742c  p.resolve(event,
+00000690: 2063 6f6e 7465 7874 290a 0a20 2020 2072   context)..    r
+000006a0: 6574 7572 6e20 7265 7370 6f6e 7365 0a60  eturn response.`
+000006b0: 6060 0a0a 2323 2045 7272 6f72 2048 616e  ``..## Error Han
+000006c0: 646c 696e 670a 4966 2074 6865 2076 616c  dling.If the val
+000006d0: 6964 6174 696f 6e20 6661 696c 732c 2074  idation fails, t
+000006e0: 6865 2064 6563 6f72 6174 6f72 2074 6872  he decorator thr
+000006f0: 6f77 7320 6120 6053 6368 656d 6156 616c  ows a `SchemaVal
+00000700: 6964 6174 6f6e 4572 726f 7260 2077 6974  idatonError` wit
+00000710: 6820 7265 6c65 7661 6e74 2069 6e66 6f72  h relevant infor
+00000720: 6d61 7469 6f6e 2061 626f 7574 2074 6865  mation about the
+00000730: 2066 6169 6c65 6420 7661 6c69 6461 7469   failed validati
+00000740: 6f6e 2e0a 0a0a 2323 204b 6e6f 7720 4973  on....## Know Is
+00000750: 7375 6573 0a57 6869 6c65 2061 6c6c 2076  sues.While all v
+00000760: 616c 6964 6174 696f 6e20 6572 726f 7273  alidation errors
+00000770: 2061 7265 2063 6175 6768 742c 2074 6865   are caught, the
+00000780: 7265 2069 7320 6f6e 6c79 206c 696d 6974  re is only limit
+00000790: 6564 2069 6e66 6f72 6d61 7469 6f6e 2061  ed information a
+000007a0: 626f 7574 2074 6865 2076 6172 696f 7573  bout the various
+000007b0: 2065 7272 6f72 732e 2054 6865 2064 6563   errors. The dec
+000007c0: 6f72 6174 6f72 2077 696c 6c20 7472 7920  orator will try 
+000007d0: 6974 7320 6265 7374 2074 6f20 7468 726f  its best to thro
+000007e0: 7720 6120 6053 6368 656d 6156 616c 6964  w a `SchemaValid
+000007f0: 6174 6f6e 4572 726f 7260 0a28 7361 6d65  atonError`.(same
+00000800: 2061 7320 7468 6520 506f 7765 7274 6f6f   as the Powertoo
+00000810: 6c73 2076 616c 6964 6174 6f72 2077 6f75  ls validator wou
+00000820: 6c64 292c 2077 6974 6820 6173 206d 7563  ld), with as muc
+00000830: 6820 6f66 2074 6865 206f 7074 696f 6e61  h of the optiona
+00000840: 6c20 6174 7472 6962 7574 6573 2061 7320  l attributes as 
+00000850: 706f 7373 6962 6c65 2e0a 0a49 6e20 7375  possible...In su
+00000860: 6d6d 6172 792c 2069 7420 6973 2070 6f73  mmary, it is pos
+00000870: 7369 626c 6520 7468 6174 206e 6f74 2061  sible that not a
+00000880: 6c6c 2060 5363 6865 6d61 5661 6c69 6461  ll `SchemaValida
+00000890: 7469 6f6e 4572 726f 7273 6027 7320 7769  tionErrors`'s wi
+000008a0: 6c6c 2068 6176 6520 6120 6e69 6365 2076  ll have a nice v
+000008b0: 616c 6964 6174 696f 6e20 6d65 7373 6167  alidation messag
+000008c0: 652c 2069 6e20 6361 7365 2079 6f75 2072  e, in case you r
+000008d0: 656c 7920 6f6e 2070 6970 696e 6720 6974  ely on piping it
+000008e0: 2073 7472 6169 6768 7420 6261 636b 2074   straight back t
+000008f0: 6f20 7468 6520 636c 6965 6e74 2e0a 0a0a  o the client....
+00000900: 2323 2043 6f6e 7472 6962 7574 696f 6e73  ## Contributions
+00000910: 0a50 6c65 6173 6520 6d61 6b65 2061 2070  .Please make a p
+00000920: 756c 6c20 7265 7175 6573 7420 616e 6420  ull request and 
+00000930: 4920 7769 6c6c 2072 6576 6965 7720 6974  I will review it
+00000940: 2041 5341 502e 0a                         ASAP..
```

### Comparing `powertools_oas_validator-0.5.3/powertools_oas_validator/middleware.py` & `powertools_oas_validator-0.5.4/powertools_oas_validator/middleware.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.3/powertools_oas_validator/overrides/unmarshallers.py` & `powertools_oas_validator-0.5.4/powertools_oas_validator/overrides/unmarshallers.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.3/powertools_oas_validator/overrides/validators.py` & `powertools_oas_validator-0.5.4/powertools_oas_validator/overrides/validators.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.3/powertools_oas_validator/services/error_handler.py` & `powertools_oas_validator-0.5.4/powertools_oas_validator/services/error_handler.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.3/powertools_oas_validator/services/event_parser.py` & `powertools_oas_validator-0.5.4/powertools_oas_validator/services/event_parser.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.3/powertools_oas_validator/services/spec_loader.py` & `powertools_oas_validator-0.5.4/powertools_oas_validator/services/spec_loader.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.3/powertools_oas_validator/services/spec_validator.py` & `powertools_oas_validator-0.5.4/powertools_oas_validator/services/spec_validator.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.3/powertools_oas_validator/types.py` & `powertools_oas_validator-0.5.4/powertools_oas_validator/types.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.3/pyproject.toml` & `powertools_oas_validator-0.5.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "powertools-oas-validator"
-version = "0.5.3"
+version = "0.5.4"
 description = ""
 authors = ["Rasmus Hansen <R.FangelHansen@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 homepage = "https://github.com/RasmusFangel/powertools-oas-validator"
 repository = "https://github.com/RasmusFangel/powertools-oas-validator"
```

### Comparing `powertools_oas_validator-0.5.3/setup.py` & `powertools_oas_validator-0.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,184 +21,187 @@
 00000140: 2e30 2e30 272c 0a20 276f 7065 6e61 7069  .0.0',. 'openapi
 00000150: 2d63 6f72 653e 3d30 2e31 372e 322c 3c30  -core>=0.17.2,<0
 00000160: 2e31 382e 3027 5d0a 0a73 6574 7570 5f6b  .18.0']..setup_k
 00000170: 7761 7267 7320 3d20 7b0a 2020 2020 276e  wargs = {.    'n
 00000180: 616d 6527 3a20 2770 6f77 6572 746f 6f6c  ame': 'powertool
 00000190: 732d 6f61 732d 7661 6c69 6461 746f 7227  s-oas-validator'
 000001a0: 2c0a 2020 2020 2776 6572 7369 6f6e 273a  ,.    'version':
-000001b0: 2027 302e 352e 3327 2c0a 2020 2020 2764   '0.5.3',.    'd
+000001b0: 2027 302e 352e 3427 2c0a 2020 2020 2764   '0.5.4',.    'd
 000001c0: 6573 6372 6970 7469 6f6e 273a 2027 272c  escription': '',
 000001d0: 0a20 2020 2027 6c6f 6e67 5f64 6573 6372  .    'long_descr
 000001e0: 6970 7469 6f6e 273a 2027 2320 706f 7765  iption': '# powe
 000001f0: 7274 6f6f 6c73 2d6f 6173 2d76 616c 6964  rtools-oas-valid
-00000200: 6174 6f72 5c6e 3c62 723e 5b21 5b50 7950  ator\n<br>[![PyP
-00000210: 4920 7665 7273 696f 6e5d 2868 7474 7073  I version](https
-00000220: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
-00000230: 2f70 792f 706f 7765 7274 6f6f 6c73 2d6f  /py/powertools-o
-00000240: 6173 2d76 616c 6964 6174 6f72 2e73 7667  as-validator.svg
-00000250: 295d 2868 7474 7073 3a2f 2f62 6164 6765  )](https://badge
-00000260: 2e66 7572 792e 696f 2f70 792f 706f 7765  .fury.io/py/powe
-00000270: 7274 6f6f 6c73 2d6f 6173 2d76 616c 6964  rtools-oas-valid
-00000280: 6174 6f72 2920 215b 5265 6c65 6173 655d  ator) ![Release]
-00000290: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000002a0: 636f 6d2f 5261 736d 7573 4661 6e67 656c  com/RasmusFangel
-000002b0: 2f70 6f77 6572 746f 6f6c 732d 6f61 732d  /powertools-oas-
-000002c0: 7661 6c69 6461 746f 722f 776f 726b 666c  validator/workfl
-000002d0: 6f77 732f 5265 6c65 6173 652f 6261 6467  ows/Release/badg
-000002e0: 652e 7376 6729 2021 5b43 495d 2868 7474  e.svg) ![CI](htt
-000002f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000300: 5261 736d 7573 4661 6e67 656c 2f70 6f77  RasmusFangel/pow
-00000310: 6572 746f 6f6c 732d 6f61 732d 7661 6c69  ertools-oas-vali
-00000320: 6461 746f 722f 776f 726b 666c 6f77 732f  dator/workflows/
-00000330: 4349 2f62 6164 6765 2e73 7667 295c 6e5c  CI/badge.svg)\n\
-00000340: 6e23 2320 496e 7472 6f64 7563 7469 6f6e  n## Introduction
-00000350: 5c6e 5c6e 5b50 6f77 6572 746f 6f6c 7320  \n\n[Powertools 
-00000360: 666f 7220 4157 5320 4c61 6d62 6461 2028  for AWS Lambda (
-00000370: 5079 7468 6f6e 295d 2868 7474 7073 3a2f  Python)](https:/
-00000380: 2f67 6974 6875 622e 636f 6d2f 6177 732d  /github.com/aws-
-00000390: 706f 7765 7274 6f6f 6c73 2f70 6f77 6572  powertools/power
-000003a0: 746f 6f6c 732d 6c61 6d62 6461 2d70 7974  tools-lambda-pyt
-000003b0: 686f 6e29 2069 7320 616e 2061 7765 736f  hon) is an aweso
-000003c0: 6d65 2073 6574 206f 6620 746f 6f6c 7320  me set of tools 
-000003d0: 666f 7220 7375 7065 7263 6861 7267 696e  for superchargin
-000003e0: 6720 796f 7572 206c 616d 6264 6173 2e20  g your lambdas. 
-000003f0: 506f 7765 7274 6f6f 6c73 2073 7570 706f  Powertools suppo
-00000400: 7274 7320 7661 6c69 6461 7469 6e67 2069  rts validating i
-00000410: 6e63 6f6d 696e 6720 7265 7175 6573 7473  ncoming requests
-00000420: 2028 6f72 2065 7665 6e74 2069 6e20 5054   (or event in PT
-00000430: 206c 696e 676f 2920 6167 6169 6e73 7420   lingo) against 
-00000440: 5b4a 534f 4e53 6368 656d 615d 2868 7474  [JSONSchema](htt
-00000450: 7073 3a2f 2f6a 736f 6e2d 7363 6865 6d61  ps://json-schema
-00000460: 2e6f 7267 2f29 2077 6869 6368 2069 7320  .org/) which is 
-00000470: 6e6f 7420 6964 6561 6c20 6966 2079 6f75  not ideal if you
-00000480: 2061 7265 2075 7369 6e67 204f 7065 6e41   are using OpenA
-00000490: 5049 2073 6368 656d 6173 2074 6f20 6465  PI schemas to de
-000004a0: 6669 6e65 2079 6f75 7220 4150 4920 636f  fine your API co
-000004b0: 6e74 7261 6374 732e 5c6e 5c6e 5468 6520  ntracts.\n\nThe 
-000004c0: 2a50 6f77 6572 746f 6f6c 7320 4f41 5320  *Powertools OAS 
-000004d0: 5661 6c69 6461 746f 722a 2061 6464 7320  Validator* adds 
-000004e0: 6120 6465 636f 7261 746f 7220 7468 6174  a decorator that
-000004f0: 2079 6f75 2063 616e 2075 7365 2077 6974   you can use wit
-00000500: 6820 796f 7572 206c 616d 6264 6120 6861  h your lambda ha
-00000510: 6e64 6c65 7273 2061 6e64 2068 6176 6520  ndlers and have 
-00000520: 7468 6520 6576 656e 7473 2076 616c 6964  the events valid
-00000530: 6174 6564 2061 6761 696e 7374 2061 6e20  ated against an 
-00000540: 4f70 656e 4150 4920 7363 6865 6d61 2069  OpenAPI schema i
-00000550: 6e73 7465 6164 2e5c 6e5c 6e5c 6e23 2320  nstead.\n\n\n## 
-00000560: 496e 7374 616c 6c61 7469 6f6e 5c6e 506f  Installation\nPo
-00000570: 6574 7279 3a5c 6e60 706f 6574 7279 2061  etry:\n`poetry a
-00000580: 6464 2070 6f77 6572 746f 6f6c 732d 6f61  dd powertools-oa
-00000590: 732d 7661 6c69 6461 746f 7260 5c6e 5c6e  s-validator`\n\n
-000005a0: 5069 703a 5c6e 6070 6970 2069 6e73 7461  Pip:\n`pip insta
-000005b0: 6c6c 2070 6f77 6572 746f 6f6c 732d 6f61  ll powertools-oa
+00000200: 6174 6f72 5c6e 3c62 723e 3c61 2068 7265  ator\n<br><a hre
+00000210: 663d 2268 7474 7073 3a2f 2f62 6164 6765  f="https://badge
+00000220: 2e66 7572 792e 696f 2f70 792f 706f 7765  .fury.io/py/powe
+00000230: 7274 6f6f 6c73 2d6f 6173 2d76 616c 6964  rtools-oas-valid
+00000240: 6174 6f72 223e 3c69 6d67 2073 7263 3d22  ator"><img src="
+00000250: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
+00000260: 7279 2e69 6f2f 7079 2f70 6f77 6572 746f  ry.io/py/powerto
+00000270: 6f6c 732d 6f61 732d 7661 6c69 6461 746f  ols-oas-validato
+00000280: 722e 7376 6722 2061 6c74 3d22 5079 5049  r.svg" alt="PyPI
+00000290: 2076 6572 7369 6f6e 223e 3c2f 613e 2020   version"></a>  
+000002a0: 215b 4349 5d28 6874 7470 733a 2f2f 6769  ![CI](https://gi
+000002b0: 7468 7562 2e63 6f6d 2f52 6173 6d75 7346  thub.com/RasmusF
+000002c0: 616e 6765 6c2f 706f 7765 7274 6f6f 6c73  angel/powertools
+000002d0: 2d6f 6173 2d76 616c 6964 6174 6f72 2f77  -oas-validator/w
+000002e0: 6f72 6b66 6c6f 7773 2f43 492f 6261 6467  orkflows/CI/badg
+000002f0: 652e 7376 6729 203c 696d 6720 7372 633d  e.svg) <img src=
+00000300: 2268 7474 7073 3a2f 2f63 6f76 6572 616c  "https://coveral
+00000310: 6c73 2e69 6f2f 7265 706f 732f 5261 736d  ls.io/repos/Rasm
+00000320: 7573 4661 6e67 656c 2f70 6f77 6572 746f  usFangel/powerto
+00000330: 6f6c 732d 6f61 732d 7661 6c69 6461 746f  ols-oas-validato
+00000340: 722f 6261 6467 652e 7376 673f 6272 616e  r/badge.svg?bran
+00000350: 6368 3d6d 6169 6e22 2061 6c74 3d22 436f  ch=main" alt="Co
+00000360: 7665 7261 6c6c 7322 3e3c 2f61 3e5c 6e5c  veralls"></a>\n\
+00000370: 6e23 2320 496e 7472 6f64 7563 7469 6f6e  n## Introduction
+00000380: 5c6e 5c6e 5b50 6f77 6572 746f 6f6c 7320  \n\n[Powertools 
+00000390: 666f 7220 4157 5320 4c61 6d62 6461 2028  for AWS Lambda (
+000003a0: 5079 7468 6f6e 295d 2868 7474 7073 3a2f  Python)](https:/
+000003b0: 2f67 6974 6875 622e 636f 6d2f 6177 732d  /github.com/aws-
+000003c0: 706f 7765 7274 6f6f 6c73 2f70 6f77 6572  powertools/power
+000003d0: 746f 6f6c 732d 6c61 6d62 6461 2d70 7974  tools-lambda-pyt
+000003e0: 686f 6e29 2069 7320 616e 2061 7765 736f  hon) is an aweso
+000003f0: 6d65 2073 6574 206f 6620 746f 6f6c 7320  me set of tools 
+00000400: 666f 7220 7375 7065 7263 6861 7267 696e  for superchargin
+00000410: 6720 796f 7572 206c 616d 6264 6173 2e20  g your lambdas. 
+00000420: 506f 7765 7274 6f6f 6c73 2073 7570 706f  Powertools suppo
+00000430: 7274 7320 7661 6c69 6461 7469 6e67 2069  rts validating i
+00000440: 6e63 6f6d 696e 6720 7265 7175 6573 7473  ncoming requests
+00000450: 2028 6f72 2065 7665 6e74 2069 6e20 5054   (or event in PT
+00000460: 206c 696e 676f 2920 6167 6169 6e73 7420   lingo) against 
+00000470: 5b4a 534f 4e53 6368 656d 615d 2868 7474  [JSONSchema](htt
+00000480: 7073 3a2f 2f6a 736f 6e2d 7363 6865 6d61  ps://json-schema
+00000490: 2e6f 7267 2f29 2077 6869 6368 2069 7320  .org/) which is 
+000004a0: 6e6f 7420 6964 6561 6c20 6966 2079 6f75  not ideal if you
+000004b0: 2061 7265 2075 7369 6e67 204f 7065 6e41   are using OpenA
+000004c0: 5049 2073 6368 656d 6173 2074 6f20 6465  PI schemas to de
+000004d0: 6669 6e65 2079 6f75 7220 4150 4920 636f  fine your API co
+000004e0: 6e74 7261 6374 732e 5c6e 5c6e 5468 6520  ntracts.\n\nThe 
+000004f0: 2a50 6f77 6572 746f 6f6c 7320 4f41 5320  *Powertools OAS 
+00000500: 5661 6c69 6461 746f 722a 2061 6464 7320  Validator* adds 
+00000510: 6120 6465 636f 7261 746f 7220 7468 6174  a decorator that
+00000520: 2079 6f75 2063 616e 2075 7365 2077 6974   you can use wit
+00000530: 6820 796f 7572 206c 616d 6264 6120 6861  h your lambda ha
+00000540: 6e64 6c65 7273 2061 6e64 2068 6176 6520  ndlers and have 
+00000550: 7468 6520 6576 656e 7473 2076 616c 6964  the events valid
+00000560: 6174 6564 2061 6761 696e 7374 2061 6e20  ated against an 
+00000570: 4f70 656e 4150 4920 7363 6865 6d61 2069  OpenAPI schema i
+00000580: 6e73 7465 6164 2e5c 6e5c 6e5c 6e23 2320  nstead.\n\n\n## 
+00000590: 496e 7374 616c 6c61 7469 6f6e 5c6e 506f  Installation\nPo
+000005a0: 6574 7279 3a5c 6e60 706f 6574 7279 2061  etry:\n`poetry a
+000005b0: 6464 2070 6f77 6572 746f 6f6c 732d 6f61  dd powertools-oa
 000005c0: 732d 7661 6c69 6461 746f 7260 5c6e 5c6e  s-validator`\n\n
-000005d0: 5c6e 2323 2055 7361 6765 5c6e 4465 636f  \n## Usage\nDeco
-000005e0: 7261 7465 2079 6f75 7220 6675 6e63 7469  rate your functi
-000005f0: 6f6e 7320 7769 7468 2060 4076 616c 6964  ons with `@valid
-00000600: 6174 655f 7265 7175 6573 7428 6f61 735f  ate_request(oas_
-00000610: 7061 7468 3d22 6f70 656e 6170 692e 7961  path="openapi.ya
-00000620: 6d6c 2229 6020 616e 6420 796f 7572 2072  ml")` and your r
-00000630: 6571 7565 7374 2f65 7665 6e74 2028 616e  equest/event (an
-00000640: 6420 7363 6865 6d61 2920 7769 6c6c 2062  d schema) will b
-00000650: 6520 7661 6c69 6461 7465 6420 6f6e 2061  e validated on a
-00000660: 2072 6571 7565 7374 2e5c 6e5c 6e5c 6e23   request.\n\n\n#
-00000670: 2323 204d 696e 696d 616c 2045 7861 6d70  ## Minimal Examp
-00000680: 6c65 5c6e 5c6e 6060 6070 7974 686f 6e5c  le\n\n```python\
-00000690: 6e66 726f 6d20 7479 7069 6e67 2069 6d70  nfrom typing imp
-000006a0: 6f72 7420 4469 6374 5c6e 6672 6f6d 2061  ort Dict\nfrom a
-000006b0: 7773 5f6c 616d 6264 615f 706f 7765 7274  ws_lambda_powert
-000006c0: 6f6f 6c73 2e65 7665 6e74 5f68 616e 646c  ools.event_handl
-000006d0: 6572 2069 6d70 6f72 7420 4150 4947 6174  er import APIGat
-000006e0: 6577 6179 5265 7374 5265 736f 6c76 6572  ewayRestResolver
-000006f0: 2c20 5265 7370 6f6e 7365 5c6e 6672 6f6d  , Response\nfrom
-00000700: 2061 7773 5f6c 616d 6264 615f 706f 7765   aws_lambda_powe
-00000710: 7274 6f6f 6c73 2e75 7469 6c69 7469 6573  rtools.utilities
-00000720: 2e74 7970 696e 6720 696d 706f 7274 204c  .typing import L
-00000730: 616d 6264 6143 6f6e 7465 7874 5c6e 6672  ambdaContext\nfr
-00000740: 6f6d 2070 6f77 6572 746f 6f6c 735f 6f61  om powertools_oa
-00000750: 735f 7661 6c69 6461 746f 722e 6d69 6464  s_validator.midd
-00000760: 6c65 7761 7265 2069 6d70 6f72 7420 7661  leware import va
-00000770: 6c69 6461 7465 5f72 6571 7565 7374 5c6e  lidate_request\n
-00000780: 5c6e 5c6e 6170 7020 3d20 4150 4947 6174  \n\napp = APIGat
-00000790: 6577 6179 5265 7374 5265 736f 6c76 6572  ewayRestResolver
-000007a0: 2829 5c6e 5c6e 4061 7070 2e70 6f73 7428  ()\n\n@app.post(
-000007b0: 222f 6578 616d 706c 6522 295c 6e64 6566  "/example")\ndef
-000007c0: 2065 7861 6d70 6c65 2829 202d 3e20 5265   example() -> Re
-000007d0: 7370 6f6e 7365 3a5c 6e20 202e 2e2e 5c6e  sponse:\n  ...\n
-000007e0: 5c6e 4076 616c 6964 6174 655f 7265 7175  \n@validate_requ
-000007f0: 6573 7428 6f61 735f 7061 7468 3d22 6f70  est(oas_path="op
-00000800: 656e 6170 692e 7961 6d6c 2229 5c6e 6465  enapi.yaml")\nde
-00000810: 6620 6c61 6d62 6461 5f68 616e 646c 6572  f lambda_handler
-00000820: 2865 7665 6e74 3a20 4469 6374 2c20 636f  (event: Dict, co
-00000830: 6e74 6578 743a 204c 616d 6264 6143 6f6e  ntext: LambdaCon
-00000840: 7465 7874 2920 2d3e 2044 6963 743a 5c6e  text) -> Dict:\n
-00000850: 2020 2020 7265 7370 6f6e 7365 203d 2061      response = a
-00000860: 7070 2e72 6573 6f6c 7665 2865 7665 6e74  pp.resolve(event
-00000870: 2c20 636f 6e74 6578 7429 5c6e 5c6e 2020  , context)\n\n  
-00000880: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
-00000890: 655c 6e60 6060 5c6e 5c6e 2323 2045 7272  e\n```\n\n## Err
-000008a0: 6f72 2048 616e 646c 696e 675c 6e49 6620  or Handling\nIf 
-000008b0: 7468 6520 7661 6c69 6461 7469 6f6e 2066  the validation f
-000008c0: 6169 6c73 2c20 7468 6520 6465 636f 7261  ails, the decora
-000008d0: 746f 7220 7468 726f 7773 2061 2060 5363  tor throws a `Sc
-000008e0: 6865 6d61 5661 6c69 6461 746f 6e45 7272  hemaValidatonErr
-000008f0: 6f72 6020 7769 7468 2072 656c 6576 616e  or` with relevan
-00000900: 7420 696e 666f 726d 6174 696f 6e20 6162  t information ab
-00000910: 6f75 7420 7468 6520 6661 696c 6564 2076  out the failed v
-00000920: 616c 6964 6174 696f 6e2e 5c6e 5c6e 5c6e  alidation.\n\n\n
-00000930: 2323 204b 6e6f 7720 4973 7375 6573 5c6e  ## Know Issues\n
-00000940: 5768 696c 6520 616c 6c20 7661 6c69 6461  While all valida
-00000950: 7469 6f6e 2065 7272 6f72 7320 6172 6520  tion errors are 
-00000960: 6361 7567 6874 2c20 7468 6572 6520 6973  caught, there is
-00000970: 206f 6e6c 7920 6c69 6d69 7465 6420 696e   only limited in
-00000980: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
-00000990: 7468 6520 7661 7269 6f75 7320 6572 726f  the various erro
-000009a0: 7273 2e20 5468 6520 6465 636f 7261 746f  rs. The decorato
-000009b0: 7220 7769 6c6c 2074 7279 2069 7473 2062  r will try its b
-000009c0: 6573 7420 746f 2074 6872 6f77 2061 2060  est to throw a `
-000009d0: 5363 6865 6d61 5661 6c69 6461 746f 6e45  SchemaValidatonE
-000009e0: 7272 6f72 605c 6e28 7361 6d65 2061 7320  rror`\n(same as 
-000009f0: 7468 6520 506f 7765 7274 6f6f 6c73 2076  the Powertools v
-00000a00: 616c 6964 6174 6f72 2077 6f75 6c64 292c  alidator would),
-00000a10: 2077 6974 6820 6173 206d 7563 6820 6f66   with as much of
-00000a20: 2074 6865 206f 7074 696f 6e61 6c20 6174   the optional at
-00000a30: 7472 6962 7574 6573 2061 7320 706f 7373  tributes as poss
-00000a40: 6962 6c65 2e5c 6e5c 6e49 6e20 7375 6d6d  ible.\n\nIn summ
-00000a50: 6172 792c 2069 7420 6973 2070 6f73 7369  ary, it is possi
-00000a60: 626c 6520 7468 6174 206e 6f74 2061 6c6c  ble that not all
-00000a70: 2060 5363 6865 6d61 5661 6c69 6461 7469   `SchemaValidati
-00000a80: 6f6e 4572 726f 7273 605c 2773 2077 696c  onErrors`\'s wil
-00000a90: 6c20 6861 7665 2061 206e 6963 6520 7661  l have a nice va
-00000aa0: 6c69 6461 7469 6f6e 206d 6573 7361 6765  lidation message
-00000ab0: 2c20 696e 2063 6173 6520 796f 7520 7265  , in case you re
-00000ac0: 6c79 206f 6e20 7069 7069 6e67 2069 7420  ly on piping it 
-00000ad0: 7374 7261 6967 6874 2062 6163 6b20 746f  straight back to
-00000ae0: 2074 6865 2063 6c69 656e 742e 5c6e 5c6e   the client.\n\n
-00000af0: 5c6e 2323 2043 6f6e 7472 6962 7574 696f  \n## Contributio
-00000b00: 6e73 5c6e 506c 6561 7365 206d 616b 6520  ns\nPlease make 
-00000b10: 6120 7075 6c6c 2072 6571 7565 7374 2061  a pull request a
-00000b20: 6e64 2049 2077 696c 6c20 7265 7669 6577  nd I will review
-00000b30: 2069 7420 4153 4150 2e5c 6e27 2c0a 2020   it ASAP.\n',.  
-00000b40: 2020 2761 7574 686f 7227 3a20 2752 6173    'author': 'Ras
-00000b50: 6d75 7320 4861 6e73 656e 272c 0a20 2020  mus Hansen',.   
-00000b60: 2027 6175 7468 6f72 5f65 6d61 696c 273a   'author_email':
-00000b70: 2027 522e 4661 6e67 656c 4861 6e73 656e   'R.FangelHansen
-00000b80: 4067 6d61 696c 2e63 6f6d 272c 0a20 2020  @gmail.com',.   
-00000b90: 2027 6d61 696e 7461 696e 6572 273a 2027   'maintainer': '
-00000ba0: 4e6f 6e65 272c 0a20 2020 2027 6d61 696e  None',.    'main
-00000bb0: 7461 696e 6572 5f65 6d61 696c 273a 2027  tainer_email': '
-00000bc0: 4e6f 6e65 272c 0a20 2020 2027 7572 6c27  None',.    'url'
-00000bd0: 3a20 2768 7474 7073 3a2f 2f67 6974 6875  : 'https://githu
-00000be0: 622e 636f 6d2f 5261 736d 7573 4661 6e67  b.com/RasmusFang
-00000bf0: 656c 2f70 6f77 6572 746f 6f6c 732d 6f61  el/powertools-oa
-00000c00: 732d 7661 6c69 6461 746f 7227 2c0a 2020  s-validator',.  
-00000c10: 2020 2770 6163 6b61 6765 7327 3a20 7061    'packages': pa
-00000c20: 636b 6167 6573 2c0a 2020 2020 2770 6163  ckages,.    'pac
-00000c30: 6b61 6765 5f64 6174 6127 3a20 7061 636b  kage_data': pack
-00000c40: 6167 655f 6461 7461 2c0a 2020 2020 2769  age_data,.    'i
-00000c50: 6e73 7461 6c6c 5f72 6571 7569 7265 7327  nstall_requires'
-00000c60: 3a20 696e 7374 616c 6c5f 7265 7175 6972  : install_requir
-00000c70: 6573 2c0a 2020 2020 2770 7974 686f 6e5f  es,.    'python_
-00000c80: 7265 7175 6972 6573 273a 2027 3e3d 332e  requires': '>=3.
-00000c90: 3130 2c3c 342e 3027 2c0a 7d0a 0a0a 7365  10,<4.0',.}...se
-00000ca0: 7475 7028 2a2a 7365 7475 705f 6b77 6172  tup(**setup_kwar
-00000cb0: 6773 290a                                gs).
+000005d0: 5069 703a 5c6e 6070 6970 2069 6e73 7461  Pip:\n`pip insta
+000005e0: 6c6c 2070 6f77 6572 746f 6f6c 732d 6f61  ll powertools-oa
+000005f0: 732d 7661 6c69 6461 746f 7260 5c6e 5c6e  s-validator`\n\n
+00000600: 5c6e 2323 2055 7361 6765 5c6e 4465 636f  \n## Usage\nDeco
+00000610: 7261 7465 2079 6f75 7220 6675 6e63 7469  rate your functi
+00000620: 6f6e 7320 7769 7468 2060 4076 616c 6964  ons with `@valid
+00000630: 6174 655f 7265 7175 6573 7428 6f61 735f  ate_request(oas_
+00000640: 7061 7468 3d22 6f70 656e 6170 692e 7961  path="openapi.ya
+00000650: 6d6c 2229 6020 616e 6420 796f 7572 2072  ml")` and your r
+00000660: 6571 7565 7374 2f65 7665 6e74 2028 616e  equest/event (an
+00000670: 6420 7363 6865 6d61 2920 7769 6c6c 2062  d schema) will b
+00000680: 6520 7661 6c69 6461 7465 6420 6f6e 2061  e validated on a
+00000690: 2072 6571 7565 7374 2e5c 6e5c 6e5c 6e23   request.\n\n\n#
+000006a0: 2323 204d 696e 696d 616c 2045 7861 6d70  ## Minimal Examp
+000006b0: 6c65 5c6e 5c6e 6060 6070 7974 686f 6e5c  le\n\n```python\
+000006c0: 6e66 726f 6d20 7479 7069 6e67 2069 6d70  nfrom typing imp
+000006d0: 6f72 7420 4469 6374 5c6e 6672 6f6d 2061  ort Dict\nfrom a
+000006e0: 7773 5f6c 616d 6264 615f 706f 7765 7274  ws_lambda_powert
+000006f0: 6f6f 6c73 2e65 7665 6e74 5f68 616e 646c  ools.event_handl
+00000700: 6572 2069 6d70 6f72 7420 4150 4947 6174  er import APIGat
+00000710: 6577 6179 5265 7374 5265 736f 6c76 6572  ewayRestResolver
+00000720: 2c20 5265 7370 6f6e 7365 5c6e 6672 6f6d  , Response\nfrom
+00000730: 2061 7773 5f6c 616d 6264 615f 706f 7765   aws_lambda_powe
+00000740: 7274 6f6f 6c73 2e75 7469 6c69 7469 6573  rtools.utilities
+00000750: 2e74 7970 696e 6720 696d 706f 7274 204c  .typing import L
+00000760: 616d 6264 6143 6f6e 7465 7874 5c6e 6672  ambdaContext\nfr
+00000770: 6f6d 2070 6f77 6572 746f 6f6c 735f 6f61  om powertools_oa
+00000780: 735f 7661 6c69 6461 746f 722e 6d69 6464  s_validator.midd
+00000790: 6c65 7761 7265 2069 6d70 6f72 7420 7661  leware import va
+000007a0: 6c69 6461 7465 5f72 6571 7565 7374 5c6e  lidate_request\n
+000007b0: 5c6e 5c6e 6170 7020 3d20 4150 4947 6174  \n\napp = APIGat
+000007c0: 6577 6179 5265 7374 5265 736f 6c76 6572  ewayRestResolver
+000007d0: 2829 5c6e 5c6e 4061 7070 2e70 6f73 7428  ()\n\n@app.post(
+000007e0: 222f 6578 616d 706c 6522 295c 6e64 6566  "/example")\ndef
+000007f0: 2065 7861 6d70 6c65 2829 202d 3e20 5265   example() -> Re
+00000800: 7370 6f6e 7365 3a5c 6e20 202e 2e2e 5c6e  sponse:\n  ...\n
+00000810: 5c6e 4076 616c 6964 6174 655f 7265 7175  \n@validate_requ
+00000820: 6573 7428 6f61 735f 7061 7468 3d22 6f70  est(oas_path="op
+00000830: 656e 6170 692e 7961 6d6c 2229 5c6e 6465  enapi.yaml")\nde
+00000840: 6620 6c61 6d62 6461 5f68 616e 646c 6572  f lambda_handler
+00000850: 2865 7665 6e74 3a20 4469 6374 2c20 636f  (event: Dict, co
+00000860: 6e74 6578 743a 204c 616d 6264 6143 6f6e  ntext: LambdaCon
+00000870: 7465 7874 2920 2d3e 2044 6963 743a 5c6e  text) -> Dict:\n
+00000880: 2020 2020 7265 7370 6f6e 7365 203d 2061      response = a
+00000890: 7070 2e72 6573 6f6c 7665 2865 7665 6e74  pp.resolve(event
+000008a0: 2c20 636f 6e74 6578 7429 5c6e 5c6e 2020  , context)\n\n  
+000008b0: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
+000008c0: 655c 6e60 6060 5c6e 5c6e 2323 2045 7272  e\n```\n\n## Err
+000008d0: 6f72 2048 616e 646c 696e 675c 6e49 6620  or Handling\nIf 
+000008e0: 7468 6520 7661 6c69 6461 7469 6f6e 2066  the validation f
+000008f0: 6169 6c73 2c20 7468 6520 6465 636f 7261  ails, the decora
+00000900: 746f 7220 7468 726f 7773 2061 2060 5363  tor throws a `Sc
+00000910: 6865 6d61 5661 6c69 6461 746f 6e45 7272  hemaValidatonErr
+00000920: 6f72 6020 7769 7468 2072 656c 6576 616e  or` with relevan
+00000930: 7420 696e 666f 726d 6174 696f 6e20 6162  t information ab
+00000940: 6f75 7420 7468 6520 6661 696c 6564 2076  out the failed v
+00000950: 616c 6964 6174 696f 6e2e 5c6e 5c6e 5c6e  alidation.\n\n\n
+00000960: 2323 204b 6e6f 7720 4973 7375 6573 5c6e  ## Know Issues\n
+00000970: 5768 696c 6520 616c 6c20 7661 6c69 6461  While all valida
+00000980: 7469 6f6e 2065 7272 6f72 7320 6172 6520  tion errors are 
+00000990: 6361 7567 6874 2c20 7468 6572 6520 6973  caught, there is
+000009a0: 206f 6e6c 7920 6c69 6d69 7465 6420 696e   only limited in
+000009b0: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
+000009c0: 7468 6520 7661 7269 6f75 7320 6572 726f  the various erro
+000009d0: 7273 2e20 5468 6520 6465 636f 7261 746f  rs. The decorato
+000009e0: 7220 7769 6c6c 2074 7279 2069 7473 2062  r will try its b
+000009f0: 6573 7420 746f 2074 6872 6f77 2061 2060  est to throw a `
+00000a00: 5363 6865 6d61 5661 6c69 6461 746f 6e45  SchemaValidatonE
+00000a10: 7272 6f72 605c 6e28 7361 6d65 2061 7320  rror`\n(same as 
+00000a20: 7468 6520 506f 7765 7274 6f6f 6c73 2076  the Powertools v
+00000a30: 616c 6964 6174 6f72 2077 6f75 6c64 292c  alidator would),
+00000a40: 2077 6974 6820 6173 206d 7563 6820 6f66   with as much of
+00000a50: 2074 6865 206f 7074 696f 6e61 6c20 6174   the optional at
+00000a60: 7472 6962 7574 6573 2061 7320 706f 7373  tributes as poss
+00000a70: 6962 6c65 2e5c 6e5c 6e49 6e20 7375 6d6d  ible.\n\nIn summ
+00000a80: 6172 792c 2069 7420 6973 2070 6f73 7369  ary, it is possi
+00000a90: 626c 6520 7468 6174 206e 6f74 2061 6c6c  ble that not all
+00000aa0: 2060 5363 6865 6d61 5661 6c69 6461 7469   `SchemaValidati
+00000ab0: 6f6e 4572 726f 7273 605c 2773 2077 696c  onErrors`\'s wil
+00000ac0: 6c20 6861 7665 2061 206e 6963 6520 7661  l have a nice va
+00000ad0: 6c69 6461 7469 6f6e 206d 6573 7361 6765  lidation message
+00000ae0: 2c20 696e 2063 6173 6520 796f 7520 7265  , in case you re
+00000af0: 6c79 206f 6e20 7069 7069 6e67 2069 7420  ly on piping it 
+00000b00: 7374 7261 6967 6874 2062 6163 6b20 746f  straight back to
+00000b10: 2074 6865 2063 6c69 656e 742e 5c6e 5c6e   the client.\n\n
+00000b20: 5c6e 2323 2043 6f6e 7472 6962 7574 696f  \n## Contributio
+00000b30: 6e73 5c6e 506c 6561 7365 206d 616b 6520  ns\nPlease make 
+00000b40: 6120 7075 6c6c 2072 6571 7565 7374 2061  a pull request a
+00000b50: 6e64 2049 2077 696c 6c20 7265 7669 6577  nd I will review
+00000b60: 2069 7420 4153 4150 2e5c 6e27 2c0a 2020   it ASAP.\n',.  
+00000b70: 2020 2761 7574 686f 7227 3a20 2752 6173    'author': 'Ras
+00000b80: 6d75 7320 4861 6e73 656e 272c 0a20 2020  mus Hansen',.   
+00000b90: 2027 6175 7468 6f72 5f65 6d61 696c 273a   'author_email':
+00000ba0: 2027 522e 4661 6e67 656c 4861 6e73 656e   'R.FangelHansen
+00000bb0: 4067 6d61 696c 2e63 6f6d 272c 0a20 2020  @gmail.com',.   
+00000bc0: 2027 6d61 696e 7461 696e 6572 273a 2027   'maintainer': '
+00000bd0: 4e6f 6e65 272c 0a20 2020 2027 6d61 696e  None',.    'main
+00000be0: 7461 696e 6572 5f65 6d61 696c 273a 2027  tainer_email': '
+00000bf0: 4e6f 6e65 272c 0a20 2020 2027 7572 6c27  None',.    'url'
+00000c00: 3a20 2768 7474 7073 3a2f 2f67 6974 6875  : 'https://githu
+00000c10: 622e 636f 6d2f 5261 736d 7573 4661 6e67  b.com/RasmusFang
+00000c20: 656c 2f70 6f77 6572 746f 6f6c 732d 6f61  el/powertools-oa
+00000c30: 732d 7661 6c69 6461 746f 7227 2c0a 2020  s-validator',.  
+00000c40: 2020 2770 6163 6b61 6765 7327 3a20 7061    'packages': pa
+00000c50: 636b 6167 6573 2c0a 2020 2020 2770 6163  ckages,.    'pac
+00000c60: 6b61 6765 5f64 6174 6127 3a20 7061 636b  kage_data': pack
+00000c70: 6167 655f 6461 7461 2c0a 2020 2020 2769  age_data,.    'i
+00000c80: 6e73 7461 6c6c 5f72 6571 7569 7265 7327  nstall_requires'
+00000c90: 3a20 696e 7374 616c 6c5f 7265 7175 6972  : install_requir
+00000ca0: 6573 2c0a 2020 2020 2770 7974 686f 6e5f  es,.    'python_
+00000cb0: 7265 7175 6972 6573 273a 2027 3e3d 332e  requires': '>=3.
+00000cc0: 3130 2c3c 342e 3027 2c0a 7d0a 0a0a 7365  10,<4.0',.}...se
+00000cd0: 7475 7028 2a2a 7365 7475 705f 6b77 6172  tup(**setup_kwar
+00000ce0: 6773 290a                                gs).
```

### Comparing `powertools_oas_validator-0.5.3/PKG-INFO` & `powertools_oas_validator-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 706f 7765  : 2.1.Name: powe
 00000020: 7274 6f6f 6c73 2d6f 6173 2d76 616c 6964  rtools-oas-valid
 00000030: 6174 6f72 0a56 6572 7369 6f6e 3a20 302e  ator.Version: 0.
-00000040: 352e 330a 5375 6d6d 6172 793a 200a 486f  5.3.Summary: .Ho
+00000040: 352e 340a 5375 6d6d 6172 793a 200a 486f  5.4.Summary: .Ho
 00000050: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
 00000060: 2f67 6974 6875 622e 636f 6d2f 5261 736d  /github.com/Rasm
 00000070: 7573 4661 6e67 656c 2f70 6f77 6572 746f  usFangel/powerto
 00000080: 6f6c 732d 6f61 732d 7661 6c69 6461 746f  ols-oas-validato
 00000090: 720a 4c69 6365 6e73 653a 204d 4954 0a41  r.License: MIT.A
 000000a0: 7574 686f 723a 2052 6173 6d75 7320 4861  uthor: Rasmus Ha
 000000b0: 6e73 656e 0a41 7574 686f 722d 656d 6169  nsen.Author-emai
@@ -49,151 +49,154 @@
 00000300: 6d2f 5261 736d 7573 4661 6e67 656c 2f70  m/RasmusFangel/p
 00000310: 6f77 6572 746f 6f6c 732d 6f61 732d 7661  owertools-oas-va
 00000320: 6c69 6461 746f 720a 4465 7363 7269 7074  lidator.Descript
 00000330: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
 00000340: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
 00000350: 0a23 2070 6f77 6572 746f 6f6c 732d 6f61  .# powertools-oa
 00000360: 732d 7661 6c69 6461 746f 720a 3c62 723e  s-validator.<br>
-00000370: 5b21 5b50 7950 4920 7665 7273 696f 6e5d  [![PyPI version]
-00000380: 2868 7474 7073 3a2f 2f62 6164 6765 2e66  (https://badge.f
-00000390: 7572 792e 696f 2f70 792f 706f 7765 7274  ury.io/py/powert
-000003a0: 6f6f 6c73 2d6f 6173 2d76 616c 6964 6174  ools-oas-validat
-000003b0: 6f72 2e73 7667 295d 2868 7474 7073 3a2f  or.svg)](https:/
-000003c0: 2f62 6164 6765 2e66 7572 792e 696f 2f70  /badge.fury.io/p
-000003d0: 792f 706f 7765 7274 6f6f 6c73 2d6f 6173  y/powertools-oas
-000003e0: 2d76 616c 6964 6174 6f72 2920 215b 5265  -validator) ![Re
-000003f0: 6c65 6173 655d 2868 7474 7073 3a2f 2f67  lease](https://g
-00000400: 6974 6875 622e 636f 6d2f 5261 736d 7573  ithub.com/Rasmus
-00000410: 4661 6e67 656c 2f70 6f77 6572 746f 6f6c  Fangel/powertool
-00000420: 732d 6f61 732d 7661 6c69 6461 746f 722f  s-oas-validator/
-00000430: 776f 726b 666c 6f77 732f 5265 6c65 6173  workflows/Releas
-00000440: 652f 6261 6467 652e 7376 6729 2021 5b43  e/badge.svg) ![C
-00000450: 495d 2868 7474 7073 3a2f 2f67 6974 6875  I](https://githu
-00000460: 622e 636f 6d2f 5261 736d 7573 4661 6e67  b.com/RasmusFang
-00000470: 656c 2f70 6f77 6572 746f 6f6c 732d 6f61  el/powertools-oa
-00000480: 732d 7661 6c69 6461 746f 722f 776f 726b  s-validator/work
-00000490: 666c 6f77 732f 4349 2f62 6164 6765 2e73  flows/CI/badge.s
-000004a0: 7667 290a 0a23 2320 496e 7472 6f64 7563  vg)..## Introduc
-000004b0: 7469 6f6e 0a0a 5b50 6f77 6572 746f 6f6c  tion..[Powertool
-000004c0: 7320 666f 7220 4157 5320 4c61 6d62 6461  s for AWS Lambda
-000004d0: 2028 5079 7468 6f6e 295d 2868 7474 7073   (Python)](https
-000004e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6177  ://github.com/aw
-000004f0: 732d 706f 7765 7274 6f6f 6c73 2f70 6f77  s-powertools/pow
-00000500: 6572 746f 6f6c 732d 6c61 6d62 6461 2d70  ertools-lambda-p
-00000510: 7974 686f 6e29 2069 7320 616e 2061 7765  ython) is an awe
-00000520: 736f 6d65 2073 6574 206f 6620 746f 6f6c  some set of tool
-00000530: 7320 666f 7220 7375 7065 7263 6861 7267  s for supercharg
-00000540: 696e 6720 796f 7572 206c 616d 6264 6173  ing your lambdas
-00000550: 2e20 506f 7765 7274 6f6f 6c73 2073 7570  . Powertools sup
-00000560: 706f 7274 7320 7661 6c69 6461 7469 6e67  ports validating
-00000570: 2069 6e63 6f6d 696e 6720 7265 7175 6573   incoming reques
-00000580: 7473 2028 6f72 2065 7665 6e74 2069 6e20  ts (or event in 
-00000590: 5054 206c 696e 676f 2920 6167 6169 6e73  PT lingo) agains
-000005a0: 7420 5b4a 534f 4e53 6368 656d 615d 2868  t [JSONSchema](h
-000005b0: 7474 7073 3a2f 2f6a 736f 6e2d 7363 6865  ttps://json-sche
-000005c0: 6d61 2e6f 7267 2f29 2077 6869 6368 2069  ma.org/) which i
-000005d0: 7320 6e6f 7420 6964 6561 6c20 6966 2079  s not ideal if y
-000005e0: 6f75 2061 7265 2075 7369 6e67 204f 7065  ou are using Ope
-000005f0: 6e41 5049 2073 6368 656d 6173 2074 6f20  nAPI schemas to 
-00000600: 6465 6669 6e65 2079 6f75 7220 4150 4920  define your API 
-00000610: 636f 6e74 7261 6374 732e 0a0a 5468 6520  contracts...The 
-00000620: 2a50 6f77 6572 746f 6f6c 7320 4f41 5320  *Powertools OAS 
-00000630: 5661 6c69 6461 746f 722a 2061 6464 7320  Validator* adds 
-00000640: 6120 6465 636f 7261 746f 7220 7468 6174  a decorator that
-00000650: 2079 6f75 2063 616e 2075 7365 2077 6974   you can use wit
-00000660: 6820 796f 7572 206c 616d 6264 6120 6861  h your lambda ha
-00000670: 6e64 6c65 7273 2061 6e64 2068 6176 6520  ndlers and have 
-00000680: 7468 6520 6576 656e 7473 2076 616c 6964  the events valid
-00000690: 6174 6564 2061 6761 696e 7374 2061 6e20  ated against an 
-000006a0: 4f70 656e 4150 4920 7363 6865 6d61 2069  OpenAPI schema i
-000006b0: 6e73 7465 6164 2e0a 0a0a 2323 2049 6e73  nstead....## Ins
-000006c0: 7461 6c6c 6174 696f 6e0a 506f 6574 7279  tallation.Poetry
-000006d0: 3a0a 6070 6f65 7472 7920 6164 6420 706f  :.`poetry add po
-000006e0: 7765 7274 6f6f 6c73 2d6f 6173 2d76 616c  wertools-oas-val
-000006f0: 6964 6174 6f72 600a 0a50 6970 3a0a 6070  idator`..Pip:.`p
-00000700: 6970 2069 6e73 7461 6c6c 2070 6f77 6572  ip install power
-00000710: 746f 6f6c 732d 6f61 732d 7661 6c69 6461  tools-oas-valida
-00000720: 746f 7260 0a0a 0a23 2320 5573 6167 650a  tor`...## Usage.
-00000730: 4465 636f 7261 7465 2079 6f75 7220 6675  Decorate your fu
-00000740: 6e63 7469 6f6e 7320 7769 7468 2060 4076  nctions with `@v
-00000750: 616c 6964 6174 655f 7265 7175 6573 7428  alidate_request(
-00000760: 6f61 735f 7061 7468 3d22 6f70 656e 6170  oas_path="openap
-00000770: 692e 7961 6d6c 2229 6020 616e 6420 796f  i.yaml")` and yo
-00000780: 7572 2072 6571 7565 7374 2f65 7665 6e74  ur request/event
-00000790: 2028 616e 6420 7363 6865 6d61 2920 7769   (and schema) wi
-000007a0: 6c6c 2062 6520 7661 6c69 6461 7465 6420  ll be validated 
-000007b0: 6f6e 2061 2072 6571 7565 7374 2e0a 0a0a  on a request....
-000007c0: 2323 2320 4d69 6e69 6d61 6c20 4578 616d  ### Minimal Exam
-000007d0: 706c 650a 0a60 6060 7079 7468 6f6e 0a66  ple..```python.f
-000007e0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000007f0: 7420 4469 6374 0a66 726f 6d20 6177 735f  t Dict.from aws_
-00000800: 6c61 6d62 6461 5f70 6f77 6572 746f 6f6c  lambda_powertool
-00000810: 732e 6576 656e 745f 6861 6e64 6c65 7220  s.event_handler 
-00000820: 696d 706f 7274 2041 5049 4761 7465 7761  import APIGatewa
-00000830: 7952 6573 7452 6573 6f6c 7665 722c 2052  yRestResolver, R
-00000840: 6573 706f 6e73 650a 6672 6f6d 2061 7773  esponse.from aws
-00000850: 5f6c 616d 6264 615f 706f 7765 7274 6f6f  _lambda_powertoo
-00000860: 6c73 2e75 7469 6c69 7469 6573 2e74 7970  ls.utilities.typ
-00000870: 696e 6720 696d 706f 7274 204c 616d 6264  ing import Lambd
-00000880: 6143 6f6e 7465 7874 0a66 726f 6d20 706f  aContext.from po
-00000890: 7765 7274 6f6f 6c73 5f6f 6173 5f76 616c  wertools_oas_val
-000008a0: 6964 6174 6f72 2e6d 6964 646c 6577 6172  idator.middlewar
-000008b0: 6520 696d 706f 7274 2076 616c 6964 6174  e import validat
-000008c0: 655f 7265 7175 6573 740a 0a0a 6170 7020  e_request...app 
-000008d0: 3d20 4150 4947 6174 6577 6179 5265 7374  = APIGatewayRest
-000008e0: 5265 736f 6c76 6572 2829 0a0a 4061 7070  Resolver()..@app
-000008f0: 2e70 6f73 7428 222f 6578 616d 706c 6522  .post("/example"
-00000900: 290a 6465 6620 6578 616d 706c 6528 2920  ).def example() 
-00000910: 2d3e 2052 6573 706f 6e73 653a 0a20 202e  -> Response:.  .
-00000920: 2e2e 0a0a 4076 616c 6964 6174 655f 7265  ....@validate_re
-00000930: 7175 6573 7428 6f61 735f 7061 7468 3d22  quest(oas_path="
-00000940: 6f70 656e 6170 692e 7961 6d6c 2229 0a64  openapi.yaml").d
-00000950: 6566 206c 616d 6264 615f 6861 6e64 6c65  ef lambda_handle
-00000960: 7228 6576 656e 743a 2044 6963 742c 2063  r(event: Dict, c
-00000970: 6f6e 7465 7874 3a20 4c61 6d62 6461 436f  ontext: LambdaCo
-00000980: 6e74 6578 7429 202d 3e20 4469 6374 3a0a  ntext) -> Dict:.
-00000990: 2020 2020 7265 7370 6f6e 7365 203d 2061      response = a
-000009a0: 7070 2e72 6573 6f6c 7665 2865 7665 6e74  pp.resolve(event
-000009b0: 2c20 636f 6e74 6578 7429 0a0a 2020 2020  , context)..    
-000009c0: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
-000009d0: 6060 600a 0a23 2320 4572 726f 7220 4861  ```..## Error Ha
-000009e0: 6e64 6c69 6e67 0a49 6620 7468 6520 7661  ndling.If the va
-000009f0: 6c69 6461 7469 6f6e 2066 6169 6c73 2c20  lidation fails, 
-00000a00: 7468 6520 6465 636f 7261 746f 7220 7468  the decorator th
-00000a10: 726f 7773 2061 2060 5363 6865 6d61 5661  rows a `SchemaVa
-00000a20: 6c69 6461 746f 6e45 7272 6f72 6020 7769  lidatonError` wi
-00000a30: 7468 2072 656c 6576 616e 7420 696e 666f  th relevant info
-00000a40: 726d 6174 696f 6e20 6162 6f75 7420 7468  rmation about th
-00000a50: 6520 6661 696c 6564 2076 616c 6964 6174  e failed validat
-00000a60: 696f 6e2e 0a0a 0a23 2320 4b6e 6f77 2049  ion....## Know I
-00000a70: 7373 7565 730a 5768 696c 6520 616c 6c20  ssues.While all 
-00000a80: 7661 6c69 6461 7469 6f6e 2065 7272 6f72  validation error
-00000a90: 7320 6172 6520 6361 7567 6874 2c20 7468  s are caught, th
-00000aa0: 6572 6520 6973 206f 6e6c 7920 6c69 6d69  ere is only limi
-00000ab0: 7465 6420 696e 666f 726d 6174 696f 6e20  ted information 
-00000ac0: 6162 6f75 7420 7468 6520 7661 7269 6f75  about the variou
-00000ad0: 7320 6572 726f 7273 2e20 5468 6520 6465  s errors. The de
-00000ae0: 636f 7261 746f 7220 7769 6c6c 2074 7279  corator will try
-00000af0: 2069 7473 2062 6573 7420 746f 2074 6872   its best to thr
-00000b00: 6f77 2061 2060 5363 6865 6d61 5661 6c69  ow a `SchemaVali
-00000b10: 6461 746f 6e45 7272 6f72 600a 2873 616d  datonError`.(sam
-00000b20: 6520 6173 2074 6865 2050 6f77 6572 746f  e as the Powerto
-00000b30: 6f6c 7320 7661 6c69 6461 746f 7220 776f  ols validator wo
-00000b40: 756c 6429 2c20 7769 7468 2061 7320 6d75  uld), with as mu
-00000b50: 6368 206f 6620 7468 6520 6f70 7469 6f6e  ch of the option
-00000b60: 616c 2061 7474 7269 6275 7465 7320 6173  al attributes as
-00000b70: 2070 6f73 7369 626c 652e 0a0a 496e 2073   possible...In s
-00000b80: 756d 6d61 7279 2c20 6974 2069 7320 706f  ummary, it is po
-00000b90: 7373 6962 6c65 2074 6861 7420 6e6f 7420  ssible that not 
-00000ba0: 616c 6c20 6053 6368 656d 6156 616c 6964  all `SchemaValid
-00000bb0: 6174 696f 6e45 7272 6f72 7360 2773 2077  ationErrors`'s w
-00000bc0: 696c 6c20 6861 7665 2061 206e 6963 6520  ill have a nice 
-00000bd0: 7661 6c69 6461 7469 6f6e 206d 6573 7361  validation messa
-00000be0: 6765 2c20 696e 2063 6173 6520 796f 7520  ge, in case you 
-00000bf0: 7265 6c79 206f 6e20 7069 7069 6e67 2069  rely on piping i
-00000c00: 7420 7374 7261 6967 6874 2062 6163 6b20  t straight back 
-00000c10: 746f 2074 6865 2063 6c69 656e 742e 0a0a  to the client...
-00000c20: 0a23 2320 436f 6e74 7269 6275 7469 6f6e  .## Contribution
-00000c30: 730a 506c 6561 7365 206d 616b 6520 6120  s.Please make a 
-00000c40: 7075 6c6c 2072 6571 7565 7374 2061 6e64  pull request and
-00000c50: 2049 2077 696c 6c20 7265 7669 6577 2069   I will review i
-00000c60: 7420 4153 4150 2e0a 0a                   t ASAP...
+00000370: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000380: 2f62 6164 6765 2e66 7572 792e 696f 2f70  /badge.fury.io/p
+00000390: 792f 706f 7765 7274 6f6f 6c73 2d6f 6173  y/powertools-oas
+000003a0: 2d76 616c 6964 6174 6f72 223e 3c69 6d67  -validator"><img
+000003b0: 2073 7263 3d22 6874 7470 733a 2f2f 6261   src="https://ba
+000003c0: 6467 652e 6675 7279 2e69 6f2f 7079 2f70  dge.fury.io/py/p
+000003d0: 6f77 6572 746f 6f6c 732d 6f61 732d 7661  owertools-oas-va
+000003e0: 6c69 6461 746f 722e 7376 6722 2061 6c74  lidator.svg" alt
+000003f0: 3d22 5079 5049 2076 6572 7369 6f6e 223e  ="PyPI version">
+00000400: 3c2f 613e 2020 215b 4349 5d28 6874 7470  </a>  ![CI](http
+00000410: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f52  s://github.com/R
+00000420: 6173 6d75 7346 616e 6765 6c2f 706f 7765  asmusFangel/powe
+00000430: 7274 6f6f 6c73 2d6f 6173 2d76 616c 6964  rtools-oas-valid
+00000440: 6174 6f72 2f77 6f72 6b66 6c6f 7773 2f43  ator/workflows/C
+00000450: 492f 6261 6467 652e 7376 6729 203c 696d  I/badge.svg) <im
+00000460: 6720 7372 633d 2268 7474 7073 3a2f 2f63  g src="https://c
+00000470: 6f76 6572 616c 6c73 2e69 6f2f 7265 706f  overalls.io/repo
+00000480: 732f 5261 736d 7573 4661 6e67 656c 2f70  s/RasmusFangel/p
+00000490: 6f77 6572 746f 6f6c 732d 6f61 732d 7661  owertools-oas-va
+000004a0: 6c69 6461 746f 722f 6261 6467 652e 7376  lidator/badge.sv
+000004b0: 673f 6272 616e 6368 3d6d 6169 6e22 2061  g?branch=main" a
+000004c0: 6c74 3d22 436f 7665 7261 6c6c 7322 3e3c  lt="Coveralls"><
+000004d0: 2f61 3e0a 0a23 2320 496e 7472 6f64 7563  /a>..## Introduc
+000004e0: 7469 6f6e 0a0a 5b50 6f77 6572 746f 6f6c  tion..[Powertool
+000004f0: 7320 666f 7220 4157 5320 4c61 6d62 6461  s for AWS Lambda
+00000500: 2028 5079 7468 6f6e 295d 2868 7474 7073   (Python)](https
+00000510: 3a2f 2f67 6974 6875 622e 636f 6d2f 6177  ://github.com/aw
+00000520: 732d 706f 7765 7274 6f6f 6c73 2f70 6f77  s-powertools/pow
+00000530: 6572 746f 6f6c 732d 6c61 6d62 6461 2d70  ertools-lambda-p
+00000540: 7974 686f 6e29 2069 7320 616e 2061 7765  ython) is an awe
+00000550: 736f 6d65 2073 6574 206f 6620 746f 6f6c  some set of tool
+00000560: 7320 666f 7220 7375 7065 7263 6861 7267  s for supercharg
+00000570: 696e 6720 796f 7572 206c 616d 6264 6173  ing your lambdas
+00000580: 2e20 506f 7765 7274 6f6f 6c73 2073 7570  . Powertools sup
+00000590: 706f 7274 7320 7661 6c69 6461 7469 6e67  ports validating
+000005a0: 2069 6e63 6f6d 696e 6720 7265 7175 6573   incoming reques
+000005b0: 7473 2028 6f72 2065 7665 6e74 2069 6e20  ts (or event in 
+000005c0: 5054 206c 696e 676f 2920 6167 6169 6e73  PT lingo) agains
+000005d0: 7420 5b4a 534f 4e53 6368 656d 615d 2868  t [JSONSchema](h
+000005e0: 7474 7073 3a2f 2f6a 736f 6e2d 7363 6865  ttps://json-sche
+000005f0: 6d61 2e6f 7267 2f29 2077 6869 6368 2069  ma.org/) which i
+00000600: 7320 6e6f 7420 6964 6561 6c20 6966 2079  s not ideal if y
+00000610: 6f75 2061 7265 2075 7369 6e67 204f 7065  ou are using Ope
+00000620: 6e41 5049 2073 6368 656d 6173 2074 6f20  nAPI schemas to 
+00000630: 6465 6669 6e65 2079 6f75 7220 4150 4920  define your API 
+00000640: 636f 6e74 7261 6374 732e 0a0a 5468 6520  contracts...The 
+00000650: 2a50 6f77 6572 746f 6f6c 7320 4f41 5320  *Powertools OAS 
+00000660: 5661 6c69 6461 746f 722a 2061 6464 7320  Validator* adds 
+00000670: 6120 6465 636f 7261 746f 7220 7468 6174  a decorator that
+00000680: 2079 6f75 2063 616e 2075 7365 2077 6974   you can use wit
+00000690: 6820 796f 7572 206c 616d 6264 6120 6861  h your lambda ha
+000006a0: 6e64 6c65 7273 2061 6e64 2068 6176 6520  ndlers and have 
+000006b0: 7468 6520 6576 656e 7473 2076 616c 6964  the events valid
+000006c0: 6174 6564 2061 6761 696e 7374 2061 6e20  ated against an 
+000006d0: 4f70 656e 4150 4920 7363 6865 6d61 2069  OpenAPI schema i
+000006e0: 6e73 7465 6164 2e0a 0a0a 2323 2049 6e73  nstead....## Ins
+000006f0: 7461 6c6c 6174 696f 6e0a 506f 6574 7279  tallation.Poetry
+00000700: 3a0a 6070 6f65 7472 7920 6164 6420 706f  :.`poetry add po
+00000710: 7765 7274 6f6f 6c73 2d6f 6173 2d76 616c  wertools-oas-val
+00000720: 6964 6174 6f72 600a 0a50 6970 3a0a 6070  idator`..Pip:.`p
+00000730: 6970 2069 6e73 7461 6c6c 2070 6f77 6572  ip install power
+00000740: 746f 6f6c 732d 6f61 732d 7661 6c69 6461  tools-oas-valida
+00000750: 746f 7260 0a0a 0a23 2320 5573 6167 650a  tor`...## Usage.
+00000760: 4465 636f 7261 7465 2079 6f75 7220 6675  Decorate your fu
+00000770: 6e63 7469 6f6e 7320 7769 7468 2060 4076  nctions with `@v
+00000780: 616c 6964 6174 655f 7265 7175 6573 7428  alidate_request(
+00000790: 6f61 735f 7061 7468 3d22 6f70 656e 6170  oas_path="openap
+000007a0: 692e 7961 6d6c 2229 6020 616e 6420 796f  i.yaml")` and yo
+000007b0: 7572 2072 6571 7565 7374 2f65 7665 6e74  ur request/event
+000007c0: 2028 616e 6420 7363 6865 6d61 2920 7769   (and schema) wi
+000007d0: 6c6c 2062 6520 7661 6c69 6461 7465 6420  ll be validated 
+000007e0: 6f6e 2061 2072 6571 7565 7374 2e0a 0a0a  on a request....
+000007f0: 2323 2320 4d69 6e69 6d61 6c20 4578 616d  ### Minimal Exam
+00000800: 706c 650a 0a60 6060 7079 7468 6f6e 0a66  ple..```python.f
+00000810: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+00000820: 7420 4469 6374 0a66 726f 6d20 6177 735f  t Dict.from aws_
+00000830: 6c61 6d62 6461 5f70 6f77 6572 746f 6f6c  lambda_powertool
+00000840: 732e 6576 656e 745f 6861 6e64 6c65 7220  s.event_handler 
+00000850: 696d 706f 7274 2041 5049 4761 7465 7761  import APIGatewa
+00000860: 7952 6573 7452 6573 6f6c 7665 722c 2052  yRestResolver, R
+00000870: 6573 706f 6e73 650a 6672 6f6d 2061 7773  esponse.from aws
+00000880: 5f6c 616d 6264 615f 706f 7765 7274 6f6f  _lambda_powertoo
+00000890: 6c73 2e75 7469 6c69 7469 6573 2e74 7970  ls.utilities.typ
+000008a0: 696e 6720 696d 706f 7274 204c 616d 6264  ing import Lambd
+000008b0: 6143 6f6e 7465 7874 0a66 726f 6d20 706f  aContext.from po
+000008c0: 7765 7274 6f6f 6c73 5f6f 6173 5f76 616c  wertools_oas_val
+000008d0: 6964 6174 6f72 2e6d 6964 646c 6577 6172  idator.middlewar
+000008e0: 6520 696d 706f 7274 2076 616c 6964 6174  e import validat
+000008f0: 655f 7265 7175 6573 740a 0a0a 6170 7020  e_request...app 
+00000900: 3d20 4150 4947 6174 6577 6179 5265 7374  = APIGatewayRest
+00000910: 5265 736f 6c76 6572 2829 0a0a 4061 7070  Resolver()..@app
+00000920: 2e70 6f73 7428 222f 6578 616d 706c 6522  .post("/example"
+00000930: 290a 6465 6620 6578 616d 706c 6528 2920  ).def example() 
+00000940: 2d3e 2052 6573 706f 6e73 653a 0a20 202e  -> Response:.  .
+00000950: 2e2e 0a0a 4076 616c 6964 6174 655f 7265  ....@validate_re
+00000960: 7175 6573 7428 6f61 735f 7061 7468 3d22  quest(oas_path="
+00000970: 6f70 656e 6170 692e 7961 6d6c 2229 0a64  openapi.yaml").d
+00000980: 6566 206c 616d 6264 615f 6861 6e64 6c65  ef lambda_handle
+00000990: 7228 6576 656e 743a 2044 6963 742c 2063  r(event: Dict, c
+000009a0: 6f6e 7465 7874 3a20 4c61 6d62 6461 436f  ontext: LambdaCo
+000009b0: 6e74 6578 7429 202d 3e20 4469 6374 3a0a  ntext) -> Dict:.
+000009c0: 2020 2020 7265 7370 6f6e 7365 203d 2061      response = a
+000009d0: 7070 2e72 6573 6f6c 7665 2865 7665 6e74  pp.resolve(event
+000009e0: 2c20 636f 6e74 6578 7429 0a0a 2020 2020  , context)..    
+000009f0: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
+00000a00: 6060 600a 0a23 2320 4572 726f 7220 4861  ```..## Error Ha
+00000a10: 6e64 6c69 6e67 0a49 6620 7468 6520 7661  ndling.If the va
+00000a20: 6c69 6461 7469 6f6e 2066 6169 6c73 2c20  lidation fails, 
+00000a30: 7468 6520 6465 636f 7261 746f 7220 7468  the decorator th
+00000a40: 726f 7773 2061 2060 5363 6865 6d61 5661  rows a `SchemaVa
+00000a50: 6c69 6461 746f 6e45 7272 6f72 6020 7769  lidatonError` wi
+00000a60: 7468 2072 656c 6576 616e 7420 696e 666f  th relevant info
+00000a70: 726d 6174 696f 6e20 6162 6f75 7420 7468  rmation about th
+00000a80: 6520 6661 696c 6564 2076 616c 6964 6174  e failed validat
+00000a90: 696f 6e2e 0a0a 0a23 2320 4b6e 6f77 2049  ion....## Know I
+00000aa0: 7373 7565 730a 5768 696c 6520 616c 6c20  ssues.While all 
+00000ab0: 7661 6c69 6461 7469 6f6e 2065 7272 6f72  validation error
+00000ac0: 7320 6172 6520 6361 7567 6874 2c20 7468  s are caught, th
+00000ad0: 6572 6520 6973 206f 6e6c 7920 6c69 6d69  ere is only limi
+00000ae0: 7465 6420 696e 666f 726d 6174 696f 6e20  ted information 
+00000af0: 6162 6f75 7420 7468 6520 7661 7269 6f75  about the variou
+00000b00: 7320 6572 726f 7273 2e20 5468 6520 6465  s errors. The de
+00000b10: 636f 7261 746f 7220 7769 6c6c 2074 7279  corator will try
+00000b20: 2069 7473 2062 6573 7420 746f 2074 6872   its best to thr
+00000b30: 6f77 2061 2060 5363 6865 6d61 5661 6c69  ow a `SchemaVali
+00000b40: 6461 746f 6e45 7272 6f72 600a 2873 616d  datonError`.(sam
+00000b50: 6520 6173 2074 6865 2050 6f77 6572 746f  e as the Powerto
+00000b60: 6f6c 7320 7661 6c69 6461 746f 7220 776f  ols validator wo
+00000b70: 756c 6429 2c20 7769 7468 2061 7320 6d75  uld), with as mu
+00000b80: 6368 206f 6620 7468 6520 6f70 7469 6f6e  ch of the option
+00000b90: 616c 2061 7474 7269 6275 7465 7320 6173  al attributes as
+00000ba0: 2070 6f73 7369 626c 652e 0a0a 496e 2073   possible...In s
+00000bb0: 756d 6d61 7279 2c20 6974 2069 7320 706f  ummary, it is po
+00000bc0: 7373 6962 6c65 2074 6861 7420 6e6f 7420  ssible that not 
+00000bd0: 616c 6c20 6053 6368 656d 6156 616c 6964  all `SchemaValid
+00000be0: 6174 696f 6e45 7272 6f72 7360 2773 2077  ationErrors`'s w
+00000bf0: 696c 6c20 6861 7665 2061 206e 6963 6520  ill have a nice 
+00000c00: 7661 6c69 6461 7469 6f6e 206d 6573 7361  validation messa
+00000c10: 6765 2c20 696e 2063 6173 6520 796f 7520  ge, in case you 
+00000c20: 7265 6c79 206f 6e20 7069 7069 6e67 2069  rely on piping i
+00000c30: 7420 7374 7261 6967 6874 2062 6163 6b20  t straight back 
+00000c40: 746f 2074 6865 2063 6c69 656e 742e 0a0a  to the client...
+00000c50: 0a23 2320 436f 6e74 7269 6275 7469 6f6e  .## Contribution
+00000c60: 730a 506c 6561 7365 206d 616b 6520 6120  s.Please make a 
+00000c70: 7075 6c6c 2072 6571 7565 7374 2061 6e64  pull request and
+00000c80: 2049 2077 696c 6c20 7265 7669 6577 2069   I will review i
+00000c90: 7420 4153 4150 2e0a 0a                   t ASAP...
```

