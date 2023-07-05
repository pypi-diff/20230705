# Comparing `tmp/aws-ddk-core-1.0.1.tar.gz` & `tmp/aws-ddk-core-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ddk-core-1.0.1.tar", last modified: Tue Jun 13 18:39:14 2023, max compression
+gzip compressed data, was "aws-ddk-core-1.1.0.tar", last modified: Wed Jul  5 17:36:01 2023, max compression
```

## Comparing `aws-ddk-core-1.0.1.tar` & `aws-ddk-core-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-06-13 18:39:14.557881 aws-ddk-core-1.0.1/
--rw-r--r--   0 hansonlu (569507325) 1896053708    11358 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/LICENSE
--rw-r--r--   0 hansonlu (569507325) 1896053708       23 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/MANIFEST.in
--rw-r--r--   0 hansonlu (569507325) 1896053708       67 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/NOTICE
--rw-r--r--   0 hansonlu (569507325) 1896053708     6364 2023-06-13 18:39:14.557461 aws-ddk-core-1.0.1/PKG-INFO
--rw-r--r--   0 hansonlu (569507325) 1896053708     5387 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/README.md
--rw-r--r--   0 hansonlu (569507325) 1896053708      234 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/pyproject.toml
--rw-r--r--   0 hansonlu (569507325) 1896053708       38 2023-06-13 18:39:14.558003 aws-ddk-core-1.0.1/setup.cfg
--rw-r--r--   0 hansonlu (569507325) 1896053708     2039 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/setup.py
-drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-06-13 18:39:14.541234 aws-ddk-core-1.0.1/src/
-drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-06-13 18:39:14.546616 aws-ddk-core-1.0.1/src/aws_ddk_core/
--rw-r--r--   0 hansonlu (569507325) 1896053708   542656 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/src/aws_ddk_core/__init__.py
-drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-06-13 18:39:14.549755 aws-ddk-core-1.0.1/src/aws_ddk_core/_jsii/
--rw-r--r--   0 hansonlu (569507325) 1896053708      573 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/src/aws_ddk_core/_jsii/__init__.py
--rw-r--r--   0 hansonlu (569507325) 1896053708  5017715 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/src/aws_ddk_core/_jsii/aws-ddk-core@1.0.1.jsii.tgz
--rw-r--r--   0 hansonlu (569507325) 1896053708        1 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/src/aws_ddk_core/py.typed
-drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-06-13 18:39:14.548849 aws-ddk-core-1.0.1/src/aws_ddk_core.egg-info/
--rw-r--r--   0 hansonlu (569507325) 1896053708     6364 2023-06-13 18:39:14.000000 aws-ddk-core-1.0.1/src/aws_ddk_core.egg-info/PKG-INFO
--rw-r--r--   0 hansonlu (569507325) 1896053708      400 2023-06-13 18:39:14.000000 aws-ddk-core-1.0.1/src/aws_ddk_core.egg-info/SOURCES.txt
--rw-r--r--   0 hansonlu (569507325) 1896053708        1 2023-06-13 18:39:14.000000 aws-ddk-core-1.0.1/src/aws_ddk_core.egg-info/dependency_links.txt
--rw-r--r--   0 hansonlu (569507325) 1896053708      313 2023-06-13 18:39:14.000000 aws-ddk-core-1.0.1/src/aws_ddk_core.egg-info/requires.txt
--rw-r--r--   0 hansonlu (569507325) 1896053708       13 2023-06-13 18:39:14.000000 aws-ddk-core-1.0.1/src/aws_ddk_core.egg-info/top_level.txt
+drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-07-05 17:36:01.329074 aws-ddk-core-1.1.0/
+-rw-r--r--   0 hansonlu (569507325) 1896053708    11358 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/LICENSE
+-rw-r--r--   0 hansonlu (569507325) 1896053708       23 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/MANIFEST.in
+-rw-r--r--   0 hansonlu (569507325) 1896053708       67 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/NOTICE
+-rw-r--r--   0 hansonlu (569507325) 1896053708     6364 2023-07-05 17:36:01.328621 aws-ddk-core-1.1.0/PKG-INFO
+-rw-r--r--   0 hansonlu (569507325) 1896053708     5387 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/README.md
+-rw-r--r--   0 hansonlu (569507325) 1896053708      234 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/pyproject.toml
+-rw-r--r--   0 hansonlu (569507325) 1896053708       38 2023-07-05 17:36:01.329215 aws-ddk-core-1.1.0/setup.cfg
+-rw-r--r--   0 hansonlu (569507325) 1896053708     2039 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/setup.py
+drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-07-05 17:36:01.289561 aws-ddk-core-1.1.0/src/
+drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-07-05 17:36:01.315267 aws-ddk-core-1.1.0/src/aws_ddk_core/
+-rw-r--r--   0 hansonlu (569507325) 1896053708   646858 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/src/aws_ddk_core/__init__.py
+drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-07-05 17:36:01.318823 aws-ddk-core-1.1.0/src/aws_ddk_core/_jsii/
+-rw-r--r--   0 hansonlu (569507325) 1896053708      573 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/src/aws_ddk_core/_jsii/__init__.py
+-rw-r--r--   0 hansonlu (569507325) 1896053708  5062250 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/src/aws_ddk_core/_jsii/aws-ddk-core@1.1.0.jsii.tgz
+-rw-r--r--   0 hansonlu (569507325) 1896053708        1 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/src/aws_ddk_core/py.typed
+drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-07-05 17:36:01.317655 aws-ddk-core-1.1.0/src/aws_ddk_core.egg-info/
+-rw-r--r--   0 hansonlu (569507325) 1896053708     6364 2023-07-05 17:36:01.000000 aws-ddk-core-1.1.0/src/aws_ddk_core.egg-info/PKG-INFO
+-rw-r--r--   0 hansonlu (569507325) 1896053708      400 2023-07-05 17:36:01.000000 aws-ddk-core-1.1.0/src/aws_ddk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 hansonlu (569507325) 1896053708        1 2023-07-05 17:36:01.000000 aws-ddk-core-1.1.0/src/aws_ddk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 hansonlu (569507325) 1896053708      313 2023-07-05 17:36:01.000000 aws-ddk-core-1.1.0/src/aws_ddk_core.egg-info/requires.txt
+-rw-r--r--   0 hansonlu (569507325) 1896053708       13 2023-07-05 17:36:01.000000 aws-ddk-core-1.1.0/src/aws_ddk_core.egg-info/top_level.txt
```

### Comparing `aws-ddk-core-1.0.1/LICENSE` & `aws-ddk-core-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-ddk-core-1.0.1/PKG-INFO` & `aws-ddk-core-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ddk-core
-Version: 1.0.1
+Version: 1.1.0
 Summary: AWS DataOps Development Kit
 Home-page: https://github.com/awslabs/aws-ddk/tree/main
 Author: AWS Professional Services<aws-proserve-orion-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-ddk/tree/main
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-ddk-core-1.0.1/README.md` & `aws-ddk-core-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-ddk-core-1.0.1/setup.py` & `aws-ddk-core-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-ddk-core",
-    "version": "1.0.1",
+    "version": "1.1.0",
     "description": "AWS DataOps Development Kit",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/aws-ddk/tree/main",
     "long_description_content_type": "text/markdown",
     "author": "AWS Professional Services<aws-proserve-orion-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,29 +22,29 @@
     },
     "packages": [
         "aws_ddk_core",
         "aws_ddk_core._jsii"
     ],
     "package_data": {
         "aws_ddk_core._jsii": [
-            "aws-ddk-core@1.0.1.jsii.tgz"
+            "aws-ddk-core@1.1.0.jsii.tgz"
         ],
         "aws_ddk_core": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.71.0, <3.0.0",
-        "aws-cdk.aws-glue-alpha>=2.71.0.a0, <3.0.0",
-        "aws-cdk.aws-kinesisfirehose-alpha>=2.71.0.a0, <3.0.0",
-        "aws-cdk.aws-kinesisfirehose-destinations-alpha>=2.71.0.a0, <3.0.0",
-        "aws-cdk.integ-tests-alpha>=2.71.0.a0, <3.0.0",
+        "aws-cdk-lib>=2.85.0, <3.0.0",
+        "aws-cdk.aws-glue-alpha>=2.85.0.a0, <3.0.0",
+        "aws-cdk.aws-kinesisfirehose-alpha>=2.85.0.a0, <3.0.0",
+        "aws-cdk.aws-kinesisfirehose-destinations-alpha>=2.85.0.a0, <3.0.0",
+        "aws-cdk.integ-tests-alpha>=2.85.0.a0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.83.0, <2.0.0",
+        "jsii>=1.84.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `aws-ddk-core-1.0.1/src/aws_ddk_core/__init__.py` & `aws-ddk-core-1.1.0/src/aws_ddk_core/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -131,15 +131,17 @@
 import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
 import aws_cdk.aws_kinesis as _aws_cdk_aws_kinesis_ceddda9d
 import aws_cdk.aws_kinesisfirehose_alpha as _aws_cdk_aws_kinesisfirehose_alpha_30daaf29
 import aws_cdk.aws_kinesisfirehose_destinations_alpha as _aws_cdk_aws_kinesisfirehose_destinations_alpha_8ee8dbdc
 import aws_cdk.aws_kms as _aws_cdk_aws_kms_ceddda9d
 import aws_cdk.aws_lambda as _aws_cdk_aws_lambda_ceddda9d
 import aws_cdk.aws_logs as _aws_cdk_aws_logs_ceddda9d
+import aws_cdk.aws_mwaa as _aws_cdk_aws_mwaa_ceddda9d
 import aws_cdk.aws_s3 as _aws_cdk_aws_s3_ceddda9d
+import aws_cdk.aws_s3_deployment as _aws_cdk_aws_s3_deployment_ceddda9d
 import aws_cdk.aws_sns as _aws_cdk_aws_sns_ceddda9d
 import aws_cdk.aws_sqs as _aws_cdk_aws_sqs_ceddda9d
 import aws_cdk.aws_stepfunctions as _aws_cdk_aws_stepfunctions_ceddda9d
 import aws_cdk.aws_stepfunctions_tasks as _aws_cdk_aws_stepfunctions_tasks_ceddda9d
 import aws_cdk.pipelines as _aws_cdk_pipelines_ceddda9d
 import constructs as _constructs_77d1e7e8
 
@@ -1056,14 +1058,15 @@
         permissions_boundary_arn: typing.Optional[builtins.str] = None,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
+        suppress_template_indentation: typing.Optional[builtins.bool] = None,
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a stack.
 
         Includes termination protection settings, multi-level (application, environment,
@@ -1076,14 +1079,15 @@
         :param permissions_boundary_arn: ARN of the permissions boundary managed policy.
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
+        :param suppress_template_indentation: Enable this flag to suppress indentation in generated CloudFormation templates. If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation`` context key will be used. If that is not specified, then the default value ``false`` will be used. Default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__403bc1fd4d529dd1acdcfdf6824076a7e78329d131f442981f447f8f5298a7cc)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
@@ -1094,14 +1098,15 @@
             permissions_boundary_arn=permissions_boundary_arn,
             analytics_reporting=analytics_reporting,
             cross_region_references=cross_region_references,
             description=description,
             env=env,
             permissions_boundary=permissions_boundary,
             stack_name=stack_name,
+            suppress_template_indentation=suppress_template_indentation,
             synthesizer=synthesizer,
             tags=tags,
             termination_protection=termination_protection,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
@@ -1174,14 +1179,15 @@
     name_mapping={
         "analytics_reporting": "analyticsReporting",
         "cross_region_references": "crossRegionReferences",
         "description": "description",
         "env": "env",
         "permissions_boundary": "permissionsBoundary",
         "stack_name": "stackName",
+        "suppress_template_indentation": "suppressTemplateIndentation",
         "synthesizer": "synthesizer",
         "tags": "tags",
         "termination_protection": "terminationProtection",
         "config": "config",
         "environment_id": "environmentId",
         "permissions_boundary_arn": "permissionsBoundaryArn",
     },
@@ -1192,14 +1198,15 @@
         *,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
+        suppress_template_indentation: typing.Optional[builtins.bool] = None,
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
         config: typing.Optional[typing.Union[builtins.str, typing.Union["Configuration", typing.Dict[builtins.str, typing.Any]]]] = None,
         environment_id: typing.Optional[builtins.str] = None,
         permissions_boundary_arn: typing.Optional[builtins.str] = None,
     ) -> None:
@@ -1207,14 +1214,15 @@
 
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
+        :param suppress_template_indentation: Enable this flag to suppress indentation in generated CloudFormation templates. If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation`` context key will be used. If that is not specified, then the default value ``false`` will be used. Default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         :param config: Configuration or path to file which contains the configuration.
         :param environment_id: Identifier of the environment. Default: "dev"
         :param permissions_boundary_arn: ARN of the permissions boundary managed policy.
         '''
@@ -1224,14 +1232,15 @@
             type_hints = typing.get_type_hints(_typecheckingstub__a429ca722d1fec889b8120d065d6c339e922faac9a9e70454e565500ff82514c)
             check_type(argname="argument analytics_reporting", value=analytics_reporting, expected_type=type_hints["analytics_reporting"])
             check_type(argname="argument cross_region_references", value=cross_region_references, expected_type=type_hints["cross_region_references"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument permissions_boundary", value=permissions_boundary, expected_type=type_hints["permissions_boundary"])
             check_type(argname="argument stack_name", value=stack_name, expected_type=type_hints["stack_name"])
+            check_type(argname="argument suppress_template_indentation", value=suppress_template_indentation, expected_type=type_hints["suppress_template_indentation"])
             check_type(argname="argument synthesizer", value=synthesizer, expected_type=type_hints["synthesizer"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument termination_protection", value=termination_protection, expected_type=type_hints["termination_protection"])
             check_type(argname="argument config", value=config, expected_type=type_hints["config"])
             check_type(argname="argument environment_id", value=environment_id, expected_type=type_hints["environment_id"])
             check_type(argname="argument permissions_boundary_arn", value=permissions_boundary_arn, expected_type=type_hints["permissions_boundary_arn"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -1243,14 +1252,16 @@
             self._values["description"] = description
         if env is not None:
             self._values["env"] = env
         if permissions_boundary is not None:
             self._values["permissions_boundary"] = permissions_boundary
         if stack_name is not None:
             self._values["stack_name"] = stack_name
+        if suppress_template_indentation is not None:
+            self._values["suppress_template_indentation"] = suppress_template_indentation
         if synthesizer is not None:
             self._values["synthesizer"] = synthesizer
         if tags is not None:
             self._values["tags"] = tags
         if termination_protection is not None:
             self._values["termination_protection"] = termination_protection
         if config is not None:
@@ -1382,14 +1393,27 @@
 
         :default: - Derived from construct path.
         '''
         result = self._values.get("stack_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def suppress_template_indentation(self) -> typing.Optional[builtins.bool]:
+        '''Enable this flag to suppress indentation in generated CloudFormation templates.
+
+        If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation``
+        context key will be used. If that is not specified, then the
+        default value ``false`` will be used.
+
+        :default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
+        '''
+        result = self._values.get("suppress_template_indentation")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def synthesizer(self) -> typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer]:
         '''Synthesis method to use while deploying this stack.
 
         The Stack Synthesizer controls aspects of synthesis and deployment,
         like how assets are referenced and what IAM roles to use. For more
         information, see the README of the main CDK package.
 
@@ -1564,38 +1588,41 @@
         account: typing.Optional[builtins.str] = None,
         additional_install_commands: typing.Optional[typing.Sequence[builtins.str]] = None,
         cdk_version: typing.Optional[builtins.str] = None,
         codeartifact_domain: typing.Optional[builtins.str] = None,
         codeartifact_domain_owner: typing.Optional[builtins.str] = None,
         codeartifact_repository: typing.Optional[builtins.str] = None,
         code_pipeline_source: typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer] = None,
+        env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         partition: typing.Optional[builtins.str] = None,
         region: typing.Optional[builtins.str] = None,
         role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     ) -> _aws_cdk_pipelines_ceddda9d.CodeBuildStep:
         '''
         :param account: 
         :param additional_install_commands: 
         :param cdk_version: 
         :param codeartifact_domain: 
         :param codeartifact_domain_owner: 
         :param codeartifact_repository: 
         :param code_pipeline_source: 
+        :param env: 
         :param partition: 
         :param region: 
         :param role_policy_statements: 
         '''
         props = GetSynthActionProps(
             account=account,
             additional_install_commands=additional_install_commands,
             cdk_version=cdk_version,
             codeartifact_domain=codeartifact_domain,
             codeartifact_domain_owner=codeartifact_domain_owner,
             codeartifact_repository=codeartifact_repository,
             code_pipeline_source=code_pipeline_source,
+            env=env,
             partition=partition,
             region=region,
             role_policy_statements=role_policy_statements,
         )
 
         return typing.cast(_aws_cdk_pipelines_ceddda9d.CodeBuildStep, jsii.sinvoke(cls, "getSynthAction", [props]))
 
@@ -1666,14 +1693,15 @@
         permissions_boundary_arn: typing.Optional[builtins.str] = None,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
+        suppress_template_indentation: typing.Optional[builtins.bool] = None,
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Creates a new CICD Pipeline stack.
 
         :param scope: Parent of this stack, usually an ``App`` or a ``Stage``, but could be any construct.
@@ -1685,14 +1713,15 @@
         :param permissions_boundary_arn: ARN of the permissions boundary managed policy.
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
+        :param suppress_template_indentation: Enable this flag to suppress indentation in generated CloudFormation templates. If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation`` context key will be used. If that is not specified, then the default value ``false`` will be used. Default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2a4f7374970c6409060af558e7802348870a4c4a3b9f9232e789f1488d18fb90)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
@@ -1705,14 +1734,15 @@
             permissions_boundary_arn=permissions_boundary_arn,
             analytics_reporting=analytics_reporting,
             cross_region_references=cross_region_references,
             description=description,
             env=env,
             permissions_boundary=permissions_boundary,
             stack_name=stack_name,
+            suppress_template_indentation=suppress_template_indentation,
             synthesizer=synthesizer,
             tags=tags,
             termination_protection=termination_protection,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
@@ -1835,37 +1865,40 @@
         self,
         *,
         additional_install_commands: typing.Optional[typing.Sequence[builtins.str]] = None,
         cdk_version: typing.Optional[builtins.str] = None,
         codeartifact_domain: typing.Optional[builtins.str] = None,
         codeartifact_domain_owner: typing.Optional[builtins.str] = None,
         codeartifact_repository: typing.Optional[builtins.str] = None,
+        env: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         synth_action: typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildStep] = None,
     ) -> "CICDPipelineStack":
         '''Add synth action.
 
         During synth can connect and pull artifacts from a private artifactory.
 
         :param additional_install_commands: Additional install commands.
         :param cdk_version: CDK versio to use during the synth action. Default: "latest"
         :param codeartifact_domain: Name of the CodeArtifact domain.
         :param codeartifact_domain_owner: CodeArtifact domain owner account.
         :param codeartifact_repository: Name of the CodeArtifact repository to pull artifacts from.
