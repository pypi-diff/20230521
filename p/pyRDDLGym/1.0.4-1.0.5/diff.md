# Comparing `tmp/pyRDDLGym-1.0.4.tar.gz` & `tmp/pyRDDLGym-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRDDLGym-1.0.4.tar", last modified: Fri Apr  7 15:21:51 2023, max compression
+gzip compressed data, was "pyRDDLGym-1.0.5.tar", last modified: Sun May 21 18:31:13 2023, max compression
```

## Comparing `pyRDDLGym-1.0.4.tar` & `pyRDDLGym-1.0.5.tar`

### file list

```diff
@@ -1,241 +1,242 @@
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.021423 pyRDDLGym-1.0.4/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1264 2022-12-08 22:55:23.000000 pyRDDLGym-1.0.4/LICENSE.MD
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       87 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/MANIFEST.in
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      911 2023-04-07 15:21:51.021094 pyRDDLGym-1.0.4/PKG-INFO
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     8094 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/README.md
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.970905 pyRDDLGym-1.0.4/pyRDDLGym/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.972403 pyRDDLGym-1.0.4/pyRDDLGym/Core/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.974969 pyRDDLGym-1.0.4/pyRDDLGym/Core/Compiler/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     8347 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Compiler/RDDLDecompiler.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    11135 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Compiler/RDDLLevelAnalysis.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    17227 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Compiler/RDDLLiftedModel.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    18950 2023-04-06 22:49:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Compiler/RDDLModel.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    45925 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Compiler/RDDLObjectsTracer.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5216 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Compiler/RDDLValueInitializer.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Compiler/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.975483 pyRDDLGym-1.0.4/pyRDDLGym/Core/Debug/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2168 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Debug/Logger.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-01-27 22:40:35.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Debug/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.976020 pyRDDLGym-1.0.4/pyRDDLGym/Core/Env/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5797 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Env/RDDLConstraints.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    11038 2023-04-06 22:49:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Env/RDDLEnv.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Env/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.976325 pyRDDLGym-1.0.4/pyRDDLGym/Core/ErrorHandling/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1330 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/ErrorHandling/RDDLException.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/ErrorHandling/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.976653 pyRDDLGym-1.0.4/pyRDDLGym/Core/Grounder/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    27395 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Grounder/RDDLGrounder.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Grounder/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.979788 pyRDDLGym-1.0.4/pyRDDLGym/Core/Jax/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    20098 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Jax/JaxParameterTuning.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    32816 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlanner.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    11953 2023-04-06 22:49:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlannerUCT.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    69234 2023-04-07 15:03:00.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Jax/JaxRDDLCompiler.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    18597 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Jax/JaxRDDLLogic.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    12925 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Jax/JaxRDDLModelError.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     6948 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Jax/JaxRDDLSimulator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Jax/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.983971 pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1620 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/RDDLReader.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        1 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1146 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/cpf.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    10193 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/domain.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7819 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/expr.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1293 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/instance.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1221 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/nonfluents.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    38755 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/parser.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)   123443 2023-02-22 22:24:57.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/parsetab.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3242 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/pvariable.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    10773 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/rddl.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      801 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/utils.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.984554 pyRDDLGym-1.0.4/pyRDDLGym/Core/Simulator/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    49061 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Simulator/RDDLSimulator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/Simulator/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/Core/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.986439 pyRDDLGym-1.0.4/pyRDDLGym/Examples/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.963405 pyRDDLGym-1.0.4/pyRDDLGym/Examples/CartPole/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.987338 pyRDDLGym-1.0.4/pyRDDLGym/Examples/CartPole/Continuous/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      238 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/CartPole/Continuous/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3419 2023-03-21 16:55:28.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/CartPole/Continuous/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      945 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/CartPole/Continuous/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.988439 pyRDDLGym-1.0.4/pyRDDLGym/Examples/CartPole/Discrete/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      256 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/CartPole/Discrete/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3510 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/CartPole/Discrete/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      928 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/CartPole/Discrete/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.989790 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Elevators/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      218 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Elevators/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    10524 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Elevators/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1408 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Elevators/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1628 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Elevators/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5211 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/ExampleManager.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.990958 pyRDDLGym-1.0.4/pyRDDLGym/Examples/HVAC/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      161 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/HVAC/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5768 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/HVAC/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      364 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/HVAC/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      389 2023-04-07 02:46:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/HVAC/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      455 2023-04-07 02:46:06.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/HVAC/instance2.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3652 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerator.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.992913 pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2687 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/HVACInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1630 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/MarsRoverInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3058 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/MountainCarInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3264 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/PowerGenInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3594 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/RaceCarInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4086 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/RecSimInstanceGen.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2285 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/ReservoirInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1819 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/UAVInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.993537 pyRDDLGym-1.0.4/pyRDDLGym/Examples/MarsRover/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      210 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/MarsRover/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4495 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/MarsRover/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1411 2023-03-30 14:37:35.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/MarsRover/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.994973 pyRDDLGym-1.0.4/pyRDDLGym/Examples/MountainCar/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      219 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/MountainCar/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4408 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/MountainCar/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2551 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/MountainCar/domain_old.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    14859 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/MountainCar/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      960 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/MountainCar/instance0_old.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.964645 pyRDDLGym-1.0.4/pyRDDLGym/Examples/NewLanguageExamples/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.995971 pyRDDLGym-1.0.4/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      101 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2890 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      655 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.996775 pyRDDLGym-1.0.4/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      105 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1401 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      193 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.964977 pyRDDLGym-1.0.4/pyRDDLGym/Examples/PowerGen/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.997589 pyRDDLGym-1.0.4/pyRDDLGym/Examples/PowerGen/Continuous/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      239 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/PowerGen/Continuous/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4403 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/PowerGen/Continuous/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1610 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/PowerGen/Continuous/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.998446 pyRDDLGym-1.0.4/pyRDDLGym/Examples/PowerGen/Discrete/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      164 2023-02-27 22:52:10.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/PowerGen/Discrete/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3383 2023-02-27 22:52:10.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/PowerGen/Discrete/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1630 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/PowerGen/Discrete/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.999104 pyRDDLGym-1.0.4/pyRDDLGym/Examples/PropDBN/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       87 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/PropDBN/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2283 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/PropDBN/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      268 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/PropDBN/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.000085 pyRDDLGym-1.0.4/pyRDDLGym/Examples/RaceCar/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      176 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/RaceCar/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4995 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/RaceCar/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     9478 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/RaceCar/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      995 2023-04-07 02:51:57.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/RaceCar/instance1.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.001321 pyRDDLGym-1.0.4/pyRDDLGym/Examples/RecSim/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      189 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/RecSim/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4153 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/RecSim/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1327 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/RecSim/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    15525 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/RecSim/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    85747 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/RecSim/instance2.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.965557 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Reservoir/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.002291 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Reservoir/Continuous/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      237 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Reservoir/Continuous/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4435 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Reservoir/Continuous/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      391 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Reservoir/Continuous/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      710 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Reservoir/Continuous/instance1.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.003033 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Reservoir/Discrete/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      162 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Reservoir/Discrete/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4544 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Reservoir/Discrete/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      390 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Reservoir/Discrete/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      709 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Reservoir/Discrete/instance1.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.003565 pyRDDLGym-1.0.4/pyRDDLGym/Examples/SupplyChain/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      118 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/SupplyChain/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3550 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/SupplyChain/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      635 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/SupplyChain/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.004123 pyRDDLGym-1.0.4/pyRDDLGym/Examples/SupplyChainNet/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      129 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/SupplyChainNet/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4622 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/SupplyChainNet/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1747 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/SupplyChainNet/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.005186 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.966046 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/Deprecated/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.006196 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    20730 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7653 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     9656 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    24387 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance2.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.006401 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/Experiments/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     6386 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/Experiments/webster_exp_equal_split.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       91 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    16438 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4951 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    25150 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    23064 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/netgen.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.966487 pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.007204 pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Continuous/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      241 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Continuous/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5492 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Continuous/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1053 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Continuous/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1063 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Continuous/instance1.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.007873 pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Discrete/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      185 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Discrete/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5440 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Discrete/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      831 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Discrete/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.008569 pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Mixed/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      179 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Mixed/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5491 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Mixed/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      831 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Mixed/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.009314 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Wildfire/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      121 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Wildfire/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4280 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Wildfire/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1398 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/Wildfire/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Examples/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2603 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/GymExample.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5499 2023-04-06 22:49:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/JaxExample.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1704 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/JaxTuningExample.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.009898 pyRDDLGym-1.0.4/pyRDDLGym/Planner/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3415 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.4/pyRDDLGym/Planner/JaxConfigManager.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Planner/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.010602 pyRDDLGym-1.0.4/pyRDDLGym/Policies/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1340 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.4/pyRDDLGym/Policies/Agents.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     9818 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Policies/RDDLSimAgent.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/Policies/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      396 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/RDDLSimClientExample.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.015569 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2924 2023-01-23 22:29:35.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/CartPoleViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7420 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/ChartViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5528 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/ColorViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     8708 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/ElevatorViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    12057 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/HVACViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     6278 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/MarsRoverViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4797 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/MountainCarViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3950 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/MovieGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     8522 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/PowerGenViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2880 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/RacecarViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7180 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/RecSimViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    11691 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/ReservoirViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      516 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/StateViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2767 2023-01-23 22:29:35.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/TextViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    20753 2023-03-02 18:32:16.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/TrafficViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4754 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/UAVsViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5987 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/WildfireViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    20186 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/visualize_dbn.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.017189 pyRDDLGym-1.0.4/pyRDDLGym/XADD/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2383 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.4/pyRDDLGym/XADD/RDDLLevelAnalysisXADD.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    17224 2023-03-22 17:18:24.000000 pyRDDLGym-1.0.4/pyRDDLGym/XADD/RDDLModelXADD.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     6162 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.4/pyRDDLGym/XADD/RDDLSimulatorXADD.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       41 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.4/pyRDDLGym/XADD/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      111 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.4/pyRDDLGym/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      701 2022-12-29 01:36:27.000000 pyRDDLGym-1.0.4/pyRDDLGym/testDiscrete.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:51.020769 pyRDDLGym-1.0.4/pyRDDLGym/tests/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7362 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/tests/RDDLGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/tests/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    13792 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/tests/_deprecated.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1265 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/tests/testGymDrone.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1672 2022-10-24 03:39:07.000000 pyRDDLGym-1.0.4/pyRDDLGym/tests/testViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1267 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/tests/test_basic.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      658 2023-03-22 00:25:03.000000 pyRDDLGym-1.0.4/pyRDDLGym/tests/test_dbn_vis.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1055 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/tests/test_termination.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2534 2023-03-22 00:25:03.000000 pyRDDLGym-1.0.4/pyRDDLGym/tests/test_xadd.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5114 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/tests/unit_test_mars_rover.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2782 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.4/pyRDDLGym/tests/unit_test_power_gen.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:21:50.972240 pyRDDLGym-1.0.4/pyRDDLGym.egg-info/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      911 2023-04-07 15:21:50.000000 pyRDDLGym-1.0.4/pyRDDLGym.egg-info/PKG-INFO
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7859 2023-04-07 15:21:50.000000 pyRDDLGym-1.0.4/pyRDDLGym.egg-info/SOURCES.txt
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        1 2023-04-07 15:21:50.000000 pyRDDLGym-1.0.4/pyRDDLGym.egg-info/dependency_links.txt
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       67 2023-04-07 15:21:50.000000 pyRDDLGym-1.0.4/pyRDDLGym.egg-info/requires.txt
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       10 2023-04-07 15:21:50.000000 pyRDDLGym-1.0.4/pyRDDLGym.egg-info/top_level.txt
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       38 2023-04-07 15:21:51.021499 pyRDDLGym-1.0.4/setup.cfg
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2810 2023-04-07 15:18:53.000000 pyRDDLGym-1.0.4/setup.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.433329 pyRDDLGym-1.0.5/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1264 2022-12-08 22:55:23.000000 pyRDDLGym-1.0.5/LICENSE.MD
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       87 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/MANIFEST.in
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      911 2023-05-21 18:31:13.433129 pyRDDLGym-1.0.5/PKG-INFO
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     8094 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/README.md
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.389524 pyRDDLGym-1.0.5/pyRDDLGym/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.390646 pyRDDLGym-1.0.5/pyRDDLGym/Core/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.393009 pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     8347 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLDecompiler.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    11135 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLLevelAnalysis.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    17227 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLLiftedModel.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    18950 2023-04-06 22:49:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLModel.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    47583 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLObjectsTracer.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5216 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLValueInitializer.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.393444 pyRDDLGym-1.0.5/pyRDDLGym/Core/Debug/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2168 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Debug/Logger.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-01-27 22:40:35.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Debug/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.393927 pyRDDLGym-1.0.5/pyRDDLGym/Core/Env/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5797 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Env/RDDLConstraints.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    11884 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Env/RDDLEnv.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Env/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.394569 pyRDDLGym-1.0.5/pyRDDLGym/Core/ErrorHandling/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1378 2023-04-20 23:10:37.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/ErrorHandling/RDDLException.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/ErrorHandling/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.395017 pyRDDLGym-1.0.5/pyRDDLGym/Core/Grounder/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    27395 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Grounder/RDDLGrounder.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Grounder/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.397465 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    20186 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxParameterTuning.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    53645 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlanner.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    11956 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlannerUCT.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    69234 2023-04-07 15:03:00.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLCompiler.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    18972 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLLogic.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    12925 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLModelError.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     6948 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLSimulator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.401663 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1620 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/RDDLReader.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        1 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1146 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/cpf.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    10193 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/domain.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7819 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/expr.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1293 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/instance.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1221 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/nonfluents.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    38755 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/parser.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)   123443 2023-02-22 22:24:57.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/parsetab.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3242 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/pvariable.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    10773 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/rddl.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      801 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/utils.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.402131 pyRDDLGym-1.0.5/pyRDDLGym/Core/Simulator/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    49061 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Simulator/RDDLSimulator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Simulator/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.402978 pyRDDLGym-1.0.5/pyRDDLGym/Examples/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.383566 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.403748 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Continuous/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      238 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Continuous/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3419 2023-03-21 16:55:28.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Continuous/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      945 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Continuous/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.404717 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Discrete/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      256 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Discrete/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3510 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Discrete/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      928 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Discrete/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.405762 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Elevators/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      218 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Elevators/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    10524 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Elevators/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1408 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Elevators/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1628 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Elevators/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5211 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/ExampleManager.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.406842 pyRDDLGym-1.0.5/pyRDDLGym/Examples/HVAC/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      161 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/HVAC/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5768 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/HVAC/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      364 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/HVAC/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      389 2023-04-07 02:46:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/HVAC/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      455 2023-04-07 02:46:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/HVAC/instance2.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3652 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerator.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.408545 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2687 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/HVACInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1630 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/MarsRoverInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3058 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/MountainCarInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3264 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/PowerGenInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3594 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/RaceCarInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4086 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/RecSimInstanceGen.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2285 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/ReservoirInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1819 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/UAVInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.408999 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MarsRover/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      210 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MarsRover/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4495 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MarsRover/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1411 2023-03-30 14:37:35.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MarsRover/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.410020 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      219 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4408 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2551 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/domain_old.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    14883 2023-04-16 21:02:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      960 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/instance0_old.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.384261 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.410691 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      101 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2890 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      655 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.411286 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      105 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1401 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      193 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.384514 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.411853 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Continuous/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      239 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Continuous/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4403 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Continuous/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1610 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Continuous/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.412541 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Discrete/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      164 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Discrete/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3383 2023-02-27 22:52:10.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Discrete/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1630 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Discrete/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.413123 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PropDBN/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       87 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PropDBN/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2283 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PropDBN/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      268 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PropDBN/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.413926 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RaceCar/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      176 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RaceCar/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4995 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RaceCar/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     9478 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RaceCar/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      995 2023-04-07 02:51:57.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RaceCar/instance1.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.415033 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      189 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4153 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1327 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    15525 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    85747 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/instance2.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.385035 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.416040 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Continuous/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      237 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Continuous/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4435 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Continuous/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      391 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Continuous/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      710 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Continuous/instance1.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.416776 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Discrete/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      162 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Discrete/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4544 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Discrete/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      390 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Discrete/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      709 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Discrete/instance1.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.417387 pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChain/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      118 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChain/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3550 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChain/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      635 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChain/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.417930 pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChainNet/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      129 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChainNet/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4622 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChainNet/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1747 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChainNet/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.419175 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.385415 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.420256 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    20730 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7653 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     9656 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    24387 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance2.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.420482 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Experiments/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     6386 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Experiments/webster_exp_equal_split.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       91 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    16438 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4951 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    25150 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    23064 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/netgen.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.385822 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.421402 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Continuous/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      241 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Continuous/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5492 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Continuous/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1053 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Continuous/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1063 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Continuous/instance1.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.422188 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Discrete/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      185 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Discrete/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5440 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Discrete/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      831 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Discrete/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.422945 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Mixed/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      179 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Mixed/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5491 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Mixed/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      831 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Mixed/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.423667 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Wildfire/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      121 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Wildfire/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4280 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Wildfire/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1398 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Wildfire/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2603 2023-04-20 22:35:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/GymExample.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5584 2023-04-20 22:35:43.000000 pyRDDLGym-1.0.5/pyRDDLGym/JaxExample.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4439 2023-04-20 22:35:43.000000 pyRDDLGym-1.0.5/pyRDDLGym/JaxLossPlotExample.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1704 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/JaxTuningExample.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.424083 pyRDDLGym-1.0.5/pyRDDLGym/Planner/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3989 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.5/pyRDDLGym/Planner/JaxConfigManager.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Planner/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.424709 pyRDDLGym-1.0.5/pyRDDLGym/Policies/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1340 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.5/pyRDDLGym/Policies/Agents.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     9818 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Policies/RDDLSimAgent.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Policies/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      396 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/RDDLSimClientExample.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.428852 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2924 2023-01-23 22:29:35.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/CartPoleViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7420 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/ChartViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5528 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/ColorViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     8708 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/ElevatorViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    12057 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/HVACViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     6278 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/MarsRoverViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4797 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/MountainCarViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3950 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/MovieGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     8522 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/PowerGenViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2880 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/RacecarViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7180 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/RecSimViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    11691 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/ReservoirViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      516 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/StateViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2767 2023-01-23 22:29:35.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/TextViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    20753 2023-03-02 18:32:16.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/TrafficViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4754 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/UAVsViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5987 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/WildfireViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    20186 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/visualize_dbn.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.430115 pyRDDLGym-1.0.5/pyRDDLGym/XADD/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2383 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.5/pyRDDLGym/XADD/RDDLLevelAnalysisXADD.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    17224 2023-03-22 17:18:24.000000 pyRDDLGym-1.0.5/pyRDDLGym/XADD/RDDLModelXADD.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     6162 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.5/pyRDDLGym/XADD/RDDLSimulatorXADD.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       41 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.5/pyRDDLGym/XADD/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      111 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      701 2022-12-29 01:36:27.000000 pyRDDLGym-1.0.5/pyRDDLGym/testDiscrete.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.432856 pyRDDLGym-1.0.5/pyRDDLGym/tests/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7362 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/RDDLGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    13792 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/_deprecated.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1265 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/testGymDrone.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1672 2022-10-24 03:39:07.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/testViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1267 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/test_basic.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      658 2023-03-22 00:25:03.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/test_dbn_vis.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1055 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/test_termination.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2534 2023-03-22 00:25:03.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/test_xadd.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5114 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/unit_test_mars_rover.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2782 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/unit_test_power_gen.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.390508 pyRDDLGym-1.0.5/pyRDDLGym.egg-info/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      911 2023-05-21 18:31:13.000000 pyRDDLGym-1.0.5/pyRDDLGym.egg-info/PKG-INFO
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7891 2023-05-21 18:31:13.000000 pyRDDLGym-1.0.5/pyRDDLGym.egg-info/SOURCES.txt
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        1 2023-05-21 18:31:13.000000 pyRDDLGym-1.0.5/pyRDDLGym.egg-info/dependency_links.txt
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       67 2023-05-21 18:31:13.000000 pyRDDLGym-1.0.5/pyRDDLGym.egg-info/requires.txt
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       10 2023-05-21 18:31:13.000000 pyRDDLGym-1.0.5/pyRDDLGym.egg-info/top_level.txt
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       38 2023-05-21 18:31:13.433389 pyRDDLGym-1.0.5/setup.cfg
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2810 2023-05-21 18:26:33.000000 pyRDDLGym-1.0.5/setup.py
```

### Comparing `pyRDDLGym-1.0.4/LICENSE.MD` & `pyRDDLGym-1.0.5/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/PKG-INFO` & `pyRDDLGym-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pyRDDLGym
-Version: 1.0.4
+Version: 1.0.5
 Summary: pyRDDLGym: RDDL automatic generation tool for OpenAI Gym
 Home-page: https://github.com/ataitler/pyRDDLGym
 Author: Ayal Taitler, Michael Gimelfarb, Scott Sanner, Jihwan Jeong, Sriram Gopalakrishnan, Martin Mladenov, jack liu
