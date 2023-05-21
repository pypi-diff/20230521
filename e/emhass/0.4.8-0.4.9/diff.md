# Comparing `tmp/emhass-0.4.8-py3-none-any.whl.zip` & `tmp/emhass-0.4.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 51988 bytes, number of entries: 15
+Zip file size: 52683 bytes, number of entries: 15
 -rw-rw-r--  2.0 unx        0 b- defN 22-Mar-05 11:24 emhass/__init__.py
--rw-rw-r--  2.0 unx    33594 b- defN 23-Mar-10 18:04 emhass/command_line.py
+-rw-rw-r--  2.0 unx    34580 b- defN 23-May-14 16:22 emhass/command_line.py
 -rw-rw-r--  2.0 unx    43072 b- defN 23-Mar-17 07:44 emhass/forecast.py
--rw-rw-r--  2.0 unx    14966 b- defN 23-Mar-06 20:51 emhass/machine_learning_forecaster.py
+-rw-rw-r--  2.0 unx    14964 b- defN 23-May-14 15:59 emhass/machine_learning_forecaster.py
 -rw-rw-r--  2.0 unx    30582 b- defN 23-Mar-05 16:55 emhass/optimization.py
 -rw-rw-r--  2.0 unx    15888 b- defN 23-Mar-06 21:25 emhass/retrieve_hass.py
--rw-rw-r--  2.0 unx    22445 b- defN 23-Mar-10 17:38 emhass/utils.py
+-rw-rw-r--  2.0 unx    23107 b- defN 23-May-14 16:13 emhass/utils.py
 -rw-rw-r--  2.0 unx    18255 b- defN 23-Mar-10 18:05 emhass/web_server.py
 -rw-rw-r--  2.0 unx     6760 b- defN 22-May-19 14:34 emhass/static/style.css
 -rw-rw-r--  2.0 unx     6615 b- defN 23-Mar-10 22:01 emhass/templates/index.html
--rw-rw-r--  2.0 unx    24995 b- defN 23-Mar-17 07:46 emhass-0.4.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-17 07:46 emhass-0.4.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       53 b- defN 23-Mar-17 07:46 emhass-0.4.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        7 b- defN 23-Mar-17 07:46 emhass-0.4.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1187 b- defN 23-Mar-17 07:46 emhass-0.4.8.dist-info/RECORD
-15 files, 218511 bytes uncompressed, 50050 bytes compressed:  77.1%
+-rw-rw-r--  2.0 unx    27317 b- defN 23-May-20 16:17 emhass-0.4.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-20 16:17 emhass-0.4.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       53 b- defN 23-May-20 16:17 emhass-0.4.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-20 16:17 emhass-0.4.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1187 b- defN 23-May-20 16:17 emhass-0.4.9.dist-info/RECORD
+15 files, 222479 bytes uncompressed, 50745 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: emhass/static/style.css
 Comment: 
 
 Filename: emhass/templates/index.html
 Comment: 
 
-Filename: emhass-0.4.8.dist-info/METADATA
+Filename: emhass-0.4.9.dist-info/METADATA
 Comment: 
 
-Filename: emhass-0.4.8.dist-info/WHEEL
+Filename: emhass-0.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: emhass-0.4.8.dist-info/entry_points.txt
+Filename: emhass-0.4.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: emhass-0.4.8.dist-info/top_level.txt
+Filename: emhass-0.4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: emhass-0.4.8.dist-info/RECORD
+Filename: emhass-0.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## emhass/command_line.py

```diff
@@ -513,14 +513,28 @@
     # Publish total value of cost function
     custom_cost_fun_id = params['passed_data']['custom_cost_fun_id']
     col_cost_fun = [i for i in opt_res_latest.columns if 'cost_fun_' in i]
     input_data_dict['rh'].post_data(opt_res_latest[col_cost_fun], idx_closest, 
                                     custom_cost_fun_id["entity_id"], 
                                     custom_cost_fun_id["unit_of_measurement"],
                                     custom_cost_fun_id["friendly_name"])
+    # Publish unit_load_cost
+    custom_unit_load_cost_id = params['passed_data']['custom_unit_load_cost_id']
+    input_data_dict['rh'].post_data(opt_res_latest['unit_load_cost'], idx_closest, 
+                                    custom_unit_load_cost_id["entity_id"], 
+                                    custom_unit_load_cost_id["unit_of_measurement"],
+                                    custom_unit_load_cost_id["friendly_name"])
+    cols_published = cols_published+["unit_load_cost"]
+    # Publish unit_prod_price
+    custom_unit_prod_price_id = params['passed_data']['custom_unit_prod_price_id']
+    input_data_dict['rh'].post_data(opt_res_latest['unit_prod_price'], idx_closest, 
+                                    custom_unit_prod_price_id["entity_id"], 
+                                    custom_unit_prod_price_id["unit_of_measurement"],
+                                    custom_unit_prod_price_id["friendly_name"])
+    cols_published = cols_published+["unit_prod_price"]
     # Create a DF resuming what has been published
     opt_res = opt_res_latest[cols_published].loc[[opt_res_latest.index[idx_closest]]]
     return opt_res
     
         
 def main():
     r"""Define the main command line entry function.
```

## emhass/machine_learning_forecaster.py

```diff
@@ -113,15 +113,15 @@
         self.logger.info("Performing a forecast model fit for "+self.model_type)
         # Preparing the data: adding exogenous features
         self.data_exo = pd.DataFrame(index=self.data.index)
         self.data_exo = mlforecaster.add_date_features(self.data_exo)
         self.data_exo[self.var_model] = self.data[self.var_model]
         self.data_exo = self.data_exo.interpolate(method='linear', axis=0, limit=None)
         # train/test split
-        self.date_train = self.data_exo.index[-1]-pd.Timedelta('15days')+self.data_exo.index.freq # The last 15 days
+        self.date_train = self.data_exo.index[-1]-pd.Timedelta('5days')+self.data_exo.index.freq # The last 5 days
         self.date_split = self.data_exo.index[-1]-pd.Timedelta(split_date_delta)+self.data_exo.index.freq # The last 48h
         self.data_train = self.data_exo.loc[:self.date_split,:]
         self.data_test  = self.data_exo.loc[self.date_split:,:]
         self.steps = len(self.data_test)
         # Pick correct sklearn model
         if self.sklearn_model == 'LinearRegression':
             base_model = LinearRegression()
```