+        :param env: Environment variables to set.
         :param role_policy_statements: Additional policies to add to the synth action role.
         :param synth_action: Override synth action.
 
         :return: reference to this pipeline.
         '''
         props = SynthActionProps(
             additional_install_commands=additional_install_commands,
             cdk_version=cdk_version,
             codeartifact_domain=codeartifact_domain,
             codeartifact_domain_owner=codeartifact_domain_owner,
             codeartifact_repository=codeartifact_repository,
+            env=env,
             role_policy_statements=role_policy_statements,
             synth_action=synth_action,
         )
 
         return typing.cast("CICDPipelineStack", jsii.invoke(self, "addSynthAction", [props]))
 
     @jsii.member(jsii_name="addTestStage")
@@ -2086,14 +2119,15 @@
     name_mapping={
         "analytics_reporting": "analyticsReporting",
         "cross_region_references": "crossRegionReferences",
         "description": "description",
         "env": "env",
         "permissions_boundary": "permissionsBoundary",
         "stack_name": "stackName",
+        "suppress_template_indentation": "suppressTemplateIndentation",
         "synthesizer": "synthesizer",
         "tags": "tags",
         "termination_protection": "terminationProtection",
         "config": "config",
         "environment_id": "environmentId",
         "permissions_boundary_arn": "permissionsBoundaryArn",
         "cdk_language": "cdkLanguage",
@@ -2106,14 +2140,15 @@
         *,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
+        suppress_template_indentation: typing.Optional[builtins.bool] = None,
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
         config: typing.Optional[typing.Union[builtins.str, typing.Union["Configuration", typing.Dict[builtins.str, typing.Any]]]] = None,
         environment_id: typing.Optional[builtins.str] = None,
         permissions_boundary_arn: typing.Optional[builtins.str] = None,
         cdk_language: typing.Optional[builtins.str] = None,
@@ -2123,14 +2158,15 @@
 
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
+        :param suppress_template_indentation: Enable this flag to suppress indentation in generated CloudFormation templates. If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation`` context key will be used. If that is not specified, then the default value ``false`` will be used. Default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         :param config: Configuration or path to file which contains the configuration.
         :param environment_id: Identifier of the environment. Default: "dev"
         :param permissions_boundary_arn: ARN of the permissions boundary managed policy.
         :param cdk_language: Language of the CDK construct definitions. Default: "typescript"
@@ -2142,14 +2178,15 @@
             type_hints = typing.get_type_hints(_typecheckingstub__a92abb1f3b57ec36ef721160ab799be2851ede5d3e872162fc75be713f4d3293)
             check_type(argname="argument analytics_reporting", value=analytics_reporting, expected_type=type_hints["analytics_reporting"])
             check_type(argname="argument cross_region_references", value=cross_region_references, expected_type=type_hints["cross_region_references"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument permissions_boundary", value=permissions_boundary, expected_type=type_hints["permissions_boundary"])
             check_type(argname="argument stack_name", value=stack_name, expected_type=type_hints["stack_name"])
+            check_type(argname="argument suppress_template_indentation", value=suppress_template_indentation, expected_type=type_hints["suppress_template_indentation"])
             check_type(argname="argument synthesizer", value=synthesizer, expected_type=type_hints["synthesizer"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument termination_protection", value=termination_protection, expected_type=type_hints["termination_protection"])
             check_type(argname="argument config", value=config, expected_type=type_hints["config"])
             check_type(argname="argument environment_id", value=environment_id, expected_type=type_hints["environment_id"])
             check_type(argname="argument permissions_boundary_arn", value=permissions_boundary_arn, expected_type=type_hints["permissions_boundary_arn"])
             check_type(argname="argument cdk_language", value=cdk_language, expected_type=type_hints["cdk_language"])
@@ -2163,14 +2200,16 @@
             self._values["description"] = description
         if env is not None:
             self._values["env"] = env
         if permissions_boundary is not None:
             self._values["permissions_boundary"] = permissions_boundary
         if stack_name is not None:
             self._values["stack_name"] = stack_name
+        if suppress_template_indentation is not None:
+            self._values["suppress_template_indentation"] = suppress_template_indentation
         if synthesizer is not None:
             self._values["synthesizer"] = synthesizer
         if tags is not None:
             self._values["tags"] = tags
         if termination_protection is not None:
             self._values["termination_protection"] = termination_protection
         if config is not None:
@@ -2306,14 +2345,27 @@
 
         :default: - Derived from construct path.
         '''
         result = self._values.get("stack_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def suppress_template_indentation(self) -> typing.Optional[builtins.bool]:
+        '''Enable this flag to suppress indentation in generated CloudFormation templates.
+
+        If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation``
+        context key will be used. If that is not specified, then the
+        default value ``false`` will be used.
+
+        :default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
+        '''
+        result = self._values.get("suppress_template_indentation")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def synthesizer(self) -> typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer]:
         '''Synthesis method to use while deploying this stack.
 
         The Stack Synthesizer controls aspects of synthesis and deployment,
         like how assets are referenced and what IAM roles to use. For more
         information, see the README of the main CDK package.
 
@@ -3407,14 +3459,15 @@
         "account": "account",
         "additional_install_commands": "additionalInstallCommands",
         "cdk_version": "cdkVersion",
         "codeartifact_domain": "codeartifactDomain",
         "codeartifact_domain_owner": "codeartifactDomainOwner",
         "codeartifact_repository": "codeartifactRepository",
         "code_pipeline_source": "codePipelineSource",
+        "env": "env",
         "partition": "partition",
         "region": "region",
         "role_policy_statements": "rolePolicyStatements",
     },
 )
 class GetSynthActionProps:
     def __init__(
@@ -3423,39 +3476,42 @@
         account: typing.Optional[builtins.str] = None,
         additional_install_commands: typing.Optional[typing.Sequence[builtins.str]] = None,
         cdk_version: typing.Optional[builtins.str] = None,
         codeartifact_domain: typing.Optional[builtins.str] = None,
         codeartifact_domain_owner: typing.Optional[builtins.str] = None,
         codeartifact_repository: typing.Optional[builtins.str] = None,
         code_pipeline_source: typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer] = None,
+        env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         partition: typing.Optional[builtins.str] = None,
         region: typing.Optional[builtins.str] = None,
         role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     ) -> None:
         '''
         :param account: 
         :param additional_install_commands: 
         :param cdk_version: 
         :param codeartifact_domain: 
         :param codeartifact_domain_owner: 
         :param codeartifact_repository: 
         :param code_pipeline_source: 
+        :param env: 
         :param partition: 
         :param region: 
         :param role_policy_statements: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b411e230303f93f36fe42f88f3ae59e51d4746a608fa21c8fe560bb5fe18a352)
             check_type(argname="argument account", value=account, expected_type=type_hints["account"])
             check_type(argname="argument additional_install_commands", value=additional_install_commands, expected_type=type_hints["additional_install_commands"])
             check_type(argname="argument cdk_version", value=cdk_version, expected_type=type_hints["cdk_version"])
             check_type(argname="argument codeartifact_domain", value=codeartifact_domain, expected_type=type_hints["codeartifact_domain"])
             check_type(argname="argument codeartifact_domain_owner", value=codeartifact_domain_owner, expected_type=type_hints["codeartifact_domain_owner"])
             check_type(argname="argument codeartifact_repository", value=codeartifact_repository, expected_type=type_hints["codeartifact_repository"])
             check_type(argname="argument code_pipeline_source", value=code_pipeline_source, expected_type=type_hints["code_pipeline_source"])
+            check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument partition", value=partition, expected_type=type_hints["partition"])
             check_type(argname="argument region", value=region, expected_type=type_hints["region"])
             check_type(argname="argument role_policy_statements", value=role_policy_statements, expected_type=type_hints["role_policy_statements"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if account is not None:
             self._values["account"] = account
         if additional_install_commands is not None:
@@ -3466,14 +3522,16 @@
             self._values["codeartifact_domain"] = codeartifact_domain
         if codeartifact_domain_owner is not None:
             self._values["codeartifact_domain_owner"] = codeartifact_domain_owner
         if codeartifact_repository is not None:
             self._values["codeartifact_repository"] = codeartifact_repository
         if code_pipeline_source is not None:
             self._values["code_pipeline_source"] = code_pipeline_source
+        if env is not None:
+            self._values["env"] = env
         if partition is not None:
             self._values["partition"] = partition
         if region is not None:
             self._values["region"] = region
         if role_policy_statements is not None:
             self._values["role_policy_statements"] = role_policy_statements
 
@@ -3511,14 +3569,19 @@
     def code_pipeline_source(
         self,
     ) -> typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer]:
         result = self._values.get("code_pipeline_source")
         return typing.cast(typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer], result)
 
     @builtins.property
+    def env(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
+        result = self._values.get("env")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
+
+    @builtins.property
     def partition(self) -> typing.Optional[builtins.str]:
         result = self._values.get("partition")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def region(self) -> typing.Optional[builtins.str]:
         result = self._values.get("region")
@@ -3729,14 +3792,820 @@
             policy=policy,
             removal_policy=removal_policy,
         )
 
         return typing.cast(_aws_cdk_aws_kms_ceddda9d.Key, jsii.sinvoke(cls, "key", [scope, id, props]))
 
 
