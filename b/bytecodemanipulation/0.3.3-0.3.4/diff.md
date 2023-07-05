# Comparing `tmp/bytecodemanipulation-0.3.3.tar.gz` & `tmp/bytecodemanipulation-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytecodemanipulation-0.3.3.tar", last modified: Fri Jun 23 14:20:57 2023, max compression
+gzip compressed data, was "bytecodemanipulation-0.3.4.tar", last modified: Wed Jul  5 11:00:12 2023, max compression
```

## Comparing `bytecodemanipulation-0.3.3.tar` & `bytecodemanipulation-0.3.4.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.368648 bytecodemanipulation-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-06-23 14:20:57.368648 bytecodemanipulation-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.352648 bytecodemanipulation-0.3.3/bytecodemanipulation/
--rw-r--r--   0 runner    (1001) docker     (123)    22008 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/Emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/Mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    19747 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/MutableFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/MutableFunctionHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27037 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/Optimiser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/Specialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/TypeEnforcer.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/annotated_std.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.352648 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/AbstractBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    12247 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/Emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/Lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/Parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/syntax_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.352648 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/util/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/util/CommonUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/util/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/util/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.352648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.352648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15377 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/builtin_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.356648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/CompoundExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.360648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/AssertAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/AssertStaticInstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    14138 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/CallAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/IfAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/JumpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LabelAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LoadAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    25406 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/MacroAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    19276 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/OpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/RawAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/StoreAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/WhileAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/YieldAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.360648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/ExceptionInstructionCodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/LocationInformationHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/assembly_instructions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.364648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    13524 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/specialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.364648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/assembly_instructions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.364648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/CallAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/ClassDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/IfAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/JumpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/LoadFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/LoadGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/specialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.364648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_12/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/mixin_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.368648 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/
--rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/AbstractOpcodeTransformerStage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/CacheEntryCreation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/CodeObjectBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/ExceptionTable.py
--rw-r--r--   0 runner    (1001) docker     (123)    25688 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/Instruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/OpcodeReplacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/Opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/optimise_self.py
--rw-r--r--   0 runner    (1001) docker     (123)    17426 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/optimiser_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.352648 bytecodemanipulation-0.3.3/bytecodemanipulation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-06-23 14:20:57.000000 bytecodemanipulation-0.3.3/bytecodemanipulation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-06-23 14:20:57.000000 bytecodemanipulation-0.3.3/bytecodemanipulation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:20:57.000000 bytecodemanipulation-0.3.3/bytecodemanipulation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 14:20:57.000000 bytecodemanipulation-0.3.3/bytecodemanipulation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 14:20:57.368648 bytecodemanipulation-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-23 14:20:50.000000 bytecodemanipulation-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.368648 bytecodemanipulation-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    54986 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_Assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_InlineSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_Mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_MutableFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_Operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_Optimiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_Specializations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_StandardLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_issues.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.484822 bytecodemanipulation-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-07-05 11:00:12.484822 bytecodemanipulation-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.452822 bytecodemanipulation-0.3.4/bytecodemanipulation/
+-rw-r--r--   0 runner    (1001) docker     (123)    22008 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/Emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/Mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19747 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/MutableFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/MutableFunctionHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27037 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/Optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/Specialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/TypeEnforcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/annotated_std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.452822 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/
+-rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/AbstractBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12247 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/Emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/Lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21487 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/Parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/syntax_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.456822 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/util/CommonUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/util/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/util/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.456822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.456822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15377 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/builtin_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.460822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/CompoundExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.468822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/AssertAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/AssertStaticInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15500 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/CallAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/IfAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/JumpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LabelAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LoadAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27035 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/MacroAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20630 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/OpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/RawAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/StoreAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/WhileAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/YieldAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.468822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/ExceptionInstructionCodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/LocationInformationHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/assembly_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.476822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22437 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/specialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.476822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/assembly_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.480822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/CallAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/ClassDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/IfAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/JumpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/LoadFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/LoadGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/specialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.480822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_12/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/mixin_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.484822 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/AbstractOpcodeTransformerStage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/CacheEntryCreation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/CodeObjectBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/ExceptionTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25709 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/Instruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/OpcodeReplacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/Opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/optimise_self.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17702 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/optimiser_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.452822 bytecodemanipulation-0.3.4/bytecodemanipulation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-07-05 11:00:12.000000 bytecodemanipulation-0.3.4/bytecodemanipulation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-07-05 11:00:12.000000 bytecodemanipulation-0.3.4/bytecodemanipulation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:00:12.000000 bytecodemanipulation-0.3.4/bytecodemanipulation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-05 11:00:12.000000 bytecodemanipulation-0.3.4/bytecodemanipulation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 11:00:12.484822 bytecodemanipulation-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-05 11:00:05.000000 bytecodemanipulation-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.484822 bytecodemanipulation-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    58018 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_Assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_InlineSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_Mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_MutableFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_Operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_Optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_Specializations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_StandardLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_issues.py
```

### Comparing `bytecodemanipulation-0.3.3/LICENSE` & `bytecodemanipulation-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/PKG-INFO` & `bytecodemanipulation-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytecodemanipulation
-Version: 0.3.3
+Version: 0.3.4
 Summary: High level python bytecode manipulation
 Home-page: https://github.com/uuk0/PyBytecodeManipulator
 Author: uuk
 Author-email: uuk1301@gmail.com
 Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `bytecodemanipulation-0.3.3/README.md` & `bytecodemanipulation-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/Emulator.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/Emulator.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/Mixin.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/Mixin.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/MutableFunction.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/MutableFunction.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/MutableFunctionHelpers.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/MutableFunctionHelpers.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/Optimiser.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/Optimiser.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/Specialization.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/Specialization.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/AbstractBase.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/AbstractBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,18 @@
         self._name_counter = 1
         self.globals_dict = {}
         self.module_file: str = None
         self.last_base_token: AbstractToken = None
         self.macro_parameter_namespace: typing.Dict[str] = {}
         self.filled_locals = set()
 
+        self.current_macro_assembly = None
+
+        self.closure_locals: typing.Set[str] = set()
+
     def scope_name_generator(self, suffix="") -> str:
         name = f"%INTERNAL:{self._name_counter}"
         self._name_counter += 1
 
         if suffix:
             name += "/" + suffix
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/Emitter.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/Emitter.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/Lexer.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/Lexer.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/Parser.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/Parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,15 +107,18 @@
         IdentifierExpression,
     )
     import bytecodemanipulation.assembler.util.parser as parser_file
 
 
 def create_instruction(token: AbstractToken, *args, **kwargs) -> Instruction:
     instr = Instruction(*args, **kwargs)
-    instr.source_location = token.line, token.column, token.span
+
+    if token is not None:
+        instr.source_location = token.line, token.column, token.span
+
     return instr
 
 
 Instruction.create_with_token = create_instruction
 
 parser_file.raise_syntax_error = _syntax_wrapper
 
@@ -362,19 +365,36 @@
             while self.try_consume(SpecialToken("|")):
                 prefix += "|"
 
             if prefix == "":
                 while self.try_consume(SpecialToken(":")):
                     prefix += ":"
 
+            elif error := self.try_consume(SpecialToken(":")):
+                raise throw_positioned_error(
+                    scope,
+                    error,
+                    "Cannot parse '|' and ':' for <local variable name>",
+                )
+
             expr = LocalAccessExpression(self.parse_identifier_like(scope), start_token, prefix=prefix)
 
         elif start_token.text == "§":
             self.consume(SpecialToken("§"), err_arg=scope)
-            expr = DerefAccessExpression(self.parse_identifier_like(scope), start_token)
+
+            identifier = self.try_parse_identifier_like()
+
+            if identifier is None:
+                raise throw_positioned_error(
+                    scope,
+                    [start_token, self[0]],
+                    "Expected <identifier-like> after '§' for cell-var reference",
+                )
+
+            expr = DerefAccessExpression(identifier, start_token)
 
         elif start_token.text == "&":
             self.consume(SpecialToken("&"), err_arg=scope)
             expr = MacroParameterAccessExpression(
                 self.parse_identifier_like(scope), start_token
             )
 
@@ -566,7 +586,40 @@
             raise throw_positioned_error(
                 scope,
                 self[0],
                 "expected <identifier> or &<identifier>",
             )
 
         return identifier
+
+    def try_parse_jump_target(self) -> typing.List[IIdentifierAccessor] | None:
+        self.save()
+        tokens = []
+
+        if not (t := self.try_parse_identifier_like()):
+            return
+
+        tokens.append(t)
+
+        while self.try_consume(SpecialToken(":")):
+            t = self.try_parse_identifier_like()
+
+            if t is None:
+                self.rollback()
+                return
+
+            tokens.append(t)
+
+        self.discard_save()
+        return tokens
+
+    def parse_jump_target(self, scope: ParsingScope) -> typing.List[IIdentifierAccessor]:
+        tokens = self.try_parse_jump_target()
+
+        if tokens is None:
+            raise throw_positioned_error(
+                scope,
+                self[0],
+                "expected <identifier-like>[{':' <identifier like>}] for jump target"
+            )
+
+        return tokens
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/hook.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/hook.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/syntax_errors.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/syntax_errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,17 @@
                 print()
             already_seen_line = True
 
             file = scope.module_file.replace("\\", "/")
             print(f'File "{file}", line {line + 1}', file=sys.stderr)
         previous_line_no = line
 
+        if line >= len(content):
+            continue
+
         print(content[line].removesuffix("\n"), file=sys.stderr)
         print(error_location, file=sys.stderr)
 
 
 def throw_positioned_error(
     scope: ParsingScope,
     token: AbstractToken | typing.List[AbstractToken | None] | None,
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/target.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/target.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/util/parser.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/util/parser.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/util/tokenizer.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/util/tokenizer.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/builtin_spec.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/builtin_spec.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/CompoundExpression.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/CompoundExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.get_name(scope)
 
         if value not in scope.filled_locals:
             # todo: why is it warning for some stream tests?
-            warnings.warn(SyntaxWarning(f"Expected local variable '{value}' to be set ahead of time, but might be not set (cannot infer for custom jumps)"), stacklevel=1)
+            warnings.warn(SyntaxWarning(f"Expected local variable '{value}' to be set ahead of time, but might be not set (cannot infer for custom jumps)"), stacklevel=2)
 
         return [
             Instruction.create_with_token(
                 self.token, Opcodes.LOAD_FAST, self.prefix + value
             )
         ]
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,46 @@
 import builtins
+import os
+import sys
 import types
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
+root = __file__
+for _ in range(5):
+    root = os.path.dirname(root)
+
+
+with open(root+"/setup.py", mode="r") as f :
+    line = list(f.readlines())[8].strip()
+
+    if not line.startswith("version="):
+        raise RuntimeError("could not find version information")
+
+    parts = list(map(int, line.removeprefix("version=\"").removesuffix("\",").split(".")))
+    BCM_VERSION = parts[0] * 10000 + parts[1] * 100 + parts[2]
+
+
 class ModuleAccessExpression(AbstractAccessExpression):
     IS_STATIC = True
     PREFIX = "~"
     _CACHE = builtins.__dict__.copy()
 
+    _CACHE.update({
+        "PY_VERSION": sys.version_info.major * 100 + sys.version_info.minor,
+        "BCM_VERSION": BCM_VERSION,
+    })
+
     @classmethod
     def _cached_lookup(cls, module_name: str) -> types.ModuleType:
         if module_name not in cls._CACHE:
             module = cls._CACHE[module_name] = __import__(module_name)
             return module
 
         return cls._CACHE[module_name]
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/AssertAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/AssertAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/AssertStaticInstruction.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/AssertStaticInstruction.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/CallAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/CallAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,17 +270,50 @@
                     raise throw_positioned_error(
                         scope,
                         parser.try_inspect(),
                         "*<arg> only allowed before keyword arguments!",
                     )
 
             elif not has_seen_keyword_arg:
+                if is_macro and ((inner_opening_bracket := parser[0]) == SpecialToken("[")):
+                    parser.consume(SpecialToken("["))
+
+                    to_be_stored_at = []
+
+                    while not parser.try_inspect() == SpecialToken("]"):
+                        parser.try_consume(SpecialToken("$"))
+                        base = parser.try_parse_identifier_like()
+
+                        if base is None:
+                            raise throw_positioned_error(
+                                scope,
+                                [inner_opening_bracket, parser[0]],
+                                "Expected <expression> after ','",
+                            )
+
+                        to_be_stored_at.append(base)
+
+                        if not parser.try_consume(SpecialToken(",")):
+                            break
+
+                    if not parser.try_consume(SpecialToken("]")):
+                        raise throw_positioned_error(
+                            scope,
+                            [inner_opening_bracket, parser[0]],
+                            "Expected ']' closing '['",
+                        )
+
+                    expr = parser.parse_body(scope=scope)
+                    expr.to_be_stored_at = to_be_stored_at
+                    is_dynamic = False
+
                 # todo: maybe parse here also partial variable names
-                if is_macro and parser[0] == SpecialToken("{"):
+                elif is_macro and parser[0] == SpecialToken("{"):
                     expr = parser.parse_body(scope=scope)
+                    expr.to_be_stored_at = []
                     is_dynamic = False
 
                 else:
                     is_dynamic = is_partial and bool(
                         parser.try_consume(SpecialToken("?"))
                     )
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,45 +29,77 @@
 
     @classmethod
     def consume(
         cls, parser: "Parser", scope: ParsingScope
     ) -> "AbstractClassDefinitionAssembly":
         name = parser.parse_identifier_like(scope)
 
+        if name is None:
+            raise throw_positioned_error(
+                scope,
+                parser[0],
+                "Expected <identifier like>"
+            )
+
         namespace = None
 
-        if parser.try_consume(SpecialToken("<")):
-            namespace = [parser.consume(IdentifierToken, err_arg=scope).text]
+        if opening_bracket := parser.try_consume(SpecialToken("<")):
+            # todo: maybe use try_parse_identifier_like() instead
+            namespace_f = parser.try_consume(IdentifierToken)
+
+            if namespace_f is None:
+                raise throw_positioned_error(
+                    scope,
+                    parser[0],
+                    "<name> expected",
+                )
+
+            namespace = [namespace_f.text]
 
             while parser.try_consume(SpecialToken(":")):
-                namespace.append(parser.consume(IdentifierToken, err_arg=scope).text)
+                p = parser.try_consume(IdentifierToken)
 
-            parser.consume(SpecialToken(">"), err_arg=scope)
+                if p is None:
+                    raise throw_positioned_error(
+                        scope,
+                        [namespace_f, parser[0]],
+                        "<name> expected after ':' to complete namespace name",
+                    )
+
+                namespace.append(p.text)
+
+            if parser.try_consume(SpecialToken(">")) is None:
+                raise throw_positioned_error(
+                    scope,
+                    [opening_bracket, parser[0]],
+                    "expected '>' to close namespace declaration",
+                )
 
         parents = []
 
-        if parser.try_consume(SpecialToken("(")):
+        if opening_bracket := parser.try_consume(SpecialToken("(")):
             if parent := parser.try_consume_access_to_value():
                 parents.append(parent)
 
                 while parser.try_consume(SpecialToken(",")):
                     if parser[0] == SpecialToken(")"):
                         break
 
                     parent = parser.try_consume_access_to_value()
                     if parent is None:
                         raise throw_positioned_error(
                             scope,
                             parser[0],
-                            "Expected <expression>",
+                            "Expected <expression> for parent",
                         )
+
                     parents.append(parent)
 
             if not parser.try_consume(SpecialToken(")")):
-                raise throw_positioned_error(scope, parser[0], "Expected ')'")
+                raise throw_positioned_error(scope, [opening_bracket, parser[0]], "Expected ')'")
 
         if not parents:
             parents = [ConstantAccessExpression(object)]
 
         code_block = parser.parse_body(scope=scope, namespace_part=namespace)
         return cls(
             name,
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,47 +45,49 @@
     @classmethod
     def consume(
         cls, parser: "Parser", scope: ParsingScope
     ) -> "AbstractForEachAssembly":
         initial = parser.try_consume_access_to_value()
         if initial is None:
             raise throw_positioned_error(
-                scope, parser[0], "<expression> expected"
+                scope, parser[0], "initial <expression> expected"
             )
+
         variables = [initial]
 
         while parser.try_consume(SpecialToken(",")):
 
             expr = parser.try_consume_access_to_value()
 
             if expr is None:
                 raise throw_positioned_error(
-                    scope, parser[0], "<expression> expected"
+                    scope, parser[0], "further <expression> expected after ','"
                 )
 
             variables.append(expr)
 
         if not parser.try_consume(IdentifierToken("IN")):
             raise throw_positioned_error(scope, parser[0], "'IN' expected")
 
         source = parser.try_consume_access_to_value()
         if not source:
             raise throw_positioned_error(
-                scope, parser[0], "<expression> expected"
+                scope, parser[0], "base iterator <expression> expected"
             )
+
         sources = [source]
 
         multi = None
         while parser.try_consume(SpecialToken(",")) or (
             multi := parser.try_consume(SpecialToken("*"))
         ):
             source = parser.try_consume_access_to_value()
             if not source:
                 raise throw_positioned_error(
-                    scope, parser[0], "<expression> expected"
+                    scope, parser[0], f"further iterator <expression> expected after '{'*' if multi else ','}'"
                 )
 
             if multi:
                 s = sources[-1]
 
                 if isinstance(s, cls.ForEachMultiplier):
                     s.items.append(source)
@@ -104,15 +106,15 @@
             )
 
         body = parser.parse_body(scope=scope)
         return cls(
             variables,
             sources,
             body,
-            scope.last_base_token,
+            typing.cast(IdentifierToken, scope.last_base_token),
         )
 
     def __init__(
         self,
         variables: typing.List[AbstractAccessExpression],
         sources: typing.List[AbstractAccessExpression],
         body: CompoundExpression,
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
-from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.data.shared.instructions.CallAssembly import (
     AbstractCallAssembly,
 )
 from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
@@ -35,14 +34,21 @@
         while parser.try_consume(SpecialToken("|")):
             prefix += "|"
 
         if prefix == "":
             while parser.try_consume(SpecialToken(":")):
                 prefix += ":"
 
+        elif error := parser.try_consume(SpecialToken(":")):
+            raise throw_positioned_error(
+                scope,
+                error,
+                "Cannot parse '|' and ':' as inter-fix for <function name>",
+            )
+
         func_name = parser.parse_identifier_like(scope)
 
         bound_variables: typing.List[typing.Tuple[IIdentifierAccessor, bool]] = []
         args = []
 
         if parser.try_consume(SpecialToken("<")):
             is_static = bool(parser.try_consume(SpecialToken("!")))
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/IfAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/WhileAssembly.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,108 +6,108 @@
 from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
+from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
     CompoundExpression,
 )
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 
 
-class AbstractIFAssembly(AbstractAssemblyInstruction, abc.ABC):
-    # IF <expression> ['\'' <label name> '\''] '{' <body> '}'
-    NAME = "IF"
+class AbstractWhileAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # # WHILE <expression> ['\'' <label name> '\''] '{' <body> '}'
+    NAME = "WHILE"
 
     @classmethod
-    def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractIFAssembly":
-        source = parser.try_parse_data_source(
+    def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractWhileAssembly":
+        condition = parser.try_parse_data_source(
             allow_primitives=True, include_bracket=False, scope=scope
         )
 
-        if source is None:
+        if condition is None:
             raise throw_positioned_error(
                 scope, parser.try_inspect(), "expected <expression>"
             )
 
         if parser.try_consume(SpecialToken("'")):
-            label_name = parser.parse_identifier_like(scope)
+            label_name = parser.parse_jump_target(scope)
+
             if not parser.try_consume(SpecialToken("'")):
                 raise throw_positioned_error(
                     scope, parser.try_inspect(), "expected '"
                 )
+
         else:
             label_name = None
 
         body = parser.parse_body(scope=scope)
 
         return cls(
-            source,
+            condition,
             body,
             label_name,
         )
 
     def __init__(
         self,
         source: AbstractSourceExpression,
         body: CompoundExpression,
-        label_name: IIdentifierAccessor | str = None,
+        label_name: typing.List[IIdentifierAccessor] | str | None = None,
     ):
         self.source = source
         self.body = body
         self.label_name = (
             label_name
             if not isinstance(label_name, str)
-            else StaticIdentifier(label_name)
-        )
+            else [StaticIdentifier(e) for e in label_name.split(":")]
+        ) if label_name is not None else None
 
     def copy(self):
-        return type(self)(self.source.copy(), self.body.copy(), self.label_name)
+        return type(self)(self.source.copy(), self.body.copy(), self.label_name.copy())
 
     def __eq__(self, other):
         return (
             type(self) == type(other)
             and self.source == other.source
             and self.body == other.body
             and self.label_name == other.label_name
         )
 
     def __repr__(self):
         c = "'"
-        return f"IF({self.source}{'' if self.label_name is None else ', label='+c+repr(self.label_name)+c}) -> {{{self.body}}}"
+        return f"WHILE({self.source}{'' if self.label_name is None else ', label='+c+repr(self.label_name)+c}) -> {{{self.body}}}"
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
-            self,
-            (
-                self.source.visit_parts(visitor, parents + [self]),
-                self.body.visit_parts(visitor, parents + [self]),
-            ),
-            parents,
+            self, (self.source.visit_parts(visitor), self.body.visit_parts(visitor))
         )
 
     def visit_assembly_instructions(
         self, visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any]
     ):
         return visitor(self, (self.body.visit_assembly_instructions(visitor),))
 
-    def get_labels(self, scope: ParsingScope) -> typing.Set[str]:
+    def get_labels(self, scope: ParsingScope):
+        name = ":".join(e(scope) for e in self.label_name)
+
         return (
             set()
             if self.label_name is None
             else {
-                self.label_name(scope),
-                self.label_name(scope) + "_END",
-                self.label_name(scope) + "_HEAD",
+                name,
+                name + ":END",
+                name + ":INNER",
             }
         ) | self.body.get_labels(scope)
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/JumpAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,94 +1,74 @@
 import abc
 import typing
 
-from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
+from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
+from bytecodemanipulation.assembler.util.tokenizer import IntegerToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
-from bytecodemanipulation.data.shared.instructions.OpAssembly import AbstractOpAssembly
 
 
-class AbstractJumpAssembly(AbstractAssemblyInstruction, abc.ABC):
-    NAME = "JUMP"
+class AbstractStoreGlobalAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # STORE_GLOBAL <name> [<source>]
+    NAME = "STORE_GLOBAL"
 
-    @classmethod
-    def consume(cls, parser: "Parser", scope) -> "AbstractJumpAssembly":
-        has_quotes = parser.try_consume(SpecialToken("'"))
-
-        label_target = parser.consume(IdentifierToken)
-
-        if has_quotes:
-            parser.consume(SpecialToken("'"))
-
-        if parser.try_consume(IdentifierToken("IF")):
-            condition = parser.try_parse_data_source(
-                allow_primitives=True, include_bracket=False, allow_op=True
+    def __init__(
+        self,
+        name_token: IdentifierToken | IntegerToken | str | int,
+        source: AbstractSourceExpression | None = None,
+    ):
+        self.name_token = (
+            name_token
+            if not isinstance(name_token, (str, int))
+            else (
+                IdentifierToken(name_token)
+                if isinstance(name_token, str)
+                else IntegerToken(str(name_token))
             )
+        )
+        self.source = source
 
-        elif parser.try_consume(SpecialToken("(")):
-            parser.save()
-            condition = parser.try_parse_data_source(
-                allow_primitives=True, include_bracket=False, allow_op=True
+    @classmethod
+    def consume(cls, parser: "Parser", scope) -> "AbstractStoreGlobalAssembly":
+        parser.try_consume(SpecialToken("@"))
+        name = parser.try_consume([IdentifierToken, IntegerToken])
+
+        if name is None:
+            raise throw_positioned_error(
+                scope, parser.try_inspect(), "expected <name> or <integer>"
             )
 
-            if condition is None or not parser.try_consume(SpecialToken(")")):
-                parser.rollback()
-                condition = AbstractOpAssembly.IMPLEMENTATION.consume(parser, None)
-                parser.consume(SpecialToken(")"))
-            else:
-                parser.discard_save()
+        source = parser.try_parse_data_source()
 
-        else:
-            condition = None
+        return cls(name, source)
 
-        return cls(label_target, condition)
-
-    def __init__(
-        self,
-        label_name_token: IdentifierToken | str,
-        condition: AbstractAccessExpression | None = None,
-    ):
-        self.label_name_token = (
-            label_name_token
-            if isinstance(label_name_token, IdentifierToken)
-            else IdentifierToken(label_name_token)
+    def __eq__(self, other):
+        return (
+            type(self) == type(other)
+            and self.name_token == other.name_token
+            and self.source == other.source
         )
-        self.condition = condition
+
+    def __repr__(self):
+        return f"STORE_GLOBAL({self.name_token}, source={self.source or 'TOS'})"
+
+    def copy(self) -> "AbstractStoreGlobalAssembly":
+        return type(self)(self.name_token, self.source.copy() if self.source else None)
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
-            self,
-            (
-                self.condition.visit_parts(visitor, parents + [self])
-                if self.condition
-                else None,
-            ),
-            parents,
-        )
-
-    def __eq__(self, other):
-        return (
-            type(self) == type(other)
-            and self.label_name_token == other.label_name_token
-            and self.condition == other.condition
-        )
-
-    def __repr__(self):
-        return f"JUMP({self.label_name_token.text}{'' if self.condition is None else ', IF '+repr(self.condition)})"
-
-    def copy(self) -> "AbstractJumpAssembly":
-        return type(self)(
-            self.label_name_token, self.condition.copy() if self.condition else None
+            self, (self.source.visit_parts(visitor, []) if self.source else None,)
         )
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LabelAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LabelAssembly.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,35 +16,37 @@
 @Parser.register
 class LabelAssembly(AbstractAssemblyInstruction):
     # LABEL <name>
     NAME = "LABEL"
 
     @classmethod
     def consume(cls, parser: "Parser", scope: ParsingScope) -> "LabelAssembly":
-        name = parser.try_parse_identifier_like()
+        name = parser.try_parse_jump_target()
 
         if name is None:
             raise throw_positioned_error(
                 scope, parser[0], "expected <identifier like>"
             )
 
         return cls(name)
 
-    def __init__(self, name: IIdentifierAccessor | str):
-        self.name = name if not isinstance(name, str) else StaticIdentifier(name)
+    def __init__(self, name: typing.List[IIdentifierAccessor] | str):
+        self.name = name if not isinstance(name, str) else [StaticIdentifier(e) for e in name.split(":")]
 
     def __repr__(self):
         return f"LABEL({self.name})"
 
     def __eq__(self, other):
         return type(self) == type(other) and self.name == other.name
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        return [Instruction(Opcodes.BYTECODE_LABEL, self.name(scope))]
+        name = ":".join(e(scope) for e in self.name)
+
+        return [Instruction(Opcodes.BYTECODE_LABEL, name)]
 
     def copy(self) -> "LabelAssembly":
         return type(self)(self.name)
 
     def get_labels(self, scope: ParsingScope) -> typing.Set[StaticIdentifier]:
-        return {StaticIdentifier(self.name(scope))}
+        return {StaticIdentifier(":".join(e(scope) for e in self.name))}
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LoadAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LoadAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/MacroAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/MacroAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import traceback
 import typing
 from abc import ABC
 
+from bytecodemanipulation.assembler.util.tokenizer import IntegerToken
 from bytecodemanipulation.MutableFunctionHelpers import capture_local
 
 from bytecodemanipulation.MutableFunctionHelpers import outer_return
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
@@ -101,14 +102,17 @@
             arg_accessor: AbstractAccessExpression | CompoundExpression,
         ) -> bool:
             return True
 
     class CodeBlockDataType(AbstractDataType):
         IDENTIFIER = "CODE_BLOCK"
 
+        def __init__(self, count=0):
+            self.count = count
+
         def is_match(
             self,
             arg: "MacroAssembly.MacroArg",
             arg_accessor: AbstractAccessExpression | CompoundExpression,
         ) -> bool:
             return isinstance(arg_accessor, CompoundExpression)
 
@@ -293,26 +297,43 @@
             )
 
         def add_definition(self, macro: "MacroAssembly", override=False):
             # todo: do a safety check!
             self.assemblies.append(macro)
 
     @classmethod
-    def _try_parse_arg_data_type(cls, parser: "Parser") -> AbstractDataType | None:
+    def _try_parse_arg_data_type(cls, parser: "Parser", scope: ParsingScope) -> AbstractDataType | None:
         if identifier := parser.try_inspect(IdentifierToken):
             if identifier.text == "CODE_BLOCK":
                 parser.consume(identifier)
-                inst = cls.CodeBlockDataType()
+
+                count = 0
+                if opening_bracket := parser.try_consume(SpecialToken("[")):
+                    if not (expr := parser.try_consume(IntegerToken)) or not expr.text.isdigit() or (count := int(expr.text)) < 0:
+                        raise throw_positioned_error(
+                            scope,
+                            [opening_bracket, parser[0]],
+                            "expected <integer> after '[' to declare count",
+                        )
+
+                    if not parser.try_consume(SpecialToken("]")):
+                        raise throw_positioned_error(
+                            scope,
+                            [opening_bracket, parser[0]],
+                            "expected ']' closing '[' in CODE_BLOCK",
+                        )
+
+                inst = cls.CodeBlockDataType(count=count)
                 return inst
 
             elif identifier.text == "VARIABLE_ARG":
                 parser.consume(identifier)
                 # todo: add check that it is the only * arg
                 if parser.try_consume(SpecialToken("[")):
-                    inner_type = cls._try_parse_arg_data_type(parser)
+                    inner_type = cls._try_parse_arg_data_type(parser, scope)
                     if inner_type is None:
                         return
 
                     inst = cls.VariableArgCountDataType(inner_type)
                     parser.consume(SpecialToken("]"))
                 else:
                     inst = cls.VariableArgCountDataType(None)
@@ -346,31 +367,31 @@
                 parameter_name = parser.consume(IdentifierToken)
 
                 arg = MacroAssembly.MacroArg(parameter_name, is_static)
                 arg.index = i
                 i += 1
                 args.append(arg)
 
-                data_type = cls._try_parse_arg_data_type(parser)
+                data_type = cls._try_parse_arg_data_type(parser, scope)
 
                 parser.save()
                 if data_type is not None:
                     arg.data_type_annotation = data_type
                     parser.discard_save()
                 else:
                     parser.rollback()
 
                 if not parser.try_consume(SpecialToken(",")):
-                    parser.consume(SpecialToken(")"))
+                    parser.consume(SpecialToken(")"), err_arg=scope)
                     break
 
         if parser.try_consume(SpecialToken("-")):
             parser.consume(SpecialToken(">"), err_arg=scope)
 
-            return_type = cls._try_parse_arg_data_type(parser)
+            return_type = cls._try_parse_arg_data_type(parser, scope)
         else:
             return_type = None
 
         body = parser.parse_body(scope=scope)
 
         return cls(
             name,
@@ -435,18 +456,28 @@
     ) -> typing.List[Instruction]:
         if len(args) != len(self.args):
             raise RuntimeError("Argument count must be equal!")
 
         scope = scope.copy()
         scope.scope_path = self.scope_path
         scope.module_file = self.module_path
+        scope.current_macro_assembly = self
 
         bytecode = []
 
         for arg_decl, arg_code in zip(self.args, args):
+            if isinstance(arg_decl.data_type_annotation, MacroAssembly.CodeBlockDataType):
+                if isinstance(arg_code, CompoundExpression) and hasattr(arg_code, "to_be_stored_at"):
+                    if len(arg_code.to_be_stored_at) != arg_decl.data_type_annotation.count:
+                        raise throw_positioned_error(
+                            scope,
+                            arg_decl.name,
+                            f"Expected {arg_decl.data_type_annotation.count} dynamic name entries, got {len(arg_code.to_be_stored_at)}"
+                        )
+
             if arg_decl.is_static:
                 scope.macro_parameter_namespace[arg_decl.name.text] = arg_decl.name.text
             else:
                 scope.macro_parameter_namespace[arg_decl.name.text] = arg_code
 
         inner_bytecode = self.body.emit_bytecodes(function, scope)
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,86 +1,91 @@
 import typing
 
-from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
+from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.Lexer import SpecialToken
-from bytecodemanipulation.assembler.Parser import Parser
+from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
+from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
+    CompoundExpression,
+)
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
-class MacroPasteAssembly(AbstractAssemblyInstruction):
-    # MACRO_PASTE <macro param name> ['->' <target>]
-    NAME = "MACRO_PASTE"
+if typing.TYPE_CHECKING:
+    from bytecodemanipulation.assembler.Parser import Parser
+
+
+class NamespaceAssembly(AbstractAssemblyInstruction):
+    # 'NAMESPACE' [{<namespace> ':'}] <name> '{' <code> '}'
+    NAME = "NAMESPACE"
 
     @classmethod
     def register(cls):
+        from bytecodemanipulation.assembler.Parser import Parser
+
         Parser.register(cls)
 
     @classmethod
-    def consume(cls, parser: "Parser", scope) -> "MacroPasteAssembly":
-        # Parse an optional § infront of the name
-        parser.try_consume(SpecialToken("&"))
-
-        name = parser.consume(IdentifierToken)
-
-        if parser.try_consume_multi([SpecialToken("-"), SpecialToken(">")]):
-            target = parser.try_consume_access_to_value(
-                allow_primitives=False, scope=scope
-            )
-        else:
-            target = None
+    def consume(cls, parser: "Parser", scope: ParsingScope) -> "NamespaceAssembly":
+        name = [parser.consume(IdentifierToken)]
+
+        while parser.try_consume(SpecialToken(":")):
+            name.append(parser.consume(IdentifierToken))
 
-        return cls(name, target)
+        assembly = parser.parse_body(namespace_part=[e.text for e in name], scope=scope)
 
-    def __init__(self, name: IdentifierToken, target: AbstractAccessExpression = None):
+        return cls(
+            name,
+            assembly,
+        )
+
+    def __init__(
+        self, name: typing.List[IdentifierToken], assembly: CompoundExpression
+    ):
         self.name = name
-        self.target = target
+        self.assembly = assembly
 
     def __repr__(self):
-        return f"MACRO_PASTE({self.name.text}{'' if self.target is None else '-> '+repr(self.target)})"
+        return (
+            f"NAMESPACE::'{':'.join(e.text for e in self.name)}'({repr(self.assembly)})"
+        )
 
     def __eq__(self, other):
         return (
-            type(self) == type(other)
+            type(self) is type(other)
             and self.name == other.name
-            and self.target == other.target
+            and self.assembly == other.assembly
         )
 
-    def copy(self) -> "MacroPasteAssembly":
-        return type(self)(self.name, self.target.copy() if self.target else None)
+    def copy(self):
+        return type(self)(self.name, self.assembly.copy())
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        if self.name.text in scope.macro_parameter_namespace and hasattr(
-            scope.macro_parameter_namespace[self.name.text], "emit_bytecodes"
-        ):
-            instructions = scope.macro_parameter_namespace[self.name.text].emit_bytecodes(
-                function, scope
-            )
-
-            for instr in instructions:
-                if instr.has_local():
-                    if instr.arg_value.startswith("|"):
-                        instr.change_arg_value(instr.arg_value[1:])
-                    else:
-                        instr.change_arg_value(":" + instr.arg_value)
-
-            return instructions + (
-                []
-                if self.target is None
-                else self.target.emit_store_bytecodes(function, scope)
-            )
-
-        return [
-            Instruction(Opcodes.MACRO_PARAMETER_EXPANSION, self.name.text)
-        ] + (
-            []
-            if self.target is None
-            else self.target.emit_store_bytecodes(function, scope)
+        return self.assembly.emit_bytecodes(
+            function, scope.copy(sub_scope_name=[e.text for e in self.name])
+        )
+
+    def visit_parts(
+        self,
+        visitor: typing.Callable[
+            [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
+            typing.Any,
+        ],
+        parents: list,
+    ):
+        return visitor(
+            self,
+            (
+                self.assembly.visit_parts(
+                    visitor,
+                    parents + [self],
+                ),
+            ),
+            parents,
         )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,91 +1,68 @@
+import abc
 import typing
 
+from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
-from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.Lexer import SpecialToken
+from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
+from bytecodemanipulation.assembler.util.tokenizer import IntegerToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
-from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
-    CompoundExpression,
-)
-from bytecodemanipulation.opcodes.Instruction import Instruction
-from bytecodemanipulation.MutableFunction import MutableFunction
-
-
-if typing.TYPE_CHECKING:
-    from bytecodemanipulation.assembler.Parser import Parser
 
 
-class NamespaceAssembly(AbstractAssemblyInstruction):
-    # 'NAMESPACE' [{<namespace> ':'}] <name> '{' <code> '}'
-    NAME = "NAMESPACE"
-
-    @classmethod
-    def register(cls):
-        from bytecodemanipulation.assembler.Parser import Parser
+class AbstractStoreFastAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # STORE_FAST <name> [<source>]
+    NAME = "STORE_FAST"
 
-        Parser.register(cls)
+    def __init__(
+        self,
+        name_token: IdentifierToken | IntegerToken | str | int,
+        source: AbstractSourceExpression | None = None,
+    ):
+        self.name_token = (
+            name_token
+            if not isinstance(name_token, (str, int))
+            else (
+                IdentifierToken(name_token)
+                if isinstance(name_token, str)
+                else IntegerToken(str(name_token))
+            )
+        )
+        self.source = source
 
     @classmethod
-    def consume(cls, parser: "Parser", scope: ParsingScope) -> "NamespaceAssembly":
-        name = [parser.consume(IdentifierToken)]
-
-        while parser.try_consume(SpecialToken(":")):
-            name.append(parser.consume(IdentifierToken))
+    def consume(cls, parser: "Parser", scope) -> "AbstractStoreFastAssembly":
+        parser.try_consume(SpecialToken("$"))
+        name = parser.consume([IdentifierToken, IntegerToken])
 
-        assembly = parser.parse_body(namespace_part=[e.text for e in name], scope=scope)
+        source = parser.try_parse_data_source()
 
-        return cls(
-            name,
-            assembly,
-        )
-
-    def __init__(
-        self, name: typing.List[IdentifierToken], assembly: CompoundExpression
-    ):
-        self.name = name
-        self.assembly = assembly
-
-    def __repr__(self):
-        return (
-            f"NAMESPACE::'{':'.join(e.text for e in self.name)}'({repr(self.assembly)})"
-        )
+        return cls(name, source)
 
     def __eq__(self, other):
         return (
-            type(self) is type(other)
-            and self.name == other.name
-            and self.assembly == other.assembly
+            type(self) == type(other)
+            and self.name_token == other.name_token
+            and self.source == other.source
         )
 
-    def copy(self):
-        return type(self)(self.name, self.assembly.copy())
+    def __repr__(self):
+        return f"STORE_FAST({self.name_token}, source={self.source or 'TOS'})"
 
-    def emit_bytecodes(
-        self, function: MutableFunction, scope: ParsingScope
-    ) -> typing.List[Instruction]:
-        return self.assembly.emit_bytecodes(
-            function, scope.copy(sub_scope_name=[e.text for e in self.name])
-        )
+    def copy(self) -> "AbstractStoreFastAssembly":
+        return type(self)(self.name, self.source.copy() if self.source else None)
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
-            self,
-            (
-                self.assembly.visit_parts(
-                    visitor,
-                    parents + [self],
-                ),
-            ),
-            parents,
+            self, (self.source.visit_parts(visitor) if self.target else None,)
         )
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/OpAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/OpAssembly.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typing
 import abc
 import typing
 from collections import namedtuple
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
+from bytecodemanipulation.assembler.target import assembly
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
@@ -27,14 +28,17 @@
         self,
         function: MutableFunction,
         scope: ParsingScope,
         *parameters: AbstractSourceExpression,
     ) -> typing.List[Instruction]:
         raise NotImplementedError
 
+    def evaluate_static_value(self, scope: ParsingScope, *parameters: AbstractSourceExpression):
+        raise NotImplementedError
+
 
 OperatorArgValue = namedtuple("OperatorArgValue", "index")
 
 
 class OpcodeBaseOperator(AbstractOperator):
     def __init__(
         self,
@@ -45,16 +49,18 @@
             int | str,
             typing.Callable[
                 [MutableFunction, ParsingScope, typing.List[AbstractSourceExpression]],
                 typing.Any,
             ],
         ]
         | OperatorArgValue,
+        static_eval: typing.Callable[[ParsingScope, typing.List[AbstractSourceExpression]], typing.Any] = None
     ):
         self.opcodes = opcodes
+        self.static_eval = static_eval
 
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         *parameters: AbstractSourceExpression,
     ) -> typing.List[Instruction]:
@@ -83,14 +89,20 @@
             elif hasattr(opcode, "emit_bytecodes"):
                 bytecode += opcode.emit_bytecodes(function, scope)
             else:
                 raise ValueError(opcode)
 
         return bytecode
 
+    def evaluate_static_value(self, scope: ParsingScope, *parameters: AbstractSourceExpression):
+        if not self.static_eval:
+            raise NotImplementedError
+
+        return self.static_eval(scope, list(parameters))
+
 
 class AbstractOpAssembly(
     AbstractAssemblyInstruction, AbstractAccessExpression, abc.ABC
 ):
     """
     OP ... [-> <target>]
     - <expr> +|-|*|/|//|**|%|&|"|"|^|>>|<<|@|is|!is|in|!in|<|<=|==|!=|>|>=|xor|!xor|:=|isinstance|issubclass|hasattr|getattr <expr>
@@ -135,14 +147,17 @@
 
         def __eq__(self, other):
             raise NotImplementedError
 
         def __repr__(self):
             raise NotImplementedError
 
+        def evaluate_static_value(self, scope: ParsingScope):
+            raise NotImplementedError
+
     class SingleOperation(IOperation):
         def __init__(
             self,
             operator: str,
             operator_token: typing.List[AbstractToken],
             expression: AbstractSourceExpression,
             base: typing.Type["AbstractOpAssembly"] = None,
@@ -177,14 +192,17 @@
             except:
                 raise throw_positioned_error(
                     scope,
                     self.operator_token,
                     "during emitting bytecode of singleton operator",
                 )
 
+        def evaluate_static_value(self, scope: ParsingScope):
+            return self.base.SINGLE_OPS[self.operator].evaluate_static_value(scope, self.expression)
+
         def visit_parts(
             self,
             visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any],
             parents: list,
         ):
             return visitor(
                 self,
@@ -245,14 +263,17 @@
             except:
                 raise throw_positioned_error(
                     scope,
                     self.operator_token,
                     "during emitting bytecode of binary operation",
                 )
 
+        def evaluate_static_value(self, scope: ParsingScope):
+            return self.base.BINARY_OPS[self.operator].evaluate_static_value(scope, self.lhs, self.rhs)
+
         def visit_parts(
             self,
             visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any],
             parents: list,
         ):
             return visitor(
                 self,
@@ -300,21 +321,26 @@
         def emit_bytecodes(
             self, function: MutableFunction, scope: ParsingScope
         ) -> typing.List[Instruction]:
             try:
                 return self.base.PREFIX_OPERATORS[self.operator][0].emit_bytecodes(
                     function, scope, *self.args
                 )
+            except SyntaxError:
+                raise
             except:
                 raise throw_positioned_error(
                     scope,
                     self.operator_token,
                     "during emitting bytecode of binary operation",
                 )
 
+        def evaluate_static_value(self, scope: ParsingScope):
+            return self.base.PREFIX_OPERATORS[self.operator][0].evaluate_static_value(scope, *self.args)
+
         def visit_parts(
             self,
             visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any],
             parents: list,
         ):
             return visitor(
                 self,
@@ -562,14 +588,17 @@
         )
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         raise RuntimeError(f"cannot assign to an '{self.operation}' operator!")
 
+    def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
+        return self.operation.evaluate_static_value(scope)
+
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/RawAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/RawAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/StoreAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/StoreAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/YieldAssembly.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,92 @@
 import abc
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
-from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
-from bytecodemanipulation.assembler.util.tokenizer import IntegerToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 
 
-class AbstractStoreFastAssembly(AbstractAssemblyInstruction, abc.ABC):
-    # STORE_FAST <name> [<source>]
-    NAME = "STORE_FAST"
+class AbstractYieldAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # YIELD [*] [<expr>] [-> <target>]
+    NAME = "YIELD"
 
     def __init__(
         self,
-        name_token: IdentifierToken | IntegerToken | str | int,
-        source: AbstractSourceExpression | None = None,
+        expr: AbstractSourceExpression | None = None,
+        is_star: bool = False,
+        target: AbstractSourceExpression | None = None,
     ):
-        self.name_token = (
-            name_token
-            if not isinstance(name_token, (str, int))
-            else (
-                IdentifierToken(name_token)
-                if isinstance(name_token, str)
-                else IntegerToken(str(name_token))
-            )
-        )
-        self.source = source
+        self.expr = expr
+        self.is_star = is_star
+        self.target = target
 
     @classmethod
-    def consume(cls, parser: "Parser", scope) -> "AbstractStoreFastAssembly":
-        parser.try_consume(SpecialToken("$"))
-        name = parser.consume([IdentifierToken, IntegerToken])
+    def consume(cls, parser: "Parser", scope) -> "AbstractYieldAssembly":
+        is_star = bool(parser.try_consume(SpecialToken("*")))
 
-        source = parser.try_parse_data_source()
+        expr = parser.try_parse_data_source(
+            allow_primitives=True, allow_op=True, include_bracket=False
+        )
 
-        return cls(name, source)
+        if parser.try_consume(SpecialToken("-")) and parser.try_consume(
+            SpecialToken(">")
+        ):
+            target = parser.try_parse_data_source(
+                allow_primitives=True, allow_op=True, include_bracket=False
+            )
 
-    def __eq__(self, other):
-        return (
-            type(self) == type(other)
-            and self.name_token == other.name_token
-            and self.source == other.source
-        )
+            if target is None:
+                raise throw_positioned_error(
+                    scope, parser.try_inspect(), "expected <expression>"
+                )
 
-    def __repr__(self):
-        return f"STORE_FAST({self.name_token}, source={self.source or 'TOS'})"
+        else:
+            target = None
 
-    def copy(self) -> "AbstractStoreFastAssembly":
-        return type(self)(self.name, self.source.copy() if self.source else None)
+        return cls(expr, is_star, target)
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
-            self, (self.source.visit_parts(visitor) if self.target else None,)
+            self,
+            (
+                self.expr.visit_parts(visitor, parents + [self]) if self.expr else None,
+                self.target.visit_parts(
+                    visitor,
+                    parents + [self],
+                )
+                if self.target
+                else None,
+            ),
+            parents,
+        )
+
+    def __eq__(self, other):
+        return (
+            type(self) == type(other)
+            and self.expr == other.expr
+            and self.is_star == other.is_star
+            and self.target == other.target
+        )
+
+    def __repr__(self):
+        return f"YIELD{'' if not self.is_star else '*'}({self.expr if self.expr else ''}{(', ' if self.expr else '->') + repr(self.target) if self.target else ''})"
+
+    def copy(self) -> "AbstractYieldAssembly":
+        return type(self)(
+            self.expr.copy() if self.expr else None,
+            self.is_star,
+            self.target.copy() if self.target else None,
         )
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/JumpAssembly.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,98 @@
 import abc
 import typing
 
-from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
+from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
+from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
+from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
-from bytecodemanipulation.assembler.util.tokenizer import IntegerToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
+from bytecodemanipulation.data.shared.instructions.OpAssembly import AbstractOpAssembly
 
 
-class AbstractStoreGlobalAssembly(AbstractAssemblyInstruction, abc.ABC):
-    # STORE_GLOBAL <name> [<source>]
-    NAME = "STORE_GLOBAL"
+class AbstractJumpAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # JUMP <label name> ['IF' <expression>]
 
-    def __init__(
-        self,
-        name_token: IdentifierToken | IntegerToken | str | int,
-        source: AbstractSourceExpression | None = None,
-    ):
-        self.name_token = (
-            name_token
-            if not isinstance(name_token, (str, int))
-            else (
-                IdentifierToken(name_token)
-                if isinstance(name_token, str)
-                else IntegerToken(str(name_token))
-            )
-        )
-        self.source = source
+    NAME = "JUMP"
 
     @classmethod
-    def consume(cls, parser: "Parser", scope) -> "AbstractStoreGlobalAssembly":
-        parser.try_consume(SpecialToken("@"))
-        name = parser.try_consume([IdentifierToken, IntegerToken])
-
-        if name is None:
-            raise throw_positioned_error(
-                scope, parser.try_inspect(), "expected <name> or <integer>"
+    def consume(cls, parser: "Parser", scope) -> "AbstractJumpAssembly":
+        has_quotes = parser.try_consume(SpecialToken("'"))
+
+        label_target = parser.parse_jump_target(scope)
+
+        if has_quotes:
+            parser.consume(SpecialToken("'"))
+
+        if parser.try_consume(IdentifierToken("IF")):
+            condition = parser.try_parse_data_source(
+                allow_primitives=True, include_bracket=False, allow_op=True
             )
 
-        source = parser.try_parse_data_source()
+        elif parser.try_consume(SpecialToken("(")):
+            parser.save()
+            condition = parser.try_parse_data_source(
+                allow_primitives=True, include_bracket=False, allow_op=True
+            )
 
-        return cls(name, source)
+            if condition is None or not parser.try_consume(SpecialToken(")")):
+                parser.rollback()
+                condition = AbstractOpAssembly.IMPLEMENTATION.consume(parser, None)
+                parser.consume(SpecialToken(")"))
+            else:
+                parser.discard_save()
 
-    def __eq__(self, other):
-        return (
-            type(self) == type(other)
-            and self.name_token == other.name_token
-            and self.source == other.source
-        )
+        else:
+            condition = None
 
-    def __repr__(self):
-        return f"STORE_GLOBAL({self.name_token}, source={self.source or 'TOS'})"
+        return cls(label_target, condition)
 
-    def copy(self) -> "AbstractStoreGlobalAssembly":
-        return type(self)(self.name_token, self.source.copy() if self.source else None)
+    def __init__(
+        self,
+        label_name_token: typing.List[IIdentifierAccessor] | str,
+        condition: AbstractAccessExpression | None = None,
+    ):
+        self.label_name_token = (
+            label_name_token
+            if not isinstance(label_name_token, str)
+            else [StaticIdentifier(e) for e in label_name_token.split(":")]
+        )
+        self.condition = condition
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
-            self, (self.source.visit_parts(visitor, []) if self.source else None,)
+            self,
+            (
+                self.condition.visit_parts(visitor, parents + [self])
+                if self.condition
+                else None,
+            ),
+            parents,
+        )
+
+    def __eq__(self, other):
+        return (
+            type(self) == type(other)
+            and self.label_name_token == other.label_name_token
+            and self.condition == other.condition
+        )
+
+    def __repr__(self):
+        return f"JUMP({':'.join(map(repr, self.label_name_token))}{'' if self.condition is None else ', IF '+repr(self.condition)})"
+
+    def copy(self) -> "AbstractJumpAssembly":
+        return type(self)(
+            self.label_name_token.copy(), self.condition.copy() if self.condition else None
         )
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/WhileAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/IfAssembly.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,104 +6,112 @@
 from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
-from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
     CompoundExpression,
 )
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 
 
-class AbstractWhileAssembly(AbstractAssemblyInstruction, abc.ABC):
-    # # WHILE <expression> ['\'' <label name> '\''] '{' <body> '}'
-    NAME = "WHILE"
+class AbstractIFAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # IF <expression> ['\'' <label name> '\''] '{' <body> '}'
+    NAME = "IF"
 
     @classmethod
-    def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractWhileAssembly":
-        condition = parser.try_parse_data_source(
+    def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractIFAssembly":
+        source = parser.try_parse_data_source(
             allow_primitives=True, include_bracket=False, scope=scope
         )
 
-        if condition is None:
+        if source is None:
             raise throw_positioned_error(
                 scope, parser.try_inspect(), "expected <expression>"
             )
 
         if parser.try_consume(SpecialToken("'")):
-            label_name = parser.parse_identifier_like(scope)
+            label_name = parser.parse_jump_target(scope)
+
             if not parser.try_consume(SpecialToken("'")):
                 raise throw_positioned_error(
-                    scope, parser.try_inspect(), "expected '"
+                    scope, parser.try_inspect(), "expected ' after label name declaration"
                 )
+
         else:
             label_name = None
 
         body = parser.parse_body(scope=scope)
 
         return cls(
-            condition,
+            source,
             body,
             label_name,
         )
 
     def __init__(
         self,
         source: AbstractSourceExpression,
         body: CompoundExpression,
-        label_name: IIdentifierAccessor | None = None,
+        label_name: typing.List[IIdentifierAccessor] | str = None,
     ):
         self.source = source
         self.body = body
         self.label_name = (
             label_name
             if not isinstance(label_name, str)
-            else StaticIdentifier(label_name)
-        )
+            else [StaticIdentifier(e) for e in label_name.split(":")]
+        ) if label_name is not None else None
 
     def copy(self):
-        return type(self)(self.source.copy(), self.body.copy(), self.label_name)
+        return type(self)(self.source.copy(), self.body.copy(), self.label_name.copy())
 
     def __eq__(self, other):
         return (
             type(self) == type(other)
             and self.source == other.source
             and self.body == other.body
             and self.label_name == other.label_name
         )
 
     def __repr__(self):
-        c = "'"
-        return f"WHILE({self.source}{'' if self.label_name is None else ', label='+c+repr(self.label_name)+c}) -> {{{self.body}}}"
+        c = '"'
+        return f"IF({self.source}{'' if self.label_name is None else ', label='+c+':'.join(map(repr, self.label_name))+c}) -> {{{self.body}}}"
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
-            self, (self.source.visit_parts(visitor), self.body.visit_parts(visitor))
+            self,
+            (
+                self.source.visit_parts(visitor, parents + [self]),
+                self.body.visit_parts(visitor, parents + [self]),
+            ),
+            parents,
         )
 
     def visit_assembly_instructions(
         self, visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any]
     ):
         return visitor(self, (self.body.visit_assembly_instructions(visitor),))
 
-    def get_labels(self, scope: ParsingScope):
+    def get_labels(self, scope: ParsingScope) -> typing.Set[str]:
+        label_name = ":".join(e(scope) for e in self.label_name) if self.label_name is not None else None
+
         return (
             set()
             if self.label_name is None
             else {
-                self.label_name(scope),
-                self.label_name(scope) + "_END",
-                self.label_name(scope) + "_INNER",
+                label_name,
+                label_name + ":END",
+                label_name + ":HEAD",
             }
         ) | self.body.get_labels(scope)
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/ExceptionInstructionCodec.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/ExceptionInstructionCodec.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/LocationInformationHandler.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/LocationInformationHandler.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/assembly_instructions.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/assembly_instructions.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,15 @@
+import functools
+import inspect
 import typing
 
+from bytecodemanipulation.assembler.AbstractBase import MacroExpandedIdentifier
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.data.shared.expressions.LocalAccessExpression import LocalAccessExpression
+from bytecodemanipulation.data.shared.expressions.MacroParameterAcessExpression import MacroParameterAccessExpression
 from bytecodemanipulation.data.shared.instructions.FunctionDefinitionAssembly import (
     AbstractFunctionDefinitionAssembly,
 )
 from bytecodemanipulation.data.v3_10.instructions.CallAssembly import CallAssembly
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
 from bytecodemanipulation.assembler.Parser import Parser
@@ -47,19 +53,22 @@
             tar = lambda: None
 
         target = MutableFunction(tar)
         inner_bytecode = []
 
         if self.bound_variables:
             for name, is_static in self.bound_variables:
-                # print(name, name(scope), is_static)
-                inner_bytecode += [
-                    Instruction(Opcodes.LOAD_DEREF, name(scope) + "%inner"),
-                    Instruction(Opcodes.STORE_DEREF, name(scope)),
-                ]
+                scope.closure_locals.add(name(scope))
+
+        local_variable_buffer = scope.scope_name_generator("outer_locals")
+
+        target.argument_count = len(self.args)
+        if self.bound_variables:
+            target.argument_names.insert(0, local_variable_buffer)
+            target.argument_count += 1
 
         inner_bytecode += self.body.emit_bytecodes(target, inner_scope)
         inner_bytecode[-1].next_instruction = target.instruction_entry_point
 
         for i, instr in enumerate(inner_bytecode[:-1]):
             instr.next_instruction = inner_bytecode[i + 1]
 
@@ -71,14 +80,39 @@
                     if instruction.next_instruction is not None
                     else instruction
                 )
                 instruction.change_opcode(Opcodes.NOP)
 
         inner_bytecode[0].apply_visitor(LambdaInstructionWalker(walk_label))
 
+        def rewrite_outer_access(instruction: Instruction):
+            if instruction.opcode == Opcodes.LOAD_DEREF and instruction.arg_value in scope.closure_locals:
+                instruction.insert_after([
+                    Instruction(Opcodes.LOAD_FAST, local_variable_buffer),
+                    Instruction(Opcodes.LOAD_CONST, instruction.arg_value),
+                    Instruction(Opcodes.BINARY_SUBSCR),
+                ])
+                instruction.change_opcode(Opcodes.NOP)
+            elif instruction.opcode == Opcodes.STORE_DEREF and instruction.arg_value in scope.closure_locals:
+                instruction.insert_after([
+                    Instruction(Opcodes.LOAD_FAST, local_variable_buffer),
+                    Instruction(Opcodes.LOAD_CONST, instruction.arg_value),
+                    Instruction(Opcodes.STORE_SUBSCR),
+                ])
+                instruction.change_opcode(Opcodes.NOP)
+            elif instruction.opcode == Opcodes.DELETE_DEREF and instruction.arg_value in scope.closure_locals:
+                instruction.insert_after([
+                    Instruction(Opcodes.LOAD_FAST, local_variable_buffer),
+                    Instruction(Opcodes.LOAD_CONST, instruction.arg_value),
+                    Instruction(Opcodes.DELETE_SUBSCR),
+                ])
+                instruction.change_opcode(Opcodes.NOP)
+
+        inner_bytecode[0].apply_visitor(LambdaInstructionWalker(rewrite_outer_access))
+
         def resolve_jump_to_label(ins: Instruction):
             if ins.has_jump() and isinstance(ins.arg_value, JumpToLabel):
                 ins.change_arg_value(label_targets[ins.arg_value.name])
 
         inner_bytecode[0].apply_visitor(LambdaInstructionWalker(resolve_jump_to_label))
 
         target.instruction_entry_point = inner_bytecode[0]
@@ -103,43 +137,18 @@
 
             defaults += [
                 Instruction(Opcodes.BUILD_TUPLE, arg=c),
             ]
 
             bytecode += defaults
 
-        if self.bound_variables:
-            if any(map(lambda e: e[1], self.bound_variables)):
-                raise NotImplementedError("Static variables")
-
-            flags |= 0x08
-
-            for name, is_static in self.bound_variables:
-                bytecode += [
-                    Instruction(Opcodes.LOAD_FAST, name(scope)),
-                    Instruction(
-                        Opcodes.STORE_DEREF, name(scope) + "%inner"
-                    ),
-                ]
-
-            bytecode += [
-                Instruction(Opcodes.LOAD_CLOSURE, name(scope) + "%inner")
-                for name, is_static in self.bound_variables
-            ]
-            bytecode.append(
-                Instruction(
-                    Opcodes.BUILD_TUPLE, arg=len(self.bound_variables)
-                )
-            )
-
-        target.argument_count = len(self.args)
-
         for arg in self.args:
             if isinstance(arg, CallAssembly.Arg):
                 target.argument_names.append(arg.source(scope))
+
             elif isinstance(arg, CallAssembly.KwArg):
                 target.argument_names.append(arg.key(scope))
 
         target.prepare_previous_instructions()
         code_object = target.create_code_obj()
 
         bytecode += [
@@ -147,15 +156,33 @@
             Instruction(
                 Opcodes.LOAD_CONST,
                 self.func_name(scope) if self.func_name else "<lambda>",
             ),
             Instruction(Opcodes.MAKE_FUNCTION, arg=flags),
         ]
 
+        if self.bound_variables:
+            # <function> = functools.partial(<function>, <bound local dict>)
+
+            bytecode += [
+                Instruction(Opcodes.LOAD_CONST, functools.partial),
+                Instruction(Opcodes.ROT_TWO),
+                Instruction(Opcodes.LOAD_CONST, inspect.currentframe),
+                Instruction(Opcodes.CALL_FUNCTION, arg=0),
+                Instruction(Opcodes.LOAD_ATTR, "f_locals"),
+                Instruction(Opcodes.CALL_FUNCTION, arg=2),
+            ]
+
         if self.target:
             bytecode += self.target.emit_store_bytecodes(function, scope)
+        elif not self.func_name:
+            raise throw_positioned_error(
+                scope,
+                [],
+                "Expected either 'target' or <valid name>",
+            )
         else:
             bytecode += [
                 Instruction(Opcodes.STORE_FAST, self.prefix + self.func_name(scope)),
             ]
 
         return bytecode
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,43 @@
+import typing
+
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.data.shared.instructions.IfAssembly import AbstractIFAssembly
+from bytecodemanipulation.data.shared.instructions.YieldAssembly import (
+    AbstractYieldAssembly,
+)
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
-class IFAssembly(AbstractIFAssembly):
-    def emit_bytecodes(self, function: MutableFunction, scope: ParsingScope):
+class YieldAssembly(AbstractYieldAssembly):
+    def emit_bytecodes(
+        self, function: MutableFunction, scope: ParsingScope
+    ) -> typing.List[Instruction]:
+        bytecode = []
+
+        if self.expr:
+            bytecode += self.expr.emit_bytecodes(function, scope)
+
+        if self.is_star:
+            bytecode += [
+                Instruction(Opcodes.GET_YIELD_FROM_ITER),
+                Instruction(Opcodes.LOAD_CONST, None),
+                Instruction(Opcodes.YIELD_FROM),
+            ]
+
+        else:
+            bytecode += [
+                Instruction(Opcodes.YIELD_VALUE),
+            ]
+
+        if self.target:
+            bytecode += self.target.emit_store_bytecodes(function, scope)
 
-        if self.label_name is None:
-            end = Instruction(Opcodes.NOP)
         else:
-            end = Instruction(
-                Opcodes.BYTECODE_LABEL, self.label_name.text + "_END"
-            )
-
-        return (
-            (
-                []
-                if self.label_name is None
-                else [
-                    Instruction(
-                        Opcodes.BYTECODE_LABEL,
-                        self.label_name.text + "_HEAD",
-                    )
-                ]
-            )
-            + self.source.emit_bytecodes(function, scope)
-            + [Instruction("POP_JUMP_IF_FALSE", end)]
-            + (
-                []
-                if self.label_name is None
-                else [
-                    Instruction(
-                        Opcodes.BYTECODE_LABEL, self.label_name.text
-                    )
-                ]
-            )
-            + self.body.emit_bytecodes(function, scope)
-            + [end]
-        )
+            bytecode += [Instruction(Opcodes.POP_TOP)]
+
+        # print(bytecode)
+
+        return bytecode
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/JumpAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/assembly_instructions.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/assembly_instructions.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/CallAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/CallAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/ClassDefinitionAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/ClassDefinitionAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 @Parser.register
 class ClassDefinitionAssembly(AbstractClassDefinitionAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        inner_scope = scope.copy(sub_scope_name=self.name(scope))
+        inner_scope = scope.copy(sub_scope_name=self.name(scope), shared_locals=False)
 
         target = MutableFunction(lambda: None)
 
         inner_bytecode = [
             Instruction(Opcodes.LOAD_NAME, "__name__"),
             Instruction(Opcodes.STORE_NAME, "__module__"),
             Instruction(Opcodes.LOAD_CONST, self.name(scope)),
@@ -35,20 +35,20 @@
                 instr.change_opcode(Opcodes.STORE_NAME, arg_value=instr.arg_value)
             elif instr.opcode == Opcodes.DELETE_FAST:
                 instr.change_opcode(Opcodes.DELETE_NAME, arg_value=instr.arg_value)
 
         inner_bytecode += raw_inner_code
 
         if inner_bytecode:
-            inner_bytecode[-1].next_instruction = target.instructions[0]
+            inner_bytecode[-1].next_instruction = target.instruction_entry_point
 
         for i, instr in enumerate(inner_bytecode[:-1]):
             instr.next_instruction = inner_bytecode[i + 1]
 
-        target.assemble_instructions_from_tree(inner_bytecode[0])
+        target.instruction_entry_point = inner_bytecode[0]
         target.reassign_to_function()
 
         code_obj = target.target.__code__
 
         bytecode = [
             Instruction(Opcodes.LOAD_BUILD_CLASS),
             Instruction(Opcodes.LOAD_CONST, code_obj),
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,18 @@
             bytecode.append(
                 Instruction(
                     function, -1, Opcodes.BUILD_TUPLE, arg=len(self.bound_variables)
                 )
             )
 
         target.argument_count = len(self.args)
+
+        if self.bound_variables:
+            target.argument_count += 1
+
         code_object = target.create_code_obj()
 
         bytecode += [
             Instruction("LOAD_CONST", code_object),
             Instruction(
                 function,
                 -1,
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/IfAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/IfAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/JumpAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,26 +14,28 @@
 @Parser.register
 class JumpAssembly(AbstractJumpAssembly):
     # JUMP <label name> [(IF <condition access>) | ('(' <expression> | <op expression> ')')]
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        if not scope.exists_label(self.label_name_token.text):
+        label_name = ":".join(e(scope) for e in self.label_name_token)
+
+        if not scope.exists_label(label_name):
             raise ValueError(
-                f"Label '{self.label_name_token.text}' is not valid in this context!"
+                f"Label '{label_name}' is not valid in this context!"
             )
 
         if self.condition is None:
             return [
                 Instruction(
                     Opcodes.JUMP_ABSOLUTE,
-                    JumpToLabel(self.label_name_token.text),
+                    JumpToLabel(label_name),
                 )
             ]
 
         return self.condition.emit_bytecodes(function, scope) + [
             Instruction(
                 Opcodes.POP_JUMP_IF_TRUE,
-                JumpToLabel(self.label_name_token.text),
+                JumpToLabel(label_name),
             )
         ]
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/LoadFastAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/LoadFastAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/LoadGlobalAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/LoadGlobalAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,40 +7,40 @@
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class WHILEAssembly(AbstractWhileAssembly):
     def emit_bytecodes(self, function: MutableFunction, scope: ParsingScope):
+        name = ":".join(e(scope) for e in self.label_name) if self.label_name is not None else None
+
         if self.label_name is None:
-            end = Instruction("NOP")
+            end = Instruction(Opcodes.NOP)
         else:
             end = Instruction(
-                function, -1, Opcodes.BYTECODE_LABEL, self.label_name.text + "_END"
+                Opcodes.BYTECODE_LABEL, name + ":END"
             )
 
         CONDITION = self.source.emit_bytecodes(function, scope)
 
         if self.label_name:
             CONDITION.insert(
                 0,
-                Instruction(Opcodes.BYTECODE_LABEL, self.label_name.text),
+                Instruction(Opcodes.BYTECODE_LABEL, name),
             )
 
         HEAD = Instruction("POP_JUMP_IF_FALSE", end)
 
         BODY = self.body.emit_bytecodes(function, scope)
 
         if self.label_name:
             BODY.insert(
                 0,
                 Instruction(
-                    function,
-                    -1,
                     Opcodes.BYTECODE_LABEL,
-                    self.label_name.text + "_INNER",
+                    name + ":INNER",
                 ),
             )
 
         JUMP_BACK = Instruction("JUMP_ABSOLUTE", CONDITION[0])
 
         return CONDITION + [HEAD] + BODY + [JUMP_BACK, end]
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/data_loader.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/data_loader.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/mixin_util.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/mixin_util.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/AbstractOpcodeTransformerStage.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/AbstractOpcodeTransformerStage.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,17 @@
                 cls.visit(
                     function,
                     metadata,
                     instr,
                 )
             except StopIteration:
                 return
+            except:
+                print(instr)
+                raise
 
             if not instr.has_stop_flow() and not instr.has_unconditional_jump():
                 visiting.add(instr.next_instruction)
 
             if instr.has_jump():
                 visiting.add(instr.arg_value)
 
@@ -136,15 +139,18 @@
     @classmethod
     def visit(cls, function: "MutableFunction", builder: CodeObjectBuilder, target: "Instruction") -> typing.Any:
         if target.has_local():
             target.arg = builder.reserve_local_name(target.arg_value)
         elif target.has_name():
             target.arg = builder.reserve_name(target.arg_value)
         elif target.has_cell_variable():
-            target.arg = builder.reserve_cell_name(target.arg_value)
+            if target.arg_value.startswith("*"):
+                target.arg = builder.reserve_cell_name(target.arg_value)
+            else:
+                target.arg = builder.reserve_free_name(target.arg_value)
         elif target.has_constant():
             target.arg = builder.reserve_constant(target.arg_value)
 
 
 class ExtendedArgInserter(AbstractInstructionWalkerTransform):
     @classmethod
     def visit(cls, function: "MutableFunction", builder: CodeObjectBuilder, target: "Instruction") -> typing.Any:
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/CacheEntryCreation.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/CacheEntryCreation.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/ExceptionTable.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/ExceptionTable.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/Instruction.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/Instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -683,15 +683,15 @@
             Opcodes.UNARY_NEGATIVE,
             Opcodes.UNARY_INVERT,
             Opcodes.UNARY_POSITIVE,
             Opcodes.STATIC_ATTRIBUTE_ACCESS,
         ):
             return 1, 1, None
 
-        if self.opcode in (Opcodes.STORE_ATTR,):
+        if self.opcode in (Opcodes.STORE_ATTR, Opcodes.STORE_SUBSCR):
             return 2, 0, None
 
         if self.opcode in (
             Opcodes.POP_TOP,
             Opcodes.POP_JUMP_IF_TRUE,
             Opcodes.POP_JUMP_IF_FALSE,
             Opcodes.STORE_FAST,
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/OpcodeReplacer.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/OpcodeReplacer.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/Opcodes.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/Opcodes.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/optimiser_util.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/optimiser_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,34 +258,43 @@
         ):
             method = OPCODE_TO_ATTR_DOUBLE[
                 instruction.opcode
                 if instruction.opcode in OPCODE_TO_ATTR_DOUBLE
                 else (instruction.opcode, instruction.arg)
             ]
 
-            arg = next(instruction.trace_stack_position(1))
-            target = next(instruction.trace_stack_position(0))
+            target = next(instruction.trace_stack_position(1))
+            arg = next(instruction.trace_stack_position(0))
 
             if arg.opcode == target.opcode == Opcodes.LOAD_CONST:
                 value = target.arg_value
 
+                add_target = True
+
                 if isinstance(method, str):
+                    if not hasattr(value, method):
+                        return
+
                     method = getattr(value, method)
+                    add_target = False
 
                     if not callable(method) or not (
                         type(value) in CONSTANT_BUILTIN_TYPES
                         or (
                             hasattr(method, "_OPTIMISER_CONTAINER")
                             and getattr(method, "_OPTIMISER_CONTAINER").is_constant_op
                         )
                     ):
                         return
 
                 try:
-                    value = method(arg.arg_value, target.arg_value)
+                    if add_target:
+                        value = method(arg.arg_value, target.arg_value)
+                    else:
+                        value = method(arg.arg_value)
                 except:
                     traceback.print_exc()
                     return
 
                 instruction.change_opcode(Opcodes.LOAD_CONST)
                 instruction.change_arg_value(value)
                 target.change_opcode(Opcodes.NOP)
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation/util.py` & `bytecodemanipulation-0.3.4/bytecodemanipulation/util.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation.egg-info/PKG-INFO` & `bytecodemanipulation-0.3.4/bytecodemanipulation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytecodemanipulation
-Version: 0.3.3
+Version: 0.3.4
 Summary: High level python bytecode manipulation
 Home-page: https://github.com/uuk0/PyBytecodeManipulator
 Author: uuk
 Author-email: uuk1301@gmail.com
 Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `bytecodemanipulation-0.3.3/bytecodemanipulation.egg-info/SOURCES.txt` & `bytecodemanipulation-0.3.4/bytecodemanipulation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/setup.py` & `bytecodemanipulation-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="bytecodemanipulation",
