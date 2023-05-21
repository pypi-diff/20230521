# Comparing `tmp/Shiphelm-0.8.0.tar.gz` & `tmp/Shiphelm-0.8.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shiphelm-0.8.0.tar", last modified: Sun Apr 16 21:15:14 2023, max compression
+gzip compressed data, was "Shiphelm-0.8.2a0.tar", last modified: Sun May 21 15:12:21 2023, max compression
```

## Comparing `Shiphelm-0.8.0.tar` & `Shiphelm-0.8.2a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:14.639871 Shiphelm-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-16 21:15:14.639871 Shiphelm-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-16 21:15:14.639871 Shiphelm-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:14.635871 Shiphelm-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:14.639871 Shiphelm-0.8.0/src/Shiphelm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-16 21:15:14.000000 Shiphelm-0.8.0/src/Shiphelm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-16 21:15:14.000000 Shiphelm-0.8.0/src/Shiphelm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 21:15:14.000000 Shiphelm-0.8.0/src/Shiphelm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-16 21:15:14.000000 Shiphelm-0.8.0/src/Shiphelm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-16 21:15:14.000000 Shiphelm-0.8.0/src/Shiphelm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:14.639871 Shiphelm-0.8.0/src/shiphelm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/src/shiphelm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/src/shiphelm/helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/src/shiphelm/helmdocker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/src/shiphelm/helmkube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/src/shiphelm/helmswarm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:14.639871 Shiphelm-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-16 21:14:59.000000 Shiphelm-0.8.0/tests/test_module1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:12:21.937627 Shiphelm-0.8.2a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-21 15:12:06.000000 Shiphelm-0.8.2a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-21 15:12:06.000000 Shiphelm-0.8.2a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-21 15:12:21.937627 Shiphelm-0.8.2a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10507 2023-05-21 15:12:06.000000 Shiphelm-0.8.2a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-21 15:12:06.000000 Shiphelm-0.8.2a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-21 15:12:21.937627 Shiphelm-0.8.2a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-21 15:12:06.000000 Shiphelm-0.8.2a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:12:21.929627 Shiphelm-0.8.2a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:12:21.933627 Shiphelm-0.8.2a0/src/Shiphelm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-21 15:12:21.000000 Shiphelm-0.8.2a0/src/Shiphelm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-21 15:12:21.000000 Shiphelm-0.8.2a0/src/Shiphelm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 15:12:21.000000 Shiphelm-0.8.2a0/src/Shiphelm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-21 15:12:21.000000 Shiphelm-0.8.2a0/src/Shiphelm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 15:12:21.000000 Shiphelm-0.8.2a0/src/Shiphelm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:12:21.937627 Shiphelm-0.8.2a0/src/shiphelm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 15:12:06.000000 Shiphelm-0.8.2a0/src/shiphelm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-05-21 15:12:06.000000 Shiphelm-0.8.2a0/src/shiphelm/helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-21 15:12:06.000000 Shiphelm-0.8.2a0/src/shiphelm/helmdocker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-21 15:12:06.000000 Shiphelm-0.8.2a0/src/shiphelm/helmkube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-21 15:12:06.000000 Shiphelm-0.8.2a0/src/shiphelm/helmswarm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:12:21.937627 Shiphelm-0.8.2a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-21 15:12:06.000000 Shiphelm-0.8.2a0/tests/test_module1.py
```

### Comparing `Shiphelm-0.8.0/LICENSE` & `Shiphelm-0.8.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `Shiphelm-0.8.0/PKG-INFO` & `Shiphelm-0.8.2a0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: Shiphelm
-Version: 0.8.0
-Summary: Docker and kubernetes integration library
-Home-page: https://gameplex-software.github.io/ShipHelm/
-Author: Gameplex Software
-Author-email: info@gameplexsoftware.com
-Keywords: SkiffUI,kubernetes,docker
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 <p align="center">
 <a href="https://gameplex-software.github.io/ShipHelm/">
 <img src="https://user-images.githubusercontent.com/34868944/223447636-3e17dee3-ccdf-44cc-8d42-91378ced6708.png" width="400" />
 </a>
 </p>
 
 # Shiphelm
@@ -181,14 +159,24 @@
     detach=detach,
     ports=ports,
     environment=environment,
     volumes=volumes
 )
 ``` 
 
