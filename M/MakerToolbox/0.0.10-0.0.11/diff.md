# Comparing `tmp/makertoolbox-0.0.10.tar.gz` & `tmp/makertoolbox-0.0.11.tar.gz`

## Comparing `makertoolbox-0.0.10.tar` & `makertoolbox-0.0.11.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rwxr-xr-x   0        0        0      166 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/deploy.sh
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/pyproject.toml.bak
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/example.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/algorithms/Paths.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/algorithms/__init__.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/gpio/InputPin.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/gpio/OutputPin.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/gpio/PWMPin.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/gpio/RaspberryPi.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/gpio/__init__.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/hardware/Button.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/hardware/DCMotorDriver.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/hardware/ServoMotor.py
--rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/hardware/StepperDrivers.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/hardware/__init__.py
--rw-r--r--   0        0        0     7547 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/machines/CoreXY.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/machines/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/utility/XYPosition.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/src/MakerToolbox/utility/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/tests/__init__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/LICENSE
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/README.md
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/pyproject.toml
--rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 makertoolbox-0.0.10/PKG-INFO
+-rwxr-xr-x   0        0        0      166 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/deploy.sh
+-rwxr-xr-x   0        0        0      184 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/override-pi.sh
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/pyproject.toml.bak
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/example.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/algorithms/Paths.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/algorithms/__init__.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/gpio/InputPin.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/gpio/OutputPin.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/gpio/PWMPin.py
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/gpio/RaspberryPi.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/gpio/__init__.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/hardware/Button.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/hardware/DCMotorDriver.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/hardware/ServoMotor.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/hardware/StepperDrivers.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/hardware/__init__.py
+-rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/machines/CoreXY.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/machines/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/utility/XYPosition.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/src/MakerToolbox/utility/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/tests/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/LICENSE
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/README.md
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/pyproject.toml
+-rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 makertoolbox-0.0.11/PKG-INFO
```

### Comparing `makertoolbox-0.0.10/pyproject.toml.bak` & `makertoolbox-0.0.11/pyproject.toml.bak`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "MakerToolbox"
-version = "0.0.9"
+version = "0.0.10"
 authors = [
   { name="Jack Campbell", email="makertoolboxrepo@gmail.com" },
 ]
 description = "The MakerToolbox module provides a collection of tools for working with various electronic hardware."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `makertoolbox-0.0.10/src/MakerToolbox/example.py` & `makertoolbox-0.0.11/src/MakerToolbox/example.py`

 * *Files identical despite different names*

### Comparing `makertoolbox-0.0.10/src/MakerToolbox/algorithms/Paths.py` & `makertoolbox-0.0.11/src/MakerToolbox/algorithms/Paths.py`

 * *Files identical despite different names*

### Comparing `makertoolbox-0.0.10/src/MakerToolbox/gpio/OutputPin.py` & `makertoolbox-0.0.11/src/MakerToolbox/gpio/OutputPin.py`

 * *Files identical despite different names*

### Comparing `makertoolbox-0.0.10/src/MakerToolbox/gpio/PWMPin.py` & `makertoolbox-0.0.11/src/MakerToolbox/gpio/PWMPin.py`

 * *Files identical despite different names*

### Comparing `makertoolbox-0.0.10/src/MakerToolbox/gpio/RaspberryPi.py` & `makertoolbox-0.0.11/src/MakerToolbox/gpio/RaspberryPi.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,17 +24,19 @@
 
     class GPIO:
         """
         Placeholder GPIO class to substitute for RPi class when not running on a RPi4B
         """
         IN = 0
         OUT = 1
+        PUD_UP = 2
+        PUD_DOWN = 3
 
         @staticmethod
-        def setup(x, y):
+        def setup(x, y, pull_up_down=None):
             pass
 
         @staticmethod
         def input(x):
             return False
 
         @staticmethod