+class MWAAEnvironment(
+    _constructs_77d1e7e8.Construct,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="aws-ddk-core.MWAAEnvironment",
+):
+    def __init__(
+        self,
+        scope: _constructs_77d1e7e8.Construct,
+        id: builtins.str,
+        *,
+        additional_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+        dag_files: typing.Optional[typing.Sequence[builtins.str]] = None,
+        dag_processing_logs: typing.Optional[builtins.str] = None,
+        plugin_file: typing.Optional[builtins.str] = None,
+        requirements_file: typing.Optional[builtins.str] = None,
+        s3_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
+        scheduler_logs_level: typing.Optional[builtins.str] = None,
+        task_logs_level: typing.Optional[builtins.str] = None,
+        vpc_cidr: typing.Optional[builtins.str] = None,
+        vpc_id: typing.Optional[builtins.str] = None,
+        webserver_logs_level: typing.Optional[builtins.str] = None,
+        worker_logs_level: typing.Optional[builtins.str] = None,
+        name: builtins.str,
+        airflow_configuration_options: typing.Any = None,
+        airflow_version: typing.Optional[builtins.str] = None,
+        dag_s3_path: typing.Optional[builtins.str] = None,
+        environment_class: typing.Optional[builtins.str] = None,
+        execution_role_arn: typing.Optional[builtins.str] = None,
+        kms_key: typing.Optional[builtins.str] = None,
+        logging_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_mwaa_ceddda9d.CfnEnvironment.LoggingConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        max_workers: typing.Optional[jsii.Number] = None,
+        min_workers: typing.Optional[jsii.Number] = None,
+        network_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_mwaa_ceddda9d.CfnEnvironment.NetworkConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        plugins_s3_object_version: typing.Optional[builtins.str] = None,
+        plugins_s3_path: typing.Optional[builtins.str] = None,
+        requirements_s3_object_version: typing.Optional[builtins.str] = None,
+        requirements_s3_path: typing.Optional[builtins.str] = None,
+        schedulers: typing.Optional[jsii.Number] = None,
+        source_bucket_arn: typing.Optional[builtins.str] = None,
+        startup_script_s3_object_version: typing.Optional[builtins.str] = None,
+        startup_script_s3_path: typing.Optional[builtins.str] = None,
+        tags: typing.Any = None,
+        webserver_access_mode: typing.Optional[builtins.str] = None,
+        weekly_maintenance_window_start: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''
+        :param scope: -
+        :param id: -
+        :param additional_policy_statements: Additional policy statements to add to the airflow execution role.
+        :param dag_files: File(s) to be uploaded to dags location in s3 bucket.
+        :param dag_processing_logs: Log level for DagProcessing.
+        :param plugin_file: Plugin file to be uploaded to plugin path in S3. 'pluginsS3Path' must be specified as well.
+        :param requirements_file: Requirements file to be uploaded to plugin path in S3. 'requirementsS3Path' must be specified as well.
+        :param s3_bucket: S3 Bucket.
+        :param scheduler_logs_level: Log level for SchedulerLogs.
+        :param task_logs_level: Log level for TaskLogs.
+        :param vpc_cidr: The IP range (CIDR notation) for this VPC.
+        :param vpc_id: Existing vpc id.
+        :param webserver_logs_level: Log level for WebserverLogs.
+        :param worker_logs_level: Log level for WorkerLogs.
+        :param name: The name of your Amazon MWAA environment.
+        :param airflow_configuration_options: A list of key-value pairs containing the Airflow configuration options for your environment. For example, ``core.default_timezone: utc`` . To learn more, see `Apache Airflow configuration options <https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-env-variables.html>`_ .
+        :param airflow_version: The version of Apache Airflow to use for the environment. If no value is specified, defaults to the latest version. *Allowed Values* : ``2.0.2`` | ``1.10.12`` | ``2.2.2`` | ``2.4.3`` | ``2.5.1`` (latest)
+        :param dag_s3_path: The relative path to the DAGs folder on your Amazon S3 bucket. For example, ``dags`` . To learn more, see `Adding or updating DAGs <https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-folder.html>`_ .
+        :param environment_class: The environment class type. Valid values: ``mw1.small`` , ``mw1.medium`` , ``mw1.large`` . To learn more, see `Amazon MWAA environment class <https://docs.aws.amazon.com/mwaa/latest/userguide/environment-class.html>`_ .
+        :param execution_role_arn: The Amazon Resource Name (ARN) of the execution role in IAM that allows MWAA to access AWS resources in your environment. For example, ``arn:aws:iam::123456789:role/my-execution-role`` . To learn more, see `Amazon MWAA Execution role <https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-create-role.html>`_ .
+        :param kms_key: The AWS Key Management Service (KMS) key to encrypt and decrypt the data in your environment. You can use an AWS KMS key managed by MWAA, or a customer-managed KMS key (advanced).
+        :param logging_configuration: The Apache Airflow logs being sent to CloudWatch Logs: ``DagProcessingLogs`` , ``SchedulerLogs`` , ``TaskLogs`` , ``WebserverLogs`` , ``WorkerLogs`` .
+        :param max_workers: The maximum number of workers that you want to run in your environment. MWAA scales the number of Apache Airflow workers up to the number you specify in the ``MaxWorkers`` field. For example, ``20`` . When there are no more tasks running, and no more in the queue, MWAA disposes of the extra workers leaving the one worker that is included with your environment, or the number you specify in ``MinWorkers`` .
+        :param min_workers: The minimum number of workers that you want to run in your environment. MWAA scales the number of Apache Airflow workers up to the number you specify in the ``MaxWorkers`` field. When there are no more tasks running, and no more in the queue, MWAA disposes of the extra workers leaving the worker count you specify in the ``MinWorkers`` field. For example, ``2`` .
+        :param network_configuration: The VPC networking components used to secure and enable network traffic between the AWS resources for your environment. To learn more, see `About networking on Amazon MWAA <https://docs.aws.amazon.com/mwaa/latest/userguide/networking-about.html>`_ .
+        :param plugins_s3_object_version: The version of the plugins.zip file on your Amazon S3 bucket. To learn more, see `Installing custom plugins <https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-import-plugins.html>`_ .
+        :param plugins_s3_path: The relative path to the ``plugins.zip`` file on your Amazon S3 bucket. For example, ``plugins.zip`` . To learn more, see `Installing custom plugins <https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-import-plugins.html>`_ .
+        :param requirements_s3_object_version: The version of the requirements.txt file on your Amazon S3 bucket. To learn more, see `Installing Python dependencies <https://docs.aws.amazon.com/mwaa/latest/userguide/working-dags-dependencies.html>`_ .
+        :param requirements_s3_path: The relative path to the ``requirements.txt`` file on your Amazon S3 bucket. For example, ``requirements.txt`` . To learn more, see `Installing Python dependencies <https://docs.aws.amazon.com/mwaa/latest/userguide/working-dags-dependencies.html>`_ .
+        :param schedulers: The number of schedulers that you want to run in your environment. Valid values:. - *v2* - Accepts between 2 to 5. Defaults to 2. - *v1* - Accepts 1.
+        :param source_bucket_arn: The Amazon Resource Name (ARN) of the Amazon S3 bucket where your DAG code and supporting files are stored. For example, ``arn:aws:s3:::my-airflow-bucket-unique-name`` . To learn more, see `Create an Amazon S3 bucket for Amazon MWAA <https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-s3-bucket.html>`_ .
+        :param startup_script_s3_object_version: The version of the startup shell script in your Amazon S3 bucket. You must specify the `version ID <https://docs.aws.amazon.com/AmazonS3/latest/userguide/versioning-workflows.html>`_ that Amazon S3 assigns to the file every time you update the script. Version IDs are Unicode, UTF-8 encoded, URL-ready, opaque strings that are no more than 1,024 bytes long. The following is an example: ``3sL4kqtJlcpXroDTDmJ+rmSpXd3dIbrHY+MTRCxf3vjVBH40Nr8X8gdRQBpUMLUo`` For more information, see `Using a startup script <https://docs.aws.amazon.com/mwaa/latest/userguide/using-startup-script.html>`_ .
+        :param startup_script_s3_path: The relative path to the startup shell script in your Amazon S3 bucket. For example, ``s3://mwaa-environment/startup.sh`` . Amazon MWAA runs the script as your environment starts, and before running the Apache Airflow process. You can use this script to install dependencies, modify Apache Airflow configuration options, and set environment variables. For more information, see `Using a startup script <https://docs.aws.amazon.com/mwaa/latest/userguide/using-startup-script.html>`_ .
+        :param tags: The key-value tag pairs associated to your environment. For example, ``"Environment": "Staging"`` . To learn more, see `Tagging <https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html>`_ .
+        :param webserver_access_mode: The Apache Airflow *Web server* access mode. To learn more, see `Apache Airflow access modes <https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-networking.html>`_ . Valid values: ``PRIVATE_ONLY`` or ``PUBLIC_ONLY`` .
+        :param weekly_maintenance_window_start: The day and time of the week to start weekly maintenance updates of your environment in the following format: ``DAY:HH:MM`` . For example: ``TUE:03:30`` . You can specify a start time in 30 minute increments only. Supported input includes the following: - MON|TUE|WED|THU|FRI|SAT|SUN:([01]\\d|2[0-3]):(00|30)
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__2f57013032bd3f5e03e8cf2f82cc7c98b621d613c29a1e1844390ce9e164789e)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = MWAAEnvironmentProps(
+            additional_policy_statements=additional_policy_statements,
+            dag_files=dag_files,
+            dag_processing_logs=dag_processing_logs,
+            plugin_file=plugin_file,
+            requirements_file=requirements_file,
+            s3_bucket=s3_bucket,
+            scheduler_logs_level=scheduler_logs_level,
+            task_logs_level=task_logs_level,
+            vpc_cidr=vpc_cidr,
+            vpc_id=vpc_id,
+            webserver_logs_level=webserver_logs_level,
+            worker_logs_level=worker_logs_level,
+            name=name,
+            airflow_configuration_options=airflow_configuration_options,
+            airflow_version=airflow_version,
+            dag_s3_path=dag_s3_path,
+            environment_class=environment_class,
+            execution_role_arn=execution_role_arn,
+            kms_key=kms_key,
+            logging_configuration=logging_configuration,
+            max_workers=max_workers,
+            min_workers=min_workers,
+            network_configuration=network_configuration,
+            plugins_s3_object_version=plugins_s3_object_version,
+            plugins_s3_path=plugins_s3_path,
+            requirements_s3_object_version=requirements_s3_object_version,
+            requirements_s3_path=requirements_s3_path,
+            schedulers=schedulers,
+            source_bucket_arn=source_bucket_arn,
+            startup_script_s3_object_version=startup_script_s3_object_version,
+            startup_script_s3_path=startup_script_s3_path,
+            tags=tags,
+            webserver_access_mode=webserver_access_mode,
+            weekly_maintenance_window_start=weekly_maintenance_window_start,
+        )
+
+        jsii.create(self.__class__, self, [scope, id, props])
+
+    @jsii.member(jsii_name="createVpc")
+    def create_vpc(
+        self,
+        scope: _constructs_77d1e7e8.Construct,
+        environment_name: builtins.str,
+        vpc_cidr: builtins.str,
+    ) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
+        '''
+        :param scope: -
+        :param environment_name: -
+        :param vpc_cidr: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__274336e52a6efd650b5a38d3d50c0d6df8879c749af035d91610fec06e12c9fb)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument environment_name", value=environment_name, expected_type=type_hints["environment_name"])
+            check_type(argname="argument vpc_cidr", value=vpc_cidr, expected_type=type_hints["vpc_cidr"])
+        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, jsii.invoke(self, "createVpc", [scope, environment_name, vpc_cidr]))
+
+    @builtins.property
+    @jsii.member(jsii_name="dagProcessingLogs")
+    def dag_processing_logs(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "dagProcessingLogs"))
+
+    @builtins.property
+    @jsii.member(jsii_name="dagS3Path")
+    def dag_s3_path(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "dagS3Path"))
+
+    @builtins.property
+    @jsii.member(jsii_name="mwaaEnvironment")
+    def mwaa_environment(self) -> _aws_cdk_aws_mwaa_ceddda9d.CfnEnvironment:
+        return typing.cast(_aws_cdk_aws_mwaa_ceddda9d.CfnEnvironment, jsii.get(self, "mwaaEnvironment"))
+
+    @builtins.property
+    @jsii.member(jsii_name="s3Bucket")
+    def s3_bucket(self) -> _aws_cdk_aws_s3_ceddda9d.IBucket:
+        return typing.cast(_aws_cdk_aws_s3_ceddda9d.IBucket, jsii.get(self, "s3Bucket"))
+
+    @builtins.property
+    @jsii.member(jsii_name="schedulerLogsLevel")
+    def scheduler_logs_level(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "schedulerLogsLevel"))
+
+    @builtins.property
+    @jsii.member(jsii_name="taskLogsLevel")
+    def task_logs_level(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "taskLogsLevel"))
+
+    @builtins.property
+    @jsii.member(jsii_name="vpc")
+    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
+        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, jsii.get(self, "vpc"))
+
+    @builtins.property
+    @jsii.member(jsii_name="webserverLogsLevel")
+    def webserver_logs_level(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "webserverLogsLevel"))
+
+    @builtins.property
+    @jsii.member(jsii_name="workerLogsLevel")
+    def worker_logs_level(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "workerLogsLevel"))
+
+    @builtins.property
+    @jsii.member(jsii_name="pluginFile")
+    def plugin_file(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_s3_deployment_ceddda9d.BucketDeployment]:
+        return typing.cast(typing.Optional[_aws_cdk_aws_s3_deployment_ceddda9d.BucketDeployment], jsii.get(self, "pluginFile"))
+
+
+@jsii.data_type(
+    jsii_type="aws-ddk-core.MWAAEnvironmentProps",
+    jsii_struct_bases=[_aws_cdk_aws_mwaa_ceddda9d.CfnEnvironmentProps],
+    name_mapping={
+        "name": "name",
+        "airflow_configuration_options": "airflowConfigurationOptions",
+        "airflow_version": "airflowVersion",
+        "dag_s3_path": "dagS3Path",
+        "environment_class": "environmentClass",
+        "execution_role_arn": "executionRoleArn",
+        "kms_key": "kmsKey",
+        "logging_configuration": "loggingConfiguration",
+        "max_workers": "maxWorkers",
+        "min_workers": "minWorkers",
+        "network_configuration": "networkConfiguration",
+        "plugins_s3_object_version": "pluginsS3ObjectVersion",
+        "plugins_s3_path": "pluginsS3Path",
+        "requirements_s3_object_version": "requirementsS3ObjectVersion",
+        "requirements_s3_path": "requirementsS3Path",
+        "schedulers": "schedulers",
+        "source_bucket_arn": "sourceBucketArn",
+        "startup_script_s3_object_version": "startupScriptS3ObjectVersion",
+        "startup_script_s3_path": "startupScriptS3Path",
+        "tags": "tags",
+        "webserver_access_mode": "webserverAccessMode",
+        "weekly_maintenance_window_start": "weeklyMaintenanceWindowStart",
+        "additional_policy_statements": "additionalPolicyStatements",
+        "dag_files": "dagFiles",
+        "dag_processing_logs": "dagProcessingLogs",
+        "plugin_file": "pluginFile",
+        "requirements_file": "requirementsFile",
+        "s3_bucket": "s3Bucket",
+        "scheduler_logs_level": "schedulerLogsLevel",
+        "task_logs_level": "taskLogsLevel",
+        "vpc_cidr": "vpcCidr",
+        "vpc_id": "vpcId",
+        "webserver_logs_level": "webserverLogsLevel",
+        "worker_logs_level": "workerLogsLevel",
+    },
+)
+class MWAAEnvironmentProps(_aws_cdk_aws_mwaa_ceddda9d.CfnEnvironmentProps):
+    def __init__(
+        self,
+        *,
+        name: builtins.str,
+        airflow_configuration_options: typing.Any = None,
+        airflow_version: typing.Optional[builtins.str] = None,
+        dag_s3_path: typing.Optional[builtins.str] = None,
+        environment_class: typing.Optional[builtins.str] = None,
+        execution_role_arn: typing.Optional[builtins.str] = None,
+        kms_key: typing.Optional[builtins.str] = None,
+        logging_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_mwaa_ceddda9d.CfnEnvironment.LoggingConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        max_workers: typing.Optional[jsii.Number] = None,
+        min_workers: typing.Optional[jsii.Number] = None,
+        network_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_mwaa_ceddda9d.CfnEnvironment.NetworkConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        plugins_s3_object_version: typing.Optional[builtins.str] = None,
+        plugins_s3_path: typing.Optional[builtins.str] = None,
+        requirements_s3_object_version: typing.Optional[builtins.str] = None,
+        requirements_s3_path: typing.Optional[builtins.str] = None,
+        schedulers: typing.Optional[jsii.Number] = None,
+        source_bucket_arn: typing.Optional[builtins.str] = None,
+        startup_script_s3_object_version: typing.Optional[builtins.str] = None,
+        startup_script_s3_path: typing.Optional[builtins.str] = None,
+        tags: typing.Any = None,
+        webserver_access_mode: typing.Optional[builtins.str] = None,
+        weekly_maintenance_window_start: typing.Optional[builtins.str] = None,
+        additional_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+        dag_files: typing.Optional[typing.Sequence[builtins.str]] = None,
+        dag_processing_logs: typing.Optional[builtins.str] = None,
+        plugin_file: typing.Optional[builtins.str] = None,
+        requirements_file: typing.Optional[builtins.str] = None,
+        s3_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
+        scheduler_logs_level: typing.Optional[builtins.str] = None,
+        task_logs_level: typing.Optional[builtins.str] = None,
+        vpc_cidr: typing.Optional[builtins.str] = None,
+        vpc_id: typing.Optional[builtins.str] = None,
+        webserver_logs_level: typing.Optional[builtins.str] = None,
+        worker_logs_level: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''
+        :param name: The name of your Amazon MWAA environment.
+        :param airflow_configuration_options: A list of key-value pairs containing the Airflow configuration options for your environment. For example, ``core.default_timezone: utc`` . To learn more, see `Apache Airflow configuration options <https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-env-variables.html>`_ .
+        :param airflow_version: The version of Apache Airflow to use for the environment. If no value is specified, defaults to the latest version. *Allowed Values* : ``2.0.2`` | ``1.10.12`` | ``2.2.2`` | ``2.4.3`` | ``2.5.1`` (latest)
+        :param dag_s3_path: The relative path to the DAGs folder on your Amazon S3 bucket. For example, ``dags`` . To learn more, see `Adding or updating DAGs <https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-folder.html>`_ .
+        :param environment_class: The environment class type. Valid values: ``mw1.small`` , ``mw1.medium`` , ``mw1.large`` . To learn more, see `Amazon MWAA environment class <https://docs.aws.amazon.com/mwaa/latest/userguide/environment-class.html>`_ .
+        :param execution_role_arn: The Amazon Resource Name (ARN) of the execution role in IAM that allows MWAA to access AWS resources in your environment. For example, ``arn:aws:iam::123456789:role/my-execution-role`` . To learn more, see `Amazon MWAA Execution role <https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-create-role.html>`_ .
+        :param kms_key: The AWS Key Management Service (KMS) key to encrypt and decrypt the data in your environment. You can use an AWS KMS key managed by MWAA, or a customer-managed KMS key (advanced).
+        :param logging_configuration: The Apache Airflow logs being sent to CloudWatch Logs: ``DagProcessingLogs`` , ``SchedulerLogs`` , ``TaskLogs`` , ``WebserverLogs`` , ``WorkerLogs`` .
+        :param max_workers: The maximum number of workers that you want to run in your environment. MWAA scales the number of Apache Airflow workers up to the number you specify in the ``MaxWorkers`` field. For example, ``20`` . When there are no more tasks running, and no more in the queue, MWAA disposes of the extra workers leaving the one worker that is included with your environment, or the number you specify in ``MinWorkers`` .
+        :param min_workers: The minimum number of workers that you want to run in your environment. MWAA scales the number of Apache Airflow workers up to the number you specify in the ``MaxWorkers`` field. When there are no more tasks running, and no more in the queue, MWAA disposes of the extra workers leaving the worker count you specify in the ``MinWorkers`` field. For example, ``2`` .
+        :param network_configuration: The VPC networking components used to secure and enable network traffic between the AWS resources for your environment. To learn more, see `About networking on Amazon MWAA <https://docs.aws.amazon.com/mwaa/latest/userguide/networking-about.html>`_ .
+        :param plugins_s3_object_version: The version of the plugins.zip file on your Amazon S3 bucket. To learn more, see `Installing custom plugins <https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-import-plugins.html>`_ .
+        :param plugins_s3_path: The relative path to the ``plugins.zip`` file on your Amazon S3 bucket. For example, ``plugins.zip`` . To learn more, see `Installing custom plugins <https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-import-plugins.html>`_ .
+        :param requirements_s3_object_version: The version of the requirements.txt file on your Amazon S3 bucket. To learn more, see `Installing Python dependencies <https://docs.aws.amazon.com/mwaa/latest/userguide/working-dags-dependencies.html>`_ .
+        :param requirements_s3_path: The relative path to the ``requirements.txt`` file on your Amazon S3 bucket. For example, ``requirements.txt`` . To learn more, see `Installing Python dependencies <https://docs.aws.amazon.com/mwaa/latest/userguide/working-dags-dependencies.html>`_ .
+        :param schedulers: The number of schedulers that you want to run in your environment. Valid values:. - *v2* - Accepts between 2 to 5. Defaults to 2. - *v1* - Accepts 1.
+        :param source_bucket_arn: The Amazon Resource Name (ARN) of the Amazon S3 bucket where your DAG code and supporting files are stored. For example, ``arn:aws:s3:::my-airflow-bucket-unique-name`` . To learn more, see `Create an Amazon S3 bucket for Amazon MWAA <https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-s3-bucket.html>`_ .
+        :param startup_script_s3_object_version: The version of the startup shell script in your Amazon S3 bucket. You must specify the `version ID <https://docs.aws.amazon.com/AmazonS3/latest/userguide/versioning-workflows.html>`_ that Amazon S3 assigns to the file every time you update the script. Version IDs are Unicode, UTF-8 encoded, URL-ready, opaque strings that are no more than 1,024 bytes long. The following is an example: ``3sL4kqtJlcpXroDTDmJ+rmSpXd3dIbrHY+MTRCxf3vjVBH40Nr8X8gdRQBpUMLUo`` For more information, see `Using a startup script <https://docs.aws.amazon.com/mwaa/latest/userguide/using-startup-script.html>`_ .
+        :param startup_script_s3_path: The relative path to the startup shell script in your Amazon S3 bucket. For example, ``s3://mwaa-environment/startup.sh`` . Amazon MWAA runs the script as your environment starts, and before running the Apache Airflow process. You can use this script to install dependencies, modify Apache Airflow configuration options, and set environment variables. For more information, see `Using a startup script <https://docs.aws.amazon.com/mwaa/latest/userguide/using-startup-script.html>`_ .
+        :param tags: The key-value tag pairs associated to your environment. For example, ``"Environment": "Staging"`` . To learn more, see `Tagging <https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html>`_ .
+        :param webserver_access_mode: The Apache Airflow *Web server* access mode. To learn more, see `Apache Airflow access modes <https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-networking.html>`_ . Valid values: ``PRIVATE_ONLY`` or ``PUBLIC_ONLY`` .
+        :param weekly_maintenance_window_start: The day and time of the week to start weekly maintenance updates of your environment in the following format: ``DAY:HH:MM`` . For example: ``TUE:03:30`` . You can specify a start time in 30 minute increments only. Supported input includes the following: - MON|TUE|WED|THU|FRI|SAT|SUN:([01]\\d|2[0-3]):(00|30)
+        :param additional_policy_statements: Additional policy statements to add to the airflow execution role.
+        :param dag_files: File(s) to be uploaded to dags location in s3 bucket.
+        :param dag_processing_logs: Log level for DagProcessing.
+        :param plugin_file: Plugin file to be uploaded to plugin path in S3. 'pluginsS3Path' must be specified as well.
+        :param requirements_file: Requirements file to be uploaded to plugin path in S3. 'requirementsS3Path' must be specified as well.
+        :param s3_bucket: S3 Bucket.
+        :param scheduler_logs_level: Log level for SchedulerLogs.
+        :param task_logs_level: Log level for TaskLogs.
+        :param vpc_cidr: The IP range (CIDR notation) for this VPC.
+        :param vpc_id: Existing vpc id.
+        :param webserver_logs_level: Log level for WebserverLogs.
+        :param worker_logs_level: Log level for WorkerLogs.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__8947f25c6bd15e846e7d13e9c335c4e41f800116e21ba100b25118382fcd659c)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument airflow_configuration_options", value=airflow_configuration_options, expected_type=type_hints["airflow_configuration_options"])
+            check_type(argname="argument airflow_version", value=airflow_version, expected_type=type_hints["airflow_version"])
+            check_type(argname="argument dag_s3_path", value=dag_s3_path, expected_type=type_hints["dag_s3_path"])
+            check_type(argname="argument environment_class", value=environment_class, expected_type=type_hints["environment_class"])
+            check_type(argname="argument execution_role_arn", value=execution_role_arn, expected_type=type_hints["execution_role_arn"])
+            check_type(argname="argument kms_key", value=kms_key, expected_type=type_hints["kms_key"])
+            check_type(argname="argument logging_configuration", value=logging_configuration, expected_type=type_hints["logging_configuration"])
+            check_type(argname="argument max_workers", value=max_workers, expected_type=type_hints["max_workers"])
+            check_type(argname="argument min_workers", value=min_workers, expected_type=type_hints["min_workers"])
+            check_type(argname="argument network_configuration", value=network_configuration, expected_type=type_hints["network_configuration"])
+            check_type(argname="argument plugins_s3_object_version", value=plugins_s3_object_version, expected_type=type_hints["plugins_s3_object_version"])
+            check_type(argname="argument plugins_s3_path", value=plugins_s3_path, expected_type=type_hints["plugins_s3_path"])
+            check_type(argname="argument requirements_s3_object_version", value=requirements_s3_object_version, expected_type=type_hints["requirements_s3_object_version"])
+            check_type(argname="argument requirements_s3_path", value=requirements_s3_path, expected_type=type_hints["requirements_s3_path"])
+            check_type(argname="argument schedulers", value=schedulers, expected_type=type_hints["schedulers"])
+            check_type(argname="argument source_bucket_arn", value=source_bucket_arn, expected_type=type_hints["source_bucket_arn"])
+            check_type(argname="argument startup_script_s3_object_version", value=startup_script_s3_object_version, expected_type=type_hints["startup_script_s3_object_version"])
+            check_type(argname="argument startup_script_s3_path", value=startup_script_s3_path, expected_type=type_hints["startup_script_s3_path"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument webserver_access_mode", value=webserver_access_mode, expected_type=type_hints["webserver_access_mode"])
+            check_type(argname="argument weekly_maintenance_window_start", value=weekly_maintenance_window_start, expected_type=type_hints["weekly_maintenance_window_start"])
+            check_type(argname="argument additional_policy_statements", value=additional_policy_statements, expected_type=type_hints["additional_policy_statements"])
+            check_type(argname="argument dag_files", value=dag_files, expected_type=type_hints["dag_files"])
+            check_type(argname="argument dag_processing_logs", value=dag_processing_logs, expected_type=type_hints["dag_processing_logs"])
+            check_type(argname="argument plugin_file", value=plugin_file, expected_type=type_hints["plugin_file"])
+            check_type(argname="argument requirements_file", value=requirements_file, expected_type=type_hints["requirements_file"])
+            check_type(argname="argument s3_bucket", value=s3_bucket, expected_type=type_hints["s3_bucket"])
+            check_type(argname="argument scheduler_logs_level", value=scheduler_logs_level, expected_type=type_hints["scheduler_logs_level"])
+            check_type(argname="argument task_logs_level", value=task_logs_level, expected_type=type_hints["task_logs_level"])
+            check_type(argname="argument vpc_cidr", value=vpc_cidr, expected_type=type_hints["vpc_cidr"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument webserver_logs_level", value=webserver_logs_level, expected_type=type_hints["webserver_logs_level"])
+            check_type(argname="argument worker_logs_level", value=worker_logs_level, expected_type=type_hints["worker_logs_level"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "name": name,
+        }
+        if airflow_configuration_options is not None:
+            self._values["airflow_configuration_options"] = airflow_configuration_options
+        if airflow_version is not None:
+            self._values["airflow_version"] = airflow_version
+        if dag_s3_path is not None:
+            self._values["dag_s3_path"] = dag_s3_path
+        if environment_class is not None:
+            self._values["environment_class"] = environment_class
+        if execution_role_arn is not None:
+            self._values["execution_role_arn"] = execution_role_arn
+        if kms_key is not None:
+            self._values["kms_key"] = kms_key
+        if logging_configuration is not None:
+            self._values["logging_configuration"] = logging_configuration
+        if max_workers is not None:
+            self._values["max_workers"] = max_workers
+        if min_workers is not None:
+            self._values["min_workers"] = min_workers
+        if network_configuration is not None:
+            self._values["network_configuration"] = network_configuration
+        if plugins_s3_object_version is not None:
+            self._values["plugins_s3_object_version"] = plugins_s3_object_version
+        if plugins_s3_path is not None:
+            self._values["plugins_s3_path"] = plugins_s3_path
+        if requirements_s3_object_version is not None:
+            self._values["requirements_s3_object_version"] = requirements_s3_object_version
+        if requirements_s3_path is not None:
+            self._values["requirements_s3_path"] = requirements_s3_path
+        if schedulers is not None:
+            self._values["schedulers"] = schedulers
+        if source_bucket_arn is not None:
+            self._values["source_bucket_arn"] = source_bucket_arn
+        if startup_script_s3_object_version is not None:
+            self._values["startup_script_s3_object_version"] = startup_script_s3_object_version
+        if startup_script_s3_path is not None:
+            self._values["startup_script_s3_path"] = startup_script_s3_path
+        if tags is not None:
+            self._values["tags"] = tags
+        if webserver_access_mode is not None:
+            self._values["webserver_access_mode"] = webserver_access_mode
+        if weekly_maintenance_window_start is not None:
+            self._values["weekly_maintenance_window_start"] = weekly_maintenance_window_start
+        if additional_policy_statements is not None:
+            self._values["additional_policy_statements"] = additional_policy_statements
+        if dag_files is not None:
+            self._values["dag_files"] = dag_files
+        if dag_processing_logs is not None:
+            self._values["dag_processing_logs"] = dag_processing_logs
+        if plugin_file is not None:
+            self._values["plugin_file"] = plugin_file
+        if requirements_file is not None:
+            self._values["requirements_file"] = requirements_file
+        if s3_bucket is not None:
+            self._values["s3_bucket"] = s3_bucket
+        if scheduler_logs_level is not None:
+            self._values["scheduler_logs_level"] = scheduler_logs_level
+        if task_logs_level is not None:
+            self._values["task_logs_level"] = task_logs_level
+        if vpc_cidr is not None:
+            self._values["vpc_cidr"] = vpc_cidr
+        if vpc_id is not None:
+            self._values["vpc_id"] = vpc_id
+        if webserver_logs_level is not None:
+            self._values["webserver_logs_level"] = webserver_logs_level
+        if worker_logs_level is not None:
+            self._values["worker_logs_level"] = worker_logs_level
+
+    @builtins.property
+    def name(self) -> builtins.str:
+        '''The name of your Amazon MWAA environment.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-name
+        '''
+        result = self._values.get("name")
+        assert result is not None, "Required property 'name' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def airflow_configuration_options(self) -> typing.Any:
+        '''A list of key-value pairs containing the Airflow configuration options for your environment.
+
+        For example, ``core.default_timezone: utc`` . To learn more, see `Apache Airflow configuration options <https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-env-variables.html>`_ .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-airflowconfigurationoptions
+        '''
+        result = self._values.get("airflow_configuration_options")
+        return typing.cast(typing.Any, result)
+
+    @builtins.property
+    def airflow_version(self) -> typing.Optional[builtins.str]:
+        '''The version of Apache Airflow to use for the environment.
+
+        If no value is specified, defaults to the latest version.
+
+        *Allowed Values* : ``2.0.2`` | ``1.10.12`` | ``2.2.2`` | ``2.4.3`` | ``2.5.1`` (latest)
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-airflowversion
+        '''
+        result = self._values.get("airflow_version")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def dag_s3_path(self) -> typing.Optional[builtins.str]:
+        '''The relative path to the DAGs folder on your Amazon S3 bucket.
+
+        For example, ``dags`` . To learn more, see `Adding or updating DAGs <https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-folder.html>`_ .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-dags3path
+        '''
+        result = self._values.get("dag_s3_path")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def environment_class(self) -> typing.Optional[builtins.str]:
+        '''The environment class type.
+
+        Valid values: ``mw1.small`` , ``mw1.medium`` , ``mw1.large`` . To learn more, see `Amazon MWAA environment class <https://docs.aws.amazon.com/mwaa/latest/userguide/environment-class.html>`_ .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-environmentclass
+        '''
+        result = self._values.get("environment_class")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def execution_role_arn(self) -> typing.Optional[builtins.str]:
+        '''The Amazon Resource Name (ARN) of the execution role in IAM that allows MWAA to access AWS resources in your environment.
+
+        For example, ``arn:aws:iam::123456789:role/my-execution-role`` . To learn more, see `Amazon MWAA Execution role <https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-create-role.html>`_ .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-executionrolearn
+        '''
+        result = self._values.get("execution_role_arn")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def kms_key(self) -> typing.Optional[builtins.str]:
+        '''The AWS Key Management Service (KMS) key to encrypt and decrypt the data in your environment.
+
+        You can use an AWS KMS key managed by MWAA, or a customer-managed KMS key (advanced).
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-kmskey
+        '''
+        result = self._values.get("kms_key")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def logging_configuration(
+        self,
+    ) -> typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_mwaa_ceddda9d.CfnEnvironment.LoggingConfigurationProperty]]:
+        '''The Apache Airflow logs being sent to CloudWatch Logs: ``DagProcessingLogs`` , ``SchedulerLogs`` , ``TaskLogs`` , ``WebserverLogs`` , ``WorkerLogs`` .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-loggingconfiguration
+        '''
+        result = self._values.get("logging_configuration")
+        return typing.cast(typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_mwaa_ceddda9d.CfnEnvironment.LoggingConfigurationProperty]], result)
+
+    @builtins.property
+    def max_workers(self) -> typing.Optional[jsii.Number]:
+        '''The maximum number of workers that you want to run in your environment.
+
+        MWAA scales the number of Apache Airflow workers up to the number you specify in the ``MaxWorkers`` field. For example, ``20`` . When there are no more tasks running, and no more in the queue, MWAA disposes of the extra workers leaving the one worker that is included with your environment, or the number you specify in ``MinWorkers`` .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-maxworkers
+        '''
+        result = self._values.get("max_workers")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def min_workers(self) -> typing.Optional[jsii.Number]:
+        '''The minimum number of workers that you want to run in your environment.
+
+        MWAA scales the number of Apache Airflow workers up to the number you specify in the ``MaxWorkers`` field. When there are no more tasks running, and no more in the queue, MWAA disposes of the extra workers leaving the worker count you specify in the ``MinWorkers`` field. For example, ``2`` .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-minworkers
+        '''
+        result = self._values.get("min_workers")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def network_configuration(
+        self,
+    ) -> typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_mwaa_ceddda9d.CfnEnvironment.NetworkConfigurationProperty]]:
+        '''The VPC networking components used to secure and enable network traffic between the AWS resources for your environment.
+
+        To learn more, see `About networking on Amazon MWAA <https://docs.aws.amazon.com/mwaa/latest/userguide/networking-about.html>`_ .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-networkconfiguration
+        '''
+        result = self._values.get("network_configuration")
+        return typing.cast(typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_mwaa_ceddda9d.CfnEnvironment.NetworkConfigurationProperty]], result)
+
+    @builtins.property
+    def plugins_s3_object_version(self) -> typing.Optional[builtins.str]:
+        '''The version of the plugins.zip file on your Amazon S3 bucket. To learn more, see `Installing custom plugins <https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-import-plugins.html>`_ .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-pluginss3objectversion
+        '''
+        result = self._values.get("plugins_s3_object_version")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def plugins_s3_path(self) -> typing.Optional[builtins.str]:
+        '''The relative path to the ``plugins.zip`` file on your Amazon S3 bucket. For example, ``plugins.zip`` . To learn more, see `Installing custom plugins <https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-import-plugins.html>`_ .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-pluginss3path
+        '''
+        result = self._values.get("plugins_s3_path")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def requirements_s3_object_version(self) -> typing.Optional[builtins.str]:
+        '''The version of the requirements.txt file on your Amazon S3 bucket. To learn more, see `Installing Python dependencies <https://docs.aws.amazon.com/mwaa/latest/userguide/working-dags-dependencies.html>`_ .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-requirementss3objectversion
+        '''
+        result = self._values.get("requirements_s3_object_version")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def requirements_s3_path(self) -> typing.Optional[builtins.str]:
+        '''The relative path to the ``requirements.txt`` file on your Amazon S3 bucket. For example, ``requirements.txt`` . To learn more, see `Installing Python dependencies <https://docs.aws.amazon.com/mwaa/latest/userguide/working-dags-dependencies.html>`_ .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-requirementss3path
+        '''
+        result = self._values.get("requirements_s3_path")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def schedulers(self) -> typing.Optional[jsii.Number]:
+        '''The number of schedulers that you want to run in your environment. Valid values:.
+
+        - *v2* - Accepts between 2 to 5. Defaults to 2.
+        - *v1* - Accepts 1.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-schedulers
+        '''
+        result = self._values.get("schedulers")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def source_bucket_arn(self) -> typing.Optional[builtins.str]:
+        '''The Amazon Resource Name (ARN) of the Amazon S3 bucket where your DAG code and supporting files are stored.
+
+        For example, ``arn:aws:s3:::my-airflow-bucket-unique-name`` . To learn more, see `Create an Amazon S3 bucket for Amazon MWAA <https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-s3-bucket.html>`_ .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-sourcebucketarn
+        '''
+        result = self._values.get("source_bucket_arn")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def startup_script_s3_object_version(self) -> typing.Optional[builtins.str]:
+        '''The version of the startup shell script in your Amazon S3 bucket.
+
+        You must specify the `version ID <https://docs.aws.amazon.com/AmazonS3/latest/userguide/versioning-workflows.html>`_ that Amazon S3 assigns to the file every time you update the script.
+
+        Version IDs are Unicode, UTF-8 encoded, URL-ready, opaque strings that are no more than 1,024 bytes long. The following is an example:
+
+        ``3sL4kqtJlcpXroDTDmJ+rmSpXd3dIbrHY+MTRCxf3vjVBH40Nr8X8gdRQBpUMLUo``
+
+        For more information, see `Using a startup script <https://docs.aws.amazon.com/mwaa/latest/userguide/using-startup-script.html>`_ .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-startupscripts3objectversion
+        '''
+        result = self._values.get("startup_script_s3_object_version")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def startup_script_s3_path(self) -> typing.Optional[builtins.str]:
+        '''The relative path to the startup shell script in your Amazon S3 bucket. For example, ``s3://mwaa-environment/startup.sh`` .
+
+        Amazon MWAA runs the script as your environment starts, and before running the Apache Airflow process. You can use this script to install dependencies, modify Apache Airflow configuration options, and set environment variables. For more information, see `Using a startup script <https://docs.aws.amazon.com/mwaa/latest/userguide/using-startup-script.html>`_ .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-startupscripts3path
+        '''
+        result = self._values.get("startup_script_s3_path")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def tags(self) -> typing.Any:
+        '''The key-value tag pairs associated to your environment.
+
+        For example, ``"Environment": "Staging"`` . To learn more, see `Tagging <https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html>`_ .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-tags
+        '''
+        result = self._values.get("tags")
+        return typing.cast(typing.Any, result)
+
+    @builtins.property
+    def webserver_access_mode(self) -> typing.Optional[builtins.str]:
+        '''The Apache Airflow *Web server* access mode.
+
+        To learn more, see `Apache Airflow access modes <https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-networking.html>`_ . Valid values: ``PRIVATE_ONLY`` or ``PUBLIC_ONLY`` .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-webserveraccessmode
+        '''
+        result = self._values.get("webserver_access_mode")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def weekly_maintenance_window_start(self) -> typing.Optional[builtins.str]:
+        '''The day and time of the week to start weekly maintenance updates of your environment in the following format: ``DAY:HH:MM`` .
+
+        For example: ``TUE:03:30`` . You can specify a start time in 30 minute increments only. Supported input includes the following:
+
+        - MON|TUE|WED|THU|FRI|SAT|SUN:([01]\\d|2[0-3]):(00|30)
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-mwaa-environment.html#cfn-mwaa-environment-weeklymaintenancewindowstart
+        '''
+        result = self._values.get("weekly_maintenance_window_start")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def additional_policy_statements(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]]:
+        '''Additional policy statements to add to the airflow execution role.'''
+        result = self._values.get("additional_policy_statements")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]], result)
+
+    @builtins.property
+    def dag_files(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''File(s) to be uploaded to dags location in s3 bucket.'''
+        result = self._values.get("dag_files")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
+    def dag_processing_logs(self) -> typing.Optional[builtins.str]:
+        '''Log level for DagProcessing.'''
+        result = self._values.get("dag_processing_logs")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def plugin_file(self) -> typing.Optional[builtins.str]:
+        '''Plugin file to be uploaded to plugin path in S3.
+
+        'pluginsS3Path' must be specified as well.
+        '''
+        result = self._values.get("plugin_file")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def requirements_file(self) -> typing.Optional[builtins.str]:
+        '''Requirements file to be uploaded to plugin path in S3.
+
+        'requirementsS3Path' must be specified as well.
+        '''
+        result = self._values.get("requirements_file")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def s3_bucket(self) -> typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket]:
+        '''S3 Bucket.'''
+        result = self._values.get("s3_bucket")
+        return typing.cast(typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket], result)
+
+    @builtins.property
+    def scheduler_logs_level(self) -> typing.Optional[builtins.str]:
+        '''Log level for SchedulerLogs.'''
+        result = self._values.get("scheduler_logs_level")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def task_logs_level(self) -> typing.Optional[builtins.str]:
+        '''Log level for TaskLogs.'''
+        result = self._values.get("task_logs_level")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def vpc_cidr(self) -> typing.Optional[builtins.str]:
+        '''The IP range (CIDR notation) for this VPC.'''
+        result = self._values.get("vpc_cidr")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def vpc_id(self) -> typing.Optional[builtins.str]:
+        '''Existing vpc id.'''
+        result = self._values.get("vpc_id")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def webserver_logs_level(self) -> typing.Optional[builtins.str]:
+        '''Log level for WebserverLogs.'''
+        result = self._values.get("webserver_logs_level")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def worker_logs_level(self) -> typing.Optional[builtins.str]:
+        '''Log level for WorkerLogs.'''
+        result = self._values.get("worker_logs_level")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "MWAAEnvironmentProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="aws-ddk-core.MWAALambdasResult",
+    jsii_struct_bases=[],
+    name_mapping={"status_lambda": "statusLambda", "trigger_lambda": "triggerLambda"},
+)
+class MWAALambdasResult:
+    def __init__(
+        self,
+        *,
+        status_lambda: _aws_cdk_aws_lambda_ceddda9d.Function,
+        trigger_lambda: _aws_cdk_aws_lambda_ceddda9d.Function,
+    ) -> None:
+        '''
+        :param status_lambda: 
+        :param trigger_lambda: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__3a03e72d8a80ef31dd9345bbdbea98b4abaf3d0a8612fd59523bd5d47407ab0c)
+            check_type(argname="argument status_lambda", value=status_lambda, expected_type=type_hints["status_lambda"])
+            check_type(argname="argument trigger_lambda", value=trigger_lambda, expected_type=type_hints["trigger_lambda"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "status_lambda": status_lambda,
+            "trigger_lambda": trigger_lambda,
+        }
+
+    @builtins.property
+    def status_lambda(self) -> _aws_cdk_aws_lambda_ceddda9d.Function:
+        result = self._values.get("status_lambda")
+        assert result is not None, "Required property 'status_lambda' is missing"
+        return typing.cast(_aws_cdk_aws_lambda_ceddda9d.Function, result)
+
+    @builtins.property
+    def trigger_lambda(self) -> _aws_cdk_aws_lambda_ceddda9d.Function:
+        result = self._values.get("trigger_lambda")
+        assert result is not None, "Required property 'trigger_lambda' is missing"
+        return typing.cast(_aws_cdk_aws_lambda_ceddda9d.Function, result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "MWAALambdasResult(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 @jsii.data_type(
     jsii_type="aws-ddk-core.PermissionsBoundaryProps",
     jsii_struct_bases=[],
     name_mapping={
         "environment_id": "environmentId",
         "prefix": "prefix",
         "qualifier": "qualifier",
@@ -3840,15 +4709,15 @@
         :param id: -
         :param access_control: Specifies a canned ACL that grants predefined permissions to the bucket. Default: BucketAccessControl.PRIVATE
         :param auto_delete_objects: Whether all objects should be automatically deleted when the bucket is removed from the stack or when the stack is deleted. Requires the ``removalPolicy`` to be set to ``RemovalPolicy.DESTROY``. **Warning** if you have deployed a bucket with ``autoDeleteObjects: true``, switching this to ``false`` in a CDK version *before* ``1.126.0`` will lead to all objects in the bucket being deleted. Be sure to update your bucket resources by deploying with CDK version ``1.126.0`` or later **before** switching this value to ``false``. Default: false
         :param block_public_access: The block public access configuration of this bucket. Default: - CloudFormation defaults will apply. New buckets and objects don't allow public access, but users can modify bucket policies or object permissions to allow public access
         :param bucket_key_enabled: Whether Amazon S3 should use its own intermediary key to generate data keys. Only relevant when using KMS for encryption. - If not enabled, every object GET and PUT will cause an API call to KMS (with the attendant cost implications of that). - If enabled, S3 will use its own time-limited key instead. Only relevant, when Encryption is set to ``BucketEncryption.KMS`` or ``BucketEncryption.KMS_MANAGED``. Default: - false
         :param bucket_name: Physical name of this bucket. Default: - Assigned by CloudFormation (recommended).
         :param cors: The CORS configuration of this bucket. Default: - No CORS configuration.
-        :param encryption: The kind of server-side encryption to apply to this bucket. If you choose KMS, you can specify a KMS key via ``encryptionKey``. If encryption key is not specified, a key will automatically be created. Default: - ``Kms`` if ``encryptionKey`` is specified, or ``Unencrypted`` otherwise.
+        :param encryption: The kind of server-side encryption to apply to this bucket. If you choose KMS, you can specify a KMS key via ``encryptionKey``. If encryption key is not specified, a key will automatically be created. Default: - ``Kms`` if ``encryptionKey`` is specified, or ``Managed`` otherwise.
         :param encryption_key: External KMS key to use for bucket encryption. The 'encryption' property must be either not specified or set to "Kms". An error will be emitted if encryption is set to "Unencrypted" or "Managed". Default: - If encryption is set to "Kms" and this property is undefined, a new KMS key will be created and associated with this bucket.
         :param enforce_ssl: Enforces SSL for requests. S3.5 of the AWS Foundational Security Best Practices Regarding S3. Default: false
         :param event_bridge_enabled: Whether this bucket should send notifications to Amazon EventBridge or not. Default: false
         :param intelligent_tiering_configurations: Inteligent Tiering Configurations. Default: No Intelligent Tiiering Configurations.
         :param inventories: The inventory configuration of the bucket. Default: - No inventory configuration
         :param lifecycle_rules: Rules that define how Amazon S3 manages objects during their lifetime. Default: - No lifecycle rules.
         :param metrics: The metrics configuration of this bucket. Default: - No metrics configuration.
@@ -4017,14 +4886,15 @@
         "initial_policy": "initialPolicy",
         "insights_version": "insightsVersion",
         "layers": "layers",
         "log_retention": "logRetention",
         "log_retention_retry_options": "logRetentionRetryOptions",
         "log_retention_role": "logRetentionRole",
         "memory_size": "memorySize",
+        "params_and_secrets": "paramsAndSecrets",
         "profiling": "profiling",
         "profiling_group": "profilingGroup",
         "reserved_concurrent_executions": "reservedConcurrentExecutions",
         "role": "role",
         "runtime_management_mode": "runtimeManagementMode",
         "security_groups": "securityGroups",
         "timeout": "timeout",
@@ -4066,14 +4936,15 @@
         initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
         layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
         log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         memory_size: typing.Optional[jsii.Number] = None,
+        params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
         profiling: typing.Optional[builtins.bool] = None,
         profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
         reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
         role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
         security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
         timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -4112,14 +4983,15 @@
         :param initial_policy: Initial policy statements to add to the created Lambda Role. You can call ``addToRolePolicy`` to the created lambda to add statements post creation. Default: - No policy statements are added to the created Lambda role.
         :param insights_version: Specify the version of CloudWatch Lambda insights to use for monitoring. Default: - No Lambda Insights
         :param layers: A list of layers to add to the function's execution environment. You can configure your Lambda function to pull in additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies that can be used by multiple functions. Default: - No layers.
         :param log_retention: The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.INFINITE
         :param log_retention_retry_options: When log retention is specified, a custom resource attempts to create the CloudWatch log group. These options control the retry policy when interacting with CloudWatch APIs. Default: - Default AWS SDK retry options.
         :param log_retention_role: The IAM role for the Lambda function associated with the custom resource that sets the retention policy. Default: - A new role is created.
         :param memory_size: The amount of memory, in MB, that is allocated to your Lambda function. Lambda uses this value to proportionally allocate the amount of CPU power. For more information, see Resource Model in the AWS Lambda Developer Guide. Default: 128
+        :param params_and_secrets: Specify the configuration of Parameters and Secrets Extension. Default: - No Parameters and Secrets Extension
         :param profiling: Enable profiling. Default: - No profiling.
         :param profiling_group: Profiling Group. Default: - A new profiling group will be created if ``profiling`` is set.
         :param reserved_concurrent_executions: The maximum of concurrent executions you want to reserve for the function. Default: - No specific limit - account limit.
         :param role: Lambda execution role. This is the role that will be assumed by the function upon execution. It controls the permissions that the function will have. The Role must be assumable by the 'lambda.amazonaws.com' service principal. The default Role automatically has permissions granted for Lambda execution. If you provide a Role, you must add the relevant AWS managed policies yourself. The relevant managed policies are "service-role/AWSLambdaBasicExecutionRole" and "service-role/AWSLambdaVPCAccessExecutionRole". Default: - A unique role will be generated for this lambda function. Both supplied and generated roles can always be changed by calling ``addToRolePolicy``.
         :param runtime_management_mode: Sets the runtime management configuration for a function's version. Default: Auto
         :param security_groups: The list of security groups to associate with the Lambda's network interfaces. Only used if 'vpc' is supplied. Default: - If the function is placed within a VPC and a security group is not specified, either by this or securityGroup prop, a dedicated security group will be created for this function.
         :param timeout: The function execution time (in seconds) after which Lambda terminates the function. Because the execution time affects cost, set this value based on the function's expected execution time. Default: Duration.seconds(3)
@@ -4166,14 +5038,15 @@
             check_type(argname="argument initial_policy", value=initial_policy, expected_type=type_hints["initial_policy"])
             check_type(argname="argument insights_version", value=insights_version, expected_type=type_hints["insights_version"])
             check_type(argname="argument layers", value=layers, expected_type=type_hints["layers"])
             check_type(argname="argument log_retention", value=log_retention, expected_type=type_hints["log_retention"])
             check_type(argname="argument log_retention_retry_options", value=log_retention_retry_options, expected_type=type_hints["log_retention_retry_options"])
             check_type(argname="argument log_retention_role", value=log_retention_role, expected_type=type_hints["log_retention_role"])
             check_type(argname="argument memory_size", value=memory_size, expected_type=type_hints["memory_size"])
+            check_type(argname="argument params_and_secrets", value=params_and_secrets, expected_type=type_hints["params_and_secrets"])
             check_type(argname="argument profiling", value=profiling, expected_type=type_hints["profiling"])
             check_type(argname="argument profiling_group", value=profiling_group, expected_type=type_hints["profiling_group"])
             check_type(argname="argument reserved_concurrent_executions", value=reserved_concurrent_executions, expected_type=type_hints["reserved_concurrent_executions"])
             check_type(argname="argument role", value=role, expected_type=type_hints["role"])
             check_type(argname="argument runtime_management_mode", value=runtime_management_mode, expected_type=type_hints["runtime_management_mode"])
             check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
             check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
@@ -4241,14 +5114,16 @@
             self._values["log_retention"] = log_retention
         if log_retention_retry_options is not None:
             self._values["log_retention_retry_options"] = log_retention_retry_options
         if log_retention_role is not None:
             self._values["log_retention_role"] = log_retention_role
         if memory_size is not None:
             self._values["memory_size"] = memory_size
+        if params_and_secrets is not None:
+            self._values["params_and_secrets"] = params_and_secrets
         if profiling is not None:
             self._values["profiling"] = profiling
         if profiling_group is not None:
             self._values["profiling_group"] = profiling_group
         if reserved_concurrent_executions is not None:
             self._values["reserved_concurrent_executions"] = reserved_concurrent_executions
         if role is not None:
@@ -4584,14 +5459,27 @@
 
         :default: 128
         '''
         result = self._values.get("memory_size")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