-    version="0.3.3",
+    version="0.3.4",
     author="uuk",
     author_email="uuk1301@gmail.com",
     description="High level python bytecode manipulation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/uuk0/PyBytecodeManipulator",
     project_urls={
```

### Comparing `bytecodemanipulation-0.3.3/tests/test_Assembly.py` & `bytecodemanipulation-0.3.4/tests/test_Assembly.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import dis
 import functools
 import itertools
+import sys
 from unittest import TestCase
 
 import bytecodemanipulation.data_loader
 from bytecodemanipulation.data.shared.instructions.LabelAssembly import LabelAssembly
 from bytecodemanipulation.data.shared.instructions.PythonCodeAssembly import (
     PythonCodeAssembly,
 )
@@ -41,18 +42,14 @@
 )
 from bytecodemanipulation.data.shared.instructions.WhileAssembly import (
     AbstractWhileAssembly,
 )
 from bytecodemanipulation.data.shared.instructions.YieldAssembly import (
     AbstractYieldAssembly,
 )
-from bytecodemanipulation.data.shared.instructions.OpAssembly import AbstractOpAssembly
-from bytecodemanipulation.data.shared.instructions.CallAssembly import (
-    AbstractCallAssembly,
-)
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 bytecodemanipulation.data_loader.INIT_ASSEMBLY = False
 from bytecodemanipulation.assembler.Parser import *
 from bytecodemanipulation.assembler.target import (
     assembly,
     label,
@@ -1254,23 +1251,23 @@
 
         self.assertEqual(target(), 0)
 
     def test_macro_paste(self):
         def target():
             assembly(
                 """
-        MACRO test_macro_paste (param) {
-            MACRO_PASTE param
-        }
+MACRO test_macro_paste (param) {
+    MACRO_PASTE param
+}
 
-        LOAD 0 -> $test
-        CALL MACRO test_macro_paste({
-            LOAD 10 -> $test
-        })
-        RETURN $test
+LOAD 0 -> $test
+CALL MACRO test_macro_paste({
+    LOAD 10 -> $test
+})
+RETURN $test
         """
             )
             return -1
 
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
@@ -1517,21 +1514,79 @@
 DEF xy(a=0)
 {
     RETURN $a
 }            
 
 MACRO test_macro_func_call_keyword_expansion(keyword)
 {
-    RETURN $xy(&keyword=4)
+    RETURN $:xy(&keyword=4)
 }
 
-CALL MACRO test_macro_func_call_keyword_expansion("key")
+CALL MACRO test_macro_func_call_keyword_expansion("a")
 """)
             return 0
 
+        self.assertEqual(target(), 4)
+
+    def test_macro_paste_parameterized_code_block_1(self):
+        @apply_operations
+        def target():
+            assembly("""    
+
+MACRO test_macro_paste_parameterized_code_block_1(code CODE_BLOCK[1])
+{
+    LOAD 10 -> $var
+    MACRO_PASTE &code [$var]
+}
+
+CALL MACRO test_macro_paste_parameterized_code_block_1([$local] { RETURN $local })
+        """)
+            return 0
+
+        self.assertEqual(target(), 10)
+
+    def test_macro_paste_parameterized_code_block_non_static(self):
+        @apply_operations
+        def target():
+            assembly("""    
+
+MACRO test_macro_paste_parameterized_code_block_non_static(code CODE_BLOCK[1])
+{
+    LOAD 10 -> $var
+    MACRO_PASTE &code [$var]
+}
+
+CALL MACRO test_macro_paste_parameterized_code_block_non_static([$local] { LOAD 0 -> $|var\nRETURN $local })
+        """)
+            return -1
+
+        dis.dis(target)
+
+        self.assertEqual(target(), 0)
+
+    def test_macro_paste_parameterized_code_block_static(self):
+        @apply_operations
+        def target():
+            assembly("""    
+
+MACRO test_macro_paste_parameterized_code_block_static(code CODE_BLOCK[1])
+{
+    LOAD 10 -> $var
+    MACRO_PASTE &code [!$var]
+}
+
+CALL MACRO test_macro_paste_parameterized_code_block_static([$local] { LOAD 0 -> $|var\nRETURN $local })
+        """)
+            return 0
+
+        dis.dis(target)
+
+        self.assertEqual(target(), 10)
+
+
 class TestClassAssembly(TestCase):
     def test_class_assembly(self):
         def target():
             test = None
             assembly(
                 """
 CLASS test{}"""
@@ -1751,14 +1806,16 @@
 
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
         self.assertEqual(target(), [0, 0, 1, 2])
 
+
+class TestRawAssembly(TestCase):
     def test_raw_assembly_by_id(self):
         def target():
             assembly(
                 """
 LOAD 10
 LOAD 5
 RAW 2
@@ -1785,14 +1842,16 @@
 
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
         self.assertEqual(target(), 10)
 
+
+class TestAssert(TestCase):
     def test_assert(self):
         @apply_operations
         def target(x):
             assembly(
                 """
 ASSERT $x
 """
@@ -1898,7 +1957,101 @@
 """
             )
 
         try:
             apply_operations(target)
         except AssertionError as e:
             self.assertEqual(e.args, ("assertion failed: expected <true-ish value>",))
+
+
+class TestIfLabel(TestCase):
+    def test_if_label_jump(self):
+        @apply_operations
+        def target(x):
+            assembly("""
+
+IF $x 'label' 
+{
+    JUMP label:END
+    RETURN 0
+}
+
+RETURN 1
+""")
+
+        self.assertEqual(target(0), 1)
+        self.assertEqual(target(1), 1)
+
+    def test_version_constants(self):
+        @apply_operations
+        def target():
+            assembly("""
+
+RETURN ~PY_VERSION
+        """)
+
+        self.assertEqual(target(), sys.version_info.major * 100 + sys.version_info.minor)
+
+
+class TestStaticIf(TestCase):
+    def test_static_version_check(self):
+        version_id = sys.version_info.major * 100 + sys.version_info.minor
+
+        scope = {"__file__": __file__, "apply_operations": apply_operations, "assembly": assembly}
+
+        exec(f'''
+@apply_operations
+def target():
+    assembly("""
+IF OP(~PY_VERSION == {version_id})
+{{
+    RETURN 1
+}}
+RETURN 0
+""")''', scope)
+
+        target = scope["target"]
+
+        self.assertEqual(target(), 1)
+        compare_optimized_results(self, target, lambda: 1)
+
+
+class TestFunctionDefinitionLocalCapture(TestCase):
+    def test_simple(self):
+        @apply_operations
+        def target():
+            assembly("""
+LOAD 10 -> $test
+
+DEF func<test>()
+{
+    RETURN §test
+}
+
+RETURN $func()
+""")
+
+        self.assertEqual(target(), 10)
+
+    def test_write(self):
+        @apply_operations
+        def target():
+            assembly("""
+LOAD 0 -> $test            
+
+DEF func<test>()
+{
+    LOAD 10 -> §test
+    RETURN §test
+}
+
+CALL ~print(10) -> \\
+
+LOAD $func() -> $result
+# ASSERT OP ($test == 10)  # wont work as we currently cannot write back outside
+ASSERT OP ($test == 0) "old implementation limitation lifted?"
+RETURN $result 
+""")
+
+        dis.dis(target)
+
+        self.assertEqual(target(), 10)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bytecodemanipulation-0.3.3/tests/test_InlineSystem.py` & `bytecodemanipulation-0.3.4/tests/test_InlineSystem.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/tests/test_Mixin.py` & `bytecodemanipulation-0.3.4/tests/test_Mixin.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/tests/test_MutableFunction.py` & `bytecodemanipulation-0.3.4/tests/test_MutableFunction.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/tests/test_Operators.py` & `bytecodemanipulation-0.3.4/tests/test_Operators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import dis
 from unittest import TestCase
 
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.assembler.target import apply_operations
 from bytecodemanipulation.assembler.target import assembly
+from tests.util import compare_optimized_results
 
 
 class TestOperators(TestCase):
     def test_simple_and_true(self):
         @apply_operations
         def target():
             assembly("""RETURN OP (1 and 1)""")
@@ -360,7 +361,52 @@
 
     def test_sum_operator_advanced(self):
         @apply_operations
         def target(a):
             assembly("RETURN OP (sum ($a, $a, $a, $a))")
 
         self.assertEqual(target(2), 8)
+
+    def test_tuple_operator(self):
+        @apply_operations
+        def target():
+            assembly("RETURN OP (tuple (10, 20, 30))")
+
+        self.assertEqual(target(), (10, 20, 30))
+
+    def test_tuple_operator_static(self):
+        @apply_operations
+        def target():
+            assembly("RETURN OP (tuple (10, 20, 30))[0]")
+
+        self.assertEqual(target(), 10)
+
+        dis.dis(target)
+
+        compare_optimized_results(self, target, lambda: 10)
+
+    def test_list_operator(self):
+        @apply_operations
+        def target():
+            assembly("RETURN OP (list (10, 20, 30))")
+
+        self.assertEqual(target(), [10, 20, 30])
+
+    def test_set_operator(self):
+        @apply_operations
+        def target():
+            assembly("RETURN OP (set (10, 20, 30))")
+
+        self.assertEqual(target(), {10, 20, 30})
+
+    def test_dict_operator(self):
+        @apply_operations
+        def target():
+            assembly("RETURN OP (dict (10, 20, 30, 40))")
+
+        self.assertEqual(target(), {10: 20, 30: 40})
+
+    def test_dict_operator_failure(self):
+        def target():
+            assembly("RETURN OP (dict (10, 20, 30))")
+
+        self.assertRaises(SyntaxError, lambda: apply_operations(target))
```

### Comparing `bytecodemanipulation-0.3.3/tests/test_Optimiser.py` & `bytecodemanipulation-0.3.4/tests/test_Optimiser.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/tests/test_Specializations.py` & `bytecodemanipulation-0.3.4/tests/test_Specializations.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.3/tests/test_StandardLibrary.py` & `bytecodemanipulation-0.3.4/tests/test_StandardLibrary.py`

 * *Files 21% similar despite different names*

```diff
@@ -121,15 +121,15 @@
             data = (0, 1, 2)
             stream = None
             output = None
             assembly(
                 """
 std:stream:initialize($stream)
 std:stream:extend($stream, $data)
-std:stream:reduce($stream, $lhs, $rhs, {
+std:stream:reduce($stream, [$lhs, $rhs] {
     OP $lhs + $rhs
 })
 STORE $output
 """
             )
             return output
 
@@ -147,55 +147,47 @@
             stream = None
             output = None
             assembly(
                 """
 std:stream:initialize($stream)
 std:stream:extend($stream, $data)
 std:print($stream)
-std:stream:filter($stream, $var, {
+std:stream:filter($stream, [$var] {
     OP $var < 2 -> %
 })
 std:print($stream)
 std:stream:to_list($stream, $output)
 """
             )
             return output
 
         self.assertEqual(target(), [0, 1])
 
     def test_stream_simple_map(self):
+        @apply_operations
         def target():
             data = (0, 1, 2)
             stream = None
             output = None
             assembly(
                 """
 std:stream:initialize($stream)
 std:stream:extend($stream, $data)
-std:stream:map($stream, $var, {
+std:stream:map($stream, [$var] {
     OP $var + 1 -> $var
 })
 std:stream:to_list($stream, $output)
 """
             )
             return output
 
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
         self.assertEqual(target(), [1, 2, 3])
 
-#     def test_comprehension_list(self):
-#         def target():
-#             l = [1, 2, 3, 4]
-#             assembly("""
-# std:comprehension:list($l, $value, { OP $value + 1 -> % }) -> %
-# RETURN %""")
-#
-#         mutable = MutableFunction(target)
-#         apply_inline_assemblies(mutable)
-#         mutable.reassign_to_function()
-#
-#         dis.dis(target)
-#
-#         self.assertEqual(target(), [1, 2, 3])
+    def test_comprehension_list(self):
+        @apply_operations
+        def target():
+            l = [1, 2, 3, 4]
+            assembly("""
+std:comprehension:list($l, [$value] { OP $value + 1 -> % }) -> %
+RETURN %""")
+
+        self.assertEqual(target(), [2, 3, 4, 5])
```

### Comparing `bytecodemanipulation-0.3.3/tests/test_issues.py` & `bytecodemanipulation-0.3.4/tests/test_issues.py`

 * *Files identical despite different names*