-Author-email: ataitler@gmail.com, mike.gimelfarb@mail.utoronto.ca, ssanner@mie.utoronto.ca, jhjeong@mie.utoronto.ca, ariram.gopalakrishnan@jpmchase.com, mmladenov@google.com, xiaotian.liu@mail.utoronto.ca
+Author-email: ataitler@gmail.com, mike.gimelfarb@mail.utoronto.ca, ssanner@mie.utoronto.ca, jhjeong@mie.utoronto.ca, sriram.gopalakrishnan@jpmchase.com, mmladenov@google.com, xiaotian.liu@mail.utoronto.ca
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyRDDLGym-1.0.4/README.md` & `pyRDDLGym-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Compiler/RDDLDecompiler.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLDecompiler.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Compiler/RDDLLevelAnalysis.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLLevelAnalysis.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Compiler/RDDLLiftedModel.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLLiftedModel.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Compiler/RDDLModel.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLModel.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Compiler/RDDLObjectsTracer.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLObjectsTracer.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,34 +17,40 @@
 class RDDLTracedObjects:
     '''A generic container for storing traced information for a RDDL file.'''
     
     def __init__(self) -> None:
         self._current_id = 0
         self._cached_objects_in_scope = []
         self._cached_enum_type = []
+        self._cached_is_fluent = []
         self._cached_sim_info = []
         self._expr_from_id = {}
         