+    def params_and_secrets(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion]:
+        '''Specify the configuration of Parameters and Secrets Extension.
+
+        :default: - No Parameters and Secrets Extension
+
+        :see: https://docs.aws.amazon.com/systems-manager/latest/userguide/ps-integration-lambda-extensions.html
+        '''
+        result = self._values.get("params_and_secrets")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion], result)
+
+    @builtins.property
     def profiling(self) -> typing.Optional[builtins.bool]:
         '''Enable profiling.
 
         :default: - No profiling.
 
         :see: https://docs.aws.amazon.com/codeguru/latest/profiler-ug/setting-up-lambda.html
         '''
@@ -4955,63 +5843,75 @@
     jsii_type="aws-ddk-core.StateMachineStageProps",
     jsii_struct_bases=[StageProps],
     name_mapping={
         "description": "description",
         "name": "name",
         "additional_role_policy_statements": "additionalRolePolicyStatements",
         "alarms_enabled": "alarmsEnabled",
+        "definition": "definition",
+        "definition_file": "definitionFile",
         "state_machine_failed_executions_alarm_evaluation_periods": "stateMachineFailedExecutionsAlarmEvaluationPeriods",
         "state_machine_failed_executions_alarm_threshold": "stateMachineFailedExecutionsAlarmThreshold",
         "state_machine_input": "stateMachineInput",
         "state_machine_name": "stateMachineName",
     },
 )
 class StateMachineStageProps(StageProps):
     def __init__(
         self,
         *,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
+        definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+        definition_file: typing.Optional[builtins.str] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''Properties of a state machine stage.
 
         :param description: Description of the stage.
         :param name: Name of the stage.
         :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
         :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param definition: Steps for the state machine. Can either be provided as 'sfn.IChainable' or a JSON string.
+        :param definition_file: File containing a JSON definition for the state machine.
         :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
         :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
         :param state_machine_input: Input of the state machine.
         :param state_machine_name: Name of the state machine.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5069a8477e1d868a51858f29afe4a12917625d0a7370bc4090fd23bf809c081c)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument additional_role_policy_statements", value=additional_role_policy_statements, expected_type=type_hints["additional_role_policy_statements"])
             check_type(argname="argument alarms_enabled", value=alarms_enabled, expected_type=type_hints["alarms_enabled"])