@@ -70,20 +72,20 @@
 
 
 class GenericRPiInPin(InputPin):
     """
     Input pin implementation for generic RPi.
     """
 
-    def __init__(self, pin: int):
+    def __init__(self, pin: int, pull_up: bool = True):
         super().__init__(pin)
-        GPIO.setup(pin, GPIO.IN)
+        GPIO.setup(pin, GPIO.IN, pull_up_down=GPIO.PUD_UP if pull_up else GPIO.PUD_DOWN)
 
     def read(self) -> bool:
-        return GPIO.input(self._pin)
+        return bool(GPIO.input(self._pin))
 
 
 class GenericRPiPWMPin(PWMPin):
     """
     PWM pin implementation for generic RPi.
     """
```

### Comparing `makertoolbox-0.0.10/src/MakerToolbox/hardware/Button.py` & `makertoolbox-0.0.11/src/MakerToolbox/hardware/Button.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def is_pressed(self) -> bool:
         """
         Checks if the button is currently pressed.
 
         Returns:
             bool: True if the button is pressed, False otherwise.
         """
-        return self._pin.read() is self._pressed_value
+        return self._pin.read() == self._pressed_value
 
     def wait_for_press(self, delay: float = 0.01):
         """
         Waits until the button is pressed.
 
         Args:
             delay (float, optional): The delay in seconds between each check for button press. Defaults to 0.01.
```

### Comparing `makertoolbox-0.0.10/src/MakerToolbox/hardware/DCMotorDriver.py` & `makertoolbox-0.0.11/src/MakerToolbox/hardware/DCMotorDriver.py`

 * *Files identical despite different names*

### Comparing `makertoolbox-0.0.10/src/MakerToolbox/hardware/StepperDrivers.py` & `makertoolbox-0.0.11/src/MakerToolbox/hardware/StepperDrivers.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         """
         Moves multiple stepper motors simultaneously.
 
         Args:
             steppers (List['StepperDriver']): A list of stepper motor drivers.
             num_steps (int, optional): The number of steps to perform. Defaults to 1.
             delay_func (callable, optional): A function that calculates the delay between steps. Defaults to lambda current, total: 0.003.
-            """
+        """
         phase_counts = [len(stepper._step_phases) for stepper in steppers]
         assert max(phase_counts) == min(phase_counts)
         num_phases = max(phase_counts)
         for current_step in range(num_steps):
             delay = delay_func(current_step, num_steps)
             for x in range(num_phases):
                 for stepper in steppers:
```

### Comparing `makertoolbox-0.0.10/src/MakerToolbox/machines/CoreXY.py` & `makertoolbox-0.0.11/src/MakerToolbox/machines/CoreXY.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,182 +1,158 @@
-from ..hardware import BasicStepperDriver
+from ..hardware import BasicStepperDriver, StepperDriver
 from ..utility import XYPosition
 
 
 class CoreXY:
     """
     Class representing a CoreXY utility system.
 
     Attributes:
         stepper_a (BasicStepperDriver): Stepper driver for motor A.
         stepper_b (BasicStepperDriver): Stepper driver for motor B.
         _current_position (XYPosition): Current position of the utility system.
     """
 
-    def __init__(self, stepper_a: BasicStepperDriver, stepper_b: BasicStepperDriver):
+    def __init__(self, stepper_a: BasicStepperDriver, stepper_b: BasicStepperDriver, delay_func: callable = lambda c, t: 0.006):
         """
         Initializes a CoreXY utility system.
 
         Args:
             stepper_a (BasicStepperDriver): Stepper driver for motor A.
             stepper_b (BasicStepperDriver): Stepper driver for motor B.
         """
         self._stepper_a = stepper_a
         self._stepper_b = stepper_b
         self._current_position = XYPosition(0, 0)