-    def _append(self, expr, objects, enum_type, info) -> None:
+    def _append(self, expr, objects, enum_type, is_fluent, info) -> None:
         expr.id = self._current_id
         self._current_id += 1
                 
         self._cached_objects_in_scope.append(objects)
         self._cached_enum_type.append(enum_type)
+        self._cached_is_fluent.append(is_fluent)
         self._cached_sim_info.append(info)
         self._expr_from_id[expr.id] = expr
         
     def cached_objects_in_scope(self, expr: Expression):
         '''Returns the free variables/parameters in the scope of expression.'''
         return self._cached_objects_in_scope[expr.id]
     
     def cached_enum_type(self, expr: Expression) -> Union[str, None]:
         '''Returns the returned enum type of expression or None if not an enum.'''
         return self._cached_enum_type[expr.id]
     
+    def cached_is_fluent(self, expr: Expression) -> bool:
+        '''Returns whether the expression is fluent or non-fluent.'''
+        return self._cached_is_fluent[expr.id]
+    
     def cached_sim_info(self, expr: Expression) -> object:
         '''Returns compiled info that is specific to the expression.'''
         return self._cached_sim_info[expr.id]
     
     def lookup(self, identifier: int) -> Expression:
         '''Returns the expression with given identifier, or None if does not 
         exist.'''