+            check_type(argname="argument definition", value=definition, expected_type=type_hints["definition"])
+            check_type(argname="argument definition_file", value=definition_file, expected_type=type_hints["definition_file"])
             check_type(argname="argument state_machine_failed_executions_alarm_evaluation_periods", value=state_machine_failed_executions_alarm_evaluation_periods, expected_type=type_hints["state_machine_failed_executions_alarm_evaluation_periods"])
             check_type(argname="argument state_machine_failed_executions_alarm_threshold", value=state_machine_failed_executions_alarm_threshold, expected_type=type_hints["state_machine_failed_executions_alarm_threshold"])
             check_type(argname="argument state_machine_input", value=state_machine_input, expected_type=type_hints["state_machine_input"])
             check_type(argname="argument state_machine_name", value=state_machine_name, expected_type=type_hints["state_machine_name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if description is not None:
             self._values["description"] = description
         if name is not None:
             self._values["name"] = name
         if additional_role_policy_statements is not None:
             self._values["additional_role_policy_statements"] = additional_role_policy_statements
         if alarms_enabled is not None:
             self._values["alarms_enabled"] = alarms_enabled
+        if definition is not None:
+            self._values["definition"] = definition
+        if definition_file is not None:
+            self._values["definition_file"] = definition_file
         if state_machine_failed_executions_alarm_evaluation_periods is not None:
             self._values["state_machine_failed_executions_alarm_evaluation_periods"] = state_machine_failed_executions_alarm_evaluation_periods
         if state_machine_failed_executions_alarm_threshold is not None:
             self._values["state_machine_failed_executions_alarm_threshold"] = state_machine_failed_executions_alarm_threshold
         if state_machine_input is not None:
             self._values["state_machine_input"] = state_machine_input
         if state_machine_name is not None:
@@ -5043,14 +5943,31 @@
 
         :default: true
         '''
         result = self._values.get("alarms_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
+    def definition(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]]:
+        '''Steps for the state machine.
+
+        Can either be provided as 'sfn.IChainable' or a JSON string.
+        '''
+        result = self._values.get("definition")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]], result)
+
+    @builtins.property
+    def definition_file(self) -> typing.Optional[builtins.str]:
+        '''File containing a JSON definition for the state machine.'''
+        result = self._values.get("definition_file")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def state_machine_failed_executions_alarm_evaluation_periods(
         self,
     ) -> typing.Optional[jsii.Number]:
         '''The number of periods over which data is compared to the specified threshold.
 
         :default: 1
         '''
@@ -5099,60 +6016,66 @@
     jsii_struct_bases=[],
     name_mapping={
         "additional_install_commands": "additionalInstallCommands",
         "cdk_version": "cdkVersion",
         "codeartifact_domain": "codeartifactDomain",
         "codeartifact_domain_owner": "codeartifactDomainOwner",
         "codeartifact_repository": "codeartifactRepository",
+        "env": "env",
         "role_policy_statements": "rolePolicyStatements",
         "synth_action": "synthAction",
     },
 )
 class SynthActionProps:
     def __init__(
         self,
         *,
         additional_install_commands: typing.Optional[typing.Sequence[builtins.str]] = None,
         cdk_version: typing.Optional[builtins.str] = None,
         codeartifact_domain: typing.Optional[builtins.str] = None,
         codeartifact_domain_owner: typing.Optional[builtins.str] = None,
         codeartifact_repository: typing.Optional[builtins.str] = None,
+        env: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         synth_action: typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildStep] = None,
     ) -> None:
         '''Properties for the synth action.
 
         :param additional_install_commands: Additional install commands.
         :param cdk_version: CDK versio to use during the synth action. Default: "latest"
         :param codeartifact_domain: Name of the CodeArtifact domain.
         :param codeartifact_domain_owner: CodeArtifact domain owner account.
         :param codeartifact_repository: Name of the CodeArtifact repository to pull artifacts from.
+        :param env: Environment variables to set.
         :param role_policy_statements: Additional policies to add to the synth action role.
         :param synth_action: Override synth action.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__05acfa3cda54a17101814d614a246f97dc36de4bf27ef87f72f7aa4824dd7b35)
             check_type(argname="argument additional_install_commands", value=additional_install_commands, expected_type=type_hints["additional_install_commands"])
             check_type(argname="argument cdk_version", value=cdk_version, expected_type=type_hints["cdk_version"])
             check_type(argname="argument codeartifact_domain", value=codeartifact_domain, expected_type=type_hints["codeartifact_domain"])
             check_type(argname="argument codeartifact_domain_owner", value=codeartifact_domain_owner, expected_type=type_hints["codeartifact_domain_owner"])
             check_type(argname="argument codeartifact_repository", value=codeartifact_repository, expected_type=type_hints["codeartifact_repository"])
+            check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument role_policy_statements", value=role_policy_statements, expected_type=type_hints["role_policy_statements"])
             check_type(argname="argument synth_action", value=synth_action, expected_type=type_hints["synth_action"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if additional_install_commands is not None:
             self._values["additional_install_commands"] = additional_install_commands
         if cdk_version is not None:
             self._values["cdk_version"] = cdk_version
         if codeartifact_domain is not None:
             self._values["codeartifact_domain"] = codeartifact_domain
         if codeartifact_domain_owner is not None:
             self._values["codeartifact_domain_owner"] = codeartifact_domain_owner
         if codeartifact_repository is not None:
             self._values["codeartifact_repository"] = codeartifact_repository
+        if env is not None:
+            self._values["env"] = env
         if role_policy_statements is not None:
             self._values["role_policy_statements"] = role_policy_statements
         if synth_action is not None:
             self._values["synth_action"] = synth_action
 
     @builtins.property
     def additional_install_commands(self) -> typing.Optional[typing.List[builtins.str]]:
@@ -5184,14 +6107,20 @@
     @builtins.property
     def codeartifact_repository(self) -> typing.Optional[builtins.str]:
         '''Name of the CodeArtifact repository to pull artifacts from.'''
         result = self._values.get("codeartifact_repository")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def env(self) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
+        '''Environment variables to set.'''
+        result = self._values.get("env")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
+
+    @builtins.property
     def role_policy_statements(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]]:
         '''Additional policies to add to the synth action role.'''
         result = self._values.get("role_policy_statements")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]], result)
 
@@ -5219,14 +6148,16 @@
     jsii_type="aws-ddk-core.AppFlowIngestionStageProps",
     jsii_struct_bases=[StateMachineStageProps],
     name_mapping={
         "description": "description",
         "name": "name",
         "additional_role_policy_statements": "additionalRolePolicyStatements",
         "alarms_enabled": "alarmsEnabled",
+        "definition": "definition",
+        "definition_file": "definitionFile",
         "state_machine_failed_executions_alarm_evaluation_periods": "stateMachineFailedExecutionsAlarmEvaluationPeriods",
         "state_machine_failed_executions_alarm_threshold": "stateMachineFailedExecutionsAlarmThreshold",
         "state_machine_input": "stateMachineInput",
         "state_machine_name": "stateMachineName",
         "destination_flow_config": "destinationFlowConfig",
         "flow_execution_status_check_period": "flowExecutionStatusCheckPeriod",
         "flow_name": "flowName",
@@ -5238,14 +6169,16 @@
     def __init__(
         self,
         *,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
+        definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+        definition_file: typing.Optional[builtins.str] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         destination_flow_config: typing.Optional[typing.Union[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.DestinationFlowConfigProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         flow_execution_status_check_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         flow_name: typing.Optional[builtins.str] = None,
@@ -5254,14 +6187,16 @@
     ) -> None:
         '''Properties of the AppFlow Ingestion stage.
 
         :param description: Description of the stage.
         :param name: Name of the stage.
         :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
         :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param definition: Steps for the state machine. Can either be provided as 'sfn.IChainable' or a JSON string.
+        :param definition_file: File containing a JSON definition for the state machine.
         :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
         :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
         :param state_machine_input: Input of the state machine.
         :param state_machine_name: Name of the state machine.
         :param destination_flow_config: The flow ``appflow.CfnFlow.DestinationFlowConfigProperty`` properties.
         :param flow_execution_status_check_period: Time to wait between flow execution status checks. Default: aws_cdk.Duration.seconds(15)
         :param flow_name: Name of the AppFlow flow to run. If None, an AppFlow flow is created.
@@ -5274,14 +6209,16 @@
             source_flow_config = _aws_cdk_aws_appflow_ceddda9d.CfnFlow.SourceFlowConfigProperty(**source_flow_config)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__50f57d5c758f4bb8a7385b25c9dd1756786a7af562ac0cf743837ff675065839)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument additional_role_policy_statements", value=additional_role_policy_statements, expected_type=type_hints["additional_role_policy_statements"])
             check_type(argname="argument alarms_enabled", value=alarms_enabled, expected_type=type_hints["alarms_enabled"])
+            check_type(argname="argument definition", value=definition, expected_type=type_hints["definition"])
+            check_type(argname="argument definition_file", value=definition_file, expected_type=type_hints["definition_file"])
             check_type(argname="argument state_machine_failed_executions_alarm_evaluation_periods", value=state_machine_failed_executions_alarm_evaluation_periods, expected_type=type_hints["state_machine_failed_executions_alarm_evaluation_periods"])
             check_type(argname="argument state_machine_failed_executions_alarm_threshold", value=state_machine_failed_executions_alarm_threshold, expected_type=type_hints["state_machine_failed_executions_alarm_threshold"])
             check_type(argname="argument state_machine_input", value=state_machine_input, expected_type=type_hints["state_machine_input"])
             check_type(argname="argument state_machine_name", value=state_machine_name, expected_type=type_hints["state_machine_name"])
             check_type(argname="argument destination_flow_config", value=destination_flow_config, expected_type=type_hints["destination_flow_config"])
             check_type(argname="argument flow_execution_status_check_period", value=flow_execution_status_check_period, expected_type=type_hints["flow_execution_status_check_period"])
             check_type(argname="argument flow_name", value=flow_name, expected_type=type_hints["flow_name"])
@@ -5292,14 +6229,18 @@
             self._values["description"] = description
         if name is not None:
             self._values["name"] = name
         if additional_role_policy_statements is not None:
             self._values["additional_role_policy_statements"] = additional_role_policy_statements
         if alarms_enabled is not None:
             self._values["alarms_enabled"] = alarms_enabled
+        if definition is not None:
+            self._values["definition"] = definition
+        if definition_file is not None:
+            self._values["definition_file"] = definition_file
         if state_machine_failed_executions_alarm_evaluation_periods is not None:
             self._values["state_machine_failed_executions_alarm_evaluation_periods"] = state_machine_failed_executions_alarm_evaluation_periods
         if state_machine_failed_executions_alarm_threshold is not None:
             self._values["state_machine_failed_executions_alarm_threshold"] = state_machine_failed_executions_alarm_threshold
         if state_machine_input is not None:
             self._values["state_machine_input"] = state_machine_input
         if state_machine_name is not None:
@@ -5341,14 +6282,31 @@
 
         :default: true
         '''
         result = self._values.get("alarms_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
+    def definition(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]]:
+        '''Steps for the state machine.
+
+        Can either be provided as 'sfn.IChainable' or a JSON string.
+        '''
+        result = self._values.get("definition")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]], result)
+
+    @builtins.property
+    def definition_file(self) -> typing.Optional[builtins.str]:
+        '''File containing a JSON definition for the state machine.'''
+        result = self._values.get("definition_file")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def state_machine_failed_executions_alarm_evaluation_periods(
         self,
     ) -> typing.Optional[jsii.Number]:
         '''The number of periods over which data is compared to the specified threshold.
 
         :default: 1
         '''
@@ -5440,14 +6398,16 @@
     jsii_type="aws-ddk-core.AthenaToSQLStageProps",
     jsii_struct_bases=[StateMachineStageProps],
     name_mapping={
         "description": "description",
         "name": "name",
         "additional_role_policy_statements": "additionalRolePolicyStatements",
         "alarms_enabled": "alarmsEnabled",
+        "definition": "definition",
+        "definition_file": "definitionFile",
         "state_machine_failed_executions_alarm_evaluation_periods": "stateMachineFailedExecutionsAlarmEvaluationPeriods",
         "state_machine_failed_executions_alarm_threshold": "stateMachineFailedExecutionsAlarmThreshold",
         "state_machine_input": "stateMachineInput",
         "state_machine_name": "stateMachineName",
         "catalog_name": "catalogName",
         "database_name": "databaseName",
         "encryption_key": "encryptionKey",
@@ -5463,14 +6423,16 @@
     def __init__(
         self,
         *,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
+        definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+        definition_file: typing.Optional[builtins.str] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         catalog_name: typing.Optional[builtins.str] = None,
         database_name: typing.Optional[builtins.str] = None,
         encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.Key] = None,
@@ -5483,14 +6445,16 @@
     ) -> None:
         '''Properties for ``AthenaSQLStage``.
 
         :param description: Description of the stage.
         :param name: Name of the stage.
         :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
         :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param definition: Steps for the state machine. Can either be provided as 'sfn.IChainable' or a JSON string.
+        :param definition_file: File containing a JSON definition for the state machine.
         :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
         :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
         :param state_machine_input: Input of the state machine.
         :param state_machine_name: Name of the state machine.
         :param catalog_name: Catalog name.
         :param database_name: Database name.
         :param encryption_key: Encryption KMS key.
@@ -5505,14 +6469,16 @@
             output_location = _aws_cdk_aws_s3_ceddda9d.Location(**output_location)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d02b2a3868910a4789cbcba2028e07a331d2da507e4b4c951dd7801d735bc0ac)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument additional_role_policy_statements", value=additional_role_policy_statements, expected_type=type_hints["additional_role_policy_statements"])
             check_type(argname="argument alarms_enabled", value=alarms_enabled, expected_type=type_hints["alarms_enabled"])
+            check_type(argname="argument definition", value=definition, expected_type=type_hints["definition"])
+            check_type(argname="argument definition_file", value=definition_file, expected_type=type_hints["definition_file"])
             check_type(argname="argument state_machine_failed_executions_alarm_evaluation_periods", value=state_machine_failed_executions_alarm_evaluation_periods, expected_type=type_hints["state_machine_failed_executions_alarm_evaluation_periods"])
             check_type(argname="argument state_machine_failed_executions_alarm_threshold", value=state_machine_failed_executions_alarm_threshold, expected_type=type_hints["state_machine_failed_executions_alarm_threshold"])
             check_type(argname="argument state_machine_input", value=state_machine_input, expected_type=type_hints["state_machine_input"])
             check_type(argname="argument state_machine_name", value=state_machine_name, expected_type=type_hints["state_machine_name"])
             check_type(argname="argument catalog_name", value=catalog_name, expected_type=type_hints["catalog_name"])
             check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
             check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
@@ -5527,14 +6493,18 @@
             self._values["description"] = description
         if name is not None:
             self._values["name"] = name
         if additional_role_policy_statements is not None:
             self._values["additional_role_policy_statements"] = additional_role_policy_statements
         if alarms_enabled is not None:
             self._values["alarms_enabled"] = alarms_enabled
+        if definition is not None:
+            self._values["definition"] = definition
+        if definition_file is not None:
+            self._values["definition_file"] = definition_file
         if state_machine_failed_executions_alarm_evaluation_periods is not None:
             self._values["state_machine_failed_executions_alarm_evaluation_periods"] = state_machine_failed_executions_alarm_evaluation_periods
         if state_machine_failed_executions_alarm_threshold is not None:
             self._values["state_machine_failed_executions_alarm_threshold"] = state_machine_failed_executions_alarm_threshold
         if state_machine_input is not None:
             self._values["state_machine_input"] = state_machine_input
         if state_machine_name is not None:
@@ -5584,14 +6554,31 @@
 
         :default: true
         '''
         result = self._values.get("alarms_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
+    def definition(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]]:
+        '''Steps for the state machine.
+
+        Can either be provided as 'sfn.IChainable' or a JSON string.
+        '''
+        result = self._values.get("definition")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]], result)
+
+    @builtins.property
+    def definition_file(self) -> typing.Optional[builtins.str]:
+        '''File containing a JSON definition for the state machine.'''
+        result = self._values.get("definition_file")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def state_machine_failed_executions_alarm_evaluation_periods(
         self,
     ) -> typing.Optional[jsii.Number]:
         '''The number of periods over which data is compared to the specified threshold.
 
         :default: 1
         '''