+### Generate run command
+ShipHelm is capable of retrieving your container's inspect data and re-creating the original command that was used to run your pod, allowing you to re-create it anywhere
+
+```
+container_name = "your_container_name"
+namespace = "your_namespace"  # Default is "default"
+run_command = get_kubernetes_run_command(pod_name, namespace)
+print(f"Run command for pod {pod_name} in namespace {namespace}: {run_command}")
+```
+
 ### Get and Set Environment Variables for a Container
 
 ```
 container_environment = hd.get_container_environment(container_id)
 hd.set_container_environment(container_id, environment)
 ``` 
 
@@ -236,87 +224,97 @@
 This code will allow you to manage any compatible remote container engine
 ```
 from shiphelm.helm import helm
 
 hd = helm.reomte_connect('tcp://remote--host:2375') # create an instance of helm for romote management
 ```
 
-### Get a List of Running Containers
+### Get a List of Running pods
 
 ```
 running_containers = hd.get_running_containers()
 ``` 
 
-### Get Stats and Ports for a Container by ID
+### Get Stats and Ports for a pod by ID
 
 ```
 container_stats = hd.get_container_stats(container_id)
 container_ports = hd.get_container_ports(container_id)
 ```
 
-### Search for Containers by Name
+### Search for pods by Name
 
 ```
 containers_by_name = hd.search_containers(name)
 ``` 
 
-### Change the Ports of a Container
+### Change the Ports of a pod
 
 ```
 hd.change_container_ports(container_id, ports)
 ``` 
 
-### Rename a Container
+### Rename a pod
 
 ```
 hd.rename_container(container_id, new_name)
 ``` 
 
-### Add and Remove Containers from Networks
+### Add and Remove pods from Networks
 
 ```
 hd.add_container_to_network(container_id, network_name)
 hd.remove_container_from_network(container_id, network_name)
 ``` 
 
 ### Create and Delete Networks
 
 ```
 hd.create_network(network_name)
 hd.delete_network(network_name)
 ``` 
 
-### Run a New Container
+### Run a New pod
 
 ```
 container = hd.run_container(
     image=image,
     command=command,
     detach=detach,
     ports=ports,
     environment=environment,
     volumes=volumes
 )
 ``` 
 
-### Get and Set Environment Variables for a Container
+### Generate run command
+ShipHelm is capable of retrieving your pod's inspect data and re-creating the original command that was used to run your pod, allowing you to re-create it anywhere
+
+```
+pod_name = "your_pod_name"
+namespace = "your_namespace"  # Default is "default"
+run_command = get_kubernetes_run_command(pod_name, namespace)
+print(f"Run command for pod {pod_name} in namespace {namespace}: {run_command}")
+```
+
+### Get and Set Environment Variables for a pod
 
 ```
 container_environment = hd.get_container_environment(container_id)
 hd.set_container_environment(container_id, environment)
 ``` 
 
-### Get and Set Volumes for a Container
+### Get and Set Volumes for a pod
 
 ```
 container_volumes = hd.get_container_volumes(container_id)
 hd.set_container_volumes(container_id, volumes)
 ```
 ### Example code
-This example runs 4 instances of the  "Getting Started" container
+This example runs 4 instances of the  "Getting Started" pod
 
 ```
 from shiphelm.helm import helm
 
 hd = helm() # create an instance of helm
 container_list = hd.get_running_containers() # call the method on the instance
 print(container_list)
@@ -329,15 +327,15 @@
 
 print("Your server is up and ready for connection!")
 ```
 
 ## Dynamic engine selection
 You may have noticed that the syntax for controling both Docker and Kubernetes are identical, the way the code you write for ShipHelm is run depends on the engine you selected last.
 
-In the last example we used the follwing code to initilise ShipHelm, create an alias, and select a container engine:
+In the last example we used the follwing code to initilise ShipHelm, create an alias, and select a pod engine:
 
 ```
 from shiphelm.helm import helm
 
 hd = helm.helm() # create an instance of helm
 
 helm.set_engine_manual("kubernetes")
```