@@ -188,15 +194,15 @@
     def _trace_constant(self, expr, objects, out):
         if objects:
             shape = self.rddl.object_counts((ptype for (_, ptype) in objects))
             cached_value = np.full(shape=shape, fill_value=expr.args)
         else:
             cached_value = expr.args
             
-        out._append(expr, objects, None, cached_value)
+        out._append(expr, objects, None, False, cached_value)
         
     def _trace_pvar(self, expr, objects, out):
         var, pvars = expr.args   
         rddl = self.rddl
         
         # free variable (e.g., ?x) treated as array
         # first element True indicates value is to be returned directly by sim
@@ -218,15 +224,15 @@
             cached_value = cached_value[(...,) + (np.newaxis,) * len(ptypes[1:])]
             cached_value = np.swapaxes(cached_value, axis1=0, axis2=index_of_var)
             cached_value = np.broadcast_to(cached_value, shape=shape)
             cached_value = (True, cached_value)
             
             prange = ptypes[index_of_var]
             enum_type = prange if prange in rddl.enums else None
-            out._append(expr, objects, enum_type, cached_value)
+            out._append(expr, objects, enum_type, False, cached_value)
         
         # object can only be defined in domain - map to canonical index
         # first element True indicates value is to be returned directly by sim
         elif not pvars and rddl.is_object(var): 
             
             # check var is a domain object
             literal = rddl.object_name(var)            
@@ -241,31 +247,33 @@
             if objects:
                 shape = rddl.object_counts((ptype for (_, ptype) in objects))
                 cached_value = np.full(shape=shape, fill_value=const)
             else:
                 cached_value = const            
             cached_value = (True, cached_value)
             
-            out._append(expr, objects, enum_type, cached_value)
+            out._append(expr, objects, enum_type, False, cached_value)
         
         # if the pvar has free variables (e.g., ?x)...
         else:
             
             # recursively trace nested pvariables
+            is_fluent = rddl.variable_types[var] != 'non-fluent'
             if pvars is not None: 
                 for arg in pvars:
                     if isinstance(arg, Expression):
                         self._trace(arg, objects, out)
+                        is_fluent = is_fluent or out.cached_is_fluent(arg)
             
             # find a way to map value tensor of expr to match objects
             cached_sim_info = (False, self._map(expr, objects, out))    
                
             prange = rddl.variable_ranges.get(var, None)
             enum_type = prange if prange in rddl.enums else None