## emhass/utils.py

```diff
@@ -132,14 +132,16 @@
         })
     default_passed_dict = {'custom_pv_forecast_id': {"entity_id": "sensor.p_pv_forecast", "unit_of_measurement": "W", "friendly_name": "PV Power Forecast"},
                            'custom_load_forecast_id': {"entity_id": "sensor.p_load_forecast", "unit_of_measurement": "W", "friendly_name": "Load Power Forecast"},
                            'custom_batt_forecast_id': {"entity_id": "sensor.p_batt_forecast", "unit_of_measurement": "W", "friendly_name": "Battery Power Forecast"},
                            'custom_batt_soc_forecast_id': {"entity_id": "sensor.soc_batt_forecast", "unit_of_measurement": "%", "friendly_name": "Battery SOC Forecast"},
                            'custom_grid_forecast_id': {"entity_id": "sensor.p_grid_forecast", "unit_of_measurement": "W", "friendly_name": "Grid Power Forecast"},
                            'custom_cost_fun_id': {"entity_id": "sensor.total_cost_fun_value", "unit_of_measurement": "", "friendly_name": "Total cost function value"},
+                           'custom_unit_load_cost_id': {"entity_id": "sensor.unit_load_cost", "unit_of_measurement": "€", "friendly_name": "Unit Load Cost"},
+                           'custom_unit_prod_price_id': {"entity_id": "sensor.unit_load_cost", "unit_of_measurement": "€", "friendly_name": "Unit Prod Price"},
                            'custom_deferrable_forecast_id': custom_deferrable_forecast_id}
     if 'passed_data' in params.keys():
         for key, value in default_passed_dict.items():
             params['passed_data'][key] = value
     else:
         params['passed_data'] = default_passed_dict
     if runtimeparams is not None:
@@ -242,15 +244,15 @@
                 logger.warning("There are non numeric values on the passed data for prod_price_forecast, check for missing values (nans, null, etc)")
                 for x in list_non_digits:
                     logger.warning("This value in prod_price_forecast was detected as non digits: "+str(x))
         else:
             params['passed_data']['prod_price_forecast'] = None
         # Treat passed data for forecast model fit/predict/tune at runtime
         if 'days_to_retrieve' not in runtimeparams.keys():
-            days_to_retrieve = 30
+            days_to_retrieve = 9
         else:
             days_to_retrieve = runtimeparams['days_to_retrieve']
         params['passed_data']['days_to_retrieve'] = days_to_retrieve
         if 'model_type' not in runtimeparams.keys():
             model_type = "load_forecast"
         else:
             model_type = runtimeparams['model_type']
@@ -329,14 +331,18 @@
             params['passed_data']['custom_batt_forecast_id'] = runtimeparams['custom_batt_forecast_id']
         if 'custom_batt_soc_forecast_id' in runtimeparams.keys():
             params['passed_data']['custom_batt_soc_forecast_id'] = runtimeparams['custom_batt_soc_forecast_id']
         if 'custom_grid_forecast_id' in runtimeparams.keys():
             params['passed_data']['custom_grid_forecast_id'] = runtimeparams['custom_grid_forecast_id']
         if 'custom_cost_fun_id' in runtimeparams.keys():
             params['passed_data']['custom_cost_fun_id'] = runtimeparams['custom_cost_fun_id']
+        if 'custom_unit_load_cost_id' in runtimeparams.keys():
+            params['passed_data']['custom_unit_load_cost_id'] = runtimeparams['custom_unit_load_cost_id']
+        if 'custom_unit_prod_price_id' in runtimeparams.keys():
+            params['passed_data']['custom_unit_prod_price_id'] = runtimeparams['custom_unit_prod_price_id']
         if 'custom_deferrable_forecast_id' in runtimeparams.keys():
             params['passed_data']['custom_deferrable_forecast_id'] = runtimeparams['custom_deferrable_forecast_id']
     # Serialize the final params
     params = json.dumps(params)
     return params, retrieve_hass_conf, optim_conf
 
 def get_yaml_parse(config_path: str, use_secrets: Optional[bool] = True,
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `emhass-0.4.8.dist-info/METADATA` & `emhass-0.4.9.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emhass
-Version: 0.4.8
+Version: 0.4.9
 Summary: An Energy Management System for Home Assistant
 Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ
 Author-email: davidusb@gmail.com
 License: UNKNOWN
 Keywords: energy,management,optimization,hass
 Platform: UNKNOWN
@@ -63,30 +63,35 @@
   </a>
 </p>
 
 EHMASS is a Python module designed to optimize your home energy interfacing with Home Assistant.
 
 ## Introduction
 