-
-    def step_together(self, steps: int, delay_func: callable = None):
-        """
-        Performs a specified number of steps on both motors simultaneously.
-
-        Args:
-            steps (int): Number of steps to perform.
-            delay_func (callable, optional): Custom delay function. If provided,
-                it should take two arguments: current step and total steps,
-                and return the delay time in seconds for the current step.
-        """
-        for current in range(steps):
-            if delay_func is not None:
-                delay = delay_func(current, steps)
-            else:
-                delay = None
-            self._stepper_a.step(delay)
-            self._stepper_b.step(delay)
-
-    @staticmethod
-    def step_single(stepper: BasicStepperDriver, steps: int, delay_func: callable = None):
-        """
-        Performs a specified number of steps on a single motor.
-
-        Args:
-            stepper (BasicStepperDriver): Stepper driver to control.
-            steps (int): Number of steps to perform.
-            delay_func (callable, optional): Custom delay function. If provided,
-                it should take two arguments: current step and total steps,
-                and return the delay time in seconds for the current step.
-        """
-        for current in range(steps):
-            if delay_func is not None:
-                delay = delay_func(current, steps)
-            else:
-                delay = None
-            stepper.step(delay)
+        self._delay_func = delay_func
 
     def north(self, steps: int, delay_func: callable = None):
         """
         Moves the utility system north by a specified number of steps.
 
         Args:
             steps (int): Number of steps to move north.
             delay_func (callable, optional): Custom delay function. If provided,
                 it should take two arguments: current step and total steps,
                 and return the delay time in seconds for the current step.
         """
+        if delay_func is None:
+            delay_func = self._delay_func
         self._stepper_a.set_direction(True)
         self._stepper_b.set_direction(False)
-        self.step_together(steps, delay_func)
+        StepperDriver.move([self._stepper_a, self._stepper_b], steps, delay_func)
         self._current_position.y -= steps
 
     def south(self, steps: int, delay_func: callable = None):
         """
         Moves the utility system south by a specified number of steps.
 
         Args:
             steps (int): Number of steps to move south.
             delay_func (callable, optional): Custom delay function. If provided,
                 it should take two arguments: current step and total steps,
                 and return the delay time in seconds for the current step.
         """
+        if delay_func is None:
+            delay_func = self._delay_func
         self._stepper_a.set_direction(False)
         self._stepper_b.set_direction(True)
-        self.step_together(steps, delay_func)
+        StepperDriver.move([self._stepper_a, self._stepper_b], steps, delay_func)
         self._current_position.y += steps
 
     def east(self, steps: int, delay_func: callable = None):
         """
         Moves the utility system east by a specified number of steps.
 
         Args:
             steps (int): Number of steps to move east.
             delay_func (callable, optional): Custom delay function. If provided,
                 it should take two arguments: current step and total steps,
                 and return the delay time in seconds for the current step.
         """
-        self._stepper_a.set_direction(True)
-        self._stepper_b.set_direction(True)
-        self.step_together(steps, delay_func)
+        if delay_func is None:
+            delay_func = self._delay_func
+        self._stepper_a.set_direction(False)
+        self._stepper_b.set_direction(False)
+        StepperDriver.move([self._stepper_a, self._stepper_b], steps, delay_func)
         self._current_position.x += steps
 
     def west(self, steps: int, delay_func: callable = None):
         """
         Moves the utility system west by a specified number of steps.
 
         Args:
             steps (int): Number of steps to move west.
             delay_func (callable, optional): Custom delay function. If provided,
                 it should take two arguments: current step and total steps,
                 and return the delay time in seconds for the current step.
         """
-        self._stepper_a.set_direction(False)
-        self._stepper_b.set_direction(False)
-        self.step_together(steps, delay_func)
+        if delay_func is None:
+            delay_func = self._delay_func
+        self._stepper_a.set_direction(True)
+        self._stepper_b.set_direction(True)
+        StepperDriver.move([self._stepper_a, self._stepper_b], steps, delay_func)
         self._current_position.x -= steps
 
     def north_west(self, steps: int, delay_func: callable = None):
         """
         Moves the utility system north west by a specified number of steps.
 
         Args:
             steps (int): Number of steps to move north west.
             delay_func (callable, optional): Custom delay function. If provided,
                 it should take two arguments: current step and total steps,
                 and return the delay time in seconds for the current step.
         """