-            out._append(expr, objects, enum_type, cached_sim_info)
+            out._append(expr, objects, enum_type, is_fluent, cached_sim_info)
         
     def _map(self, expr: Expression,
              objects: Union[List[Tuple[str, str]], None],
              out: RDDLTracedObjects) -> Tuple[object, ...]:
         '''Returns information needed to reshape and transform value tensor for a
         parameterized variable to match desired output signature.
         
@@ -442,28 +450,32 @@
         return (slices, new_axis, new_shape, op_code, op_args)
     
     # ===========================================================================
     # compound expressions
     # ===========================================================================
     
     def _trace_arithmetic(self, expr, objects, out): 
+        is_fluent = False
         for (i, arg) in enumerate(expr.args):
             self._trace(arg, objects, out)
+            is_fluent = is_fluent or out.cached_is_fluent(arg)
         
             # argument cannot be object type
             RDDLObjectsTracer._check_not_enum(
                 arg, expr, out, f'Argument {i + 1} of operator {expr.etype[1]}')  
               
-        out._append(expr, objects, None, None)
+        out._append(expr, objects, None, is_fluent, None)
         
     def _trace_relational(self, expr, objects, out):
         _, op = expr.etype
         args = expr.args
+        is_fluent = False
         for arg in args:
-            self._trace(arg, objects, out)            
+            self._trace(arg, objects, out)
+            is_fluent = is_fluent or out.cached_is_fluent(arg)         
         
         # can not mix different object types or primitive and object types
         enum_types = set(map(out.cached_enum_type, args))
         if len(enum_types) != 1:
             raise RDDLTypeError(
                 f'Relational operator {op} can not compare arguments '
                 f'of different object types or mix object and non-object types.\n' + 
@@ -472,35 +484,39 @@
         # can not use operator besides == and ~= to compare object types
         enum_type, = enum_types
         if enum_type is not None and op != '==' and op != '~=':
             raise RDDLTypeError(
                 f'Relational operator {op} is not valid for comparing objects.\n' + 
                 print_stack_trace(expr))
         
-        out._append(expr, objects, None, None)
+        out._append(expr, objects, None, is_fluent, None)
     
     def _trace_logical(self, expr, objects, out):
+        is_fluent = False
         for (i, arg) in enumerate(expr.args):
             self._trace(arg, objects, out)
+            is_fluent = is_fluent or out.cached_is_fluent(arg)
             
             # argument cannot be object type
             RDDLObjectsTracer._check_not_enum(
                 arg, expr, out, f'Argument {i + 1} of operator {expr.etype[1]}')
         
-        out._append(expr, objects, None, None)
+        out._append(expr, objects, None, is_fluent, None)
     
     def _trace_func(self, expr, objects, out):
+        is_fluent = False
         for (i, arg) in enumerate(expr.args):
             self._trace(arg, objects, out)
+            is_fluent = is_fluent or out.cached_is_fluent(arg)
             
             # argument cannot be object type
             RDDLObjectsTracer._check_not_enum(
                 arg, expr, out, f'Argument {i + 1} of function {expr.etype[1]}') 
         
-        out._append(expr, objects, None, None)
+        out._append(expr, objects, None, is_fluent, None)
             
     # ===========================================================================
     # aggregation
     # ===========================================================================
     
     def _check_iteration_variables(self, objects, iter_objects, expr):
         
@@ -553,20 +569,21 @@
                     f'Aggregation <{op}> requires one iteration variable, '
                     f'got {len(pvars)}.\n' + print_stack_trace(expr))
             cached_sim_info = (new_objects, reduced_axes[0])
             (_, (_, enum_type)), = pvars
         
         # trace the aggregated expression with the new objects
         self._trace(arg, new_objects, out)
+        is_fluent = out.cached_is_fluent(arg)
         
         # argument cannot be object type
         RDDLObjectsTracer._check_not_enum(
             arg, expr, out, f'Argument of aggregation {op}')     
         
-        out._append(expr, objects, enum_type, cached_sim_info)
+        out._append(expr, objects, enum_type, is_fluent, cached_sim_info)
         
         # log information about aggregation operation
         if self.logger is not None:
             message = (f'computing object info for aggregation:'
                        f'\n\taggregation variables(s)      ={pvars}'
                        f'\n\tfree object(s) in outer scope ={objects}'
                        f'\n\tfree object(s) in inner scope ={new_objects}'
@@ -584,27 +601,29 @@
             self._trace_if(expr, objects, out)
         elif op == 'switch':
             self._trace_switch(expr, objects, out)
             
     def _trace_if(self, expr, objects, out):
         pred, *branches = expr.args
         self._trace(pred, objects, out)
+        is_fluent = out.cached_is_fluent(pred)
         for arg in branches:
             self._trace(arg, objects, out)
+            is_fluent = is_fluent or out.cached_is_fluent(arg)
         
         # can not mix different object types or primitive and object types
         enum_types = set(map(out.cached_enum_type, branches))
         if len(enum_types) != 1:
             raise RDDLTypeError(
                 f'Branches in if then else statement cannot produce values '
                 f'of different object types or mix object and non-object types.\n' + 
                 print_stack_trace(expr))     
     
         enum_type, = enum_types
-        out._append(expr, objects, enum_type, None)
+        out._append(expr, objects, enum_type, is_fluent, None)
         
     def _trace_switch(self, expr, objects, out):
         rddl = self.rddl
         pred, *cases = expr.args
         
         # predicate must be a pvar
         if not pred.is_pvariable_expression():
@@ -638,27 +657,29 @@
                 print_stack_trace(expr))
         
         # order cases by canonical ordering of objects
         cached_sim_info = self._order_cases(enum_type, case_dict, expr)
         
         # trace predicate and cases
         self._trace(pred, objects, out)
+        is_fluent = out.cached_is_fluent(pred)
         for arg in case_dict.values():
             self._trace(arg, objects, out)
+            is_fluent = is_fluent or out.cached_is_fluent(arg)
         
         # can not mix different object types or primitive and object types
         enum_types = set(map(out.cached_enum_type, case_dict.values()))
         if len(enum_types) != 1:
             raise RDDLTypeError(
                 f'Case expressions in switch statement cannot produce values '
                 f'of different object types or mix object and non-object types.\n' + 
                 print_stack_trace(expr))    
                                 
         enum_type, = enum_types
-        out._append(expr, objects, enum_type, cached_sim_info)
+        out._append(expr, objects, enum_type, is_fluent, cached_sim_info)
         
     def _order_cases(self, enum_type, case_dict, expr): 
         rddl = self.rddl
         enum_values = rddl.objects[enum_type]
         
         # check that all literals belong to enum_type
         for _case in case_dict:
@@ -737,22 +758,24 @@
                 f'Default case not allowed in Discrete distribution.\n' + 
                 print_stack_trace(expr))
             
         # order enum cases by canonical ordering of literals
         cached_sim_info, _ = self._order_cases(enum_type, case_dict, expr)
     
         # trace each case expression
+        is_fluent = False
         for (i, arg) in enumerate(case_dict.values()):
             self._trace(arg, objects, out)
+            is_fluent = is_fluent or out.cached_is_fluent(arg)
             
             # argument cannot be object type
             RDDLObjectsTracer._check_not_enum(
                 arg, expr, out, f'Expression in case {i + 1} of Discrete') 
         
-        out._append(expr, objects, enum_type, cached_sim_info)
+        out._append(expr, objects, enum_type, is_fluent, cached_sim_info)
     
     def _trace_discrete_pvar(self, expr, objects, out):
         _, name = expr.etype
         * pvars, args = expr.args
         
         # check number of iteration variables and arguments
         if len(pvars) != 1:
@@ -766,33 +789,37 @@
         
         # sampling variables are appended to scope free variables        
         iter_objects = [pvar for (_, pvar) in pvars]     
         self._check_iteration_variables(objects, iter_objects, expr)
         new_objects = objects + iter_objects
         
         # trace the arguments
+        is_fluent = False
         for (i, arg) in enumerate(args):
             self._trace(arg, new_objects, out)
+            is_fluent = is_fluent or out.cached_is_fluent(arg)
                 
             # argument cannot be object type
             RDDLObjectsTracer._check_not_enum(
                 arg, expr, out, f'Argument {i + 1} of distribution {name}') 
 
         (_, (_, enum_type)), = pvars
-        out._append(expr, objects, enum_type, None)
+        out._append(expr, objects, enum_type, is_fluent, None)
 
     def _trace_random_other(self, expr, objects, out):
+        is_fluent = False
         for (i, arg) in enumerate(expr.args):
             self._trace(arg, objects, out)
+            is_fluent = is_fluent or out.cached_is_fluent(arg)
                 
             # argument cannot be object type
             RDDLObjectsTracer._check_not_enum(
                 arg, expr, out, f'Argument {i + 1} of {expr.etype[1]}') 
         
-        out._append(expr, objects, None, None)
+        out._append(expr, objects, None, is_fluent, None)
         
     # ===========================================================================
     # random vector
     # ===========================================================================
     
     def _trace_random_vector(self, expr, objects, out):
         _, op = expr.etype
@@ -832,14 +859,15 @@
         # sample_pvars are excluded when tracing arguments (e.g., mean)
         # because they are only introduced through sampling which follows after 
         # evaluation of the arguments in a depth-first traversal
         batch_objects = [pvar for pvar in objects if pvar[0] not in sample_pvar_set]
          
         # trace all parameters
         enum_types = set()
+        is_fluent = False
         for (i, arg) in enumerate(args):
             
             # sample_pvars cannot be argument parameters
             name, pvars = arg.args
             if pvars is None:
                 pvars = []
             bad_pvars = {pvar for pvar in pvars if pvar in sample_pvar_set}
@@ -855,14 +883,15 @@
                 raise RDDLInvalidNumberOfArgumentsError(
                     f'Argument <{name}> at position {i + 1} of {op} must contain '
                     f'{required_underscores[i]} sampling parameter(s) _, '
                     f'got {len(underscores)}.\n' + print_stack_trace(expr))
             
             # trace argument
             self._trace(arg, batch_objects, out)
+            is_fluent = is_fluent or out.cached_is_fluent(arg)
             
             # argument cannot be object type
             RDDLObjectsTracer._check_not_enum(
                 arg, expr, out, f'Argument {i + 1} of {op}') 
         
             # record types represented by _
             ptypes = self.rddl.param_types[name]
@@ -882,15 +911,15 @@
             pvar, ptype = objects[index]
             if ptype != enum_type:
                 raise RDDLTypeError(
                     f'{op} sampling is performed over type <{enum_type}>, '
                     f'but destination variable <{pvar}> is of type <{ptype}>.\n' + 
                     print_stack_trace(expr))
              
-        out._append(expr, objects, None, sample_pvar_indices)
+        out._append(expr, objects, None, is_fluent, sample_pvar_indices)
 
     # ===========================================================================
     # matrix algebra
     # ===========================================================================
     
     def _trace_matrix(self, expr, objects, out):
         _, op = expr.etype
@@ -927,20 +956,21 @@
         # axes of new free variables in aggregation are appended to value array
         new_objects = objects + iter_objects
         reduced_axes = tuple(range(len(objects), len(new_objects)))   
         cached_sim_info = (new_objects, reduced_axes)
         
         # trace the matrix with the new objects
         self._trace(arg, new_objects, out)
+        is_fluent = out.cached_is_fluent(arg)
         
         # argument cannot be object type
         RDDLObjectsTracer._check_not_enum(
             arg, expr, out, f'Argument of matrix det')     
         
-        out._append(expr, objects, None, cached_sim_info)
+        out._append(expr, objects, None, is_fluent, cached_sim_info)
         
         # log information about matrix operation
         if self.logger is not None:
             message = (f'computing object info for matrix operation:'
                        f'\n\tmatrix operation              =det'
                        f'\n\tdimension variables(s)        ={pvars}'
                        f'\n\tfree object(s) in outer scope ={objects}'
@@ -984,22 +1014,23 @@
         
         # move the matrix parameters to end of objects
         batch_objects = [pvar for pvar in objects if pvar[0] not in scope_pvars]
         new_objects = batch_objects + [(pvar1, ptype1), (pvar2, ptype2)]
         
         # trace the matrix expression
         self._trace(arg, new_objects, out)
+        is_fluent = out.cached_is_fluent(arg)
         
         # argument cannot be object type
         RDDLObjectsTracer._check_not_enum(
             arg, expr, out, f'Argument of matrix {op}')     
         
         # save the location of the moved indices in objects
         pvar_indices = (index_pvar1, index_pvar2)
-        out._append(expr, objects, None, pvar_indices)
+        out._append(expr, objects, None, is_fluent, pvar_indices)
         
         # log information about matrix operation
         if self.logger is not None:
             message = (f'computing object info for matrix operation:'
                        f'\n\tmatrix operation              ={op}'
                        f'\n\tdimension variables(s)        ={pvars}'
                        f'\n\tfree object(s) in outer scope ={objects}'
```

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Compiler/RDDLValueInitializer.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLValueInitializer.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Debug/Logger.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Debug/Logger.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Env/RDDLConstraints.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Env/RDDLConstraints.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Env/RDDLEnv.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Env/RDDLEnv.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import gym
 from gym.spaces import Discrete, Dict, Box
 import numpy as np
 import pygame
 import os
 
 from pyRDDLGym.Core.ErrorHandling.RDDLException import RDDLInvalidNumberOfArgumentsError
-from pyRDDLGym.Core.ErrorHandling.RDDLException import RDDLTypeError
+from pyRDDLGym.Core.ErrorHandling.RDDLException import RDDLTypeError, RDDLLogFolderError
 
 from pyRDDLGym.Core.Compiler.RDDLLiftedModel import RDDLLiftedModel
 from pyRDDLGym.Core.Debug.Logger import Logger, SimLogger
 from pyRDDLGym.Core.Env.RDDLConstraints import RDDLConstraints
 from pyRDDLGym.Core.Parser.parser import RDDLParser
 from pyRDDLGym.Core.Parser.RDDLReader import RDDLReader
 from pyRDDLGym.Core.Simulator.RDDLSimulator import RDDLSimulator
@@ -18,33 +18,37 @@
 
 
 class RDDLEnv(gym.Env):
     
     def __init__(self, domain: str,
                  instance: str=None,
                  enforce_action_constraints: bool=False,
+                 enforce_action_count_non_bool: bool=True,
                  debug: bool=False,
                  log: bool=False,
                  simlogname: str=None,
                  backend: object=RDDLSimulator):
         '''Creates a new gym environment from the given RDDL domain + instance.
         
         :param domain: the RDDL domain
         :param instance: the RDDL instance
         :param enforce_action_constraints: whether to raise an exception if the
         action constraints are violated