#### html2text {}

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1 Name: Shiphelm Version: 0.8.0 Summary: Docker and
-kubernetes integration library Home-page: https://gameplex-software.github.io/
-ShipHelm/ Author: Gameplex Software Author-email: info@gameplexsoftware.com
-Keywords: SkiffUI,kubernetes,docker Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
-:: Software Development :: Build Tools Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: dev License-File:
-LICENSE
  [https://user-images.githubusercontent.com/34868944/223447636-3e17dee3-ccdf-
                           44cc-8d42-91378ced6708.png]
 # Shiphelm ## Table of Contents - [Shiphelm](#shiphelm) - [Installation]
 (#installation) - [Docker usage example](#docker-usage-example) - [Get a List
 of Running Containers](#get-a-list-of-running-containers) - [Get a running
 container by ID](#get-a-running-container-by-id) - [Get Stats and Ports for a
 Container by ID](#get-stats-and-ports-for-a-container-by-id) - [Search for
@@ -68,16 +56,22 @@
 ports) ``` ### Rename a Container ``` hd.rename_container(container_id,
 new_name) ``` ### Add and Remove Containers from Networks ```
 hd.add_container_to_network(container_id, network_name)
 hd.remove_container_from_network(container_id, network_name) ``` ### Create and
 Delete Networks ``` hd.create_network(network_name) hd.delete_network
 (network_name) ``` ### Run a New Container ``` container = hd.run_container
 ( image=image, command=command, detach=detach, ports=ports,
-environment=environment, volumes=volumes ) ``` ### Get and Set Environment
-Variables for a Container ``` container_environment =
+environment=environment, volumes=volumes ) ``` ### Generate run command
+ShipHelm is capable of retrieving your container's inspect data and re-creating
+the original command that was used to run your pod, allowing you to re-create
+it anywhere ``` container_name = "your_container_name" namespace =
+"your_namespace" # Default is "default" run_command =
+get_kubernetes_run_command(pod_name, namespace) print(f"Run command for pod
+{pod_name} in namespace {namespace}: {run_command}") ``` ### Get and Set
+Environment Variables for a Container ``` container_environment =
 hd.get_container_environment(container_id) hd.set_container_environment
 (container_id, environment) ``` ### Get and Set Volumes for a Container ```
 container_volumes = hd.get_container_volumes(container_id)
 hd.set_container_volumes(container_id, volumes) ``` ### Example code This
 example runs 4 instances of the Docker "Getting Started" container ``` from
 shiphelm.helmdocker import helmdocker hd = helmdocker() # create an instance of
 helmdocker container_list = hd.get_running_containers() # call the method on
@@ -88,43 +82,48 @@
                           4b8a-abb3-8aee93f57bf9.png]
 ## Kubernetes (K8S) usage example This code will allow you to manage the local
 container engine ``` from shiphelm.helm import helm hd = helm.helm() # create
 an instance of helm helm.set_engine_manual("kubernetes") ``` This code will
 allow you to manage any compatible remote container engine ``` from
 shiphelm.helm import helm hd = helm.reomte_connect('tcp://remote--host:2375') #
 create an instance of helm for romote management ``` ### Get a List of Running