@@ -5698,14 +6685,16 @@
     jsii_type="aws-ddk-core.DataBrewTransformStageProps",
     jsii_struct_bases=[StateMachineStageProps],
     name_mapping={
         "description": "description",
         "name": "name",
         "additional_role_policy_statements": "additionalRolePolicyStatements",
         "alarms_enabled": "alarmsEnabled",
+        "definition": "definition",
+        "definition_file": "definitionFile",
         "state_machine_failed_executions_alarm_evaluation_periods": "stateMachineFailedExecutionsAlarmEvaluationPeriods",
         "state_machine_failed_executions_alarm_threshold": "stateMachineFailedExecutionsAlarmThreshold",
         "state_machine_input": "stateMachineInput",
         "state_machine_name": "stateMachineName",
         "create_job": "createJob",
         "database_outputs": "databaseOutputs",
         "data_catalog_outputs": "dataCatalogOutputs",
@@ -5733,14 +6722,16 @@
     def __init__(
         self,
         *,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
+        definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+        definition_file: typing.Optional[builtins.str] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         create_job: typing.Optional[builtins.bool] = None,
         database_outputs: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DatabaseOutputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
         data_catalog_outputs: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DataCatalogOutputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
@@ -5765,14 +6756,16 @@
     ) -> None:
         '''Properties for ``DataBrewTransformStage``.
 
         :param description: Description of the stage.
         :param name: Name of the stage.
         :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
         :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param definition: Steps for the state machine. Can either be provided as 'sfn.IChainable' or a JSON string.
+        :param definition_file: File containing a JSON definition for the state machine.
         :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
         :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
         :param state_machine_input: Input of the state machine.
         :param state_machine_name: Name of the state machine.
         :param create_job: Whether to create the DataBrew job or not.
         :param database_outputs: Represents a list of JDBC database output objects which defines the output destination for a DataBrew recipe job to write into.
         :param data_catalog_outputs: One or more artifacts that represent the AWS Glue Data Catalog output from running the job.
@@ -5805,14 +6798,16 @@
             recipe = _aws_cdk_aws_databrew_ceddda9d.CfnJob.RecipeProperty(**recipe)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f6be6b9ec4e805f427307a7bc1c743a3f56ffd52c0cc37a1436d75ce69e31b9f)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument additional_role_policy_statements", value=additional_role_policy_statements, expected_type=type_hints["additional_role_policy_statements"])
             check_type(argname="argument alarms_enabled", value=alarms_enabled, expected_type=type_hints["alarms_enabled"])
+            check_type(argname="argument definition", value=definition, expected_type=type_hints["definition"])
+            check_type(argname="argument definition_file", value=definition_file, expected_type=type_hints["definition_file"])
             check_type(argname="argument state_machine_failed_executions_alarm_evaluation_periods", value=state_machine_failed_executions_alarm_evaluation_periods, expected_type=type_hints["state_machine_failed_executions_alarm_evaluation_periods"])
             check_type(argname="argument state_machine_failed_executions_alarm_threshold", value=state_machine_failed_executions_alarm_threshold, expected_type=type_hints["state_machine_failed_executions_alarm_threshold"])
             check_type(argname="argument state_machine_input", value=state_machine_input, expected_type=type_hints["state_machine_input"])
             check_type(argname="argument state_machine_name", value=state_machine_name, expected_type=type_hints["state_machine_name"])
             check_type(argname="argument create_job", value=create_job, expected_type=type_hints["create_job"])
             check_type(argname="argument database_outputs", value=database_outputs, expected_type=type_hints["database_outputs"])
             check_type(argname="argument data_catalog_outputs", value=data_catalog_outputs, expected_type=type_hints["data_catalog_outputs"])
@@ -5839,14 +6834,18 @@
             self._values["description"] = description
         if name is not None:
             self._values["name"] = name
         if additional_role_policy_statements is not None:
             self._values["additional_role_policy_statements"] = additional_role_policy_statements
         if alarms_enabled is not None:
             self._values["alarms_enabled"] = alarms_enabled
+        if definition is not None:
+            self._values["definition"] = definition
+        if definition_file is not None:
+            self._values["definition_file"] = definition_file
         if state_machine_failed_executions_alarm_evaluation_periods is not None:
             self._values["state_machine_failed_executions_alarm_evaluation_periods"] = state_machine_failed_executions_alarm_evaluation_periods
         if state_machine_failed_executions_alarm_threshold is not None:
             self._values["state_machine_failed_executions_alarm_threshold"] = state_machine_failed_executions_alarm_threshold
         if state_machine_input is not None:
             self._values["state_machine_input"] = state_machine_input
         if state_machine_name is not None:
@@ -5920,14 +6919,31 @@
 
         :default: true
         '''
         result = self._values.get("alarms_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
+    def definition(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]]:
+        '''Steps for the state machine.
+
+        Can either be provided as 'sfn.IChainable' or a JSON string.
+        '''
+        result = self._values.get("definition")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]], result)
+
+    @builtins.property
+    def definition_file(self) -> typing.Optional[builtins.str]:
+        '''File containing a JSON definition for the state machine.'''
+        result = self._values.get("definition_file")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def state_machine_failed_executions_alarm_evaluation_periods(
         self,
     ) -> typing.Optional[jsii.Number]:
         '''The number of periods over which data is compared to the specified threshold.
 
         :default: 1
         '''
@@ -6824,14 +7840,16 @@
     jsii_type="aws-ddk-core.GlueTransformStageProps",
     jsii_struct_bases=[StateMachineStageProps],
     name_mapping={
         "description": "description",
         "name": "name",
         "additional_role_policy_statements": "additionalRolePolicyStatements",
         "alarms_enabled": "alarmsEnabled",
+        "definition": "definition",
+        "definition_file": "definitionFile",
         "state_machine_failed_executions_alarm_evaluation_periods": "stateMachineFailedExecutionsAlarmEvaluationPeriods",
         "state_machine_failed_executions_alarm_threshold": "stateMachineFailedExecutionsAlarmThreshold",
         "state_machine_input": "stateMachineInput",
         "state_machine_name": "stateMachineName",
         "crawler_allow_failure": "crawlerAllowFailure",
         "crawler_name": "crawlerName",
         "crawler_props": "crawlerProps",
@@ -6850,14 +7868,16 @@
     def __init__(
         self,
         *,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
+        definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+        definition_file: typing.Optional[builtins.str] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         crawler_allow_failure: typing.Optional[builtins.bool] = None,
         crawler_name: typing.Optional[builtins.str] = None,
         crawler_props: typing.Optional[typing.Union[_aws_cdk_aws_glue_ceddda9d.CfnCrawlerProps, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -6873,14 +7893,16 @@
     ) -> None:
         '''Properties for ``GlueTransformStage``.
 
         :param description: Description of the stage.
         :param name: Name of the stage.
         :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
         :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param definition: Steps for the state machine. Can either be provided as 'sfn.IChainable' or a JSON string.
+        :param definition_file: File containing a JSON definition for the state machine.
         :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
         :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
         :param state_machine_input: Input of the state machine.
         :param state_machine_name: Name of the state machine.
         :param crawler_allow_failure: Argument to allow stepfunction success for crawler failures/execption like Glue.CrawlerRunningException. Default: true
         :param crawler_name: The name of a preexisting Glue crawler to run. If None, a Glue crawler is created.
         :param crawler_props: Properties for the Glue Crawler.
@@ -6902,14 +7924,16 @@
             targets = _aws_cdk_aws_glue_ceddda9d.CfnCrawler.TargetsProperty(**targets)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__36c864b97313236b09b597808a1574a4f4d21024bac872f4e182edbd9a3d0175)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument additional_role_policy_statements", value=additional_role_policy_statements, expected_type=type_hints["additional_role_policy_statements"])
             check_type(argname="argument alarms_enabled", value=alarms_enabled, expected_type=type_hints["alarms_enabled"])
+            check_type(argname="argument definition", value=definition, expected_type=type_hints["definition"])
+            check_type(argname="argument definition_file", value=definition_file, expected_type=type_hints["definition_file"])
             check_type(argname="argument state_machine_failed_executions_alarm_evaluation_periods", value=state_machine_failed_executions_alarm_evaluation_periods, expected_type=type_hints["state_machine_failed_executions_alarm_evaluation_periods"])
             check_type(argname="argument state_machine_failed_executions_alarm_threshold", value=state_machine_failed_executions_alarm_threshold, expected_type=type_hints["state_machine_failed_executions_alarm_threshold"])
             check_type(argname="argument state_machine_input", value=state_machine_input, expected_type=type_hints["state_machine_input"])
             check_type(argname="argument state_machine_name", value=state_machine_name, expected_type=type_hints["state_machine_name"])
             check_type(argname="argument crawler_allow_failure", value=crawler_allow_failure, expected_type=type_hints["crawler_allow_failure"])
             check_type(argname="argument crawler_name", value=crawler_name, expected_type=type_hints["crawler_name"])
             check_type(argname="argument crawler_props", value=crawler_props, expected_type=type_hints["crawler_props"])
@@ -6927,14 +7951,18 @@
             self._values["description"] = description
         if name is not None:
             self._values["name"] = name
         if additional_role_policy_statements is not None:
             self._values["additional_role_policy_statements"] = additional_role_policy_statements
         if alarms_enabled is not None:
             self._values["alarms_enabled"] = alarms_enabled
+        if definition is not None:
+            self._values["definition"] = definition
+        if definition_file is not None:
+            self._values["definition_file"] = definition_file
         if state_machine_failed_executions_alarm_evaluation_periods is not None:
             self._values["state_machine_failed_executions_alarm_evaluation_periods"] = state_machine_failed_executions_alarm_evaluation_periods
         if state_machine_failed_executions_alarm_threshold is not None:
             self._values["state_machine_failed_executions_alarm_threshold"] = state_machine_failed_executions_alarm_threshold
         if state_machine_input is not None:
             self._values["state_machine_input"] = state_machine_input
         if state_machine_name is not None:
@@ -6990,14 +8018,31 @@
 
         :default: true
         '''
         result = self._values.get("alarms_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
+    def definition(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]]:
+        '''Steps for the state machine.
+
+        Can either be provided as 'sfn.IChainable' or a JSON string.
+        '''
+        result = self._values.get("definition")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]], result)
+
+    @builtins.property
+    def definition_file(self) -> typing.Optional[builtins.str]:
+        '''File containing a JSON definition for the state machine.'''
+        result = self._values.get("definition_file")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def state_machine_failed_executions_alarm_evaluation_periods(
         self,
     ) -> typing.Optional[jsii.Number]:
         '''The number of periods over which data is compared to the specified threshold.
 
         :default: 1
         '''
@@ -7143,21 +8188,247 @@
     def __repr__(self) -> str:
         return "GlueTransformStageProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
+    jsii_type="aws-ddk-core.MWAATriggerDagsStageProps",
+    jsii_struct_bases=[StateMachineStageProps],
+    name_mapping={
+        "description": "description",
+        "name": "name",
+        "additional_role_policy_statements": "additionalRolePolicyStatements",
+        "alarms_enabled": "alarmsEnabled",
+        "definition": "definition",
+        "definition_file": "definitionFile",
+        "state_machine_failed_executions_alarm_evaluation_periods": "stateMachineFailedExecutionsAlarmEvaluationPeriods",
+        "state_machine_failed_executions_alarm_threshold": "stateMachineFailedExecutionsAlarmThreshold",
+        "state_machine_input": "stateMachineInput",
+        "state_machine_name": "stateMachineName",
+        "mwaa_environment_name": "mwaaEnvironmentName",
+        "dag_path": "dagPath",
+        "dags": "dags",
+        "status_check_period": "statusCheckPeriod",
+    },
+)
+class MWAATriggerDagsStageProps(StateMachineStageProps):
+    def __init__(
+        self,
+        *,
+        description: typing.Optional[builtins.str] = None,
+        name: typing.Optional[builtins.str] = None,
+        additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+        alarms_enabled: typing.Optional[builtins.bool] = None,
+        definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+        definition_file: typing.Optional[builtins.str] = None,
+        state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
+        state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
+        state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+        state_machine_name: typing.Optional[builtins.str] = None,
+        mwaa_environment_name: builtins.str,
+        dag_path: typing.Optional[builtins.str] = None,
+        dags: typing.Optional[typing.Sequence[builtins.str]] = None,
+        status_check_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+    ) -> None:
+        '''Properties of the MWAA Trigger Dags stage.
+
+        :param description: Description of the stage.
+        :param name: Name of the stage.
+        :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
+        :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param definition: Steps for the state machine. Can either be provided as 'sfn.IChainable' or a JSON string.
+        :param definition_file: File containing a JSON definition for the state machine.
+        :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
+        :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
+        :param state_machine_input: Input of the state machine.
+        :param state_machine_name: Name of the state machine.
+        :param mwaa_environment_name: Name of airflow environment.
+        :param dag_path: Path to array of dag id's to check.
+        :param dags: Name of dag(s) to trigger.
+        :param status_check_period: Time to wait between execution status checks. Default: aws_cdk.Duration.seconds(15)
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__22752f7fca368ed1e29dd71501fbd74daab00450e10e80bb5c02b1233ef9c8f5)
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument additional_role_policy_statements", value=additional_role_policy_statements, expected_type=type_hints["additional_role_policy_statements"])
+            check_type(argname="argument alarms_enabled", value=alarms_enabled, expected_type=type_hints["alarms_enabled"])
+            check_type(argname="argument definition", value=definition, expected_type=type_hints["definition"])
+            check_type(argname="argument definition_file", value=definition_file, expected_type=type_hints["definition_file"])
+            check_type(argname="argument state_machine_failed_executions_alarm_evaluation_periods", value=state_machine_failed_executions_alarm_evaluation_periods, expected_type=type_hints["state_machine_failed_executions_alarm_evaluation_periods"])
+            check_type(argname="argument state_machine_failed_executions_alarm_threshold", value=state_machine_failed_executions_alarm_threshold, expected_type=type_hints["state_machine_failed_executions_alarm_threshold"])
+            check_type(argname="argument state_machine_input", value=state_machine_input, expected_type=type_hints["state_machine_input"])
+            check_type(argname="argument state_machine_name", value=state_machine_name, expected_type=type_hints["state_machine_name"])
+            check_type(argname="argument mwaa_environment_name", value=mwaa_environment_name, expected_type=type_hints["mwaa_environment_name"])
+            check_type(argname="argument dag_path", value=dag_path, expected_type=type_hints["dag_path"])
+            check_type(argname="argument dags", value=dags, expected_type=type_hints["dags"])
+            check_type(argname="argument status_check_period", value=status_check_period, expected_type=type_hints["status_check_period"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "mwaa_environment_name": mwaa_environment_name,
+        }
+        if description is not None:
+            self._values["description"] = description
+        if name is not None:
+            self._values["name"] = name
+        if additional_role_policy_statements is not None:
+            self._values["additional_role_policy_statements"] = additional_role_policy_statements
+        if alarms_enabled is not None:
+            self._values["alarms_enabled"] = alarms_enabled
+        if definition is not None:
+            self._values["definition"] = definition
+        if definition_file is not None:
+            self._values["definition_file"] = definition_file
+        if state_machine_failed_executions_alarm_evaluation_periods is not None:
+            self._values["state_machine_failed_executions_alarm_evaluation_periods"] = state_machine_failed_executions_alarm_evaluation_periods
+        if state_machine_failed_executions_alarm_threshold is not None:
+            self._values["state_machine_failed_executions_alarm_threshold"] = state_machine_failed_executions_alarm_threshold
+        if state_machine_input is not None:
+            self._values["state_machine_input"] = state_machine_input
+        if state_machine_name is not None:
+            self._values["state_machine_name"] = state_machine_name
+        if dag_path is not None:
+            self._values["dag_path"] = dag_path
+        if dags is not None:
+            self._values["dags"] = dags
+        if status_check_period is not None:
+            self._values["status_check_period"] = status_check_period
+
+    @builtins.property
+    def description(self) -> typing.Optional[builtins.str]:
+        '''Description of the stage.'''
+        result = self._values.get("description")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
+        result = self._values.get("name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def additional_role_policy_statements(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]]:
+        '''Additional IAM policy statements to add to the state machine role.'''
+        result = self._values.get("additional_role_policy_statements")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]], result)
+
+    @builtins.property
+    def alarms_enabled(self) -> typing.Optional[builtins.bool]:
+        '''Enable/Disable all alarms in the stage.
+
+        :default: true
+        '''
+        result = self._values.get("alarms_enabled")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def definition(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]]:
+        '''Steps for the state machine.
+
+        Can either be provided as 'sfn.IChainable' or a JSON string.
+        '''
+        result = self._values.get("definition")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]], result)
+
+    @builtins.property
+    def definition_file(self) -> typing.Optional[builtins.str]:
+        '''File containing a JSON definition for the state machine.'''
+        result = self._values.get("definition_file")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def state_machine_failed_executions_alarm_evaluation_periods(
+        self,
+    ) -> typing.Optional[jsii.Number]:
+        '''The number of periods over which data is compared to the specified threshold.
+
+        :default: 1
+        '''
+        result = self._values.get("state_machine_failed_executions_alarm_evaluation_periods")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def state_machine_failed_executions_alarm_threshold(
+        self,
+    ) -> typing.Optional[jsii.Number]:
+        '''The number of failed state machine executions before triggering CW alarm.
+
+        :default: 1
+        '''
+        result = self._values.get("state_machine_failed_executions_alarm_threshold")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def state_machine_input(
+        self,
+    ) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
+        '''Input of the state machine.'''
+        result = self._values.get("state_machine_input")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
+
+    @builtins.property
+    def state_machine_name(self) -> typing.Optional[builtins.str]:
+        '''Name of the state machine.'''
+        result = self._values.get("state_machine_name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def mwaa_environment_name(self) -> builtins.str:
+        '''Name of airflow environment.'''
+        result = self._values.get("mwaa_environment_name")
+        assert result is not None, "Required property 'mwaa_environment_name' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def dag_path(self) -> typing.Optional[builtins.str]:
+        '''Path to array of dag id's to check.'''
+        result = self._values.get("dag_path")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def dags(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''Name of dag(s) to trigger.'''
+        result = self._values.get("dags")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
+    def status_check_period(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+        '''Time to wait between execution status checks.
+
+        :default: aws_cdk.Duration.seconds(15)
+        '''
+        result = self._values.get("status_check_period")
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "MWAATriggerDagsStageProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
     jsii_type="aws-ddk-core.RedshiftDataApiStageProps",
     jsii_struct_bases=[StateMachineStageProps],
     name_mapping={
         "description": "description",
         "name": "name",
         "additional_role_policy_statements": "additionalRolePolicyStatements",
         "alarms_enabled": "alarmsEnabled",
+        "definition": "definition",
+        "definition_file": "definitionFile",
         "state_machine_failed_executions_alarm_evaluation_periods": "stateMachineFailedExecutionsAlarmEvaluationPeriods",
         "state_machine_failed_executions_alarm_threshold": "stateMachineFailedExecutionsAlarmThreshold",
         "state_machine_input": "stateMachineInput",
         "state_machine_name": "stateMachineName",
         "redshift_cluster_identifier": "redshiftClusterIdentifier",
         "sql_statements": "sqlStatements",
         "database_name": "databaseName",
@@ -7169,14 +8440,16 @@
     def __init__(
         self,
         *,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
+        definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+        definition_file: typing.Optional[builtins.str] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         redshift_cluster_identifier: builtins.str,
         sql_statements: typing.Sequence[builtins.str],
         database_name: typing.Optional[builtins.str] = None,
@@ -7185,14 +8458,16 @@
     ) -> None:
         '''Properties for ``RedshiftDataApiStage``.
 
         :param description: Description of the stage.
         :param name: Name of the stage.
         :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
         :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param definition: Steps for the state machine. Can either be provided as 'sfn.IChainable' or a JSON string.
+        :param definition_file: File containing a JSON definition for the state machine.
         :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
         :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
         :param state_machine_input: Input of the state machine.
         :param state_machine_name: Name of the state machine.
         :param redshift_cluster_identifier: Identifier of the Redshift cluster.
         :param sql_statements: List of SQL statements to execute.
         :param database_name: Name of the database in Redshift. Default: "dev"
@@ -7201,14 +8476,16 @@
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__defbc9333f2b8b3e2d55373f9b0155e5f6e83609e9153dc24f619d747ca4f133)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument additional_role_policy_statements", value=additional_role_policy_statements, expected_type=type_hints["additional_role_policy_statements"])
             check_type(argname="argument alarms_enabled", value=alarms_enabled, expected_type=type_hints["alarms_enabled"])