+        :param enforce_action_count_non_bool: whether to include non-bool actions
+        in check that number of nondef actions don't exceed max-nondef-actions
         :param debug: whether to log compilation information to a log file
         :param log: whether to log simulation data to file
         :param backend: the subclass of RDDLSimulator to use as backend for
         simulation (currently supports numpy and Jax)
         '''
         super(RDDLEnv, self).__init__()
         self.domain_text = domain
         self.instance_text = instance
         self.enforce_action_constraints = enforce_action_constraints
+        self.enforce_action_count_non_bool = enforce_action_count_non_bool
 
         # time budget for applications limiting time on episodes.
         # hardcoded so cannot be changed externally.
         self.budget = 120
 
         # read and parse domain and instance
         reader = RDDLReader(domain, instance)
@@ -64,15 +68,20 @@
         self.simlogger = None
         if log:
             curpath = os.path.abspath(__file__)
             for _ in range(3):
                 curpath = os.path.split(curpath)[0]
             dir = os.path.join(curpath, 'Logs', simlogname, ast.domain.name)
             if not os.path.exists(dir):
-                os.makedirs(dir)
+                try:
+                    os.makedirs(dir)
+                except Exception as e:
+                    if not isinstance(e, FileExistsError):
+                        raise RDDLLogFolderError('Could not create log folder for domain ' + ast.domain.name + ' of method ' + simlogname + ' at path: ' + dir)
+
             simlog_fname = os.path.join(dir, ast.instance.name)
             self.simlogger = SimLogger(f'{simlog_fname}_log.csv')
         # self.simlogger = SimLogger(f'{log_fname}_log.csv') if log else None
         if self.simlogger:
             self.simlogger.clear(overwrite=False)
         
         # define the model sampler and bounds    
@@ -166,15 +175,22 @@
         self.to_render = False
 
     def step(self, actions):
         if self.done:
             return self.state, 0.0, self.done, {}
 
         # make sure the action length is of currect size
-        action_length = len(actions)
+        if self.enforce_action_count_non_bool:
+            action_length = len(actions)
+        else:
+            action_length = len([
+                action 
+                for action in actions 
+                if self.model.groundactionsranges()[action] == 'bool'
+            ])
         if (action_length > self.max_allowed_actions):
             raise RDDLInvalidNumberOfArgumentsError(
                 f'Invalid action, expected at most '
                 f'{self.max_allowed_actions} entries, '
                 f'but got {action_length}.')
         
         # set full action vector
```

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/ErrorHandling/RDDLException.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/ErrorHandling/RDDLException.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,7 +74,10 @@
 
 class RDDLEnvironmentNotExist(ValueError):
     pass
 
 
 class RDDLInstanceNotExist(ValueError):
     pass
+
+class RDDLLogFolderError(ValueError):
+    pass
```

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Grounder/RDDLGrounder.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Grounder/RDDLGrounder.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Jax/JaxParameterTuning.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxParameterTuning.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,16 @@
     planner = JaxRDDLBackpropPlanner(
         rddl=model,
         plan=JaxStraightLinePlan(
             initializer=jax.nn.initializers.normal(std),
             wrap_sigmoid=wrap_sigmoid),
         rollout_horizon=eval_horizon,
         action_bounds=action_bounds,
-        optimizer=optax.rmsprop(lr),
+        optimizer=optax.rmsprop,
+        optimizer_kwargs={'learning_rate': lr},
         logic=FuzzyLogic(weight=w),
         **planner_kwargs)
     policy_hyperparams = {name: wa for name in action_bounds}
             
     # perform training
     callback = train_epoch(
         key=key,
@@ -132,15 +133,16 @@
     planner = JaxRDDLBackpropPlanner(
         rddl=model,
         plan=JaxStraightLinePlan(
             initializer=jax.nn.initializers.normal(std),
             wrap_sigmoid=wrap_sigmoid),
         rollout_horizon=T,
         action_bounds=action_bounds,
-        optimizer=optax.rmsprop(lr),
+        optimizer=optax.rmsprop,
+        optimizer_kwargs={'learning_rate': lr},
         logic=FuzzyLogic(weight=w),
         **planner_kwargs)
     policy_hyperparams = {name: wa for name in action_bounds}
     
     # initialize env for evaluation (need fresh copy to avoid concurrency)
     env = RDDLEnv(domain=domain,
                   instance=instance,
```

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlannerUCT.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlannerUCT.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         
         # run SGD updates
         model_params = sgd.compiled.model_params
         params = guess
         opt_state = sgd.optimizer.init(params)        
         for epoch in range(self.max_sgd_updates):
             key, subkey = jax.random.split(key)
-            params, opt_state, _ = sgd.update(
+            params, _, opt_state, _ = sgd.update(
                 subkey, params, None, train_subs, model_params, opt_state)
             
             # stop once the actions diverge by delta
             max_delta = 0.0
             for var in action_names:
                 delta = np.linalg.norm(params[var] - guess[var])
                 max_delta = max(max_delta, delta)
```

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Jax/JaxRDDLCompiler.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLCompiler.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Jax/JaxRDDLLogic.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLLogic.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,32 @@
     
     def norm(self, x, y):
         return x * y
     
     def norms(self, x, axis):
         return jnp.prod(x, axis=axis)
 
+
+class GodelTNorm(TNorm):
+    
+    def norm(self, x, y):
+        return jnp.minimum(x, y)
+    
+    def norms(self, x, axis):
+        return jnp.min(x, axis=axis)
+
+
+class LukasiewiczTNorm(TNorm):
+    
+    def norm(self, x, y):
+        return jax.nn.relu(x + y - 1.0)
+    
+    def norms(self, x, axis):
+        return jax.nn.relu(jnp.sum(x - 1.0, axis=axis) + 1.0)
+    
     
 class FuzzyLogic:
     '''A class representing fuzzy logic in JAX.
     
     Functionality can be customized by either providing a tnorm as parameters, 
     or by overriding its methods.
     '''
@@ -55,15 +73,15 @@
         :param weight: a concentration parameter (larger means better accuracy)
         :param error: an error parameter (e.g. floor) (smaller means better accuracy)
         :param debias: which functions to de-bias approximate on forward pass
         :param eps: small positive float to mitigate underflow
         '''
         self.tnorm = tnorm
         self.complement = complement
-        self.weight = weight
+        self.weight = float(weight)
         self.debias = debias
         self.eps = eps
         
     # ===========================================================================
     # logical operators
     # ===========================================================================