-Containers ``` running_containers = hd.get_running_containers() ``` ### Get
-Stats and Ports for a Container by ID ``` container_stats =
-hd.get_container_stats(container_id) container_ports = hd.get_container_ports
-(container_id) ``` ### Search for Containers by Name ``` containers_by_name =
-hd.search_containers(name) ``` ### Change the Ports of a Container ```
-hd.change_container_ports(container_id, ports) ``` ### Rename a Container ```
-hd.rename_container(container_id, new_name) ``` ### Add and Remove Containers
-from Networks ``` hd.add_container_to_network(container_id, network_name)
-hd.remove_container_from_network(container_id, network_name) ``` ### Create and
-Delete Networks ``` hd.create_network(network_name) hd.delete_network
-(network_name) ``` ### Run a New Container ``` container = hd.run_container
-( image=image, command=command, detach=detach, ports=ports,
-environment=environment, volumes=volumes ) ``` ### Get and Set Environment
-Variables for a Container ``` container_environment =
+pods ``` running_containers = hd.get_running_containers() ``` ### Get Stats and
+Ports for a pod by ID ``` container_stats = hd.get_container_stats
+(container_id) container_ports = hd.get_container_ports(container_id) ``` ###
+Search for pods by Name ``` containers_by_name = hd.search_containers(name) ```
+### Change the Ports of a pod ``` hd.change_container_ports(container_id,
+ports) ``` ### Rename a pod ``` hd.rename_container(container_id, new_name) ```
+### Add and Remove pods from Networks ``` hd.add_container_to_network
+(container_id, network_name) hd.remove_container_from_network(container_id,
+network_name) ``` ### Create and Delete Networks ``` hd.create_network
+(network_name) hd.delete_network(network_name) ``` ### Run a New pod ```
+container = hd.run_container( image=image, command=command, detach=detach,
+ports=ports, environment=environment, volumes=volumes ) ``` ### Generate run
+command ShipHelm is capable of retrieving your pod's inspect data and re-
+creating the original command that was used to run your pod, allowing you to
+re-create it anywhere ``` pod_name = "your_pod_name" namespace =
+"your_namespace" # Default is "default" run_command =
+get_kubernetes_run_command(pod_name, namespace) print(f"Run command for pod
+{pod_name} in namespace {namespace}: {run_command}") ``` ### Get and Set
+Environment Variables for a pod ``` container_environment =
 hd.get_container_environment(container_id) hd.set_container_environment
-(container_id, environment) ``` ### Get and Set Volumes for a Container ```
+(container_id, environment) ``` ### Get and Set Volumes for a pod ```
 container_volumes = hd.get_container_volumes(container_id)
 hd.set_container_volumes(container_id, volumes) ``` ### Example code This
-example runs 4 instances of the "Getting Started" container ``` from
-shiphelm.helm import helm hd = helm() # create an instance of helm
-container_list = hd.get_running_containers() # call the method on the instance
-print(container_list) w=0 print("Preparing new server...") while w<3:
+example runs 4 instances of the "Getting Started" pod ``` from shiphelm.helm
+import helm hd = helm() # create an instance of helm container_list =
+hd.get_running_containers() # call the method on the instance print
+(container_list) w=0 print("Preparing new server...") while w<3:
 hd.run_container(image="ollyw123/helloworld", detach=1) w=w+1 print("Your
 server is up and ready for connection!") ``` ## Dynamic engine selection You
 may have noticed that the syntax for controling both Docker and Kubernetes are
 identical, the way the code you write for ShipHelm is run depends on the engine
 you selected last. In the last example we used the follwing code to initilise
-ShipHelm, create an alias, and select a container engine: ``` from
-shiphelm.helm import helm hd = helm.helm() # create an instance of helm
+ShipHelm, create an alias, and select a pod engine: ``` from shiphelm.helm
+import helm hd = helm.helm() # create an instance of helm
 helm.set_engine_manual("kubernetes") ``` f you want your cod to be able to use
 either engine that it detects locally you can use the following code instead:
 ``` from shiphelm.helm import helm hd = helm.helm() # create an instance of
 helm helm.set_engine_auto() ``` ## Remote engines via GUI To use remote engines
 you can use the following the examples above to connect programatically or use
 the below code to open a GUI configuration wizard: ``` from shiphelm.helm
 import helm hd = helm.helm() # create an instance of helm helm.remote_popup()
```

### Comparing `Shiphelm-0.8.0/setup.py` & `Shiphelm-0.8.2a0/setup.py`

 * *Files identical despite different names*

### Comparing `Shiphelm-0.8.0/src/Shiphelm.egg-info/PKG-INFO` & `Shiphelm-0.8.2a0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shiphelm
-Version: 0.8.0
+Version: 0.8.2a0
 Summary: Docker and kubernetes integration library
 Home-page: https://gameplex-software.github.io/ShipHelm/
 Author: Gameplex Software
 Author-email: info@gameplexsoftware.com
 Keywords: SkiffUI,kubernetes,docker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -181,14 +181,24 @@
     detach=detach,
     ports=ports,
     environment=environment,
     volumes=volumes
 )
 ``` 
 
+### Generate run command
+ShipHelm is capable of retrieving your container's inspect data and re-creating the original command that was used to run your pod, allowing you to re-create it anywhere
+
+```
+container_name = "your_container_name"
+namespace = "your_namespace"  # Default is "default"
+run_command = get_kubernetes_run_command(pod_name, namespace)
+print(f"Run command for pod {pod_name} in namespace {namespace}: {run_command}")
+```
+
 ### Get and Set Environment Variables for a Container
 
 ```
 container_environment = hd.get_container_environment(container_id)
 hd.set_container_environment(container_id, environment)
 ``` 
 
@@ -236,87 +246,97 @@
 This code will allow you to manage any compatible remote container engine
 ```
 from shiphelm.helm import helm
 
 hd = helm.reomte_connect('tcp://remote--host:2375') # create an instance of helm for romote management
 ```
 
-### Get a List of Running Containers
+### Get a List of Running pods
 
 ```
 running_containers = hd.get_running_containers()
 ``` 
 
-### Get Stats and Ports for a Container by ID
+### Get Stats and Ports for a pod by ID
 
 ```
 container_stats = hd.get_container_stats(container_id)
 container_ports = hd.get_container_ports(container_id)
 ```
 
-### Search for Containers by Name
+### Search for pods by Name
 
 ```
 containers_by_name = hd.search_containers(name)
 ``` 
 
-### Change the Ports of a Container
+### Change the Ports of a pod
 
 ```
 hd.change_container_ports(container_id, ports)
 ``` 
 
-### Rename a Container
+### Rename a pod
 
 ```
 hd.rename_container(container_id, new_name)
 ``` 
 
-### Add and Remove Containers from Networks
+### Add and Remove pods from Networks
 
 ```
 hd.add_container_to_network(container_id, network_name)
 hd.remove_container_from_network(container_id, network_name)
 ``` 
 
 ### Create and Delete Networks
 
 ```
 hd.create_network(network_name)
 hd.delete_network(network_name)
 ``` 
 
-### Run a New Container
+### Run a New pod
 
 ```
 container = hd.run_container(
     image=image,
     command=command,
     detach=detach,
     ports=ports,
     environment=environment,
     volumes=volumes
 )
 ``` 
 
-### Get and Set Environment Variables for a Container
+### Generate run command
+ShipHelm is capable of retrieving your pod's inspect data and re-creating the original command that was used to run your pod, allowing you to re-create it anywhere
+
+```
+pod_name = "your_pod_name"
+namespace = "your_namespace"  # Default is "default"
+run_command = get_kubernetes_run_command(pod_name, namespace)
+print(f"Run command for pod {pod_name} in namespace {namespace}: {run_command}")
+```
+
+### Get and Set Environment Variables for a pod
 
 ```
 container_environment = hd.get_container_environment(container_id)
 hd.set_container_environment(container_id, environment)
 ``` 
 
-### Get and Set Volumes for a Container
+### Get and Set Volumes for a pod
 
 ```
 container_volumes = hd.get_container_volumes(container_id)
 hd.set_container_volumes(container_id, volumes)
 ```
 ### Example code
-This example runs 4 instances of the  "Getting Started" container
+This example runs 4 instances of the  "Getting Started" pod
 
 ```
 from shiphelm.helm import helm
 
 hd = helm() # create an instance of helm
 container_list = hd.get_running_containers() # call the method on the instance
 print(container_list)