+            check_type(argname="argument definition", value=definition, expected_type=type_hints["definition"])
+            check_type(argname="argument definition_file", value=definition_file, expected_type=type_hints["definition_file"])
             check_type(argname="argument state_machine_failed_executions_alarm_evaluation_periods", value=state_machine_failed_executions_alarm_evaluation_periods, expected_type=type_hints["state_machine_failed_executions_alarm_evaluation_periods"])
             check_type(argname="argument state_machine_failed_executions_alarm_threshold", value=state_machine_failed_executions_alarm_threshold, expected_type=type_hints["state_machine_failed_executions_alarm_threshold"])
             check_type(argname="argument state_machine_input", value=state_machine_input, expected_type=type_hints["state_machine_input"])
             check_type(argname="argument state_machine_name", value=state_machine_name, expected_type=type_hints["state_machine_name"])
             check_type(argname="argument redshift_cluster_identifier", value=redshift_cluster_identifier, expected_type=type_hints["redshift_cluster_identifier"])
             check_type(argname="argument sql_statements", value=sql_statements, expected_type=type_hints["sql_statements"])
             check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
@@ -7222,14 +8499,18 @@
             self._values["description"] = description
         if name is not None:
             self._values["name"] = name
         if additional_role_policy_statements is not None:
             self._values["additional_role_policy_statements"] = additional_role_policy_statements
         if alarms_enabled is not None:
             self._values["alarms_enabled"] = alarms_enabled
+        if definition is not None:
+            self._values["definition"] = definition
+        if definition_file is not None:
+            self._values["definition_file"] = definition_file
         if state_machine_failed_executions_alarm_evaluation_periods is not None:
             self._values["state_machine_failed_executions_alarm_evaluation_periods"] = state_machine_failed_executions_alarm_evaluation_periods
         if state_machine_failed_executions_alarm_threshold is not None:
             self._values["state_machine_failed_executions_alarm_threshold"] = state_machine_failed_executions_alarm_threshold
         if state_machine_input is not None:
             self._values["state_machine_input"] = state_machine_input
         if state_machine_name is not None:
@@ -7267,14 +8548,31 @@
 
         :default: true
         '''
         result = self._values.get("alarms_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
+    def definition(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]]:
+        '''Steps for the state machine.
+
+        Can either be provided as 'sfn.IChainable' or a JSON string.
+        '''
+        result = self._values.get("definition")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]], result)
+
+    @builtins.property
+    def definition_file(self) -> typing.Optional[builtins.str]:
+        '''File containing a JSON definition for the state machine.'''
+        result = self._values.get("definition_file")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def state_machine_failed_executions_alarm_evaluation_periods(
         self,
     ) -> typing.Optional[jsii.Number]:
         '''The number of periods over which data is compared to the specified threshold.
 
         :default: 1
         '''
@@ -7838,94 +9136,101 @@
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
+        definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+        definition_file: typing.Optional[builtins.str] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''Constructs state machine stage.
 
         :param scope: Scope within which this construct is defined.
         :param id: Identifier of the stage.
         :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
         :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param definition: Steps for the state machine. Can either be provided as 'sfn.IChainable' or a JSON string.
+        :param definition_file: File containing a JSON definition for the state machine.
         :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
         :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
         :param state_machine_input: Input of the state machine.
         :param state_machine_name: Name of the state machine.
         :param description: Description of the stage.
         :param name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c9ccc4da0d6d8eb11cda39b2839889ebd93235f90bbfbdd93a92a3f816c9fd60)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = StateMachineStageProps(
             additional_role_policy_statements=additional_role_policy_statements,
             alarms_enabled=alarms_enabled,
+            definition=definition,
+            definition_file=definition_file,
             state_machine_failed_executions_alarm_evaluation_periods=state_machine_failed_executions_alarm_evaluation_periods,
             state_machine_failed_executions_alarm_threshold=state_machine_failed_executions_alarm_threshold,
             state_machine_input=state_machine_input,
             state_machine_name=state_machine_name,
             description=description,
             name=name,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @jsii.member(jsii_name="createStateMachine")
     def _create_state_machine(
         self,
-        definition: _aws_cdk_aws_stepfunctions_ceddda9d.IChainable,
         *,
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
+        definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+        definition_file: typing.Optional[builtins.str] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> CreateStateMachineResult:
         '''Constructs a state machine from the definition.
 
-        :param definition: Steps for the state machine.
         :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
         :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param definition: Steps for the state machine. Can either be provided as 'sfn.IChainable' or a JSON string.
+        :param definition_file: File containing a JSON definition for the state machine.
         :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
         :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
         :param state_machine_input: Input of the state machine.
         :param state_machine_name: Name of the state machine.
         :param description: Description of the stage.
         :param name: Name of the stage.
 
         :return: Dictionary with event pattern, targets and state machine construct.
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__642bc4c0673f5b0f2331c42eaeb1c12c1c4fce53646416b8e239dd0bd724b5d2)
-            check_type(argname="argument definition", value=definition, expected_type=type_hints["definition"])
         props = StateMachineStageProps(
             additional_role_policy_statements=additional_role_policy_statements,
             alarms_enabled=alarms_enabled,
+            definition=definition,
+            definition_file=definition_file,
             state_machine_failed_executions_alarm_evaluation_periods=state_machine_failed_executions_alarm_evaluation_periods,
             state_machine_failed_executions_alarm_threshold=state_machine_failed_executions_alarm_threshold,
             state_machine_input=state_machine_input,
             state_machine_name=state_machine_name,
             description=description,
             name=name,
         )
 
-        return typing.cast(CreateStateMachineResult, jsii.invoke(self, "createStateMachine", [definition, props]))
+        return typing.cast(CreateStateMachineResult, jsii.invoke(self, "createStateMachine", [props]))
 
     @builtins.property
     @jsii.member(jsii_name="stateMachine")
     @abc.abstractmethod
     def state_machine(self) -> _aws_cdk_aws_stepfunctions_ceddda9d.StateMachine:
         '''State machine.'''
         ...
@@ -7963,14 +9268,16 @@
         destination_flow_config: typing.Optional[typing.Union[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.DestinationFlowConfigProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         flow_execution_status_check_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         flow_name: typing.Optional[builtins.str] = None,
         flow_tasks: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.TaskProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
         source_flow_config: typing.Optional[typing.Union[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.SourceFlowConfigProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
+        definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+        definition_file: typing.Optional[builtins.str] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
@@ -7981,14 +9288,16 @@
         :param destination_flow_config: The flow ``appflow.CfnFlow.DestinationFlowConfigProperty`` properties.
         :param flow_execution_status_check_period: Time to wait between flow execution status checks. Default: aws_cdk.Duration.seconds(15)
         :param flow_name: Name of the AppFlow flow to run. If None, an AppFlow flow is created.
         :param flow_tasks: The flow tasks properties.
         :param source_flow_config: The flow ``appflow.CfnFlow.SourceFlowConfigProperty`` properties.
         :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
         :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param definition: Steps for the state machine. Can either be provided as 'sfn.IChainable' or a JSON string.
+        :param definition_file: File containing a JSON definition for the state machine.
         :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
         :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
         :param state_machine_input: Input of the state machine.
         :param state_machine_name: Name of the state machine.
         :param description: Description of the stage.
         :param name: Name of the stage.
         '''
@@ -8000,14 +9309,16 @@
             destination_flow_config=destination_flow_config,
             flow_execution_status_check_period=flow_execution_status_check_period,
             flow_name=flow_name,
             flow_tasks=flow_tasks,
             source_flow_config=source_flow_config,
             additional_role_policy_statements=additional_role_policy_statements,
             alarms_enabled=alarms_enabled,
+            definition=definition,
+            definition_file=definition_file,
             state_machine_failed_executions_alarm_evaluation_periods=state_machine_failed_executions_alarm_evaluation_periods,
             state_machine_failed_executions_alarm_threshold=state_machine_failed_executions_alarm_threshold,
             state_machine_input=state_machine_input,
             state_machine_name=state_machine_name,
             description=description,
             name=name,
         )
@@ -8073,14 +9384,16 @@
         output_location: typing.Optional[typing.Union[_aws_cdk_aws_s3_ceddda9d.Location, typing.Dict[builtins.str, typing.Any]]] = None,
         parallel: typing.Optional[builtins.bool] = None,
         query_string: typing.Optional[typing.Sequence[builtins.str]] = None,
         query_string_path: typing.Optional[builtins.str] = None,
         work_group: typing.Optional[builtins.str] = None,
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
+        definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+        definition_file: typing.Optional[builtins.str] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
@@ -8095,14 +9408,16 @@
         :param output_location: Output S3 location.
         :param parallel: flag to determine parallel or sequential execution. Default: false
         :param query_string: SQL queries that will be started.
         :param query_string_path: dynamic path in statemachine for SQL query to be started.
         :param work_group: Athena workgroup name.
         :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
         :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param definition: Steps for the state machine. Can either be provided as 'sfn.IChainable' or a JSON string.
+        :param definition_file: File containing a JSON definition for the state machine.
         :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
         :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
         :param state_machine_input: Input of the state machine.
         :param state_machine_name: Name of the state machine.
         :param description: Description of the stage.
         :param name: Name of the stage.
         '''
@@ -8118,14 +9433,16 @@
             output_location=output_location,
             parallel=parallel,
             query_string=query_string,
             query_string_path=query_string_path,
             work_group=work_group,
             additional_role_policy_statements=additional_role_policy_statements,
             alarms_enabled=alarms_enabled,
+            definition=definition,
+            definition_file=definition_file,
             state_machine_failed_executions_alarm_evaluation_periods=state_machine_failed_executions_alarm_evaluation_periods,
             state_machine_failed_executions_alarm_threshold=state_machine_failed_executions_alarm_threshold,
             state_machine_input=state_machine_input,
             state_machine_name=state_machine_name,
             description=description,
             name=name,
         )
@@ -8205,14 +9522,16 @@
         project_name: typing.Optional[builtins.str] = None,
         recipe: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.RecipeProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         tags: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_ceddda9d.CfnTag, typing.Dict[builtins.str, typing.Any]]]] = None,
         timeout: typing.Optional[jsii.Number] = None,
         validation_configurations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ValidationConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
+        definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+        definition_file: typing.Optional[builtins.str] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
@@ -8239,14 +9558,16 @@
         :param project_name: The name of the project that the job is associated with.
         :param recipe: The recipe to be used by the DataBrew job which is a series of data transformation steps.
         :param tags: Metadata tags that have been applied to the job.
         :param timeout: The job's timeout in minutes. A job that attempts to run longer than this timeout period ends with a status of ``TIMEOUT`` .
         :param validation_configurations: List of validation configurations that are applied to the profile job.
         :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
         :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param definition: Steps for the state machine. Can either be provided as 'sfn.IChainable' or a JSON string.
+        :param definition_file: File containing a JSON definition for the state machine.
         :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
         :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
         :param state_machine_input: Input of the state machine.
         :param state_machine_name: Name of the state machine.
         :param description: Description of the stage.
         :param name: Name of the stage.
         '''
@@ -8274,14 +9595,16 @@
             project_name=project_name,
             recipe=recipe,
             tags=tags,
             timeout=timeout,
             validation_configurations=validation_configurations,
             additional_role_policy_statements=additional_role_policy_statements,
             alarms_enabled=alarms_enabled,
+            definition=definition,
+            definition_file=definition_file,
             state_machine_failed_executions_alarm_evaluation_periods=state_machine_failed_executions_alarm_evaluation_periods,
             state_machine_failed_executions_alarm_threshold=state_machine_failed_executions_alarm_threshold,
             state_machine_input=state_machine_input,
             state_machine_name=state_machine_name,
             description=description,
             name=name,
         )
@@ -8358,14 +9681,16 @@
         job_run_args: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_retry_backoff_rate: typing.Optional[jsii.Number] = None,
         state_machine_retry_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         state_machine_retry_max_attempts: typing.Optional[jsii.Number] = None,
         targets: typing.Optional[typing.Union[_aws_cdk_aws_glue_ceddda9d.CfnCrawler.TargetsProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
+        definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+        definition_file: typing.Optional[builtins.str] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
@@ -8383,14 +9708,16 @@
         :param job_run_args: The input arguments to the Glue job.
         :param state_machine_retry_backoff_rate: Multiplication for how much longer the wait interval gets on every retry. Default: 2
         :param state_machine_retry_interval: How many seconds to wait initially before retrying. Default: cdk.Duration.seconds(1)
         :param state_machine_retry_max_attempts: How many times to retry this particular error. Default: 3
         :param targets: A collection of targets to crawl.
         :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
         :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param definition: Steps for the state machine. Can either be provided as 'sfn.IChainable' or a JSON string.
+        :param definition_file: File containing a JSON definition for the state machine.
         :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
         :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
         :param state_machine_input: Input of the state machine.
         :param state_machine_name: Name of the state machine.
         :param description: Description of the stage.
         :param name: Name of the stage.
         '''
@@ -8409,25 +9736,32 @@
             job_run_args=job_run_args,
             state_machine_retry_backoff_rate=state_machine_retry_backoff_rate,
             state_machine_retry_interval=state_machine_retry_interval,
             state_machine_retry_max_attempts=state_machine_retry_max_attempts,
             targets=targets,
             additional_role_policy_statements=additional_role_policy_statements,
             alarms_enabled=alarms_enabled,
+            definition=definition,
+            definition_file=definition_file,
             state_machine_failed_executions_alarm_evaluation_periods=state_machine_failed_executions_alarm_evaluation_periods,
             state_machine_failed_executions_alarm_threshold=state_machine_failed_executions_alarm_threshold,
             state_machine_input=state_machine_input,
             state_machine_name=state_machine_name,
             description=description,
             name=name,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
+    @jsii.member(jsii_name="definition")
+    def definition(self) -> _aws_cdk_aws_stepfunctions_ceddda9d.IChainable:
+        return typing.cast(_aws_cdk_aws_stepfunctions_ceddda9d.IChainable, jsii.get(self, "definition"))
+
+    @builtins.property
     @jsii.member(jsii_name="glueJob")
     def glue_job(self) -> _aws_cdk_aws_glue_alpha_ce674d29.IJob:
         return typing.cast(_aws_cdk_aws_glue_alpha_ce674d29.IJob, jsii.get(self, "glueJob"))
 
     @builtins.property
     @jsii.member(jsii_name="stateMachine")
     def state_machine(self) -> _aws_cdk_aws_stepfunctions_ceddda9d.StateMachine:
@@ -8436,14 +9770,123 @@
 
     @builtins.property
     @jsii.member(jsii_name="crawler")
     def crawler(self) -> typing.Optional[_aws_cdk_aws_glue_ceddda9d.CfnCrawler]:
         return typing.cast(typing.Optional[_aws_cdk_aws_glue_ceddda9d.CfnCrawler], jsii.get(self, "crawler"))
 
     @builtins.property
+    @jsii.member(jsii_name="crawlerName")
+    def crawler_name(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "crawlerName"))
+
+    @builtins.property
+    @jsii.member(jsii_name="eventPattern")
+    def event_pattern(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern]:
+        '''Output event pattern of the stage.
+
+        Event pattern describes the structure of output event(s) produced by this stage.
+        Event Rules use event patterns to select events and route them to targets.
+        '''
+        return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern], jsii.get(self, "eventPattern"))
+
+    @builtins.property
+    @jsii.member(jsii_name="targets")
+    def targets(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]]:
+        '''Input targets for the stage.
+
+        Targets are used by Event Rules to describe what should be invoked when a rule matches an event.
+        '''
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]], jsii.get(self, "targets"))
+
+
+class MWAATriggerDagsStage(
+    StateMachineStage,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="aws-ddk-core.MWAATriggerDagsStage",
+):
+    '''Stage that contains a step function that runs a Managed Apache Airflow (MWAA) dag or set of dags .'''
+
+    def __init__(
+        self,
+        scope: _constructs_77d1e7e8.Construct,
+        id: builtins.str,
+        *,
+        mwaa_environment_name: builtins.str,
+        dag_path: typing.Optional[builtins.str] = None,
+        dags: typing.Optional[typing.Sequence[builtins.str]] = None,
+        status_check_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+        alarms_enabled: typing.Optional[builtins.bool] = None,
+        definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+        definition_file: typing.Optional[builtins.str] = None,
+        state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
+        state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
+        state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+        state_machine_name: typing.Optional[builtins.str] = None,
+        description: typing.Optional[builtins.str] = None,
+        name: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''Constructs MWAATriggerDagsStage.
+
+        :param scope: Scope within which this construct is defined.
+        :param id: Identifier of the stage.
+        :param mwaa_environment_name: Name of airflow environment.
+        :param dag_path: Path to array of dag id's to check.
+        :param dags: Name of dag(s) to trigger.
+        :param status_check_period: Time to wait between execution status checks. Default: aws_cdk.Duration.seconds(15)
+        :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
+        :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param definition: Steps for the state machine. Can either be provided as 'sfn.IChainable' or a JSON string.
+        :param definition_file: File containing a JSON definition for the state machine.
+        :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
+        :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
+        :param state_machine_input: Input of the state machine.
+        :param state_machine_name: Name of the state machine.
+        :param description: Description of the stage.
+        :param name: Name of the stage.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__6f0213661be18de8fe8fd12f50692a50182df1c8f22c50ad38963d7b78d944a0)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = MWAATriggerDagsStageProps(
+            mwaa_environment_name=mwaa_environment_name,
+            dag_path=dag_path,
+            dags=dags,
+            status_check_period=status_check_period,
+            additional_role_policy_statements=additional_role_policy_statements,
+            alarms_enabled=alarms_enabled,
+            definition=definition,
+            definition_file=definition_file,
+            state_machine_failed_executions_alarm_evaluation_periods=state_machine_failed_executions_alarm_evaluation_periods,
+            state_machine_failed_executions_alarm_threshold=state_machine_failed_executions_alarm_threshold,
+            state_machine_input=state_machine_input,
+            state_machine_name=state_machine_name,
+            description=description,
+            name=name,
+        )
+
+        jsii.create(self.__class__, self, [scope, id, props])
+
+    @builtins.property
+    @jsii.member(jsii_name="mwaaEnvironmentName")
+    def mwaa_environment_name(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "mwaaEnvironmentName"))
+
+    @builtins.property
+    @jsii.member(jsii_name="stateMachine")
+    def state_machine(self) -> _aws_cdk_aws_stepfunctions_ceddda9d.StateMachine:
+        '''State machine.'''
+        return typing.cast(_aws_cdk_aws_stepfunctions_ceddda9d.StateMachine, jsii.get(self, "stateMachine"))
+
+    @builtins.property
     @jsii.member(jsii_name="eventPattern")
     def event_pattern(
         self,
     ) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern]:
         '''Output event pattern of the stage.
 
         Event pattern describes the structure of output event(s) produced by this stage.
@@ -8478,14 +9921,16 @@
         redshift_cluster_identifier: builtins.str,
         sql_statements: typing.Sequence[builtins.str],
         database_name: typing.Optional[builtins.str] = None,
         database_user: typing.Optional[builtins.str] = None,
         polling_time: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
+        definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+        definition_file: typing.Optional[builtins.str] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
@@ -8496,14 +9941,16 @@
         :param redshift_cluster_identifier: Identifier of the Redshift cluster.
         :param sql_statements: List of SQL statements to execute.
         :param database_name: Name of the database in Redshift. Default: "dev"
         :param database_user: Database user. Default: "awsuser"
         :param polling_time: Waiting time between checking whether the statements have finished executing. Default: cdk.Duration.seconds(15)
         :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
         :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param definition: Steps for the state machine. Can either be provided as 'sfn.IChainable' or a JSON string.
+        :param definition_file: File containing a JSON definition for the state machine.
         :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
         :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
         :param state_machine_input: Input of the state machine.
         :param state_machine_name: Name of the state machine.
         :param description: Description of the stage.
         :param name: Name of the stage.
         '''