```

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Jax/JaxRDDLModelError.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLModelError.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Jax/JaxRDDLSimulator.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLSimulator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/RDDLReader.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/RDDLReader.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/cpf.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/cpf.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/domain.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/domain.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/expr.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/expr.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/instance.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/instance.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/nonfluents.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/nonfluents.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/parser.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/parsetab.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/parsetab.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/pvariable.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/pvariable.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/rddl.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/rddl.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Parser/utils.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Core/Simulator/RDDLSimulator.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Core/Simulator/RDDLSimulator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/CartPole/Continuous/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Continuous/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/CartPole/Continuous/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Continuous/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/CartPole/Discrete/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Discrete/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/CartPole/Discrete/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Discrete/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Elevators/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Elevators/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Elevators/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Elevators/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Elevators/instance1.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Elevators/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/ExampleManager.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/ExampleManager.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/HVAC/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/HVAC/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerator.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/HVACInstanceGenerator.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/HVACInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/MarsRoverInstanceGenerator.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/MarsRoverInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/MountainCarInstanceGenerator.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/MountainCarInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/PowerGenInstanceGenerator.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/PowerGenInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/RaceCarInstanceGenerator.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/RaceCarInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/RecSimInstanceGen.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/RecSimInstanceGen.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/ReservoirInstanceGenerator.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/ReservoirInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/InstanceGenerators/UAVInstanceGenerator.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/UAVInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/MarsRover/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/MarsRover/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/MarsRover/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/MarsRover/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/MountainCar/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/MountainCar/domain_old.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/domain_old.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/MountainCar/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/instance0.rddl`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 				   s21,s22,s23,s24,s25,s26,s27,s28,s29,s30,s31,s32,s33,s34,s35,s36,s37,s38,s39,
 				   s40,s41,s42,s43,s44,s45,s46,s47,s48,s49,s50,s51,s52,s53,s54,s55,s56,s57,s58,s59,
 				   s60,s61,s62,s63,s64,s65,s66,s67,s68,s69,s70,s71,s72,s73,s74,s75,s76,s77,s78,s79,s80,
 				   s81,s82,s83,s84,s85,s86,s87,s88,s89,s90,s91,s92,s93,s94,s95,s96,s97,s98,s99,s100};
 	};
 	
 	non-fluents {
+		ACTION-PENALTY = 0.0;
 		X-START(s1) = -1.2;
 		X-START(s2) = -1.182;
 		X-START(s3) = -1.164;
 		X-START(s4) = -1.146;
 		X-START(s5) = -1.128;
 		X-START(s6) = -1.1099999999999999;
 		X-START(s7) = -1.092;
```

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/MountainCar/instance0_old.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/instance0_old.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/PowerGen/Continuous/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Continuous/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/PowerGen/Continuous/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Continuous/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/PowerGen/Discrete/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Discrete/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/PowerGen/Discrete/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Discrete/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/PropDBN/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/PropDBN/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/RaceCar/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/RaceCar/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/RaceCar/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/RaceCar/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/RaceCar/instance1.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/RaceCar/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/RecSim/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/RecSim/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/RecSim/instance1.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/RecSim/instance2.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/instance2.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Reservoir/Continuous/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Continuous/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Reservoir/Continuous/instance1.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Continuous/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Reservoir/Discrete/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Discrete/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Reservoir/Discrete/instance1.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Discrete/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/SupplyChain/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChain/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/SupplyChain/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChain/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/SupplyChainNet/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChainNet/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/SupplyChainNet/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChainNet/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance1.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance2.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance2.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/Experiments/webster_exp_equal_split.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Experiments/webster_exp_equal_split.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/instance1.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Traffic/netgen.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/netgen.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Continuous/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Continuous/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Continuous/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Continuous/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Continuous/instance1.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Continuous/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Discrete/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Discrete/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Discrete/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Discrete/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Mixed/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Mixed/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/UAV/Mixed/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Mixed/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Wildfire/domain.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Wildfire/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Examples/Wildfire/instance0.rddl` & `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Wildfire/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/GymExample.py` & `pyRDDLGym-1.0.5/pyRDDLGym/GymExample.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/JaxExample.py` & `pyRDDLGym-1.0.5/pyRDDLGym/JaxExample.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,26 +17,28 @@
         print(f'\nid = {_id}:\n' + RDDLDecompiler().decompile_expr(expr))
     
     
 def slp_train(planner, budget, **train_args):
     step = train_args['step']
     del train_args['step']
     print('\n' + 'training plan:')
-    starttime = time.time()
     for i, callback in enumerate(planner.optimize(**train_args, step=1)):
-        currtime = time.time()
-        elapsed = currtime - starttime
+        if i == 0:
+            elapsed = 0
+            starttime = time.time()
+        else:
+            elapsed = time.time() - starttime
         
         if i % step == 0:
-            print('[{:.4f} s] step={} train_return={:.6f} test_return={:.6f}'.format(
+            print('[{:.4f} s] step={} train_return={:.6f} test_return={:.6f} best_return={:.6f}'.format(
                 elapsed,
                 str(callback['iteration']).rjust(4),
                 callback['train_return'],
-                callback['test_return']))
-        
+                callback['test_return'],
+                callback['best_return']))
         if elapsed >= budget:
             print('ran out of time!')
             break
     params = callback['best_params']
     
     # key = jax.random.PRNGKey(42)
     # error = JaxRDDLModelError(planner.rddl, planner.test_policy, 
@@ -136,15 +138,15 @@
         slp_replan(env, trials, timeout, timeout_ps, save)
     else: 
         slp_no_replan(env, trials, timeout, timeout_ps, save)
     
         
 if __name__ == "__main__":
     if len(sys.argv) < 6:
-        env, trials, timeout, timeout_ps, save = 'Wildfire replan', 1, 60 * 2, 1, False
+        env, trials, timeout, timeout_ps, save = 'Wildfire', 1, 60 * 2, 1, False
     else:
         env, trials, timeout, timeout_ps, save = sys.argv[1:6]
         trials = int(trials)
         timeout = int(timeout)
         timeout_ps = int(timeout_ps)
         save = save == 'True' or save == True
     replan = env.endswith('replan')
```

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/JaxTuningExample.py` & `pyRDDLGym-1.0.5/pyRDDLGym/JaxTuningExample.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Planner/JaxConfigManager.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Planner/JaxConfigManager.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,39 +9,46 @@
 
 from pyRDDLGym.Core.Env.RDDLEnv import RDDLEnv
 from pyRDDLGym.Core.Jax import JaxRDDLBackpropPlanner
 from pyRDDLGym.Core.Jax import JaxRDDLLogic
 from pyRDDLGym.Examples.ExampleManager import ExampleManager
 
 
-def get(path: str) -> Dict[str, object]:
+def get(path: str, **optional_args) -> Dict[str, object]:
     
     # read the config file
     path = os.path.join(os.path.dirname(os.path.abspath(__file__)), path)
     config = configparser.RawConfigParser()
     config.optionxform = str 
     config.read(path)
     args = {k: literal_eval(v) 
             for section in config.sections()
                 for (k, v) in config.items(section)}
     
     # read the environment settings
     env_args = {k: args[k] for (k, v) in config.items('Environment')}
+    use_repo = env_args.get('check_rddlrepository', False)
+    if 'check_rddlrepository' in env_args:
+        del env_args['check_rddlrepository']
     
     # try to read from rddlrepository
     domain_name = env_args['domain']
     inst_name = env_args['instance']
     try:
-        print(f'reading domain {domain_name} from rddlrepository...')
+        if not use_repo:
+            raise Exception
+        warnings.warn(f'reading domain {domain_name} from rddlrepository...',
+                      stacklevel=2)
         from rddlrepository.Manager.RDDLRepoManager import RDDLRepoManager
         manager = RDDLRepoManager()
         EnvInfo = manager.get_problem(domain_name)
     except:
-        print(f'failed to read from rddlrepository, '
-              f'reading domain {domain_name} from Examples...')
+        warnings.warn(f'failed to read from rddlrepository, '
+                      f'reading domain {domain_name} from Examples...',
+                      stacklevel=2)
         EnvInfo = ExampleManager.GetEnvInfo(domain_name)
     
     env_args['domain'] = EnvInfo.get_domain()
     env_args['instance'] = EnvInfo.get_instance(inst_name)
         
     myEnv = RDDLEnv(**env_args)
     # myEnv.set_visualizer(EnvInfo.get_visualizer())
@@ -64,23 +71,29 @@
                 **opt_args['method_kwargs']['initializer_kwargs'])
         except:
             warnings.warn(f'warning: initializer <{init_method}> '
                           f'cannot take arguments, ignoring them.', stacklevel=2)
         opt_args['method_kwargs']['initializer'] = initializer
         if 'initializer_kwargs' in opt_args['method_kwargs']:
             del opt_args['method_kwargs']['initializer_kwargs']