@@ -329,15 +349,15 @@
 
 print("Your server is up and ready for connection!")
 ```
 
 ## Dynamic engine selection
 You may have noticed that the syntax for controling both Docker and Kubernetes are identical, the way the code you write for ShipHelm is run depends on the engine you selected last.
 
-In the last example we used the follwing code to initilise ShipHelm, create an alias, and select a container engine:
+In the last example we used the follwing code to initilise ShipHelm, create an alias, and select a pod engine:
 
 ```
 from shiphelm.helm import helm
 
 hd = helm.helm() # create an instance of helm
 
 helm.set_engine_manual("kubernetes")
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Shiphelm Version: 0.8.0 Summary: Docker and
+Metadata-Version: 2.1 Name: Shiphelm Version: 0.8.2a0 Summary: Docker and
 kubernetes integration library Home-page: https://gameplex-software.github.io/
 ShipHelm/ Author: Gameplex Software Author-email: info@gameplexsoftware.com
 Keywords: SkiffUI,kubernetes,docker Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
@@ -68,16 +68,22 @@
 ports) ``` ### Rename a Container ``` hd.rename_container(container_id,
 new_name) ``` ### Add and Remove Containers from Networks ```
 hd.add_container_to_network(container_id, network_name)
 hd.remove_container_from_network(container_id, network_name) ``` ### Create and
 Delete Networks ``` hd.create_network(network_name) hd.delete_network
 (network_name) ``` ### Run a New Container ``` container = hd.run_container
 ( image=image, command=command, detach=detach, ports=ports,
-environment=environment, volumes=volumes ) ``` ### Get and Set Environment
-Variables for a Container ``` container_environment =
+environment=environment, volumes=volumes ) ``` ### Generate run command
+ShipHelm is capable of retrieving your container's inspect data and re-creating
+the original command that was used to run your pod, allowing you to re-create
+it anywhere ``` container_name = "your_container_name" namespace =
+"your_namespace" # Default is "default" run_command =
+get_kubernetes_run_command(pod_name, namespace) print(f"Run command for pod
+{pod_name} in namespace {namespace}: {run_command}") ``` ### Get and Set
+Environment Variables for a Container ``` container_environment =
 hd.get_container_environment(container_id) hd.set_container_environment
 (container_id, environment) ``` ### Get and Set Volumes for a Container ```
 container_volumes = hd.get_container_volumes(container_id)
 hd.set_container_volumes(container_id, volumes) ``` ### Example code This
 example runs 4 instances of the Docker "Getting Started" container ``` from
 shiphelm.helmdocker import helmdocker hd = helmdocker() # create an instance of
 helmdocker container_list = hd.get_running_containers() # call the method on
@@ -88,43 +94,48 @@
                           4b8a-abb3-8aee93f57bf9.png]
 ## Kubernetes (K8S) usage example This code will allow you to manage the local
 container engine ``` from shiphelm.helm import helm hd = helm.helm() # create
 an instance of helm helm.set_engine_manual("kubernetes") ``` This code will
 allow you to manage any compatible remote container engine ``` from
 shiphelm.helm import helm hd = helm.reomte_connect('tcp://remote--host:2375') #
 create an instance of helm for romote management ``` ### Get a List of Running