@@ -8515,14 +9962,16 @@
             redshift_cluster_identifier=redshift_cluster_identifier,
             sql_statements=sql_statements,
             database_name=database_name,
             database_user=database_user,
             polling_time=polling_time,
             additional_role_policy_statements=additional_role_policy_statements,
             alarms_enabled=alarms_enabled,
+            definition=definition,
+            definition_file=definition_file,
             state_machine_failed_executions_alarm_evaluation_periods=state_machine_failed_executions_alarm_evaluation_periods,
             state_machine_failed_executions_alarm_threshold=state_machine_failed_executions_alarm_threshold,
             state_machine_input=state_machine_input,
             state_machine_name=state_machine_name,
             description=description,
             name=name,
         )
@@ -9030,14 +10479,19 @@
     "GetEnvironmentProps",
     "GetSynthActionProps",
     "GetTagsProps",
     "GlueFactory",
     "GlueTransformStage",
     "GlueTransformStageProps",
     "KmsFactory",
+    "MWAAEnvironment",
+    "MWAAEnvironmentProps",
+    "MWAALambdasResult",
+    "MWAATriggerDagsStage",
+    "MWAATriggerDagsStageProps",
     "PermissionsBoundaryProps",
     "RedshiftDataApiStage",
     "RedshiftDataApiStageProps",
     "S3EventStage",
     "S3EventStageProps",
     "S3Factory",
     "SnsFactory",
@@ -9167,14 +10621,15 @@
     permissions_boundary_arn: typing.Optional[builtins.str] = None,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
+    suppress_template_indentation: typing.Optional[builtins.bool] = None,
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
@@ -9201,14 +10656,15 @@
     *,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
+    suppress_template_indentation: typing.Optional[builtins.bool] = None,
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
     config: typing.Optional[typing.Union[builtins.str, typing.Union[Configuration, typing.Dict[builtins.str, typing.Any]]]] = None,
     environment_id: typing.Optional[builtins.str] = None,
     permissions_boundary_arn: typing.Optional[builtins.str] = None,
 ) -> None:
@@ -9273,14 +10729,15 @@
     permissions_boundary_arn: typing.Optional[builtins.str] = None,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
+    suppress_template_indentation: typing.Optional[builtins.bool] = None,
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
@@ -9318,14 +10775,15 @@
     *,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
+    suppress_template_indentation: typing.Optional[builtins.bool] = None,
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
     config: typing.Optional[typing.Union[builtins.str, typing.Union[Configuration, typing.Dict[builtins.str, typing.Any]]]] = None,
     environment_id: typing.Optional[builtins.str] = None,
     permissions_boundary_arn: typing.Optional[builtins.str] = None,
     cdk_language: typing.Optional[builtins.str] = None,
@@ -9476,14 +10934,15 @@
     account: typing.Optional[builtins.str] = None,
     additional_install_commands: typing.Optional[typing.Sequence[builtins.str]] = None,
     cdk_version: typing.Optional[builtins.str] = None,
     codeartifact_domain: typing.Optional[builtins.str] = None,
     codeartifact_domain_owner: typing.Optional[builtins.str] = None,
     codeartifact_repository: typing.Optional[builtins.str] = None,
     code_pipeline_source: typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer] = None,
+    env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     partition: typing.Optional[builtins.str] = None,
     region: typing.Optional[builtins.str] = None,
     role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
@@ -9535,14 +10994,112 @@
     pending_window: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     policy: typing.Optional[_aws_cdk_aws_iam_ceddda9d.PolicyDocument] = None,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__2f57013032bd3f5e03e8cf2f82cc7c98b621d613c29a1e1844390ce9e164789e(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    additional_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+    dag_files: typing.Optional[typing.Sequence[builtins.str]] = None,
+    dag_processing_logs: typing.Optional[builtins.str] = None,
+    plugin_file: typing.Optional[builtins.str] = None,
+    requirements_file: typing.Optional[builtins.str] = None,
+    s3_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
+    scheduler_logs_level: typing.Optional[builtins.str] = None,
+    task_logs_level: typing.Optional[builtins.str] = None,
+    vpc_cidr: typing.Optional[builtins.str] = None,
+    vpc_id: typing.Optional[builtins.str] = None,
+    webserver_logs_level: typing.Optional[builtins.str] = None,
+    worker_logs_level: typing.Optional[builtins.str] = None,
+    name: builtins.str,
+    airflow_configuration_options: typing.Any = None,
+    airflow_version: typing.Optional[builtins.str] = None,
+    dag_s3_path: typing.Optional[builtins.str] = None,
+    environment_class: typing.Optional[builtins.str] = None,
+    execution_role_arn: typing.Optional[builtins.str] = None,
+    kms_key: typing.Optional[builtins.str] = None,
+    logging_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_mwaa_ceddda9d.CfnEnvironment.LoggingConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    max_workers: typing.Optional[jsii.Number] = None,
+    min_workers: typing.Optional[jsii.Number] = None,
+    network_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_mwaa_ceddda9d.CfnEnvironment.NetworkConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    plugins_s3_object_version: typing.Optional[builtins.str] = None,
+    plugins_s3_path: typing.Optional[builtins.str] = None,
+    requirements_s3_object_version: typing.Optional[builtins.str] = None,
+    requirements_s3_path: typing.Optional[builtins.str] = None,
+    schedulers: typing.Optional[jsii.Number] = None,
+    source_bucket_arn: typing.Optional[builtins.str] = None,
+    startup_script_s3_object_version: typing.Optional[builtins.str] = None,
+    startup_script_s3_path: typing.Optional[builtins.str] = None,
+    tags: typing.Any = None,
+    webserver_access_mode: typing.Optional[builtins.str] = None,
+    weekly_maintenance_window_start: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__274336e52a6efd650b5a38d3d50c0d6df8879c749af035d91610fec06e12c9fb(
+    scope: _constructs_77d1e7e8.Construct,
+    environment_name: builtins.str,
+    vpc_cidr: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8947f25c6bd15e846e7d13e9c335c4e41f800116e21ba100b25118382fcd659c(
+    *,
+    name: builtins.str,
+    airflow_configuration_options: typing.Any = None,
+    airflow_version: typing.Optional[builtins.str] = None,
+    dag_s3_path: typing.Optional[builtins.str] = None,
+    environment_class: typing.Optional[builtins.str] = None,
+    execution_role_arn: typing.Optional[builtins.str] = None,
+    kms_key: typing.Optional[builtins.str] = None,
+    logging_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_mwaa_ceddda9d.CfnEnvironment.LoggingConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    max_workers: typing.Optional[jsii.Number] = None,
+    min_workers: typing.Optional[jsii.Number] = None,
+    network_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_mwaa_ceddda9d.CfnEnvironment.NetworkConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    plugins_s3_object_version: typing.Optional[builtins.str] = None,
+    plugins_s3_path: typing.Optional[builtins.str] = None,
+    requirements_s3_object_version: typing.Optional[builtins.str] = None,
+    requirements_s3_path: typing.Optional[builtins.str] = None,
+    schedulers: typing.Optional[jsii.Number] = None,
+    source_bucket_arn: typing.Optional[builtins.str] = None,
+    startup_script_s3_object_version: typing.Optional[builtins.str] = None,
+    startup_script_s3_path: typing.Optional[builtins.str] = None,
+    tags: typing.Any = None,
+    webserver_access_mode: typing.Optional[builtins.str] = None,
+    weekly_maintenance_window_start: typing.Optional[builtins.str] = None,
+    additional_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+    dag_files: typing.Optional[typing.Sequence[builtins.str]] = None,
+    dag_processing_logs: typing.Optional[builtins.str] = None,
+    plugin_file: typing.Optional[builtins.str] = None,
+    requirements_file: typing.Optional[builtins.str] = None,
+    s3_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
+    scheduler_logs_level: typing.Optional[builtins.str] = None,
+    task_logs_level: typing.Optional[builtins.str] = None,
+    vpc_cidr: typing.Optional[builtins.str] = None,
+    vpc_id: typing.Optional[builtins.str] = None,
+    webserver_logs_level: typing.Optional[builtins.str] = None,
+    worker_logs_level: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3a03e72d8a80ef31dd9345bbdbea98b4abaf3d0a8612fd59523bd5d47407ab0c(
+    *,
+    status_lambda: _aws_cdk_aws_lambda_ceddda9d.Function,
+    trigger_lambda: _aws_cdk_aws_lambda_ceddda9d.Function,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__efd5392745ac5f11de7c7110e4c4c8cc4060becd6944d345396c27f2c82152b4(
     *,
     environment_id: typing.Optional[builtins.str] = None,
     prefix: typing.Optional[builtins.str] = None,
     qualifier: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
@@ -9624,14 +11181,15 @@
     initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
     layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
     log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
     log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     memory_size: typing.Optional[jsii.Number] = None,
+    params_and_secrets: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ParamsAndSecretsLayerVersion] = None,
     profiling: typing.Optional[builtins.bool] = None,
     profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
     reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
     role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
     security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
     timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -9668,14 +11226,16 @@
 
 def _typecheckingstub__5069a8477e1d868a51858f29afe4a12917625d0a7370bc4090fd23bf809c081c(
     *,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
+    definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+    definition_file: typing.Optional[builtins.str] = None,
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
@@ -9683,26 +11243,29 @@
 def _typecheckingstub__05acfa3cda54a17101814d614a246f97dc36de4bf27ef87f72f7aa4824dd7b35(
     *,
     additional_install_commands: typing.Optional[typing.Sequence[builtins.str]] = None,
     cdk_version: typing.Optional[builtins.str] = None,
     codeartifact_domain: typing.Optional[builtins.str] = None,
     codeartifact_domain_owner: typing.Optional[builtins.str] = None,
     codeartifact_repository: typing.Optional[builtins.str] = None,
+    env: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     synth_action: typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildStep] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__50f57d5c758f4bb8a7385b25c9dd1756786a7af562ac0cf743837ff675065839(
     *,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
+    definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+    definition_file: typing.Optional[builtins.str] = None,
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     destination_flow_config: typing.Optional[typing.Union[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.DestinationFlowConfigProperty, typing.Dict[builtins.str, typing.Any]]] = None,
     flow_execution_status_check_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     flow_name: typing.Optional[builtins.str] = None,
@@ -9714,14 +11277,16 @@
 
 def _typecheckingstub__d02b2a3868910a4789cbcba2028e07a331d2da507e4b4c951dd7801d735bc0ac(
     *,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
+    definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+    definition_file: typing.Optional[builtins.str] = None,
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     catalog_name: typing.Optional[builtins.str] = None,
     database_name: typing.Optional[builtins.str] = None,
     encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.Key] = None,
@@ -9737,14 +11302,16 @@
 
 def _typecheckingstub__f6be6b9ec4e805f427307a7bc1c743a3f56ffd52c0cc37a1436d75ce69e31b9f(
     *,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
+    definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+    definition_file: typing.Optional[builtins.str] = None,
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     create_job: typing.Optional[builtins.bool] = None,
     database_outputs: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DatabaseOutputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
     data_catalog_outputs: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DataCatalogOutputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
@@ -9861,14 +11428,16 @@
 
 def _typecheckingstub__36c864b97313236b09b597808a1574a4f4d21024bac872f4e182edbd9a3d0175(
     *,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
+    definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+    definition_file: typing.Optional[builtins.str] = None,
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     crawler_allow_failure: typing.Optional[builtins.bool] = None,
     crawler_name: typing.Optional[builtins.str] = None,
     crawler_props: typing.Optional[typing.Union[_aws_cdk_aws_glue_ceddda9d.CfnCrawlerProps, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -9881,20 +11450,42 @@
     state_machine_retry_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     state_machine_retry_max_attempts: typing.Optional[jsii.Number] = None,
     targets: typing.Optional[typing.Union[_aws_cdk_aws_glue_ceddda9d.CfnCrawler.TargetsProperty, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__22752f7fca368ed1e29dd71501fbd74daab00450e10e80bb5c02b1233ef9c8f5(
+    *,
+    description: typing.Optional[builtins.str] = None,
+    name: typing.Optional[builtins.str] = None,
+    additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+    alarms_enabled: typing.Optional[builtins.bool] = None,
+    definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+    definition_file: typing.Optional[builtins.str] = None,
+    state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
+    state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
+    state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+    state_machine_name: typing.Optional[builtins.str] = None,
+    mwaa_environment_name: builtins.str,
+    dag_path: typing.Optional[builtins.str] = None,
+    dags: typing.Optional[typing.Sequence[builtins.str]] = None,
+    status_check_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__defbc9333f2b8b3e2d55373f9b0155e5f6e83609e9153dc24f619d747ca4f133(
     *,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
+    definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+    definition_file: typing.Optional[builtins.str] = None,
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     redshift_cluster_identifier: builtins.str,
     sql_statements: typing.Sequence[builtins.str],
     database_name: typing.Optional[builtins.str] = None,
@@ -9968,29 +11559,16 @@
 
 def _typecheckingstub__c9ccc4da0d6d8eb11cda39b2839889ebd93235f90bbfbdd93a92a3f816c9fd60(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
-    state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
-    state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
-    state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
-    state_machine_name: typing.Optional[builtins.str] = None,
-    description: typing.Optional[builtins.str] = None,
-    name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__642bc4c0673f5b0f2331c42eaeb1c12c1c4fce53646416b8e239dd0bd724b5d2(
-    definition: _aws_cdk_aws_stepfunctions_ceddda9d.IChainable,
-    *,
-    additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
-    alarms_enabled: typing.Optional[builtins.bool] = None,
+    definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+    definition_file: typing.Optional[builtins.str] = None,
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
 ) -> None:
@@ -10004,14 +11582,16 @@
     destination_flow_config: typing.Optional[typing.Union[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.DestinationFlowConfigProperty, typing.Dict[builtins.str, typing.Any]]] = None,
     flow_execution_status_check_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     flow_name: typing.Optional[builtins.str] = None,
     flow_tasks: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.TaskProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
     source_flow_config: typing.Optional[typing.Union[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.SourceFlowConfigProperty, typing.Dict[builtins.str, typing.Any]]] = None,
     additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
+    definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+    definition_file: typing.Optional[builtins.str] = None,
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
 ) -> None:
@@ -10029,14 +11609,16 @@
     output_location: typing.Optional[typing.Union[_aws_cdk_aws_s3_ceddda9d.Location, typing.Dict[builtins.str, typing.Any]]] = None,
     parallel: typing.Optional[builtins.bool] = None,
     query_string: typing.Optional[typing.Sequence[builtins.str]] = None,
     query_string_path: typing.Optional[builtins.str] = None,
     work_group: typing.Optional[builtins.str] = None,
     additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
+    definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+    definition_file: typing.Optional[builtins.str] = None,
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
 ) -> None:
@@ -10066,14 +11648,16 @@
     project_name: typing.Optional[builtins.str] = None,
     recipe: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.RecipeProperty, typing.Dict[builtins.str, typing.Any]]] = None,
     tags: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_ceddda9d.CfnTag, typing.Dict[builtins.str, typing.Any]]]] = None,
     timeout: typing.Optional[jsii.Number] = None,
     validation_configurations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ValidationConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
     additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
+    definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+    definition_file: typing.Optional[builtins.str] = None,
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
 ) -> None:
@@ -10094,14 +11678,38 @@
     job_run_args: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_retry_backoff_rate: typing.Optional[jsii.Number] = None,
     state_machine_retry_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     state_machine_retry_max_attempts: typing.Optional[jsii.Number] = None,
     targets: typing.Optional[typing.Union[_aws_cdk_aws_glue_ceddda9d.CfnCrawler.TargetsProperty, typing.Dict[builtins.str, typing.Any]]] = None,
     additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
+    definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+    definition_file: typing.Optional[builtins.str] = None,
+    state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
+    state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
+    state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+    state_machine_name: typing.Optional[builtins.str] = None,
+    description: typing.Optional[builtins.str] = None,
+    name: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__6f0213661be18de8fe8fd12f50692a50182df1c8f22c50ad38963d7b78d944a0(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    mwaa_environment_name: builtins.str,
+    dag_path: typing.Optional[builtins.str] = None,
+    dags: typing.Optional[typing.Sequence[builtins.str]] = None,
+    status_check_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+    additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+    alarms_enabled: typing.Optional[builtins.bool] = None,
+    definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+    definition_file: typing.Optional[builtins.str] = None,
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
 ) -> None:
@@ -10115,14 +11723,16 @@
     redshift_cluster_identifier: builtins.str,
     sql_statements: typing.Sequence[builtins.str],
     database_name: typing.Optional[builtins.str] = None,
     database_user: typing.Optional[builtins.str] = None,
     polling_time: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
+    definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+    definition_file: typing.Optional[builtins.str] = None,
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
 ) -> None:
```

### Comparing `aws-ddk-core-1.0.1/src/aws_ddk_core/_jsii/__init__.py` & `aws-ddk-core-1.1.0/src/aws_ddk_core/_jsii/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import aws_cdk.aws_glue_alpha._jsii
 import aws_cdk.aws_kinesisfirehose_alpha._jsii
 import aws_cdk.aws_kinesisfirehose_destinations_alpha._jsii
 import aws_cdk.integ_tests_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
-    "aws-ddk-core", "1.0.1", __name__[0:-6], "aws-ddk-core@1.0.1.jsii.tgz"
+    "aws-ddk-core", "1.1.0", __name__[0:-6], "aws-ddk-core@1.1.0.jsii.tgz"
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-ddk-core-1.0.1/src/aws_ddk_core.egg-info/PKG-INFO` & `aws-ddk-core-1.1.0/src/aws_ddk_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ddk-core
-Version: 1.0.1
+Version: 1.1.0
 Summary: AWS DataOps Development Kit
 Home-page: https://github.com/awslabs/aws-ddk/tree/main
 Author: AWS Professional Services<aws-proserve-orion-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-ddk/tree/main
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