-This module was conceived as an energy management optimization tool for residential electric power consumption and production systems.
-The main dependencies of this project are PVLib to model power from a PV residential installation and the PuLP Python package to perform the actual optimizations using the Linear Programming approach.
+EMHASS (Energy Management for Home Assistant) is an optimization tool designed for residential households. The package uses a Linear Programming approach to optimize energy usage while considering factors such as electricity prices, power generation from solar panels, and energy storage from batteries. EMHASS provides a high degree of configurability, making it easy to integrate with Home Assistant and other smart home systems. Whether you have solar panels, energy storage, or just a controllable load, EMHASS can provide an optimized daily schedule for your devices, allowing you to save money and minimize your environmental impact.
 
 The complete documentation for this package is [available here](https://emhass.readthedocs.io/en/latest/).
 
-## What is this?
+## What is Energy Management for Home Assistant (EMHASS)?
 
-The goal here is to optimize the energy use of your home in order to maximize a pre-defined cost function, for example: autoconsumption.
+EMHASS and Home Assistant provide a comprehensive energy management solution that can optimize energy usage and reduce costs for households. By integrating these two systems, households can take advantage of advanced energy management features that provide significant cost savings, increased energy efficiency, and greater sustainability.
 
-The main study case is a household where we have solar panels, a grid connection, one or more controllable (deferrable) electrical loads and an energy storage system with batteries. Of course, it is not necessary to have all these equipements to use EMHASS (PV panels, batteries, etc), in the minimal use case you have a controllable/deferrable load and you just want to obtain the optimized daily schedule for your load.
+EMHASS is a powerful energy management tool that generates an optimization plan based on variables such as solar power production, energy usage, and energy costs. The plan provides valuable insights into how energy can be better managed and utilized in the household. Even if households do not have all the necessary equipment, such as solar panels or batteries, EMHASS can still provide a minimal use case solution to optimize energy usage for controllable/deferrable loads.
+
+Home Assistant provides a platform for the automation of household devices based on the optimization plan generated by EMHASS. This includes devices such as batteries, pool pumps, hot water heaters, and electric vehicle (EV) chargers. By automating EV charging and other devices, households can take advantage of off-peak energy rates and optimize their EV charging schedule based on the optimization plan generated by EMHASS.
+
+One of the main benefits of integrating EMHASS and Home Assistant is the ability to customize and tailor the energy management solution to the specific needs and preferences of each household. With EMHASS, households can define their energy management objectives and constraints, such as maximizing self-consumption or minimizing energy costs, and the system will generate an optimization plan accordingly. Home Assistant provides a platform for the automation of devices based on the optimization plan, allowing households to create a fully customized and optimized energy management solution.
+
+Overall, the integration of EMHASS and Home Assistant offers a comprehensive energy management solution that provides significant cost savings, increased energy efficiency, and greater sustainability for households. By leveraging advanced energy management features and automation capabilities, households can achieve their energy management objectives while enjoying the benefits of a more efficient and sustainable energy usage, including optimized EV charging schedules.
 
 The package flow can be graphically represented as follows:
 
 ![](https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/ems_schema.png)
 
-So we have some data entering EMHASS (PV power, load, cost and selling prices forecasts), we have defined an objective function and some contraints (this is simply defined in a configuration file) and we have some controllable/deferrable loads. A call to an EMHASS optimization will yield the deferrable load schedule for future timestamps, the battery optimal power/SOC and the obtained value of the cost function. This information can published as sensors with attributes to Home Assistant and then we use the HA magic to automate our home energy consumption based on the optimization results.
+## Configuration and Installation
 
 The package is meant to be highly configurable with an object oriented modular approach and a main configuration file defined by the user.
 EMHASS was designed to be integrated with Home Assistant, hence it's name. 
 Installation instructions and example Home Assistant automation configurations are given below.
 
 You must follow these steps to make EMHASS work properly:
 
@@ -100,16 +105,14 @@
 
 5) The final step is to link the deferrable loads variables to real switchs on your installation. An example code for this using automations and the shell command integration is presented below in the **usage** section.
 
 A more detailed workflow is given below:
 
 ![](https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/workflow.png)
 