-Containers ``` running_containers = hd.get_running_containers() ``` ### Get
-Stats and Ports for a Container by ID ``` container_stats =
-hd.get_container_stats(container_id) container_ports = hd.get_container_ports
-(container_id) ``` ### Search for Containers by Name ``` containers_by_name =
-hd.search_containers(name) ``` ### Change the Ports of a Container ```
-hd.change_container_ports(container_id, ports) ``` ### Rename a Container ```
-hd.rename_container(container_id, new_name) ``` ### Add and Remove Containers
-from Networks ``` hd.add_container_to_network(container_id, network_name)
-hd.remove_container_from_network(container_id, network_name) ``` ### Create and
-Delete Networks ``` hd.create_network(network_name) hd.delete_network
-(network_name) ``` ### Run a New Container ``` container = hd.run_container
-( image=image, command=command, detach=detach, ports=ports,
-environment=environment, volumes=volumes ) ``` ### Get and Set Environment
-Variables for a Container ``` container_environment =
+pods ``` running_containers = hd.get_running_containers() ``` ### Get Stats and
+Ports for a pod by ID ``` container_stats = hd.get_container_stats
+(container_id) container_ports = hd.get_container_ports(container_id) ``` ###
+Search for pods by Name ``` containers_by_name = hd.search_containers(name) ```
+### Change the Ports of a pod ``` hd.change_container_ports(container_id,
+ports) ``` ### Rename a pod ``` hd.rename_container(container_id, new_name) ```
+### Add and Remove pods from Networks ``` hd.add_container_to_network
+(container_id, network_name) hd.remove_container_from_network(container_id,
+network_name) ``` ### Create and Delete Networks ``` hd.create_network
+(network_name) hd.delete_network(network_name) ``` ### Run a New pod ```
+container = hd.run_container( image=image, command=command, detach=detach,
+ports=ports, environment=environment, volumes=volumes ) ``` ### Generate run
+command ShipHelm is capable of retrieving your pod's inspect data and re-
+creating the original command that was used to run your pod, allowing you to
+re-create it anywhere ``` pod_name = "your_pod_name" namespace =
+"your_namespace" # Default is "default" run_command =
+get_kubernetes_run_command(pod_name, namespace) print(f"Run command for pod
+{pod_name} in namespace {namespace}: {run_command}") ``` ### Get and Set
+Environment Variables for a pod ``` container_environment =
 hd.get_container_environment(container_id) hd.set_container_environment
-(container_id, environment) ``` ### Get and Set Volumes for a Container ```
+(container_id, environment) ``` ### Get and Set Volumes for a pod ```
 container_volumes = hd.get_container_volumes(container_id)
 hd.set_container_volumes(container_id, volumes) ``` ### Example code This
-example runs 4 instances of the "Getting Started" container ``` from
-shiphelm.helm import helm hd = helm() # create an instance of helm
-container_list = hd.get_running_containers() # call the method on the instance
-print(container_list) w=0 print("Preparing new server...") while w<3:
+example runs 4 instances of the "Getting Started" pod ``` from shiphelm.helm
+import helm hd = helm() # create an instance of helm container_list =
+hd.get_running_containers() # call the method on the instance print
+(container_list) w=0 print("Preparing new server...") while w<3:
 hd.run_container(image="ollyw123/helloworld", detach=1) w=w+1 print("Your
 server is up and ready for connection!") ``` ## Dynamic engine selection You
 may have noticed that the syntax for controling both Docker and Kubernetes are
 identical, the way the code you write for ShipHelm is run depends on the engine
 you selected last. In the last example we used the follwing code to initilise
-ShipHelm, create an alias, and select a container engine: ``` from
-shiphelm.helm import helm hd = helm.helm() # create an instance of helm
+ShipHelm, create an alias, and select a pod engine: ``` from shiphelm.helm
+import helm hd = helm.helm() # create an instance of helm
 helm.set_engine_manual("kubernetes") ``` f you want your cod to be able to use
 either engine that it detects locally you can use the following code instead:
 ``` from shiphelm.helm import helm hd = helm.helm() # create an instance of
 helm helm.set_engine_auto() ``` ## Remote engines via GUI To use remote engines
 you can use the following the examples above to connect programatically or use
 the below code to open a GUI configuration wizard: ``` from shiphelm.helm
 import helm hd = helm.helm() # create an instance of helm helm.remote_popup()
```

### Comparing `Shiphelm-0.8.0/src/shiphelm/helm.py` & `Shiphelm-0.8.2a0/src/shiphelm/helm.py`

 * *Files identical despite different names*

### Comparing `Shiphelm-0.8.0/src/shiphelm/helmdocker.py` & `Shiphelm-0.8.2a0/src/shiphelm/helmdocker.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,7 +93,18 @@
         volumes = container.attrs['HostConfig']['Binds']
         return volumes
 
     def set_container_volumes(self, container_id, volumes):
         container = helmdocker.client.containers.get(container_id)
         container.reload()
         container.update(binds=volumes)
+
+    def get_run_command(self, container_id):
+        client = docker.from_env()
+        try:
+            container = client.containers.get(container_id)
+            command = ' '.join(container.attrs['Path']) + ' ' + ' '.join(container.attrs['Args'])
+            return command
+        except docker.errors.NotFound:
+            return f"Container {container_id} not found"
+        except docker.errors.APIError as e:
+            return f"Error: {e}"
```

### Comparing `Shiphelm-0.8.0/src/shiphelm/helmkube.py` & `Shiphelm-0.8.2a0/src/shiphelm/helmkube.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,121 +11,143 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ----------------------------------------------------------------------------
 
 from kubernetes import client, config
+import json
 
 class helmkube:
-    def __init__(self, remote_address = None, remote_is_TLS = None):
+    def __init__(self, remote_address = None, remote_is_TLS = None, namespace="default"):
         try:
             helmkube.kubeclient = client
             config.load_kube_config()
             helmkube.api_client = helmkube.kubeclient.ApiClient()
-            namespace = "default"  # modify as needed
         except:
             pass
             #Finish: Remote Kubernetes connection
 
-    def get_running_containers(self):
+    def get_running_containers(self, namespace="default"):
         api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
         pods = api_instance.list_pod_for_all_namespaces(watch=False)
         containers = []
         for pod in pods.items:
             for container in pod.spec.containers:
                 containers.append(container)
         return containers
 
-    def get_container_by_id(self, container_id):
+    def get_container_by_id(self, container_id, namespace="default"):
         return self.get_container_by_id(container_id)
 
-    def get_container_stats(self, container_id):
+    def get_container_stats(self, container_id, namespace="default"):
         api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
-        namespace = "default"  # modify as needed
+        
         pod_name = container_id  # use container ID as pod name
         container_name = container_id  # use container ID as container name
         container_stats = api_instance.read_namespaced_pod_container_status(
             name=pod_name,
             namespace=namespace,
             container=container_name
         )
         return container_stats
 
-    def get_container_ports(self, container_id):
+    def get_container_ports(self, container_id, namespace="default"):
         api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
-        namespace = "default"  # modify as needed
+        
         pod_name = container_id  # use container ID as pod name
         container_name = container_id  # use container ID as container name
         container = api_instance.read_namespaced_pod(
             name=pod_name,
             namespace=namespace
         )
         ports = container.spec.containers[0].ports
         return ports
 
-    def search_containers(self, name):
+    def search_containers(self, name, namespace="default"):
         api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
-        namespace = "default"  # modify as needed
+        
         label_selector = f"name={name}"
         pods = api_instance.list_namespaced_pod(
             namespace=namespace,
             label_selector=label_selector
         )
         containers = []
         for pod in pods.items:
             for container in pod.spec.containers:
                 containers.append(container)
         return containers
 
-    def change_container_ports(self, container_id, ports):
+    def change_container_ports(self, container_id, ports, namespace="default"):
         api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
-        namespace = "default"  # modify as needed
+        
         pod_name = container_id  # use container ID as pod name
         container_name = container_id  # use container ID as container name
         container = api_instance.read_namespaced_pod(
             name=pod_name,
             namespace=namespace
         )
         container.spec.containers[0].ports = ports
         api_instance.patch_namespaced_pod(
             name=pod_name,
             namespace=namespace,
             body=container
         )
 
-    def rename_container(self, container_id, new_name):
+    def rename_container(self, container_id, new_name, namespace="default"):
         api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
-        namespace = "default"  # modify as needed
         pod_name = container_id  # use container ID as pod name
         container_name = container_id  # use container ID as container name
         container = api_instance.read_namespaced_pod(
             name=pod_name,
             namespace=namespace
         )
         container.metadata.name = new_name
         api_instance.replace_namespaced_pod(
             name=pod_name,
             namespace=namespace,
             body=container
         )
+    
+    def get_run_command(container_id, namespace="default"):
+        config.load_kube_config()  # Loads kubeconfig file from default location or from environment variables
+        try:
+            api_instance = client.CoreV1Api()
+            pod = api_instance.read_namespaced_pod(id=container_id, namespace=namespace)
+
+            # Convert container command to string
+            container = pod.spec.containers[0]
+            command = " ".join(container.command)
+
+            # Convert container arguments to string
+            args = " ".join(container.args)
+
+            run_command = f"{command} {args}"
+            return run_command
+        except client.exceptions.ApiException as e:
+            error_message = json.loads(e.body)["message"]
+            return f"Error: {error_message}"
+        except IndexError:
+            return f"Pod {container_name} does not have any containers"
+        except Exception as e:
+            return f"Error: {str(e)}"
 
     @staticmethod
-    def add_container_to_network(self, container_id, network_name):
+    def add_container_to_network(self, container_id, network_name, namespace="default"):
         # Kubernetes has a different networking model, so this method is not applicable
         pass
 
     @staticmethod
-    def remove_container_from_network(self, container_id, network_name):
+    def remove_container_from_network(self, container_id, network_name, namespace="default"):
         # Kubernetes has a different networking model, so this method is not applicable
         pass
 
     @staticmethod
-    def create_service(self, service_name, app_name, container_port):
-        namespace = "default"  # modify as needed
+    def create_service(self, service_name, app_name, container_port, namespace="default"):
+        
         v1 = helmkube.kubeclient.CoreV1Api()
         service_manifest = {
             "apiVersion": "v1",
             "kind": "Service",
             "metadata": {
                 "name": service_name,
             },
@@ -142,13 +164,13 @@
                 ],
                 "type": "ClusterIP"
             }
         }
         v1.create_namespaced_service(namespace, service_manifest)
 
     @staticmethod
-    def set_container_volumes(self, container_name, volumes):
-        namespace = "default"  # modify as needed
+    def set_container_volumes(self, container_name, volumes, namespace="default"):
+        
         v1 = helmkube.kubeclient.CoreV1Api()
         container = v1.read_namespaced_pod(container_name, namespace)
         container.spec.volumes = volumes
         v1.replace_namespaced_pod(container_name, namespace, container)
```

### Comparing `Shiphelm-0.8.0/src/shiphelm/helmswarm.py` & `Shiphelm-0.8.2a0/src/shiphelm/helmswarm.py`

 * *Files identical despite different names*