-        self._stepper_a.set_direction(True)
-        self.step_single(self._stepper_a, steps * 2, delay_func)
+        if delay_func is None:
+            delay_func = self._delay_func
+        self._stepper_a.step(steps * 2, delay_func, direction=True)
         self._current_position.x -= steps
         self._current_position.y -= steps
 
     def north_east(self, steps: int, delay_func: callable = None):
         """
         Moves the utility system north east by a specified number of steps.
 
         Args:
             steps (int): Number of steps to move north east.
             delay_func (callable, optional): Custom delay function. If provided,
                 it should take two arguments: current step and total steps,
                 and return the delay time in seconds for the current step.
         """
-        self._stepper_b.set_direction(True)
-        self.step_single(self._stepper_b, steps * 2, delay_func)
+        if delay_func is None:
+            delay_func = self._delay_func
+        self._stepper_b.step(steps * 2, delay_func, direction=False)
         self._current_position.x += steps
         self._current_position.y -= steps
 
     def south_west(self, steps: int, delay_func: callable = None):
         """
         Moves the utility system south west by a specified number of steps.
 
         Args:
             steps (int): Number of steps to move south west.
             delay_func (callable, optional): Custom delay function. If provided,
                 it should take two arguments: current step and total steps,
                 and return the delay time in seconds for the current step.
         """
-        self._stepper_b.set_direction(False)
-        self.step_single(self._stepper_b, steps * 2, delay_func)
+        if delay_func is None:
+            delay_func = self._delay_func
+        self._stepper_b.step(steps * 2, delay_func, direction=True)
         self._current_position.x -= steps
         self._current_position.y += steps
 
     def south_east(self, steps: int, delay_func: callable = None):
         """
         Moves the utility system south east by a specified number of steps.
 
         Args:
             steps (int): Number of steps to move south east.
             delay_func (callable, optional): Custom delay function. If provided,
                 it should take two arguments: current step and total steps,
                 and return the delay time in seconds for the current step.
         """
-        self._stepper_a.set_direction(False)
-        self.step_single(self._stepper_a, steps * 2, delay_func)
+        if delay_func is None:
+            delay_func = self._delay_func
+        self._stepper_a.step(steps * 2, delay_func, direction=False)
         self._current_position.x += steps
         self._current_position.y += steps
```

### Comparing `makertoolbox-0.0.10/src/MakerToolbox/utility/XYPosition.py` & `makertoolbox-0.0.11/src/MakerToolbox/utility/XYPosition.py`

 * *Files identical despite different names*

### Comparing `makertoolbox-0.0.10/LICENSE` & `makertoolbox-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `makertoolbox-0.0.10/README.md` & `makertoolbox-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `makertoolbox-0.0.10/pyproject.toml` & `makertoolbox-0.0.11/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "MakerToolbox"
-version = "0.0.10"
+version = "0.0.11"
 authors = [
   { name="Jack Campbell", email="makertoolboxrepo@gmail.com" },
 ]
 description = "The MakerToolbox module provides a collection of tools for working with various electronic hardware."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `makertoolbox-0.0.10/PKG-INFO` & `makertoolbox-0.0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MakerToolbox
-Version: 0.0.10
+Version: 0.0.11
 Summary: The MakerToolbox module provides a collection of tools for working with various electronic hardware.
 Project-URL: Homepage, https://github.com/jackcampbell19/MakerToolbox
 Project-URL: Bug Tracker, https://github.com/jackcampbell19/MakerToolbox/issues
 Author-email: Jack Campbell <makertoolboxrepo@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