-## Installation
-
 ### Method 1) The EMHASS add-on for Home Assistant OS and supervised users
 
 For Home Assistant OS and HA Supervised users, I've developed an add-on that will help you use EMHASS. The add-on is more user friendly as the configuration can be modified directly in the add-on options pane and as with the standalone docker it exposes a web ui that can be used to inspect the optimization results and manually trigger a new optimization.
 
 You can find the add-on with the installation instructions here: [https://github.com/davidusb-geek/emhass-add-on](https://github.com/davidusb-geek/emhass-add-on)
 
 The add-on usage instructions can be found on the documentation pane of the add-on once installed or directly here: [EMHASS Add-on documentation](https://github.com/davidusb-geek/emhass-add-on/blob/main/emhass/DOCS.md)
@@ -167,33 +170,37 @@
 
 ## Usage
 
 ### Method 1) Add-on and docker standalone
 
 If using the add-on or the standalone docker installation, it exposes a simple webserver on port 5000. You can access it directly using your brower, ex: http://localhost:5000.
 
-With this web server you can perform RESTful POST commands on one ENDPOINT called `action` with four options:
+With this web server you can perform RESTful POST commands on multiple ENDPOINTS with prefix `action/*`:
 
 - A POST call to `action/perfect-optim` to perform a perfect optimization task on the historical data.
 - A POST call to `action/dayahead-optim` to perform a day-ahead optimization task of your home energy.
 - A POST call to `action/naive-mpc-optim` to perform a naive Model Predictive Controller optimization task. If using this option you will need to define the correct `runtimeparams` (see further below).
 - A POST call to `action/publish-data` to publish the optimization results data for the current timestamp.
+- A POST call to `action/forecast-model-fit` to train a machine learning forecaster model with the passed data (see the [dedicated section](https://emhass.readthedocs.io/en/latest/mlforecaster.html) for more help).
+- A POST call to `action/forecast-model-predict` to obtain a forecast from a pre-trained machine learning forecaster model (see the [dedicated section](https://emhass.readthedocs.io/en/latest/mlforecaster.html) for more help).
+- A POST call to `action/forecast-model-tune` to optimize the machine learning forecaster models hyperparameters using bayesian optimization (see the [dedicated section](https://emhass.readthedocs.io/en/latest/mlforecaster.html) for more help).
 
 A `curl` command can then be used to launch an optimization task like this: `curl -i -H 'Content-Type:application/json' -X POST -d '{}' http://localhost:5000/action/dayahead-optim`.
 
 ### Method 2) Legacy method using a Python virtual environment
 
 To run a command simply use the `emhass` CLI command followed by the needed arguments.
 The available arguments are:
-- `--action`: That is used to set the desired action, options are: `perfect-optim`, `dayahead-optim`, `naive-mpc-optim` and `publish-data`
+- `--action`: That is used to set the desired action, options are: `perfect-optim`, `dayahead-optim`, `naive-mpc-optim`, `publish-data`, `forecast-model-fit`, `forecast-model-predict` and `forecast-model-tune`.
 - `--config`: Define path to the config.yaml file (including the yaml file itself)
 - `--costfun`: Define the type of cost function, this is optional and the options are: `profit` (default), `cost`, `self-consumption`
 - `--log2file`: Define if we should log to a file or not, this is optional and the options are: `True` or `False` (default)
 - `--params`: Configuration as JSON. 
 - `--runtimeparams`: Data passed at runtime. This can be used to pass your own forecast data to EMHASS.
+- `--debug`: Use `True` for testing purposes.
 - `--version`: Show the current version of EMHASS.
 
 For example, the following line command can be used to perform a day-ahead optimization task:
 ```
 emhass --action 'dayahead-optim' --config '/home/user/emhass/config_emhass.yaml' --costfun 'profit'
 ```
 Before running any valuable command you need to modify the `config_emhass.yaml` and `secrets_emhass.yaml` files. These files should contain the information adapted to your own system. To do this take a look at the special section for this in the [documentation](https://emhass.readthedocs.io/en/latest/config.html).
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: emhass Version: 0.4.8 Summary: An Energy Management
+Metadata-Version: 2.1 Name: emhass Version: 0.4.9 Summary: An Energy Management
 System for Home Assistant Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ Author-email: davidusb@gmail.com License: UNKNOWN
 Keywords: energy,management,optimization,hass Platform: UNKNOWN Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8, <3.10
@@ -17,38 +17,58 @@
                                    [EMHASS]
               ****** Energy Management for Home Assistant ******
 
 [GitHub_release_(latest_by_date)] [GitHub_Workflow_Status] [https://codecov.io/
  github/davidusb-geek/emhass/branch/master/graph/badge.svg?token=BW7KSCHN90]
        [GitHub] [PyPI_-_Python_Version] [PyPI_-_Status] [Read_the_Docs]
 EHMASS is a Python module designed to optimize your home energy interfacing
-with Home Assistant. ## Introduction This module was conceived as an energy
-management optimization tool for residential electric power consumption and
-production systems. The main dependencies of this project are PVLib to model
-power from a PV residential installation and the PuLP Python package to perform
-the actual optimizations using the Linear Programming approach. The complete
-documentation for this package is [available here](https://
-emhass.readthedocs.io/en/latest/). ## What is this? The goal here is to
-optimize the energy use of your home in order to maximize a pre-defined cost
-function, for example: autoconsumption. The main study case is a household
-where we have solar panels, a grid connection, one or more controllable
-(deferrable) electrical loads and an energy storage system with batteries. Of
-course, it is not necessary to have all these equipements to use EMHASS (PV
-panels, batteries, etc), in the minimal use case you have a controllable/
-deferrable load and you just want to obtain the optimized daily schedule for
-your load. The package flow can be graphically represented as follows: ![]
-(https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/
-ems_schema.png) So we have some data entering EMHASS (PV power, load, cost and
-selling prices forecasts), we have defined an objective function and some
-contraints (this is simply defined in a configuration file) and we have some
-controllable/deferrable loads. A call to an EMHASS optimization will yield the
-deferrable load schedule for future timestamps, the battery optimal power/SOC
-and the obtained value of the cost function. This information can published as
-sensors with attributes to Home Assistant and then we use the HA magic to
-automate our home energy consumption based on the optimization results. The
+with Home Assistant. ## Introduction EMHASS (Energy Management for Home
+Assistant) is an optimization tool designed for residential households. The
+package uses a Linear Programming approach to optimize energy usage while
+considering factors such as electricity prices, power generation from solar
+panels, and energy storage from batteries. EMHASS provides a high degree of
+configurability, making it easy to integrate with Home Assistant and other
+smart home systems. Whether you have solar panels, energy storage, or just a
+controllable load, EMHASS can provide an optimized daily schedule for your
+devices, allowing you to save money and minimize your environmental impact. The
+complete documentation for this package is [available here](https://
+emhass.readthedocs.io/en/latest/). ## What is Energy Management for Home
+Assistant (EMHASS)? EMHASS and Home Assistant provide a comprehensive energy
+management solution that can optimize energy usage and reduce costs for
+households. By integrating these two systems, households can take advantage of
+advanced energy management features that provide significant cost savings,
+increased energy efficiency, and greater sustainability. EMHASS is a powerful
+energy management tool that generates an optimization plan based on variables
+such as solar power production, energy usage, and energy costs. The plan
+provides valuable insights into how energy can be better managed and utilized
+in the household. Even if households do not have all the necessary equipment,
+such as solar panels or batteries, EMHASS can still provide a minimal use case
+solution to optimize energy usage for controllable/deferrable loads. Home
+Assistant provides a platform for the automation of household devices based on
+the optimization plan generated by EMHASS. This includes devices such as
+batteries, pool pumps, hot water heaters, and electric vehicle (EV) chargers.
+By automating EV charging and other devices, households can take advantage of
+off-peak energy rates and optimize their EV charging schedule based on the
+optimization plan generated by EMHASS. One of the main benefits of integrating
+EMHASS and Home Assistant is the ability to customize and tailor the energy
+management solution to the specific needs and preferences of each household.
+With EMHASS, households can define their energy management objectives and
+constraints, such as maximizing self-consumption or minimizing energy costs,
+and the system will generate an optimization plan accordingly. Home Assistant
+provides a platform for the automation of devices based on the optimization
+plan, allowing households to create a fully customized and optimized energy
+management solution. Overall, the integration of EMHASS and Home Assistant
+offers a comprehensive energy management solution that provides significant
+cost savings, increased energy efficiency, and greater sustainability for
+households. By leveraging advanced energy management features and automation
+capabilities, households can achieve their energy management objectives while
+enjoying the benefits of a more efficient and sustainable energy usage,
+including optimized EV charging schedules. The package flow can be graphically
+represented as follows: ![](https://raw.githubusercontent.com/davidusb-geek/
+emhass/master/docs/images/ems_schema.png) ## Configuration and Installation The
 package is meant to be highly configurable with an object oriented modular
 approach and a main configuration file defined by the user. EMHASS was designed
 to be integrated with Home Assistant, hence it's name. Installation
 instructions and example Home Assistant automation configurations are given
 below. You must follow these steps to make EMHASS work properly: 1) Define all
 the parameters in the configuration file according to your installation. See
 the description for each parameter in the **configuration** section. 2) You
@@ -63,139 +83,150 @@
 optim`. 4) If youâre satisfied with the optimization results then you can set
 the optimization and data publish task commands in an automation. You can read
 more about this on the **usage** section below. 5) The final step is to link
 the deferrable loads variables to real switchs on your installation. An example
 code for this using automations and the shell command integration is presented
 below in the **usage** section. A more detailed workflow is given below: ![]
 (https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/
-workflow.png) ## Installation ### Method 1) The EMHASS add-on for Home
-Assistant OS and supervised users For Home Assistant OS and HA Supervised
-users, I've developed an add-on that will help you use EMHASS. The add-on is
-more user friendly as the configuration can be modified directly in the add-on
-options pane and as with the standalone docker it exposes a web ui that can be
-used to inspect the optimization results and manually trigger a new
-optimization. You can find the add-on with the installation instructions here:
-[https://github.com/davidusb-geek/emhass-add-on](https://github.com/davidusb-
-geek/emhass-add-on) The add-on usage instructions can be found on the
-documentation pane of the add-on once installed or directly here: [EMHASS Add-
-on documentation](https://github.com/davidusb-geek/emhass-add-on/blob/main/
-emhass/DOCS.md) These architectures are supported: `amd64`, `armv7`, `armhf`
-and `aarch64`. ### Method 2) Using Docker in standalone mode You can also
-install EMHASS using docker. This can be in the same machine as Home Assistant
-(if using the supervised install method) or in a different distant machine. To
-install first pull the latest image from docker hub: ``` docker pull davidusb/
-emhass-docker-standalone ``` You can also build your image locally. For this
-clone this repository, setup your `config_emhass.yaml` file and use the
-provided make file with this command: ``` make -f deploy_docker.mk clean_deploy
-``` Then load the image in the .tar file: ``` docker load -i .tar ``` Finally
-check your image tag with `docker images` and launch the docker itself: ```
-docker run -it --restart always -p 5000:5000 -e "LOCAL_COSTFUN=profit" -v $
-(pwd)/config_emhass.yaml:/app/config_emhass.yaml -v $(pwd)/secrets_emhass.yaml:
-/app/secrets_emhass.yaml --name DockerEMHASS  ``` ### Method 3) Legacy method
-using a Python virtual environment With this method it is recommended to
-install on a virtual environment. For this you will need `virtualenv`, install
-it using: ``` sudo apt install python3-virtualenv ``` Then create and activate
-the virtual environment: ``` virtualenv -p /usr/bin/python3 emhassenv cd
-emhassenv source bin/activate ``` Install using the distribution files: ```
-python3 -m pip install emhass ``` Clone this repository to obtain the example
-configuration files. We will suppose that this repository is cloned to: ``` /
-home/user/emhass ``` This will be the root path containing the yaml
-configuration files (`config_emhass.yaml` and `secrets_emhass.yaml`) and the
-different needed folders (a `data` folder to store the optimizations results
-and a `scripts` folder containing the bash scripts described further below). To
-upgrade the installation in the future just use: ``` python3 -m pip install --
-upgrade emhass ``` ## Usage ### Method 1) Add-on and docker standalone If using
-the add-on or the standalone docker installation, it exposes a simple webserver
-on port 5000. You can access it directly using your brower, ex: http://
-localhost:5000. With this web server you can perform RESTful POST commands on
-one ENDPOINT called `action` with four options: - A POST call to `action/
-perfect-optim` to perform a perfect optimization task on the historical data. -
-A POST call to `action/dayahead-optim` to perform a day-ahead optimization task
-of your home energy. - A POST call to `action/naive-mpc-optim` to perform a
-naive Model Predictive Controller optimization task. If using this option you
-will need to define the correct `runtimeparams` (see further below). - A POST
-call to `action/publish-data` to publish the optimization results data for the
-current timestamp. A `curl` command can then be used to launch an optimization
-task like this: `curl -i -H 'Content-Type:application/json' -X POST -d '{}'
-http://localhost:5000/action/dayahead-optim`. ### Method 2) Legacy method using
-a Python virtual environment To run a command simply use the `emhass` CLI
-command followed by the needed arguments. The available arguments are: - `--
-action`: That is used to set the desired action, options are: `perfect-optim`,
-`dayahead-optim`, `naive-mpc-optim` and `publish-data` - `--config`: Define
-path to the config.yaml file (including the yaml file itself) - `--costfun`:
-Define the type of cost function, this is optional and the options are:
-`profit` (default), `cost`, `self-consumption` - `--log2file`: Define if we
-should log to a file or not, this is optional and the options are: `True` or
-`False` (default) - `--params`: Configuration as JSON. - `--runtimeparams`:
-Data passed at runtime. This can be used to pass your own forecast data to
-EMHASS. - `--version`: Show the current version of EMHASS. For example, the
-following line command can be used to perform a day-ahead optimization task:
-``` emhass --action 'dayahead-optim' --config '/home/user/emhass/
-config_emhass.yaml' --costfun 'profit' ``` Before running any valuable command
-you need to modify the `config_emhass.yaml` and `secrets_emhass.yaml` files.
-These files should contain the information adapted to your own system. To do
-this take a look at the special section for this in the [documentation](https:/
-/emhass.readthedocs.io/en/latest/config.html). ## Home Assistant integration To
-integrate with home assistant we will need to define some shell commands in the
-`configuration.yaml` file and some basic automations in the `automations.yaml`
-file. ### Method 1) Add-on and docker standalone In `configuration.yaml`: ```
-shell_command: dayahead_optim: "curl -i -H \"Content-Type:application/json\" -
-X POST -d '{}' http://localhost:5000/action/dayahead-optim" publish_data: "curl
--i -H \"Content-Type:application/json\" -X POST -d '{}' http://localhost:5000/
-action/publish-data" ``` ### Method 2) Legacy method using a Python virtual
-environment In `configuration.yaml`: ``` shell_command: dayahead_optim: /home/
-user/emhass/scripts/dayahead_optim.sh publish_data: /home/user/emhass/scripts/
-publish_data.sh ``` Create the file `dayahead_optim.sh` with the following
-content: ``` #!/bin/bash . /home/user/emhassenv/bin/activate emhass --action
-'dayahead-optim' --config '/home/user/emhass/config_emhass.yaml' ``` And the
-file `publish_data.sh` with the following content: ``` #!/bin/bash . /home/
-user/emhassenv/bin/activate emhass --action 'publish-data' --config '/home/
-user/emhass/config_emhass.yaml' ``` Then specify user rights and make the files
-executables: ``` sudo chmod -R 755 /home/user/emhass/scripts/dayahead_optim.sh
-sudo chmod -R 755 /home/user/emhass/scripts/publish_data.sh sudo chmod +x /
-home/user/emhass/scripts/dayahead_optim.sh sudo chmod +x /home/user/emhass/
-scripts/publish_data.sh ``` ### Common for any installation method In
-`automations.yaml`: ``` - alias: EMHASS day-ahead optimization trigger:
-platform: time at: '05:30:00' action: - service: shell_command.dayahead_optim -
-alias: EMHASS publish data trigger: - minutes: /5 platform: time_pattern
-action: - service: shell_command.publish_data ``` In these automations the day-
-ahead optimization is performed everyday at 5:30am and the data is published
-every 5 minutes. The final action will be to link a sensor value in Home
-Assistant to control the switch of a desired controllable load. For example
-imagine that I want to control my water heater and that the `publish-data`
-action is publishing the optimized value of a deferrable load that I want to be
-linked to my water heater desired behavior. In this case we could use an
-automation like this one below to control the desired real switch: ```
-automation: - alias: Water Heater Optimized ON trigger: - minutes: /5 platform:
-time_pattern condition: - condition: numeric_state entity_id:
-sensor.p_deferrable0 above: 0.1 action: - service: homeassistant.turn_on
-entity_id: switch.water_heater_switch ``` A second automation should be used to
-turn off the switch: ``` automation: - alias: Water Heater Optimized OFF
-trigger: - minutes: /5 platform: time_pattern condition: - condition:
-numeric_state entity_id: sensor.p_deferrable0 below: 0.1 action: - service:
-homeassistant.turn_off entity_id: switch.water_heater_switch ``` ## The
-publish-data specificities The `publish-data` command will push to Home
-Assistant the optimization results for each deferrable load defined in the
-configuration. For example if you have defined two deferrable loads, then the
-command will publish `sensor.p_deferrable0` and `sensor.p_deferrable1` to Home
-Assistant. When the `dayahead-optim` is launched, after the optimization, a csv
-file will be saved on disk. The `publish-data` command will load the latest csv
-file and look for the closest timestamp that match the current time using the
-`datetime.now()` method in Python. This means that if EMHASS is configured for
-30min time step optimizations, the csv will be saved with timestamps 00:00, 00:
-30, 01:00, 01:30, ... and so on. If the current time is 00:05, then the closest
-timestamp of the optimization results that will be published is 00:00. If the
-current time is 00:25, then the closest timestamp of the optimization results
-that will be published is 00:30. The `publish-data` command will also publish
-PV and load forecast data on sensors `p_pv_forecast` and `p_load_forecast`. If
-using a battery, then the battery optimized power and the SOC will be published
-on sensors `p_batt_forecast` and `soc_batt_forecast`. On these sensors the
-future values are passed as nested attributes. It is possible to provide custm
-sensor names for all the data exported by the `publish-data` command. For this,
-when using the `publish-data` endpoint just add some runtime parameters as
+workflow.png) ### Method 1) The EMHASS add-on for Home Assistant OS and
+supervised users For Home Assistant OS and HA Supervised users, I've developed
+an add-on that will help you use EMHASS. The add-on is more user friendly as
+the configuration can be modified directly in the add-on options pane and as
+with the standalone docker it exposes a web ui that can be used to inspect the
+optimization results and manually trigger a new optimization. You can find the
+add-on with the installation instructions here: [https://github.com/davidusb-
+geek/emhass-add-on](https://github.com/davidusb-geek/emhass-add-on) The add-on
+usage instructions can be found on the documentation pane of the add-on once
+installed or directly here: [EMHASS Add-on documentation](https://github.com/
+davidusb-geek/emhass-add-on/blob/main/emhass/DOCS.md) These architectures are
+supported: `amd64`, `armv7`, `armhf` and `aarch64`. ### Method 2) Using Docker
+in standalone mode You can also install EMHASS using docker. This can be in the
+same machine as Home Assistant (if using the supervised install method) or in a
+different distant machine. To install first pull the latest image from docker
+hub: ``` docker pull davidusb/emhass-docker-standalone ``` You can also build
+your image locally. For this clone this repository, setup your
+`config_emhass.yaml` file and use the provided make file with this command: ```
+make -f deploy_docker.mk clean_deploy ``` Then load the image in the .tar file:
+``` docker load -i .tar ``` Finally check your image tag with `docker images`
+and launch the docker itself: ``` docker run -it --restart always -p 5000:5000
+-e "LOCAL_COSTFUN=profit" -v $(pwd)/config_emhass.yaml:/app/config_emhass.yaml
+-v $(pwd)/secrets_emhass.yaml:/app/secrets_emhass.yaml --name DockerEMHASS  ```
+### Method 3) Legacy method using a Python virtual environment With this method
+it is recommended to install on a virtual environment. For this you will need
+`virtualenv`, install it using: ``` sudo apt install python3-virtualenv ```
+Then create and activate the virtual environment: ``` virtualenv -p /usr/bin/
+python3 emhassenv cd emhassenv source bin/activate ``` Install using the
+distribution files: ``` python3 -m pip install emhass ``` Clone this repository
+to obtain the example configuration files. We will suppose that this repository
+is cloned to: ``` /home/user/emhass ``` This will be the root path containing
+the yaml configuration files (`config_emhass.yaml` and `secrets_emhass.yaml`)
+and the different needed folders (a `data` folder to store the optimizations
+results and a `scripts` folder containing the bash scripts described further
+below). To upgrade the installation in the future just use: ``` python3 -m pip
+install --upgrade emhass ``` ## Usage ### Method 1) Add-on and docker
+standalone If using the add-on or the standalone docker installation, it
+exposes a simple webserver on port 5000. You can access it directly using your
+brower, ex: http://localhost:5000. With this web server you can perform RESTful
+POST commands on multiple ENDPOINTS with prefix `action/*`: - A POST call to
+`action/perfect-optim` to perform a perfect optimization task on the historical
+data. - A POST call to `action/dayahead-optim` to perform a day-ahead
+optimization task of your home energy. - A POST call to `action/naive-mpc-
+optim` to perform a naive Model Predictive Controller optimization task. If
+using this option you will need to define the correct `runtimeparams` (see
+further below). - A POST call to `action/publish-data` to publish the
+optimization results data for the current timestamp. - A POST call to `action/
+forecast-model-fit` to train a machine learning forecaster model with the
+passed data (see the [dedicated section](https://emhass.readthedocs.io/en/
+latest/mlforecaster.html) for more help). - A POST call to `action/forecast-
+model-predict` to obtain a forecast from a pre-trained machine learning
+forecaster model (see the [dedicated section](https://emhass.readthedocs.io/en/
+latest/mlforecaster.html) for more help). - A POST call to `action/forecast-
+model-tune` to optimize the machine learning forecaster models hyperparameters
+using bayesian optimization (see the [dedicated section](https://
+emhass.readthedocs.io/en/latest/mlforecaster.html) for more help). A `curl`
+command can then be used to launch an optimization task like this: `curl -i -
+H 'Content-Type:application/json' -X POST -d '{}' http://localhost:5000/action/
+dayahead-optim`. ### Method 2) Legacy method using a Python virtual environment
+To run a command simply use the `emhass` CLI command followed by the needed
+arguments. The available arguments are: - `--action`: That is used to set the
+desired action, options are: `perfect-optim`, `dayahead-optim`, `naive-mpc-
+optim`, `publish-data`, `forecast-model-fit`, `forecast-model-predict` and
+`forecast-model-tune`. - `--config`: Define path to the config.yaml file
+(including the yaml file itself) - `--costfun`: Define the type of cost
+function, this is optional and the options are: `profit` (default), `cost`,
+`self-consumption` - `--log2file`: Define if we should log to a file or not,
+this is optional and the options are: `True` or `False` (default) - `--params`:
+Configuration as JSON. - `--runtimeparams`: Data passed at runtime. This can be
+used to pass your own forecast data to EMHASS. - `--debug`: Use `True` for
+testing purposes. - `--version`: Show the current version of EMHASS. For
+example, the following line command can be used to perform a day-ahead
+optimization task: ``` emhass --action 'dayahead-optim' --config '/home/user/
+emhass/config_emhass.yaml' --costfun 'profit' ``` Before running any valuable
+command you need to modify the `config_emhass.yaml` and `secrets_emhass.yaml`
+files. These files should contain the information adapted to your own system.
+To do this take a look at the special section for this in the [documentation]
+(https://emhass.readthedocs.io/en/latest/config.html). ## Home Assistant
+integration To integrate with home assistant we will need to define some shell
+commands in the `configuration.yaml` file and some basic automations in the
+`automations.yaml` file. ### Method 1) Add-on and docker standalone In
+`configuration.yaml`: ``` shell_command: dayahead_optim: "curl -i -H \"Content-
+Type:application/json\" -X POST -d '{}' http://localhost:5000/action/dayahead-
+optim" publish_data: "curl -i -H \"Content-Type:application/json\" -X POST -d '
+{}' http://localhost:5000/action/publish-data" ``` ### Method 2) Legacy method
+using a Python virtual environment In `configuration.yaml`: ``` shell_command:
+dayahead_optim: /home/user/emhass/scripts/dayahead_optim.sh publish_data: /
+home/user/emhass/scripts/publish_data.sh ``` Create the file
+`dayahead_optim.sh` with the following content: ``` #!/bin/bash . /home/user/
+emhassenv/bin/activate emhass --action 'dayahead-optim' --config '/home/user/
+emhass/config_emhass.yaml' ``` And the file `publish_data.sh` with the
+following content: ``` #!/bin/bash . /home/user/emhassenv/bin/activate emhass -
+-action 'publish-data' --config '/home/user/emhass/config_emhass.yaml' ``` Then
+specify user rights and make the files executables: ``` sudo chmod -R 755 /
+home/user/emhass/scripts/dayahead_optim.sh sudo chmod -R 755 /home/user/emhass/
+scripts/publish_data.sh sudo chmod +x /home/user/emhass/scripts/
+dayahead_optim.sh sudo chmod +x /home/user/emhass/scripts/publish_data.sh ```
+### Common for any installation method In `automations.yaml`: ``` - alias:
+EMHASS day-ahead optimization trigger: platform: time at: '05:30:00' action: -
+service: shell_command.dayahead_optim - alias: EMHASS publish data trigger: -
+minutes: /5 platform: time_pattern action: - service:
+shell_command.publish_data ``` In these automations the day-ahead optimization
+is performed everyday at 5:30am and the data is published every 5 minutes. The
+final action will be to link a sensor value in Home Assistant to control the
+switch of a desired controllable load. For example imagine that I want to
+control my water heater and that the `publish-data` action is publishing the
+optimized value of a deferrable load that I want to be linked to my water
+heater desired behavior. In this case we could use an automation like this one
+below to control the desired real switch: ``` automation: - alias: Water Heater
+Optimized ON trigger: - minutes: /5 platform: time_pattern condition: -
+condition: numeric_state entity_id: sensor.p_deferrable0 above: 0.1 action: -
+service: homeassistant.turn_on entity_id: switch.water_heater_switch ``` A
+second automation should be used to turn off the switch: ``` automation: -
+alias: Water Heater Optimized OFF trigger: - minutes: /5 platform: time_pattern
+condition: - condition: numeric_state entity_id: sensor.p_deferrable0 below:
+0.1 action: - service: homeassistant.turn_off entity_id:
+switch.water_heater_switch ``` ## The publish-data specificities The `publish-
+data` command will push to Home Assistant the optimization results for each
+deferrable load defined in the configuration. For example if you have defined
+two deferrable loads, then the command will publish `sensor.p_deferrable0` and
+`sensor.p_deferrable1` to Home Assistant. When the `dayahead-optim` is
+launched, after the optimization, a csv file will be saved on disk. The
+`publish-data` command will load the latest csv file and look for the closest
+timestamp that match the current time using the `datetime.now()` method in
+Python. This means that if EMHASS is configured for 30min time step
+optimizations, the csv will be saved with timestamps 00:00, 00:30, 01:00, 01:
+30, ... and so on. If the current time is 00:05, then the closest timestamp of
+the optimization results that will be published is 00:00. If the current time
+is 00:25, then the closest timestamp of the optimization results that will be
+published is 00:30. The `publish-data` command will also publish PV and load
+forecast data on sensors `p_pv_forecast` and `p_load_forecast`. If using a
+battery, then the battery optimized power and the SOC will be published on
+sensors `p_batt_forecast` and `soc_batt_forecast`. On these sensors the future
+values are passed as nested attributes. It is possible to provide custm sensor
+names for all the data exported by the `publish-data` command. For this, when
+using the `publish-data` endpoint just add some runtime parameters as
 dictionaries like this: ``` shell_command: publish_data: "curl -i -H \"Content-
 Type:application/json\" -X POST -d '{\"custom_load_forecast_id\":
 {\"entity_id\": \"sensor.p_load_forecast\", \"unit_of_measurement\": \"W\",
 \"friendly_name\": \"Load Power Forecast\"}}' http://localhost:5000/action/
 publish-data" ``` These keys are available to modify: `custom_pv_forecast_id`,
 `custom_load_forecast_id`, `custom_batt_forecast_id`,
 `custom_batt_soc_forecast_id`, `custom_grid_forecast_id`, `custom_cost_fun_id`,
```

## Comparing `emhass-0.4.8.dist-info/RECORD` & `emhass-0.4.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 emhass/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-emhass/command_line.py,sha256=IbHexJGwDnqDVvRN1V07QXmE5sm1XtO8oHhBjp87Fi4,33594
+emhass/command_line.py,sha256=QSxkOmmjTEBcBwOo7C4p70_pHPHtpqJmHi7ZmBGgF3M,34580
 emhass/forecast.py,sha256=mJY846P_VWK_Ov-F-SZg_We55Y799a5b8Lwo1bO_JK8,43072
-emhass/machine_learning_forecaster.py,sha256=FaWZv8aMS8ihx1Z6RhY6yuNkbkouZV8CujXAMmcFnAI,14966
+emhass/machine_learning_forecaster.py,sha256=C0k3bkq0pXRmfwIMigrh0aI2ZRO-qa7WFtDcPoGwFEQ,14964
 emhass/optimization.py,sha256=QL9LpOhhpo_YgmF3_lvXWPGdz-ZeH62_zUCwm2swlyM,30582
 emhass/retrieve_hass.py,sha256=lsLSiWB2XC1TTlAw_GR7YWjVXti4ZXKhICROST8UlTw,15888
-emhass/utils.py,sha256=_EuITuTur7RwI3_oBRWEmEQk1F_Ke1wZ4pOSp57VRC4,22445
+emhass/utils.py,sha256=3P2yw8_4PfRY0JawGr7lIWUrCYIL6fT6tBDdWO5PIbg,23107
 emhass/web_server.py,sha256=wQT0HD8N86zC2V28L4zVUqVfP6sj0U-ZmltoUc51rXs,18255
 emhass/static/style.css,sha256=5qGJl0MZGSaSvr0HUcGQ9UgMtDKP2CiyE-1H-jbsLuU,6760
 emhass/templates/index.html,sha256=DGP5PayjyDJnZo9LYRrGg0pYIfr-AwwITgKocmUbruU,6615
-emhass-0.4.8.dist-info/METADATA,sha256=ppNVOXjCPNrfU2_zHH4FLCuf7tibxEQUm0jbTeoeYqM,24995
-emhass-0.4.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-emhass-0.4.8.dist-info/entry_points.txt,sha256=tJULCm7mHGYb_IxyzPN_4KFYvhxv209_jq68jPiByy0,53
-emhass-0.4.8.dist-info/top_level.txt,sha256=L7fIX4awfmxQbAePtSdVg2e6x_HhghfReHfsKSpKr9I,7
-emhass-0.4.8.dist-info/RECORD,,
+emhass-0.4.9.dist-info/METADATA,sha256=oAdUtkUj4dlQnjoEgzf7sBAM0GDfKr903UCDzklNLis,27317
+emhass-0.4.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+emhass-0.4.9.dist-info/entry_points.txt,sha256=tJULCm7mHGYb_IxyzPN_4KFYvhxv209_jq68jPiByy0,53
+emhass-0.4.9.dist-info/top_level.txt,sha256=L7fIX4awfmxQbAePtSdVg2e6x_HhghfReHfsKSpKr9I,7
+emhass-0.4.9.dist-info/RECORD,,
```