+            
+    if 'method_kwargs' in opt_args and 'activation' in opt_args['method_kwargs']:
+        opt_args['method_kwargs']['activation'] = getattr(
+            jax.nn, opt_args['method_kwargs']['activation'])
+        
     opt_args['plan'] = getattr(JaxRDDLBackpropPlanner, opt_args['method'])(
         **opt_args['method_kwargs'])
-    opt_args['optimizer'] = getattr(optax, opt_args['optimizer'])(
-        **opt_args['optimizer_kwargs'])    
+    opt_args['optimizer'] = getattr(optax, opt_args['optimizer'])
     opt_args['logic'] = logic
     
     del opt_args['method']
     del opt_args['method_kwargs']
-    del opt_args['optimizer_kwargs']
+    if optional_args is not None:
+        for name, value in optional_args.items():
+            opt_args[name] = value
     optimizer = JaxRDDLBackpropPlanner.JaxRDDLBackpropPlanner(**opt_args)
     
     # read the train/test arguments
     train_args = {k: args[k] for (k, v) in config.items('Training')}
     train_args['key'] = jax.random.PRNGKey(train_args['key'])
     
     return myEnv, optimizer, train_args, (domain_name, inst_name)
```

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Policies/Agents.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Policies/Agents.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Policies/RDDLSimAgent.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Policies/RDDLSimAgent.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/CartPoleViz.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/CartPoleViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/ChartViz.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/ChartViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/ColorViz.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/ColorViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/ElevatorViz.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/ElevatorViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/HVACViz.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/HVACViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/MarsRoverViz.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/MarsRoverViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/MountainCarViz.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/MountainCarViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/MovieGenerator.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/MovieGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/PowerGenViz.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/PowerGenViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/RacecarViz.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/RacecarViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/RecSimViz.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/RecSimViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/ReservoirViz.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/ReservoirViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/StateViz.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/StateViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/TextViz.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/TextViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/TrafficViz.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/TrafficViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/UAVsViz.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/UAVsViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/WildfireViz.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/WildfireViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/Visualizer/visualize_dbn.py` & `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/visualize_dbn.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/XADD/RDDLLevelAnalysisXADD.py` & `pyRDDLGym-1.0.5/pyRDDLGym/XADD/RDDLLevelAnalysisXADD.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/XADD/RDDLModelXADD.py` & `pyRDDLGym-1.0.5/pyRDDLGym/XADD/RDDLModelXADD.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/XADD/RDDLSimulatorXADD.py` & `pyRDDLGym-1.0.5/pyRDDLGym/XADD/RDDLSimulatorXADD.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/testDiscrete.py` & `pyRDDLGym-1.0.5/pyRDDLGym/testDiscrete.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/tests/RDDLGenerator.py` & `pyRDDLGym-1.0.5/pyRDDLGym/tests/RDDLGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/tests/_deprecated.py` & `pyRDDLGym-1.0.5/pyRDDLGym/tests/_deprecated.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/tests/testGymDrone.py` & `pyRDDLGym-1.0.5/pyRDDLGym/tests/testGymDrone.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/tests/testViz.py` & `pyRDDLGym-1.0.5/pyRDDLGym/tests/testViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/tests/test_basic.py` & `pyRDDLGym-1.0.5/pyRDDLGym/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/tests/test_dbn_vis.py` & `pyRDDLGym-1.0.5/pyRDDLGym/tests/test_dbn_vis.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/tests/test_termination.py` & `pyRDDLGym-1.0.5/pyRDDLGym/tests/test_termination.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/tests/test_xadd.py` & `pyRDDLGym-1.0.5/pyRDDLGym/tests/test_xadd.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/tests/unit_test_mars_rover.py` & `pyRDDLGym-1.0.5/pyRDDLGym/tests/unit_test_mars_rover.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym/tests/unit_test_power_gen.py` & `pyRDDLGym-1.0.5/pyRDDLGym/tests/unit_test_power_gen.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym.egg-info/PKG-INFO` & `pyRDDLGym-1.0.5/pyRDDLGym.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pyRDDLGym
-Version: 1.0.4
+Version: 1.0.5
 Summary: pyRDDLGym: RDDL automatic generation tool for OpenAI Gym
 Home-page: https://github.com/ataitler/pyRDDLGym
 Author: Ayal Taitler, Michael Gimelfarb, Scott Sanner, Jihwan Jeong, Sriram Gopalakrishnan, Martin Mladenov, jack liu
-Author-email: ataitler@gmail.com, mike.gimelfarb@mail.utoronto.ca, ssanner@mie.utoronto.ca, jhjeong@mie.utoronto.ca, ariram.gopalakrishnan@jpmchase.com, mmladenov@google.com, xiaotian.liu@mail.utoronto.ca
+Author-email: ataitler@gmail.com, mike.gimelfarb@mail.utoronto.ca, ssanner@mie.utoronto.ca, jhjeong@mie.utoronto.ca, sriram.gopalakrishnan@jpmchase.com, mmladenov@google.com, xiaotian.liu@mail.utoronto.ca
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyRDDLGym-1.0.4/pyRDDLGym.egg-info/SOURCES.txt` & `pyRDDLGym-1.0.5/pyRDDLGym.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE.MD
 MANIFEST.in
 README.md
 setup.py
 pyRDDLGym/GymExample.py
 pyRDDLGym/JaxExample.py
+pyRDDLGym/JaxLossPlotExample.py
 pyRDDLGym/JaxTuningExample.py
 pyRDDLGym/RDDLSimClientExample.py
 pyRDDLGym/__init__.py
 pyRDDLGym/testDiscrete.py
 pyRDDLGym.egg-info/PKG-INFO
 pyRDDLGym.egg-info/SOURCES.txt
 pyRDDLGym.egg-info/dependency_links.txt
```

### Comparing `pyRDDLGym-1.0.4/setup.py` & `pyRDDLGym-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 from setuptools import setup, find_packages
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 setup(
       name='pyRDDLGym',
-      version='1.0.4',
+      version='1.0.5',
       author="Ayal Taitler, Michael Gimelfarb, Scott Sanner, Jihwan Jeong, Sriram Gopalakrishnan, Martin Mladenov, jack liu",
-      author_email="ataitler@gmail.com, mike.gimelfarb@mail.utoronto.ca, ssanner@mie.utoronto.ca, jhjeong@mie.utoronto.ca, ariram.gopalakrishnan@jpmchase.com, mmladenov@google.com, xiaotian.liu@mail.utoronto.ca",
+      author_email="ataitler@gmail.com, mike.gimelfarb@mail.utoronto.ca, ssanner@mie.utoronto.ca, jhjeong@mie.utoronto.ca, sriram.gopalakrishnan@jpmchase.com, mmladenov@google.com, xiaotian.liu@mail.utoronto.ca",
       description="pyRDDLGym: RDDL automatic generation tool for OpenAI Gym",
       # long_description=long_description,
       license="MIT License",
       url="https://github.com/ataitler/pyRDDLGym",
       packages=find_packages(),
       install_requires=['ply', 'pillow>=9.2.0', 'matplotlib>=3.5.0', 'numpy>=1.22', 'gym>=0.24.0', 'pygame'],
       python_requires=">=3.8",
```

